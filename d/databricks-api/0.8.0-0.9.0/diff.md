# Comparing `tmp/databricks_api-0.8.0.tar.gz` & `tmp/databricks_api-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_api-0.8.0.tar", max compression
+gzip compressed data, was "databricks_api-0.9.0.tar", max compression
```

## Comparing `databricks_api-0.8.0.tar` & `databricks_api-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1063 2022-06-17 21:39:43.454838 databricks_api-0.8.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1078 2020-04-01 23:43:56.044447 databricks_api-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0    15981 2022-06-17 21:37:01.739631 databricks_api-0.8.0/README.rst
--rw-r--r--   0        0        0      162 2022-06-17 21:24:03.758405 databricks_api-0.8.0/databricks_api/__init__.py
--rw-r--r--   0        0        0      915 2020-11-17 15:39:55.095252 databricks_api-0.8.0/databricks_api/_stubs.py
--rw-r--r--   0        0        0       49 2022-06-17 21:39:43.455157 databricks_api-0.8.0/databricks_api/_version.py
--rw-r--r--   0        0        0      880 2022-06-17 21:39:43.455459 databricks_api-0.8.0/databricks_api/databricks.py
--rw-r--r--   0        0        0      710 2022-06-17 21:32:47.130219 databricks_api-0.8.0/databricks_api/databricks.pyi
--rw-r--r--   0        0        0     1480 2022-06-17 21:39:43.455753 databricks_api-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    17508 2022-06-17 21:39:59.126903 databricks_api-0.8.0/setup.py
--rw-r--r--   0        0        0    17055 2022-06-17 21:39:59.127737 databricks_api-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1126 2023-06-08 16:35:35.222483 databricks_api-0.9.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1078 2020-04-01 23:43:56.044447 databricks_api-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0    16181 2023-06-08 16:35:00.168877 databricks_api-0.9.0/README.rst
+-rw-r--r--   0        0        0      162 2022-06-17 21:24:03.758405 databricks_api-0.9.0/databricks_api/__init__.py
+-rw-r--r--   0        0        0      915 2020-11-17 15:39:55.095252 databricks_api-0.9.0/databricks_api/_stubs.py
+-rw-r--r--   0        0        0       49 2023-06-08 16:35:10.766616 databricks_api-0.9.0/databricks_api/_version.py
+-rw-r--r--   0        0        0     1337 2023-06-08 16:35:00.169696 databricks_api-0.9.0/databricks_api/databricks.py
+-rw-r--r--   0        0        0      710 2022-06-17 21:32:47.130219 databricks_api-0.9.0/databricks_api/databricks.pyi
+-rw-r--r--   0        0        0     1480 2023-06-08 16:35:06.143448 databricks_api-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    17306 1970-01-01 00:00:00.000000 databricks_api-0.9.0/PKG-INFO
```

### Comparing `databricks_api-0.8.0/CHANGELOG.rst` & `databricks_api-0.9.0/CHANGELOG.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 Changelog
 ---------
+0.9.0: 2023-06-08
+~~~~~~~~~~~~~~~~~
+
+* add deprecation warning
 
 0.8.0: 2022-06-17
 ~~~~~~~~~~~~~~~~~
 
 * free the dependency constraint on ``databricks-cli``
 * remove clutter from ``__version__`` module
 * add ``__cli_version__`` variable referencing the ``databricks-cli`` version
```

### Comparing `databricks_api-0.8.0/LICENSE.txt` & `databricks_api-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databricks_api-0.8.0/README.rst` & `databricks_api-0.9.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 databricks-api
 ==============
 
+**Please switch to the official Databricks SDK for Python (https://github.com/databricks/databricks-sdk-py) by running the following command:**
+
+.. code-block:: bash
+
+    pip install databricks-sdk
+
+
 |pypi| |pyversions|
 
 .. |pypi| image:: https://img.shields.io/pypi/v/databricks-api.svg
     :target: https://pypi.python.org/pypi/databricks-api
 
 .. |pyversions| image:: https://img.shields.io/pypi/pyversions/databricks-api.svg
     :target: https://pypi.python.org/pypi/databricks-api
```

### Comparing `databricks_api-0.8.0/databricks_api/_stubs.py` & `databricks_api-0.9.0/databricks_api/_stubs.py`

 * *Files identical despite different names*

### Comparing `databricks_api-0.8.0/databricks_api/databricks.py` & `databricks_api-0.9.0/databricks_api/databricks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 
+import warnings
 import databricks_cli.sdk.service as services
 from databricks_cli.sdk import ApiClient
 
 __all__ = ["DatabricksAPI"]
 
 
 def camel_to_snake(name):
@@ -16,14 +17,24 @@
         if "Service" in service_name:
             camel_name = camel_to_snake(service_name.replace("Service", ""))
             yield service_name, camel_name, service
 
 
 class DatabricksAPI:
     def __init__(self, **kwargs):
+        warnings.warn(
+            """
+        ==================================================================
+        Please switch to the official Databricks SDK for Python by running
+        `pip install databricks-sdk`. See more information and sources at
+        https://github.com/databricks/databricks-sdk-py
+        ==================================================================""",
+            DeprecationWarning,
+        )
+
         if "host" in kwargs:
             if not kwargs["host"].startswith("https://"):
                 kwargs["host"] = "https://" + kwargs["host"]
 
         self.client = ApiClient(**kwargs)
 
         for _, camel_name, service in _get_services():
```

### Comparing `databricks_api-0.8.0/databricks_api/databricks.pyi` & `databricks_api-0.9.0/databricks_api/databricks.pyi`

 * *Files identical despite different names*

### Comparing `databricks_api-0.8.0/pyproject.toml` & `databricks_api-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     | dist
   )/
 )
 '''
 
 [tool.poetry]
 name = "databricks_api"
-version = "0.8.0"
+version = "0.9.0"
 description = "Databricks API client auto-generated from the official databricks-cli package"
 authors = ["Christopher Flynn <crf204@gmail.com>"]
 readme = "README.rst"
 license = "MIT"
 repository = "https://github.com/crflynn/databricks-api"
 homepage = "https://github.com/crflynn/databricks-api"
 packages = [
```

### Comparing `databricks_api-0.8.0/PKG-INFO` & `databricks_api-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 Metadata-Version: 2.1
 Name: databricks-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: Databricks API client auto-generated from the official databricks-cli package
 Home-page: https://github.com/crflynn/databricks-api
 License: MIT
 Keywords: databricks,api,client
 Author: Christopher Flynn
 Author-email: crf204@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: databricks-cli
 Project-URL: Repository, https://github.com/crflynn/databricks-api
 Description-Content-Type: text/x-rst
 
 databricks-api
 ==============
 
+**Please switch to the official Databricks SDK for Python (https://github.com/databricks/databricks-sdk-py) by running the following command:**
+
+.. code-block:: bash
+
+    pip install databricks-sdk
+
+
 |pypi| |pyversions|
 
 .. |pypi| image:: https://img.shields.io/pypi/v/databricks-api.svg
     :target: https://pypi.python.org/pypi/databricks-api
 
 .. |pyversions| image:: https://img.shields.io/pypi/pyversions/databricks-api.svg
     :target: https://pypi.python.org/pypi/databricks-api
```

