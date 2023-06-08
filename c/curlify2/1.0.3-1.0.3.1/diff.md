# Comparing `tmp/curlify2-1.0.3.tar.gz` & `tmp/curlify2-1.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curlify2-1.0.3.tar", max compression
+gzip compressed data, was "curlify2-1.0.3.1.tar", max compression
```

## Comparing `curlify2-1.0.3.tar` & `curlify2-1.0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-06-07 13:17:59.078986 curlify2-1.0.3/LICENSE
--rw-r--r--   0        0        0     1175 2023-06-07 13:17:59.079166 curlify2-1.0.3/README.md
--rw-r--r--   0        0        0       52 2023-06-07 13:17:59.079287 curlify2-1.0.3/curlify2/__init__.py
--rw-r--r--   0        0        0      629 2023-06-07 13:17:59.079375 curlify2-1.0.3/curlify2/curlify.py
--rw-r--r--   0        0        0      695 2023-06-08 03:00:51.963510 curlify2-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2051 1970-01-01 00:00:00.000000 curlify2-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-07 13:17:59.078986 curlify2-1.0.3.1/LICENSE
+-rw-r--r--   0        0        0     1175 2023-06-07 13:17:59.079166 curlify2-1.0.3.1/README.md
+-rw-r--r--   0        0        0       52 2023-06-07 13:17:59.079287 curlify2-1.0.3.1/curlify2/__init__.py
+-rw-r--r--   0        0        0      629 2023-06-07 13:17:59.079375 curlify2-1.0.3.1/curlify2/curlify.py
+-rw-r--r--   0        0        0      681 2023-06-08 03:02:38.687418 curlify2-1.0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 curlify2-1.0.3.1/PKG-INFO
```

### Comparing `curlify2-1.0.3/LICENSE` & `curlify2-1.0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `curlify2-1.0.3/README.md` & `curlify2-1.0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `curlify2-1.0.3/curlify2/curlify.py` & `curlify2-1.0.3.1/curlify2/curlify.py`

 * *Files identical despite different names*

### Comparing `curlify2-1.0.3/PKG-INFO` & `curlify2-1.0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 Metadata-Version: 2.1
 Name: curlify2
-Version: 1.0.3
+Version: 1.0.3.1
 Summary: Library to convert python requests and httpx object to curl command.
 Home-page: https://github.com/marcuxyz/curlify2
 License: MIT
 Keywords: python,curl,requests,curlify,httpx,convert to curl
 Author: Marcus Pereira
 Author-email: marcus@negros.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.24.0,<3.0.0)
-Requires-Dist: responses (>=0.12.0,<0.13.0)
 Project-URL: Repository, https://github.com/marcuxyz/curlify2
 Description-Content-Type: text/markdown
 
 The library convert python 'requests' and 'httpx' object in curl command. Curlify2 is a enhancement of [curlify]('https://github.com/ofw/curlify').
 
 
 ## Installation
```

