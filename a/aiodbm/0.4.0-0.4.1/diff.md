# Comparing `tmp/aiodbm-0.4.0.tar.gz` & `tmp/aiodbm-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodbm-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodbm-0.4.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodbm-0.4.0.tar` & `aiodbm-0.4.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2023-06-06 13:50:04.064326 aiodbm-0.4.0/LICENSE
--rw-r--r--   0        0        0     3725 2023-06-06 13:50:04.064326 aiodbm-0.4.0/README.rst
--rw-r--r--   0        0        0      795 2023-06-06 13:50:04.064326 aiodbm-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      158 2023-06-06 13:50:04.064326 aiodbm-0.4.0/src/aiodbm/__init__.py
--rw-r--r--   0        0        0     6796 2023-06-06 13:50:04.064326 aiodbm-0.4.0/src/aiodbm/core.py
--rw-r--r--   0        0        0     3103 2023-06-06 13:50:04.064326 aiodbm-0.4.0/src/aiodbm/threads.py
--rw-r--r--   0        0        0     4417 1970-01-01 00:00:00.000000 aiodbm-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-08 14:03:44.312835 aiodbm-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3862 2023-06-08 14:03:44.312835 aiodbm-0.4.1/README.rst
+-rw-r--r--   0        0        0      795 2023-06-08 14:03:44.312835 aiodbm-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-06-08 14:03:44.312835 aiodbm-0.4.1/src/aiodbm/__init__.py
+-rw-r--r--   0        0        0     6796 2023-06-08 14:03:44.312835 aiodbm-0.4.1/src/aiodbm/core.py
+-rw-r--r--   0        0        0     3103 2023-06-08 14:03:44.312835 aiodbm-0.4.1/src/aiodbm/threads.py
+-rw-r--r--   0        0        0     4554 1970-01-01 00:00:00.000000 aiodbm-0.4.1/PKG-INFO
```

### Comparing `aiodbm-0.4.0/LICENSE` & `aiodbm-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodbm-0.4.0/README.rst` & `aiodbm-0.4.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -13,55 +13,64 @@
 
 * Full coverage of Python's DBM and GDBM API
 * Typing support
 * Docstrings and documentation
 * Fully tested
 
 Why use DBM?
-------------
+---------------
 
-DBM is a fast, embedded key-value store.
+`DBM <https://en.wikipedia.org/wiki/DBM_(computing)>`_ is a fast and easy to use, embedded key-value store.
 It is supported by Python's standard library [1]_ and can be used on most systems without requiring additional dependencies [2]_.
 
-Compared to Sqlite - the other popular embedded database support by Python's standard library - it can be significantly faster,
-but also does not provide any of sqlite's advanced features like transactions or process safety. [3]_
+Compared to Sqlite - the other embedded database supported by Python's standard library - it is significantly faster when used as key/value store.
+
+According to our measurement we see that aiodbm is about 140x faster on writes and about 3.5x faster on reads [3]_ on Linux:
 
-If you are are looking for a simple and fast key-value store (e.g. for caching) - especially on Linux systems,
-where the GDBM variant is available - DBM can be a good solution.
+.. image:: https://raw.githubusercontent.com/ErikKalkoken/aiodbm/main/measurements/measurements.png
+  :width: 800
+  :alt: Throughput measurements for aiodbm vs. aiosqlite
+
+So if you are looking for a fast and an easy to use key-value store (e.g. for caching) on Linux systems, DBM can be a good solution. And aiodbm allows you use DBM in your asyncio programs.
 
 Caveats
 -------
 
-While Python's DBM library should ensure, that aiodbm works with any DBM variant and on any system,
-this library has been developed and tested primarily with GDBM on Linux.
 On non Linux-like systems Python might use it's "dumb" DBM implementation, which will be much slower.
 
 DBM is not process safe. If you need a key-value store in a multi process context (e.g. a web server running with gunicorn) we'd recommend to use Redis or something similar instead.
 
 Usage
 -----
 
-Here is a basic example on how to use the queue:
+Here is a basic example on how to use the library:
 
 .. code:: python
 
-    import asyncio
+   import asyncio
+
+   import aiodbm
 
-    import aiodbm
 
+   async def main():
+      # opening/creating database
+      async with aiodbm.open("example.dbm", "c") as db:
 
-    async def main():
-        async with aiodbm.open("example.dbm", "c") as db:  # opening/creating database
-            await db.set("alpha", "green")  # creating new key alpha with value green
-            value = await db.get("alpha")  # fetching value for key alpha
-            print(value)
-            await db.delete("alpha")  # delete key alpha
+         # creating new key alpha with value green
+         await db.set("alpha", "green")
 
+         # fetching value for key alpha
+         value = await db.get("alpha")
+         print(value)
 
-    asyncio.run(main())
+         # delete key alpha
+         await db.delete("alpha")
+
+
+   asyncio.run(main())
 
 
 Installation
 ------------
 
 You can install this library directly from PyPI with the following command:
 
@@ -70,17 +79,19 @@
     pip install aiodbm
 
 ------------
 
 Reference
 ---------
 
-.. [1] Python's DBM module: https://docs.python.org/3/library/dbm.html
+.. [1] See also Python's DBM module: https://docs.python.org/3/library/dbm.html
+
 .. [2] The newer DBM variants GDBM or NDBM are preinstalled on most Linux/Unix systems: https://en.wikipedia.org/wiki/DBM_(computing)#Availability
-.. [3] Python benchmark with DBM, Sqlite and other embedded databases: https://charlesleifer.com/blog/completely-un-scientific-benchmarks-of-some-embedded-databases-with-python/
+
+.. [3] We compared the asyncio versions with 10.000 write and read operations of key/value pairs on Linux with GDBM. See also measurements folder for more details.
 
 .. _DBM: https://en.wikipedia.org/wiki/DBM_(computing)
 .. _benchmark: https://charlesleifer.com/blog/completely-un-scientific-benchmarks-of-some-embedded-databases-with-python/
 
 .. |release| image:: https://img.shields.io/pypi/v/aiodbm?label=release
    :target: https://pypi.org/project/aiodbm/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodbm
```

### Comparing `aiodbm-0.4.0/pyproject.toml` & `aiodbm-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodbm-0.4.0/src/aiodbm/core.py` & `aiodbm-0.4.1/src/aiodbm/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         async with open("example.dbm", "c") as db:
             ...
 
     Usage B:
 
     .. code-block:: Python
 
-        db = async open("example.dbm", "c"):
+        db = await open("example.dbm", "c"):
         ...
         await db.close()
     """
 
     def connector():
         filepath = str(file)
         return dbm.open(filepath, *args, **kwargs)
```

### Comparing `aiodbm-0.4.0/src/aiodbm/threads.py` & `aiodbm-0.4.1/src/aiodbm/threads.py`

 * *Files identical despite different names*

### Comparing `aiodbm-0.4.0/PKG-INFO` & `aiodbm-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodbm
-Version: 0.4.0
+Version: 0.4.1
 Summary: An AsyncIO bridge for DBM.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -30,55 +30,64 @@
 
 * Full coverage of Python's DBM and GDBM API
 * Typing support
 * Docstrings and documentation
 * Fully tested
 
 Why use DBM?
-------------
+---------------
 
-DBM is a fast, embedded key-value store.
+`DBM <https://en.wikipedia.org/wiki/DBM_(computing)>`_ is a fast and easy to use, embedded key-value store.
 It is supported by Python's standard library [1]_ and can be used on most systems without requiring additional dependencies [2]_.
 
-Compared to Sqlite - the other popular embedded database support by Python's standard library - it can be significantly faster,
-but also does not provide any of sqlite's advanced features like transactions or process safety. [3]_
+Compared to Sqlite - the other embedded database supported by Python's standard library - it is significantly faster when used as key/value store.
+
+According to our measurement we see that aiodbm is about 140x faster on writes and about 3.5x faster on reads [3]_ on Linux:
 
-If you are are looking for a simple and fast key-value store (e.g. for caching) - especially on Linux systems,
-where the GDBM variant is available - DBM can be a good solution.
+.. image:: https://raw.githubusercontent.com/ErikKalkoken/aiodbm/main/measurements/measurements.png
+  :width: 800
+  :alt: Throughput measurements for aiodbm vs. aiosqlite
+
+So if you are looking for a fast and an easy to use key-value store (e.g. for caching) on Linux systems, DBM can be a good solution. And aiodbm allows you use DBM in your asyncio programs.
 
 Caveats
 -------
 
-While Python's DBM library should ensure, that aiodbm works with any DBM variant and on any system,
-this library has been developed and tested primarily with GDBM on Linux.
 On non Linux-like systems Python might use it's "dumb" DBM implementation, which will be much slower.
 
 DBM is not process safe. If you need a key-value store in a multi process context (e.g. a web server running with gunicorn) we'd recommend to use Redis or something similar instead.
 
 Usage
 -----
 
-Here is a basic example on how to use the queue:
+Here is a basic example on how to use the library:
 
 .. code:: python
 
-    import asyncio
+   import asyncio
+
+   import aiodbm
 
-    import aiodbm
 
+   async def main():
+      # opening/creating database
+      async with aiodbm.open("example.dbm", "c") as db:
 
-    async def main():
-        async with aiodbm.open("example.dbm", "c") as db:  # opening/creating database
-            await db.set("alpha", "green")  # creating new key alpha with value green
-            value = await db.get("alpha")  # fetching value for key alpha
-            print(value)
-            await db.delete("alpha")  # delete key alpha
+         # creating new key alpha with value green
+         await db.set("alpha", "green")
 
+         # fetching value for key alpha
+         value = await db.get("alpha")
+         print(value)
 
-    asyncio.run(main())
+         # delete key alpha
+         await db.delete("alpha")
+
+
+   asyncio.run(main())
 
 
 Installation
 ------------
 
 You can install this library directly from PyPI with the following command:
 
@@ -87,17 +96,19 @@
     pip install aiodbm
 
 ------------
 
 Reference
 ---------
 
-.. [1] Python's DBM module: https://docs.python.org/3/library/dbm.html
+.. [1] See also Python's DBM module: https://docs.python.org/3/library/dbm.html
+
 .. [2] The newer DBM variants GDBM or NDBM are preinstalled on most Linux/Unix systems: https://en.wikipedia.org/wiki/DBM_(computing)#Availability
-.. [3] Python benchmark with DBM, Sqlite and other embedded databases: https://charlesleifer.com/blog/completely-un-scientific-benchmarks-of-some-embedded-databases-with-python/
+
+.. [3] We compared the asyncio versions with 10.000 write and read operations of key/value pairs on Linux with GDBM. See also measurements folder for more details.
 
 .. _DBM: https://en.wikipedia.org/wiki/DBM_(computing)
 .. _benchmark: https://charlesleifer.com/blog/completely-un-scientific-benchmarks-of-some-embedded-databases-with-python/
 
 .. |release| image:: https://img.shields.io/pypi/v/aiodbm?label=release
    :target: https://pypi.org/project/aiodbm/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodbm
```

