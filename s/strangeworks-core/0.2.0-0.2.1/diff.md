# Comparing `tmp/strangeworks_core-0.2.0.tar.gz` & `tmp/strangeworks_core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_core-0.2.0.tar", max compression
+gzip compressed data, was "strangeworks_core-0.2.1.tar", max compression
```

## Comparing `strangeworks_core-0.2.0.tar` & `strangeworks_core-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,28 @@
--rw-r--r--   0        0        0      655 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/README.md
--rw-r--r--   0        0        0      875 2023-05-15 19:35:59.137470 strangeworks_core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      109 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/__init__.py
--rw-r--r--   0        0        0       19 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/config/__init__.py
--rw-r--r--   0        0        0      647 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/config/base.py
--rw-r--r--   0        0        0     3340 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/config/config.py
--rw-r--r--   0        0        0      874 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/config/defaults.py
--rw-r--r--   0        0        0     1846 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/config/env.py
--rw-r--r--   0        0        0     6262 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/config/file.py
--rw-r--r--   0        0        0       19 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/errors/__init__.py
--rw-r--r--   0        0        0     2613 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/errors/error.py
--rw-r--r--   0        0        0       19 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/platform/__init__.py
--rw-r--r--   0        0        0     2457 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/platform/auth.py
--rw-r--r--   0        0        0     4842 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/platform/gql.py
--rw-r--r--   0        0        0    10844 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/platform/rest_client.py
--rw-r--r--   0        0        0     3275 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/platform/transport.py
--rw-r--r--   0        0        0       19 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/types/__init__.py
--rw-r--r--   0        0        0     3572 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/types/backend.py
--rw-r--r--   0        0        0     2024 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/types/file.py
--rw-r--r--   0        0        0     5748 2023-05-15 19:35:40.357252 strangeworks_core-0.2.0/strangeworks_core/types/job.py
--rw-r--r--   0        0        0     1088 2023-05-15 19:35:40.361252 strangeworks_core-0.2.0/strangeworks_core/types/product.py
--rw-r--r--   0        0        0     2732 2023-05-15 19:35:40.361252 strangeworks_core-0.2.0/strangeworks_core/types/resource.py
--rw-r--r--   0        0        0      553 2023-05-15 19:35:40.361252 strangeworks_core-0.2.0/strangeworks_core/utils.py
--rw-r--r--   0        0        0     1383 1970-01-01 00:00:00.000000 strangeworks_core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      655 2023-06-08 19:51:40.847974 strangeworks_core-0.2.1/README.md
+-rw-r--r--   0        0        0      891 2023-06-08 19:51:57.848067 strangeworks_core-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/__init__.py
+-rw-r--r--   0        0        0       19 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/batch/__init__.py
+-rw-r--r--   0        0        0    12246 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/batch/utils.py
+-rw-r--r--   0        0        0       19 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/__init__.py
+-rw-r--r--   0        0        0      647 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/base.py
+-rw-r--r--   0        0        0     3340 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/config.py
+-rw-r--r--   0        0        0      874 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/defaults.py
+-rw-r--r--   0        0        0     1846 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/env.py
+-rw-r--r--   0        0        0     6262 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/config/file.py
+-rw-r--r--   0        0        0       19 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/errors/__init__.py
+-rw-r--r--   0        0        0     2613 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/errors/error.py
+-rw-r--r--   0        0        0       19 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/platform/__init__.py
+-rw-r--r--   0        0        0     2457 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/platform/auth.py
+-rw-r--r--   0        0        0     4880 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/platform/gql.py
+-rw-r--r--   0        0        0    10844 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/platform/rest_client.py
+-rw-r--r--   0        0        0     3275 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/platform/transport.py
+-rw-r--r--   0        0        0       19 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/__init__.py
+-rw-r--r--   0        0        0     3572 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/backend.py
+-rw-r--r--   0        0        0     2024 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/file.py
+-rw-r--r--   0        0        0      647 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/func.py
+-rw-r--r--   0        0        0     5748 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/job.py
+-rw-r--r--   0        0        0      760 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/machine.py
+-rw-r--r--   0        0        0     1088 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/product.py
+-rw-r--r--   0        0        0     2732 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/types/resource.py
+-rw-r--r--   0        0        0      553 2023-06-08 19:51:40.851974 strangeworks_core-0.2.1/strangeworks_core/utils.py
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 strangeworks_core-0.2.1/PKG-INFO
```

### Comparing `strangeworks_core-0.2.0/README.md` & `strangeworks_core-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/pyproject.toml` & `strangeworks_core-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 
 name = "strangeworks-core"
-version = "0.2.0"
+version = "0.2.1"
 
 description = "Strangeworks Core provides the infrastructure to interact with the platform."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_core"}]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.2"
 tomlkit = "^0.11.6"
 gql = "^3.4.0"
 requests-toolbelt = "^1.0.0"
+dill = "^0.3.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 pytest-cov = "^4.0.0"
```

### Comparing `strangeworks_core-0.2.0/strangeworks_core/config/base.py` & `strangeworks_core-0.2.1/strangeworks_core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/config/config.py` & `strangeworks_core-0.2.1/strangeworks_core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/config/defaults.py` & `strangeworks_core-0.2.1/strangeworks_core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/config/env.py` & `strangeworks_core-0.2.1/strangeworks_core/config/env.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/config/file.py` & `strangeworks_core-0.2.1/strangeworks_core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/errors/error.py` & `strangeworks_core-0.2.1/strangeworks_core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/platform/auth.py` & `strangeworks_core-0.2.1/strangeworks_core/platform/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/platform/gql.py` & `strangeworks_core-0.2.1/strangeworks_core/platform/gql.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
                 ),
                 auth_token=auth_token,
                 headers=headers,
                 retries=retries,
                 timeout=timeout,
             )
         )
+        self.info: APIInfo = api_type
 
     def execute(self, op: Operation, **kvargs):
         """Execute an operation on the platform.
 
         Parameters
         ----------
         op: Operation
```

### Comparing `strangeworks_core-0.2.0/strangeworks_core/platform/rest_client.py` & `strangeworks_core-0.2.1/strangeworks_core/platform/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/platform/transport.py` & `strangeworks_core-0.2.1/strangeworks_core/platform/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/types/backend.py` & `strangeworks_core-0.2.1/strangeworks_core/types/backend.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/types/file.py` & `strangeworks_core-0.2.1/strangeworks_core/types/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/types/job.py` & `strangeworks_core-0.2.1/strangeworks_core/types/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/types/product.py` & `strangeworks_core-0.2.1/strangeworks_core/types/product.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/types/resource.py` & `strangeworks_core-0.2.1/strangeworks_core/types/resource.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/strangeworks_core/utils.py` & `strangeworks_core-0.2.1/strangeworks_core/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.0/PKG-INFO` & `strangeworks_core-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: strangeworks-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: Strangeworks Core provides the infrastructure to interact with the platform.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: tomlkit (>=0.11.6,<0.12.0)
 Description-Content-Type: text/markdown
 
 # Strangeworks Python Core Library
```

