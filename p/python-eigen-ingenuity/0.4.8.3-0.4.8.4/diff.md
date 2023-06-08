# Comparing `tmp/python-eigen-ingenuity-0.4.8.3.tar.gz` & `tmp/python-eigen-ingenuity-0.4.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-eigen-ingenuity-0.4.8.3.tar", last modified: Thu Jun  8 10:06:44 2023, max compression
+gzip compressed data, was "python-eigen-ingenuity-0.4.8.4.tar", last modified: Thu Jun  8 10:12:56 2023, max compression
```

## Comparing `python-eigen-ingenuity-0.4.8.3.tar` & `python-eigen-ingenuity-0.4.8.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 10:06:44.438701 python-eigen-ingenuity-0.4.8.3/
--rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.3/LICENSE
--rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.8.3/MANIFEST.in
--rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-06-08 10:06:44.438461 python-eigen-ingenuity-0.4.8.3/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.3/README.md
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 10:06:44.436943 python-eigen-ingenuity-0.4.8.3/eigeningenuity/
--rw-r--r--   0 berhic     (501) staff       (20)     1203 2023-06-08 09:07:24.000000 python-eigen-ingenuity-0.4.8.3/eigeningenuity/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)    16232 2023-05-18 14:59:11.000000 python-eigen-ingenuity-0.4.8.3/eigeningenuity/assetmodel.py
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 10:06:44.437268 python-eigen-ingenuity-0.4.8.3/eigeningenuity/core/
--rw-r--r--   0 berhic     (501) staff       (20)     7741 2023-05-23 15:25:59.000000 python-eigen-ingenuity-0.4.8.3/eigeningenuity/core/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.3/eigeningenuity/core/debug.py
--rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.8.3/eigeningenuity/elastic.py
--rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.8.3/eigeningenuity/events.py
--rw-r--r--   0 berhic     (501) staff       (20)    36274 2023-05-24 08:12:38.000000 python-eigen-ingenuity-0.4.8.3/eigeningenuity/historian.py
--rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.8.3/eigeningenuity/smartdash.py
--rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.8.3/eigeningenuity/sql.py
--rw-r--r--   0 berhic     (501) staff       (20)    15524 2023-06-08 10:06:11.000000 python-eigen-ingenuity-0.4.8.3/eigeningenuity/util.py
--rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.3/pyproject.toml
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 10:06:44.438197 python-eigen-ingenuity-0.4.8.3/python_eigen_ingenuity.egg-info/
--rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-06-08 10:06:44.000000 python-eigen-ingenuity-0.4.8.3/python_eigen_ingenuity.egg-info/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)      551 2023-06-08 10:06:44.000000 python-eigen-ingenuity-0.4.8.3/python_eigen_ingenuity.egg-info/SOURCES.txt
--rw-r--r--   0 berhic     (501) staff       (20)        1 2023-06-08 10:06:44.000000 python-eigen-ingenuity-0.4.8.3/python_eigen_ingenuity.egg-info/dependency_links.txt
--rw-r--r--   0 berhic     (501) staff       (20)       29 2023-06-08 10:06:44.000000 python-eigen-ingenuity-0.4.8.3/python_eigen_ingenuity.egg-info/requires.txt
--rw-r--r--   0 berhic     (501) staff       (20)       15 2023-06-08 10:06:44.000000 python-eigen-ingenuity-0.4.8.3/python_eigen_ingenuity.egg-info/top_level.txt
--rw-r--r--   0 berhic     (501) staff       (20)       38 2023-06-08 10:06:44.438749 python-eigen-ingenuity-0.4.8.3/setup.cfg
--rw-r--r--   0 berhic     (501) staff       (20)      719 2023-06-08 10:06:31.000000 python-eigen-ingenuity-0.4.8.3/setup.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 10:12:56.282847 python-eigen-ingenuity-0.4.8.4/
+-rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.4/LICENSE
+-rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.8.4/MANIFEST.in
+-rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-06-08 10:12:56.282611 python-eigen-ingenuity-0.4.8.4/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.4/README.md
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 10:12:56.281294 python-eigen-ingenuity-0.4.8.4/eigeningenuity/
+-rw-r--r--   0 berhic     (501) staff       (20)     1203 2023-06-08 09:07:24.000000 python-eigen-ingenuity-0.4.8.4/eigeningenuity/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)    16232 2023-05-18 14:59:11.000000 python-eigen-ingenuity-0.4.8.4/eigeningenuity/assetmodel.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 10:12:56.281607 python-eigen-ingenuity-0.4.8.4/eigeningenuity/core/
+-rw-r--r--   0 berhic     (501) staff       (20)     7741 2023-05-23 15:25:59.000000 python-eigen-ingenuity-0.4.8.4/eigeningenuity/core/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.4/eigeningenuity/core/debug.py
+-rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.8.4/eigeningenuity/elastic.py
+-rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.8.4/eigeningenuity/events.py
+-rw-r--r--   0 berhic     (501) staff       (20)    36274 2023-05-24 08:12:38.000000 python-eigen-ingenuity-0.4.8.4/eigeningenuity/historian.py
+-rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.8.4/eigeningenuity/smartdash.py
+-rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.8.4/eigeningenuity/sql.py
+-rw-r--r--   0 berhic     (501) staff       (20)    15606 2023-06-08 10:12:14.000000 python-eigen-ingenuity-0.4.8.4/eigeningenuity/util.py
+-rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.4/pyproject.toml
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 10:12:56.282374 python-eigen-ingenuity-0.4.8.4/python_eigen_ingenuity.egg-info/
+-rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-06-08 10:12:56.000000 python-eigen-ingenuity-0.4.8.4/python_eigen_ingenuity.egg-info/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)      551 2023-06-08 10:12:56.000000 python-eigen-ingenuity-0.4.8.4/python_eigen_ingenuity.egg-info/SOURCES.txt
+-rw-r--r--   0 berhic     (501) staff       (20)        1 2023-06-08 10:12:56.000000 python-eigen-ingenuity-0.4.8.4/python_eigen_ingenuity.egg-info/dependency_links.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       29 2023-06-08 10:12:56.000000 python-eigen-ingenuity-0.4.8.4/python_eigen_ingenuity.egg-info/requires.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       15 2023-06-08 10:12:56.000000 python-eigen-ingenuity-0.4.8.4/python_eigen_ingenuity.egg-info/top_level.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       38 2023-06-08 10:12:56.282894 python-eigen-ingenuity-0.4.8.4/setup.cfg
+-rw-r--r--   0 berhic     (501) staff       (20)      719 2023-06-08 10:12:48.000000 python-eigen-ingenuity-0.4.8.4/setup.py
```

### Comparing `python-eigen-ingenuity-0.4.8.3/LICENSE` & `python-eigen-ingenuity-0.4.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/PKG-INFO` & `python-eigen-ingenuity-0.4.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.8.3
+Version: 0.4.8.4
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.8.3/README.md` & `python-eigen-ingenuity-0.4.8.4/README.md`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/eigeningenuity/__init__.py` & `python-eigen-ingenuity-0.4.8.4/eigeningenuity/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/eigeningenuity/assetmodel.py` & `python-eigen-ingenuity-0.4.8.4/eigeningenuity/assetmodel.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/eigeningenuity/core/__init__.py` & `python-eigen-ingenuity-0.4.8.4/eigeningenuity/core/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/eigeningenuity/core/debug.py` & `python-eigen-ingenuity-0.4.8.4/eigeningenuity/core/debug.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/eigeningenuity/elastic.py` & `python-eigen-ingenuity-0.4.8.4/eigeningenuity/elastic.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/eigeningenuity/events.py` & `python-eigen-ingenuity-0.4.8.4/eigeningenuity/events.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/eigeningenuity/historian.py` & `python-eigen-ingenuity-0.4.8.4/eigeningenuity/historian.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/eigeningenuity/smartdash.py` & `python-eigen-ingenuity-0.4.8.4/eigeningenuity/smartdash.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/eigeningenuity/sql.py` & `python-eigen-ingenuity-0.4.8.4/eigeningenuity/sql.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/eigeningenuity/util.py` & `python-eigen-ingenuity-0.4.8.4/eigeningenuity/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,22 @@
 
 def _authenticate_azure_user(baseurl):
     global cache
     ENCRYPTION_KEY = b'nn4yG-HkjZQBBBsfMrGeTfPDG5omNa_GNVIOF4DM9-w='
 
     if not os.path.exists(os.path.dirname(__file__) + '/.azure'):
         os.mkdir(os.path.dirname(__file__) + "/.azure")
+
     if os.path.exists(os.path.dirname(__file__) + "/.azure/token_cache.bin"):
-        cache.deserialize(decrypt(open(os.path.dirname(__file__) + "/.azure/token_cache.bin", "r").read(),ENCRYPTION_KEY))
+        encryptedToken = open(os.path.dirname(__file__) + "/.azure/token_cache.bin", "rb").read()
+        if encryptedToken != b'':
+            cache.deserialize(decrypt(encryptedToken,ENCRYPTION_KEY))
+
     atexit.register(lambda:
-        open(os.path.dirname(__file__) + "/.azure/token_cache.bin", "w").write(encrypt(cache.serialize(),ENCRYPTION_KEY))
+        open(os.path.dirname(__file__) + "/.azure/token_cache.bin", "wb").write(encrypt(cache.serialize(),ENCRYPTION_KEY))
         if cache.has_state_changed else None
         )
 
     client_id = os.environ["CLIENTID"]
     tenant_id = os.environ["TENANTID"]
     authority = f'https://login.microsoftonline.com/{tenant_id}'
     scope=[f"{baseurl}/user_impersonation"]
```

### Comparing `python-eigen-ingenuity-0.4.8.3/python_eigen_ingenuity.egg-info/PKG-INFO` & `python-eigen-ingenuity-0.4.8.4/python_eigen_ingenuity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.8.3
+Version: 0.4.8.4
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.8.3/python_eigen_ingenuity.egg-info/SOURCES.txt` & `python-eigen-ingenuity-0.4.8.4/python_eigen_ingenuity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8.3/setup.py` & `python-eigen-ingenuity-0.4.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README = (HERE / "README.md").read_text()
 
 pkgname = 'python-eigen-ingenuity'
 
 # Invoke setup
 setup(
     name=pkgname,
-    version='0.4.8.3',
+    version='0.4.8.4',
     author='Murray Callander',
     author_email='info@eigen.co',
     url='https://www.eigen.co/',
     description="A python library used to query data from the Eigen Ingenuity system",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages("."),
```

