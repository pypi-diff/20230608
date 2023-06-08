# Comparing `tmp/amass-0.3.0.tar.gz` & `tmp/amass-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amass-0.3.0.tar", max compression
+gzip compressed data, was "amass-0.3.1.tar", max compression
```

## Comparing `amass-0.3.0.tar` & `amass-0.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11342 2023-06-08 17:41:01.246189 amass-0.3.0/LICENSE
--rw-r--r--   0        0        0       36 2023-06-08 17:41:01.246189 amass-0.3.0/README.md
--rw-r--r--   0        0        0    13684 2023-06-08 17:41:01.246189 amass-0.3.0/amass/__init__.py
--rw-r--r--   0        0        0     2752 2023-06-08 17:41:01.246189 amass-0.3.0/amass/cli.py
--rw-r--r--   0        0        0     1634 2023-06-08 17:41:01.246189 amass-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      900 1970-01-01 00:00:00.000000 amass-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-06-08 17:43:11.891934 amass-0.3.1/LICENSE
+-rw-r--r--   0        0        0       36 2023-06-08 17:43:11.891934 amass-0.3.1/README.md
+-rw-r--r--   0        0        0    13684 2023-06-08 17:43:11.891934 amass-0.3.1/amass/__init__.py
+-rw-r--r--   0        0        0     2752 2023-06-08 17:43:11.891934 amass-0.3.1/amass/cli.py
+-rw-r--r--   0        0        0     1628 2023-06-08 17:43:11.891934 amass-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      882 1970-01-01 00:00:00.000000 amass-0.3.1/PKG-INFO
```

### Comparing `amass-0.3.0/LICENSE` & `amass-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `amass-0.3.0/amass/__init__.py` & `amass-0.3.1/amass/__init__.py`

 * *Files identical despite different names*

### Comparing `amass-0.3.0/amass/cli.py` & `amass-0.3.1/amass/cli.py`

 * *Files identical despite different names*

### Comparing `amass-0.3.0/pyproject.toml` & `amass-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amass"
-version = "0.3.0"
+version = "0.3.1"
 description = "Vendor libraries from cdnjs"
 authors = ["James Meakin <amass@jmsmkn.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/jmsmkn/amass"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -16,15 +16,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 click = "*"
 aiohttp = "*"
 packaging = "*"
 tomlkit = "*"
-beautifulsoup4 = "^4.12.2"
+beautifulsoup4 = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-randomly = "*"
 pytest-cov = "*"
 pytest-asyncio = "*"
```

### Comparing `amass-0.3.0/PKG-INFO` & `amass-0.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amass
-Version: 0.3.0
+Version: 0.3.1
 Summary: Vendor libraries from cdnjs
 Home-page: https://github.com/jmsmkn/amass
 License: Apache-2.0
 Author: James Meakin
 Author-email: amass@jmsmkn.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 3 - Alpha
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: beautifulsoup4
 Requires-Dist: click
 Requires-Dist: packaging
 Requires-Dist: tomlkit
 Project-URL: Repository, https://github.com/jmsmkn/amass
 Description-Content-Type: text/markdown
 
 # amass
```

