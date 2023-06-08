# Comparing `tmp/HanLabImport-0.1.0.tar.gz` & `tmp/HanLabImport-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HanLabImport-0.1.0.tar", last modified: Tue Jun  6 12:28:21 2023, max compression
+gzip compressed data, was "HanLabImport-0.1.1.tar", last modified: Thu Jun  8 00:53:17 2023, max compression
```

## Comparing `HanLabImport-0.1.0.tar` & `HanLabImport-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/HanLabImport/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/HanLabImport/config/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/config/HanLab.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/HanLabImport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-06 12:28:21.000000 HanLabImport-0.1.0/HanLabImport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-06 12:28:21.000000 HanLabImport-0.1.0/HanLabImport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:28:21.000000 HanLabImport-0.1.0/HanLabImport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 12:28:21.000000 HanLabImport-0.1.0/HanLabImport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 12:28:21.000000 HanLabImport-0.1.0/HanLabImport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:53:17.886245 HanLabImport-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:53:17.886245 HanLabImport-0.1.1/HanLabImport/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-08 00:53:02.000000 HanLabImport-0.1.1/HanLabImport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:53:17.886245 HanLabImport-0.1.1/HanLabImport/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-08 00:53:02.000000 HanLabImport-0.1.1/HanLabImport/config/HanLab.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 00:53:02.000000 HanLabImport-0.1.1/HanLabImport/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-08 00:53:02.000000 HanLabImport-0.1.1/HanLabImport/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-06-08 00:53:02.000000 HanLabImport-0.1.1/HanLabImport/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 00:53:02.000000 HanLabImport-0.1.1/HanLabImport/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:53:17.886245 HanLabImport-0.1.1/HanLabImport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-08 00:53:17.000000 HanLabImport-0.1.1/HanLabImport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-08 00:53:17.000000 HanLabImport-0.1.1/HanLabImport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:53:17.000000 HanLabImport-0.1.1/HanLabImport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 00:53:17.000000 HanLabImport-0.1.1/HanLabImport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 00:53:17.000000 HanLabImport-0.1.1/HanLabImport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 00:53:02.000000 HanLabImport-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-08 00:53:17.886245 HanLabImport-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-08 00:53:02.000000 HanLabImport-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 00:53:02.000000 HanLabImport-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:53:17.886245 HanLabImport-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-08 00:53:02.000000 HanLabImport-0.1.1/setup.py
```

### Comparing `HanLabImport-0.1.0/HanLabImport/config/HanLab.cfg` & `HanLabImport-0.1.1/HanLabImport/config/HanLab.cfg`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.1.0/HanLabImport/config/config.py` & `HanLabImport-0.1.1/HanLabImport/config/config.py`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.1.0/HanLabImport.egg-info/PKG-INFO` & `HanLabImport-0.1.1/HanLabImport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HanLabImport
-Version: 0.1.0
+Version: 0.1.1
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabImport
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabImport/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `HanLabImport-0.1.0/LICENSE` & `HanLabImport-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.1.0/PKG-INFO` & `HanLabImport-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HanLabImport
-Version: 0.1.0
+Version: 0.1.1
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabImport
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabImport/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `HanLabImport-0.1.0/README.md` & `HanLabImport-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.1.0/setup.py` & `HanLabImport-0.1.1/setup.py`

 * *Files identical despite different names*

