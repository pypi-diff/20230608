# Comparing `tmp/formal-sdk-0.2.0.tar.gz` & `tmp/formal-sdk-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formal-sdk-0.2.0.tar", last modified: Thu Jun  8 13:44:59 2023, max compression
+gzip compressed data, was "formal-sdk-0.4.0.tar", last modified: Thu Jun  8 13:45:15 2023, max compression
```

## Comparing `formal-sdk-0.2.0.tar` & `formal-sdk-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:59.913540 formal-sdk-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 13:44:42.000000 formal-sdk-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 13:44:42.000000 formal-sdk-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-08 13:44:59.909540 formal-sdk-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-08 13:44:42.000000 formal-sdk-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 13:44:42.000000 formal-sdk-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:44:59.913540 formal-sdk-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:59.909540 formal-sdk-0.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-08 13:44:42.000000 formal-sdk-0.2.0/src/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:59.909540 formal-sdk-0.2.0/src/formal_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:42.000000 formal-sdk-0.2.0/src/formal_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 13:44:42.000000 formal-sdk-0.2.0/src/formal_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-08 13:44:42.000000 formal-sdk-0.2.0/src/formal_sdk/datastore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:59.909540 formal-sdk-0.2.0/src/formal_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-08 13:44:59.000000 formal-sdk-0.2.0/src/formal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 13:44:59.000000 formal-sdk-0.2.0/src/formal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:44:59.000000 formal-sdk-0.2.0/src/formal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 13:44:59.000000 formal-sdk-0.2.0/src/formal_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 13:44:59.000000 formal-sdk-0.2.0/src/formal_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:45:15.558930 formal-sdk-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 13:44:56.000000 formal-sdk-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 13:44:56.000000 formal-sdk-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-08 13:45:15.558930 formal-sdk-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-08 13:44:56.000000 formal-sdk-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 13:44:56.000000 formal-sdk-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:45:15.558930 formal-sdk-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:45:15.558930 formal-sdk-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-08 13:44:56.000000 formal-sdk-0.4.0/src/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:45:15.558930 formal-sdk-0.4.0/src/formal_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:44:56.000000 formal-sdk-0.4.0/src/formal_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 13:44:56.000000 formal-sdk-0.4.0/src/formal_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-08 13:44:56.000000 formal-sdk-0.4.0/src/formal_sdk/datastore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:45:15.558930 formal-sdk-0.4.0/src/formal_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-08 13:45:15.000000 formal-sdk-0.4.0/src/formal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 13:45:15.000000 formal-sdk-0.4.0/src/formal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:45:15.000000 formal-sdk-0.4.0/src/formal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 13:45:15.000000 formal-sdk-0.4.0/src/formal_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 13:45:15.000000 formal-sdk-0.4.0/src/formal_sdk.egg-info/top_level.txt
```

### Comparing `formal-sdk-0.2.0/LICENSE` & `formal-sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formal-sdk-0.2.0/PKG-INFO` & `formal-sdk-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 0.2.0
+Version: 0.4.0
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `formal-sdk-0.2.0/README.md` & `formal-sdk-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `formal-sdk-0.2.0/pyproject.toml` & `formal-sdk-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "formal-sdk"
-version = "0.2.0"
+version = "0.4.0"
 authors = [
   { name="Formal", email="hello@joinformal.com" },
 ]
 description = "Formal SDK"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `formal-sdk-0.2.0/src/example.py` & `formal-sdk-0.4.0/src/example.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-0.2.0/src/formal_sdk/datastore.py` & `formal-sdk-0.4.0/src/formal_sdk/datastore.py`

 * *Files identical despite different names*

### Comparing `formal-sdk-0.2.0/src/formal_sdk.egg-info/PKG-INFO` & `formal-sdk-0.4.0/src/formal_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 0.2.0
+Version: 0.4.0
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

