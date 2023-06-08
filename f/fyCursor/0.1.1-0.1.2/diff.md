# Comparing `tmp/fyCursor-0.1.1.tar.gz` & `tmp/fyCursor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyCursor-0.1.1.tar", last modified: Tue Jun  6 22:06:14 2023, max compression
+gzip compressed data, was "fyCursor-0.1.2.tar", last modified: Thu Jun  8 20:29:54 2023, max compression
```

## Comparing `fyCursor-0.1.1.tar` & `fyCursor-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:06:14.532587 fyCursor-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-06 22:06:04.000000 fyCursor-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-06 22:06:14.532587 fyCursor-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-06 22:06:04.000000 fyCursor-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:06:14.532587 fyCursor-0.1.1/fyCursor/
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:06:14.532587 fyCursor-0.1.1/fyCursor/core/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/core/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-06 22:06:04.000000 fyCursor-0.1.1/fyCursor/core/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 22:06:14.532587 fyCursor-0.1.1/fyCursor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-06 22:06:14.000000 fyCursor-0.1.1/fyCursor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-06 22:06:14.000000 fyCursor-0.1.1/fyCursor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 22:06:14.000000 fyCursor-0.1.1/fyCursor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 22:06:14.000000 fyCursor-0.1.1/fyCursor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 22:06:14.532587 fyCursor-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-06 22:06:04.000000 fyCursor-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:29:54.347142 fyCursor-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-08 20:29:34.000000 fyCursor-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-08 20:29:54.347142 fyCursor-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-08 20:29:34.000000 fyCursor-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:29:54.347142 fyCursor-0.1.2/fyCursor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:29:54.347142 fyCursor-0.1.2/fyCursor/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/core/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-06-08 20:29:34.000000 fyCursor-0.1.2/fyCursor/core/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:29:54.347142 fyCursor-0.1.2/fyCursor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-08 20:29:54.000000 fyCursor-0.1.2/fyCursor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-08 20:29:54.000000 fyCursor-0.1.2/fyCursor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:29:54.000000 fyCursor-0.1.2/fyCursor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 20:29:54.000000 fyCursor-0.1.2/fyCursor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:29:54.347142 fyCursor-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-08 20:29:34.000000 fyCursor-0.1.2/setup.py
```

### Comparing `fyCursor-0.1.1/LICENSE` & `fyCursor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.1/PKG-INFO` & `fyCursor-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,16 +13,20 @@
 # fyCursor
 A simple cursor for managing sqlite3 databases
 
 ## Installation 
 You can simply use pip: &nbsp;
 \$`pip3 install fyCursor`
 
+<!-- Repobeats analytics -->
+#  Analytics 
+![Alt](https://repobeats.axiom.co/api/embed/0dda89a6c675987fd8c7d580fc77c9a05cd58b62.svg "Repobeats analytics image")
+
 # Changelog 📄
-### 📀 v0.1.0
+### 📀 v0.1.x
 - New fyCursor methods:
     - create_table (BETA)
 - Table and Fields (‼️ BETA):
     - Table class:
         - TableError
         - ``insert`` method
         - ``create`` method
```

### Comparing `fyCursor-0.1.1/fyCursor/__init__.py` & `fyCursor-0.1.2/fyCursor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         database=database,
     )
     return connection.cursor(fyCursor)  # type: ignore
 
 
 __title__ = "fyCursor"
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 __author__ = "felixyeahh"
 __author_email__ = "<felixyeah@outlook.com>"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Baffu Team"
```

### Comparing `fyCursor-0.1.1/fyCursor/__main__.py` & `fyCursor-0.1.2/fyCursor/__main__.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.1/fyCursor/core/cursor.py` & `fyCursor-0.1.2/fyCursor/core/cursor.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.1/fyCursor/core/fields.py` & `fyCursor-0.1.2/fyCursor/core/fields.py`

 * *Files identical despite different names*

### Comparing `fyCursor-0.1.1/fyCursor/core/table.py` & `fyCursor-0.1.2/fyCursor/core/table.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .fields import Field
-from .._types.cursor import fyCursor
+from ..types.cursor import fyCursor
 from typing import Any, Optional
 
 
 class TableError(BaseException):
     """Raised if something went wrong while creating a table class"""
```

### Comparing `fyCursor-0.1.1/fyCursor.egg-info/PKG-INFO` & `fyCursor-0.1.2/fyCursor.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyCursor
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple sqlite3 cursor
 Author: felixyeahh
 Author-email: <felixyeah@outlook.com>
 License: MIT
 Keywords: python,sqlite3,database
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,16 +13,20 @@
 # fyCursor
 A simple cursor for managing sqlite3 databases
 
 ## Installation 
 You can simply use pip: &nbsp;
 \$`pip3 install fyCursor`
 
+<!-- Repobeats analytics -->
+#  Analytics 
+![Alt](https://repobeats.axiom.co/api/embed/0dda89a6c675987fd8c7d580fc77c9a05cd58b62.svg "Repobeats analytics image")
+
 # Changelog 📄
-### 📀 v0.1.0
+### 📀 v0.1.x
 - New fyCursor methods:
     - create_table (BETA)
 - Table and Fields (‼️ BETA):
     - Table class:
         - TableError
         - ``insert`` method
         - ``create`` method
```

### Comparing `fyCursor-0.1.1/setup.py` & `fyCursor-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     LONG_DESCRIPTION = "\n" + fh.read()
 
 # Setting up
 setup(
     name="fyCursor",
-    version="0.1.1",
+    version="0.1.2",
     description='Simple sqlite3 cursor',
     author="felixyeahh",
     author_email="<felixyeah@outlook.com>",
     license="MIT",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
```

