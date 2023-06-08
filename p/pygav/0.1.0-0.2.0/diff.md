# Comparing `tmp/pygav-0.1.0.tar.gz` & `tmp/pygav-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygav-0.1.0.tar", last modified: Wed Jun  7 16:17:28 2023, max compression
+gzip compressed data, was "pygav-0.2.0.tar", last modified: Thu Jun  8 12:26:51 2023, max compression
```

## Comparing `pygav-0.1.0.tar` & `pygav-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-07 16:17:28.645563 pygav-0.1.0/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      483 2022-06-04 21:24:31.000000 pygav-0.1.0/LICENSE
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1437 2023-06-07 16:17:28.641563 pygav-0.1.0/PKG-INFO
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      437 2023-06-07 10:34:10.000000 pygav-0.1.0/README.md
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-07 16:17:28.641563 pygav-0.1.0/pygav/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        0 2022-06-04 19:41:44.000000 pygav-0.1.0/pygav/__init__.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1406 2023-06-07 16:15:36.000000 pygav-0.1.0/pygav/data.py
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      715 2023-06-07 10:49:39.000000 pygav-0.1.0/pygav/utils.py
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-07 16:17:28.641563 pygav-0.1.0/pygav.egg-info/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)     1437 2023-06-07 16:17:28.000000 pygav-0.1.0/pygav.egg-info/PKG-INFO
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      243 2023-06-07 16:17:28.000000 pygav-0.1.0/pygav.egg-info/SOURCES.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        1 2023-06-07 16:17:28.000000 pygav-0.1.0/pygav.egg-info/dependency_links.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)       82 2023-06-07 16:17:28.000000 pygav-0.1.0/pygav.egg-info/requires.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)        6 2023-06-07 16:17:28.000000 pygav-0.1.0/pygav.egg-info/top_level.txt
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      788 2023-06-07 16:16:18.000000 pygav-0.1.0/pyproject.toml
--rw-rw-r--   0 ngav      (1000) ngav      (1000)       38 2023-06-07 16:17:28.645563 pygav-0.1.0/setup.cfg
-drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-07 16:17:28.641563 pygav-0.1.0/tests/
--rw-rw-r--   0 ngav      (1000) ngav      (1000)      258 2023-06-07 10:51:03.000000 pygav-0.1.0/tests/test_utils.py
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-08 12:26:51.772113 pygav-0.2.0/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      483 2022-06-04 21:24:31.000000 pygav-0.2.0/LICENSE
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1415 2023-06-08 12:26:51.772113 pygav-0.2.0/PKG-INFO
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      447 2023-06-08 12:23:02.000000 pygav-0.2.0/README.md
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-08 12:26:51.772113 pygav-0.2.0/pygav/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        0 2022-06-04 19:41:44.000000 pygav-0.2.0/pygav/__init__.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     4679 2023-06-08 12:21:25.000000 pygav-0.2.0/pygav/data.py
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      715 2023-06-07 10:49:39.000000 pygav-0.2.0/pygav/utils.py
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-08 12:26:51.772113 pygav-0.2.0/pygav.egg-info/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)     1415 2023-06-08 12:26:51.000000 pygav-0.2.0/pygav.egg-info/PKG-INFO
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      243 2023-06-08 12:26:51.000000 pygav-0.2.0/pygav.egg-info/SOURCES.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        1 2023-06-08 12:26:51.000000 pygav-0.2.0/pygav.egg-info/dependency_links.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)       82 2023-06-08 12:26:51.000000 pygav-0.2.0/pygav.egg-info/requires.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)        6 2023-06-08 12:26:51.000000 pygav-0.2.0/pygav.egg-info/top_level.txt
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      753 2023-06-08 11:48:59.000000 pygav-0.2.0/pyproject.toml
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)       38 2023-06-08 12:26:51.772113 pygav-0.2.0/setup.cfg
+drwxrwxr-x   0 ngav      (1000) ngav      (1000)        0 2023-06-08 12:26:51.772113 pygav-0.2.0/tests/
+-rw-rw-r--   0 ngav      (1000) ngav      (1000)      258 2023-06-07 10:51:03.000000 pygav-0.2.0/tests/test_utils.py
```

### Comparing `pygav-0.1.0/PKG-INFO` & `pygav-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pygav
-Version: 0.1.0
+Version: 0.2.0
 Summary: Useful stuff
-Author-email: Nikos Gavalas <ngavalas@protonmail.com>
+Author: Nikos Gavalas
 License:             DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                             Version 2, December 2004
         
          Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>
         
          Everyone is permitted to copy and distribute verbatim or modified
          copies of this license document, and changing it is allowed as long
@@ -24,18 +24,18 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![tests status](https://github.com/nikosgavalas/pygav/actions/workflows/main.yml/badge.svg)
 
-Some random python stuff I find useful
+Some random python stuff I find useful.
 
 To run tests: Install `pytest` and run `pytest`.
 
-How to publish this package (notes to my future self):
+<!-- How to publish this package (notes to my future self):
 1. make sure you have `build` and `twine` installed
 2. `python -m build`
 3. `twine check dist/*`
 4. `twine upload -r testpypi dist/*`
 5. check everything is fine on testpypi
-6. `twine upload dist/*`
+6. `twine upload dist/*` -->
```

### Comparing `pygav-0.1.0/pygav/utils.py` & `pygav-0.2.0/pygav/utils.py`

 * *Files identical despite different names*

### Comparing `pygav-0.1.0/pygav.egg-info/PKG-INFO` & `pygav-0.2.0/pygav.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pygav
-Version: 0.1.0
+Version: 0.2.0
 Summary: Useful stuff
-Author-email: Nikos Gavalas <ngavalas@protonmail.com>
+Author: Nikos Gavalas
 License:             DO WHAT THE FUCK YOU WANT TO PUBLIC LICENSE
                             Version 2, December 2004
         
          Copyright (C) 2004 Sam Hocevar <sam@hocevar.net>
         
          Everyone is permitted to copy and distribute verbatim or modified
          copies of this license document, and changing it is allowed as long
@@ -24,18 +24,18 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![tests status](https://github.com/nikosgavalas/pygav/actions/workflows/main.yml/badge.svg)
 
-Some random python stuff I find useful
+Some random python stuff I find useful.
 
 To run tests: Install `pytest` and run `pytest`.
 
-How to publish this package (notes to my future self):
+<!-- How to publish this package (notes to my future self):
 1. make sure you have `build` and `twine` installed
 2. `python -m build`
 3. `twine check dist/*`
 4. `twine upload -r testpypi dist/*`
 5. check everything is fine on testpypi
-6. `twine upload dist/*`
+6. `twine upload dist/*` -->
```

### Comparing `pygav-0.1.0/pyproject.toml` & `pygav-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygav"
-version = "0.1.0"
+version = "0.2.0"
 description = "Useful stuff"
 readme = "README.md"
-authors = [{ name = "Nikos Gavalas", email = "ngavalas@protonmail.com" }]
+authors = [{ name = "Nikos Gavalas" }]
 license = { file = "LICENSE" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
 ]
 keywords = ["utilities"]
 dependencies = [
```

