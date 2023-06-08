# Comparing `tmp/curlify2-1.0.1.tar.gz` & `tmp/curlify2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curlify2-1.0.1.tar", max compression
+gzip compressed data, was "curlify2-1.0.2.tar", max compression
```

## Comparing `curlify2-1.0.1.tar` & `curlify2-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1175 2021-07-21 00:09:52.941808 curlify2-1.0.1/README.md
--rw-r--r--   0        0        0       52 2021-07-21 00:09:52.942003 curlify2-1.0.1/curlify2/__init__.py
--rw-r--r--   0        0        0      629 2021-07-21 00:09:52.942156 curlify2-1.0.1/curlify2/curlify.py
--rw-r--r--   0        0        0      697 2021-07-21 00:09:52.943032 curlify2-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1951 2021-07-21 00:11:29.524562 curlify2-1.0.1/setup.py
--rw-r--r--   0        0        0     1951 2021-07-21 00:11:29.524699 curlify2-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-07 13:17:59.078986 curlify2-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1175 2023-06-07 13:17:59.079166 curlify2-1.0.2/README.md
+-rw-r--r--   0        0        0       52 2023-06-07 13:17:59.079287 curlify2-1.0.2/curlify2/__init__.py
+-rw-r--r--   0        0        0      629 2023-06-07 13:17:59.079375 curlify2-1.0.2/curlify2/curlify.py
+-rw-r--r--   0        0        0      695 2023-06-08 02:47:47.781210 curlify2-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2051 1970-01-01 00:00:00.000000 curlify2-1.0.2/PKG-INFO
```

### Comparing `curlify2-1.0.1/README.md` & `curlify2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `curlify2-1.0.1/curlify2/curlify.py` & `curlify2-1.0.2/curlify2/curlify.py`

 * *Files identical despite different names*

### Comparing `curlify2-1.0.1/pyproject.toml` & `curlify2-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "curlify2"
-version = "1.0.1"
+version = "1.0.2"
 description = "Library to convert python requests and httpx object to curl command."
 authors = ["Marcus Pereira <marcus@negros.dev>"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/marcuxyz/curlify2"
 homepage = "https://github.com/marcuxyz/curlify2"
 keywords = ["python", "curl", "requests", "curlify", "httpx", "convert to curl"]
 
 [tool.poetry.dependencies]
-python = ">=3.6.2,<4.0"
+python = ">=3.7,<4.0"
 requests = "^2.24.0"
 responses = "^0.12.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.1.2"
 responses = "^0.12.0"
 black = ">=21.7b0"
-pytest-httpx = "^0.10.0"
+pytest-httpx = "^0.22.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `curlify2-1.0.1/PKG-INFO` & `curlify2-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: curlify2
-Version: 1.0.1
+Version: 1.0.2
 Summary: Library to convert python requests and httpx object to curl command.
 Home-page: https://github.com/marcuxyz/curlify2
 License: MIT
 Keywords: python,curl,requests,curlify,httpx,convert to curl
 Author: Marcus Pereira
 Author-email: marcus@negros.dev
-Requires-Python: >=3.6.2,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: responses (>=0.12.0,<0.13.0)
 Project-URL: Repository, https://github.com/marcuxyz/curlify2
 Description-Content-Type: text/markdown
 
 The library convert python 'requests' and 'httpx' object in curl command. Curlify2 is a enhancement of [curlify]('https://github.com/ofw/curlify').
```

