# Comparing `tmp/bspcpy-1.0.3.tar.gz` & `tmp/bspcpy-1.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bspcpy-1.0.3.tar", last modified: Thu Jun  8 01:31:20 2023, max compression
+gzip compressed data, was "bspcpy-1.0.3.1.tar", last modified: Thu Jun  8 01:34:50 2023, max compression
```

## Comparing `bspcpy-1.0.3.tar` & `bspcpy-1.0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-06-08 01:31:20.125227 bspcpy-1.0.3/
--rw-r--r--   0 alan      (1000) alan      (1000)     1067 2023-04-03 19:03:41.000000 bspcpy-1.0.3/LICENSE
--rw-r--r--   0 alan      (1000) alan      (1000)     2959 2023-06-08 01:31:20.125227 bspcpy-1.0.3/PKG-INFO
--rw-r--r--   0 alan      (1000) alan      (1000)     1347 2023-03-04 03:19:34.000000 bspcpy-1.0.3/README.md
-drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-06-08 01:31:20.125227 bspcpy-1.0.3/bspc/
--rw-r--r--   0 alan      (1000) alan      (1000)       79 2023-06-08 01:21:34.000000 bspcpy-1.0.3/bspc/__init__.py
--rw-r--r--   0 alan      (1000) alan      (1000)    12757 2023-03-22 01:14:02.000000 bspcpy-1.0.3/bspc/classes.py
--rw-r--r--   0 alan      (1000) alan      (1000)     2079 2023-03-22 01:08:33.000000 bspcpy-1.0.3/bspc/query.py
-drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-06-08 01:31:20.125227 bspcpy-1.0.3/bspcpy.egg-info/
--rw-r--r--   0 alan      (1000) alan      (1000)     2959 2023-06-08 01:31:20.000000 bspcpy-1.0.3/bspcpy.egg-info/PKG-INFO
--rw-r--r--   0 alan      (1000) alan      (1000)      218 2023-06-08 01:31:20.000000 bspcpy-1.0.3/bspcpy.egg-info/SOURCES.txt
--rw-r--r--   0 alan      (1000) alan      (1000)        1 2023-06-08 01:31:20.000000 bspcpy-1.0.3/bspcpy.egg-info/dependency_links.txt
--rw-r--r--   0 alan      (1000) alan      (1000)        5 2023-06-08 01:31:20.000000 bspcpy-1.0.3/bspcpy.egg-info/top_level.txt
--rw-r--r--   0 alan      (1000) alan      (1000)      442 2023-06-08 01:31:05.000000 bspcpy-1.0.3/pyproject.toml
--rw-r--r--   0 alan      (1000) alan      (1000)       79 2023-06-08 01:31:20.125227 bspcpy-1.0.3/setup.cfg
--rw-r--r--   0 alan      (1000) alan      (1000)      342 2023-03-04 03:09:52.000000 bspcpy-1.0.3/setup.py
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-06-08 01:34:50.948559 bspcpy-1.0.3.1/
+-rw-r--r--   0 alan      (1000) alan      (1000)     1067 2023-04-03 19:03:41.000000 bspcpy-1.0.3.1/LICENSE
+-rw-r--r--   0 alan      (1000) alan      (1000)     2961 2023-06-08 01:34:50.948559 bspcpy-1.0.3.1/PKG-INFO
+-rw-r--r--   0 alan      (1000) alan      (1000)     1347 2023-03-04 03:19:34.000000 bspcpy-1.0.3.1/README.md
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-06-08 01:34:50.948559 bspcpy-1.0.3.1/bspc/
+-rw-r--r--   0 alan      (1000) alan      (1000)       93 2023-06-08 01:33:54.000000 bspcpy-1.0.3.1/bspc/__init__.py
+-rw-r--r--   0 alan      (1000) alan      (1000)    12757 2023-03-22 01:14:02.000000 bspcpy-1.0.3.1/bspc/classes.py
+-rw-r--r--   0 alan      (1000) alan      (1000)     2079 2023-03-22 01:08:33.000000 bspcpy-1.0.3.1/bspc/query.py
+drwxr-xr-x   0 alan      (1000) alan      (1000)        0 2023-06-08 01:34:50.948559 bspcpy-1.0.3.1/bspcpy.egg-info/
+-rw-r--r--   0 alan      (1000) alan      (1000)     2961 2023-06-08 01:34:50.000000 bspcpy-1.0.3.1/bspcpy.egg-info/PKG-INFO
+-rw-r--r--   0 alan      (1000) alan      (1000)      218 2023-06-08 01:34:50.000000 bspcpy-1.0.3.1/bspcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)        1 2023-06-08 01:34:50.000000 bspcpy-1.0.3.1/bspcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)        5 2023-06-08 01:34:50.000000 bspcpy-1.0.3.1/bspcpy.egg-info/top_level.txt
+-rw-r--r--   0 alan      (1000) alan      (1000)      444 2023-06-08 01:34:33.000000 bspcpy-1.0.3.1/pyproject.toml
+-rw-r--r--   0 alan      (1000) alan      (1000)       79 2023-06-08 01:34:50.948559 bspcpy-1.0.3.1/setup.cfg
+-rw-r--r--   0 alan      (1000) alan      (1000)      342 2023-03-04 03:09:52.000000 bspcpy-1.0.3.1/setup.py
```

### Comparing `bspcpy-1.0.3/LICENSE` & `bspcpy-1.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bspcpy-1.0.3/PKG-INFO` & `bspcpy-1.0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bspcpy
-Version: 1.0.3
+Version: 1.0.3.1
 Summary: bspc wrapper for python
 Home-page: https://github.com/AlanJs26/bspcpy
 Author: AlanJS26
 Author-email: AlanJS26 <alanjoses.29@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Alan José
```

### Comparing `bspcpy-1.0.3/README.md` & `bspcpy-1.0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bspcpy-1.0.3/bspc/classes.py` & `bspcpy-1.0.3.1/bspc/classes.py`

 * *Files identical despite different names*

### Comparing `bspcpy-1.0.3/bspc/query.py` & `bspcpy-1.0.3.1/bspc/query.py`

 * *Files identical despite different names*

### Comparing `bspcpy-1.0.3/bspcpy.egg-info/PKG-INFO` & `bspcpy-1.0.3.1/bspcpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bspcpy
-Version: 1.0.3
+Version: 1.0.3.1
 Summary: bspc wrapper for python
 Home-page: https://github.com/AlanJs26/bspcpy
 Author: AlanJS26
 Author-email: AlanJS26 <alanjoses.29@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Alan José
```

