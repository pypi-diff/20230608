# Comparing `tmp/watchmen_cli-16.5.7.tar.gz` & `tmp/watchmen_cli-16.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_cli-16.5.7.tar", max compression
+gzip compressed data, was "watchmen_cli-16.5.8.tar", max compression
```

## Comparing `watchmen_cli-16.5.7.tar` & `watchmen_cli-16.5.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      540 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/pyproject.toml
--rw-r--r--   0        0        0        1 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/src/watchmen_cli/__init__.py
--rw-r--r--   0        0        0        1 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/src/watchmen_cli/common/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/src/watchmen_cli/common/client.py
--rw-r--r--   0        0        0      546 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/src/watchmen_cli/common/constants.py
--rw-r--r--   0        0        0      173 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/src/watchmen_cli/common/exception.py
--rw-r--r--   0        0        0     2005 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/src/watchmen_cli/main.py
--rw-r--r--   0        0        0       35 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/src/watchmen_cli/service/__init__.py
--rw-r--r--   0        0        0     2862 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/src/watchmen_cli/service/deployment.py
--rw-r--r--   0        0        0     2502 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/src/watchmen_cli/service/rerun.py
--rw-r--r--   0        0        0      581 2023-06-07 11:34:15.603986 watchmen_cli-16.5.7/src/watchmen_cli/settings.py
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 watchmen_cli-16.5.7/PKG-INFO
+-rw-r--r--   0        0        0      540 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/src/watchmen_cli/__init__.py
+-rw-r--r--   0        0        0        1 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/src/watchmen_cli/common/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/src/watchmen_cli/common/client.py
+-rw-r--r--   0        0        0      546 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/src/watchmen_cli/common/constants.py
+-rw-r--r--   0        0        0      173 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/src/watchmen_cli/common/exception.py
+-rw-r--r--   0        0        0     2005 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/src/watchmen_cli/main.py
+-rw-r--r--   0        0        0       35 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/src/watchmen_cli/service/__init__.py
+-rw-r--r--   0        0        0     2862 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/src/watchmen_cli/service/deployment.py
+-rw-r--r--   0        0        0     2502 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/src/watchmen_cli/service/rerun.py
+-rw-r--r--   0        0        0      581 2023-06-08 03:33:39.183630 watchmen_cli-16.5.8/src/watchmen_cli/settings.py
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 watchmen_cli-16.5.8/PKG-INFO
```

### Comparing `watchmen_cli-16.5.7/pyproject.toml` & `watchmen_cli-16.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "watchmen-cli"
-version = "16.5.7"
+version = "16.5.8"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_cli", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 fire = "^0.4.0"
 requests = "^2.27.1"
-watchmen-utilities = "16.5.7"
+watchmen-utilities = "16.5.8"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `watchmen_cli-16.5.7/src/watchmen_cli/common/client.py` & `watchmen_cli-16.5.8/src/watchmen_cli/common/client.py`

 * *Files identical despite different names*

### Comparing `watchmen_cli-16.5.7/src/watchmen_cli/common/constants.py` & `watchmen_cli-16.5.8/src/watchmen_cli/common/constants.py`

 * *Files identical despite different names*

### Comparing `watchmen_cli-16.5.7/src/watchmen_cli/main.py` & `watchmen_cli-16.5.8/src/watchmen_cli/main.py`

 * *Files identical despite different names*

### Comparing `watchmen_cli-16.5.7/src/watchmen_cli/service/deployment.py` & `watchmen_cli-16.5.8/src/watchmen_cli/service/deployment.py`

 * *Files identical despite different names*

### Comparing `watchmen_cli-16.5.7/src/watchmen_cli/service/rerun.py` & `watchmen_cli-16.5.8/src/watchmen_cli/service/rerun.py`

 * *Files identical despite different names*

### Comparing `watchmen_cli-16.5.7/src/watchmen_cli/settings.py` & `watchmen_cli-16.5.8/src/watchmen_cli/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_cli-16.5.7/PKG-INFO` & `watchmen_cli-16.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-cli
-Version: 16.5.7
+Version: 16.5.8
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fire (>=0.4.0,<0.5.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: watchmen-utilities (==16.5.7)
+Requires-Dist: watchmen-utilities (==16.5.8)
```

