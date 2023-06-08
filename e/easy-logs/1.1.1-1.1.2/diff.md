# Comparing `tmp/easy_logs-1.1.1.tar.gz` & `tmp/easy_logs-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_logs-1.1.1.tar", last modified: Thu Jun  8 07:15:44 2023, max compression
+gzip compressed data, was "easy_logs-1.1.2.tar", last modified: Thu Jun  8 07:18:15 2023, max compression
```

## Comparing `easy_logs-1.1.1.tar` & `easy_logs-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:15:44.843630 easy_logs-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-08 07:15:44.843630 easy_logs-1.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:15:44.843630 easy_logs-1.1.1/easy_logs/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 07:15:30.000000 easy_logs-1.1.1/easy_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-08 07:15:30.000000 easy_logs-1.1.1/easy_logs/_configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-08 07:15:30.000000 easy_logs-1.1.1/easy_logs/_logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-08 07:15:30.000000 easy_logs-1.1.1/easy_logs/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:15:44.843630 easy_logs-1.1.1/easy_logs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-08 07:15:44.000000 easy_logs-1.1.1/easy_logs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 07:15:44.000000 easy_logs-1.1.1/easy_logs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:15:44.000000 easy_logs-1.1.1/easy_logs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 07:15:44.000000 easy_logs-1.1.1/easy_logs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 07:15:44.843630 easy_logs-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-08 07:15:30.000000 easy_logs-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:18:15.104111 easy_logs-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-08 07:18:15.104111 easy_logs-1.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:18:15.104111 easy_logs-1.1.2/easy_logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 07:18:05.000000 easy_logs-1.1.2/easy_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-08 07:18:05.000000 easy_logs-1.1.2/easy_logs/_configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-08 07:18:05.000000 easy_logs-1.1.2/easy_logs/_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-08 07:18:05.000000 easy_logs-1.1.2/easy_logs/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:18:15.104111 easy_logs-1.1.2/easy_logs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-08 07:18:15.000000 easy_logs-1.1.2/easy_logs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 07:18:15.000000 easy_logs-1.1.2/easy_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:18:15.000000 easy_logs-1.1.2/easy_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 07:18:15.000000 easy_logs-1.1.2/easy_logs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 07:18:15.104111 easy_logs-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-08 07:18:05.000000 easy_logs-1.1.2/setup.py
```

### Comparing `easy_logs-1.1.1/PKG-INFO` & `easy_logs-1.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_logs
-Version: 1.1.1
+Version: 1.1.2
 Summary: package for easy colored logs with predefined configurations.
 Home-page: https://github.com/michalskibinski109/easy_logging
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,8 +12,8 @@
 Description-Content-Type: text/markdown
 
 
 ![example workflow](https://github.com/michalskibinski109/easy_logs/actions/workflows/python-app.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/easy_logs.svg)](https://badge.fury.io/py/miskibin)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 # easy_logs
-[Documentation](https://github.com/michalskibinski109/easy_logs/readme.md)
+[Documentation](https://github.com/michalskibinski109/easy_logs/tree/main#readme)
```

### Comparing `easy_logs-1.1.1/easy_logs/__init__.py` & `easy_logs-1.1.2/easy_logs/__init__.py`

 * *Files identical despite different names*

### Comparing `easy_logs-1.1.1/easy_logs/_configurations.py` & `easy_logs-1.1.2/easy_logs/_configurations.py`

 * *Files identical despite different names*

### Comparing `easy_logs-1.1.1/easy_logs/_logging_utils.py` & `easy_logs-1.1.2/easy_logs/_logging_utils.py`

 * *Files identical despite different names*

### Comparing `easy_logs-1.1.1/easy_logs/main.py` & `easy_logs-1.1.2/easy_logs/main.py`

 * *Files identical despite different names*

### Comparing `easy_logs-1.1.1/easy_logs.egg-info/PKG-INFO` & `easy_logs-1.1.2/easy_logs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-logs
-Version: 1.1.1
+Version: 1.1.2
 Summary: package for easy colored logs with predefined configurations.
 Home-page: https://github.com/michalskibinski109/easy_logging
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,8 +12,8 @@
 Description-Content-Type: text/markdown
 
 
 ![example workflow](https://github.com/michalskibinski109/easy_logs/actions/workflows/python-app.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/easy_logs.svg)](https://badge.fury.io/py/miskibin)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 # easy_logs
-[Documentation](https://github.com/michalskibinski109/easy_logs/readme.md)
+[Documentation](https://github.com/michalskibinski109/easy_logs/tree/main#readme)
```

### Comparing `easy_logs-1.1.1/setup.py` & `easy_logs-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 
 LONG_DESCRIPTION = """
 ![example workflow](https://github.com/michalskibinski109/easy_logs/actions/workflows/python-app.yml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/easy_logs.svg)](https://badge.fury.io/py/miskibin)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 # easy_logs
-[Documentation](https://github.com/michalskibinski109/easy_logs/readme.md)
+[Documentation](https://github.com/michalskibinski109/easy_logs/tree/main#readme)
 """
 
 setuptools.setup(
     name="easy_logs",
-    version="1.1.1",
+    version="1.1.2",
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
     description="package for easy colored logs with predefined configurations.",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     files_to_include=["easy_logs"],
     package_data={"readme": ["readme.md"]},
```

