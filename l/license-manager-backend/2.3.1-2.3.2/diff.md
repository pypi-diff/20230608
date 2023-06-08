# Comparing `tmp/license_manager_backend-2.3.1.tar.gz` & `tmp/license_manager_backend-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_backend-2.3.1.tar", max compression
+gzip compressed data, was "license_manager_backend-2.3.2.tar", max compression
```

## Comparing `license_manager_backend-2.3.1.tar` & `license_manager_backend-2.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       25 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/README.rst
--rw-r--r--   0        0        0       60 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/__init__.py
--rw-r--r--   0        0        0      453 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/api/__init__.py
--rw-r--r--   0        0        0     9062 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/api/booking.py
--rw-r--r--   0        0        0     7864 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/api/config.py
--rw-r--r--   0        0        0     9015 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/api/license.py
--rw-r--r--   0        0        0     3665 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/api_schemas.py
--rw-r--r--   0        0        0      464 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/compat.py
--rw-r--r--   0        0        0     1147 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/config.py
--rw-r--r--   0        0        0      914 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/constants.py
--rw-r--r--   0        0        0      209 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/exceptions.py
--rw-r--r--   0        0        0     1754 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/helpers.py
--rw-r--r--   0        0        0     2858 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/lm_backend/main.py
--rw-r--r--   0        0        0     1316 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/lm_backend/security.py
--rw-r--r--   0        0        0     1830 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/lm_backend/storage.py
--rw-r--r--   0        0        0     2541 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/lm_backend/table_schemas.py
--rw-r--r--   0        0        0     1099 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/lm_backend/version.py
--rw-r--r--   0        0        0     2011 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 license_manager_backend-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/README.rst
+-rw-r--r--   0        0        0       60 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/api/__init__.py
+-rw-r--r--   0        0        0     9062 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/api/booking.py
+-rw-r--r--   0        0        0     7864 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/api/config.py
+-rw-r--r--   0        0        0     9015 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/api/license.py
+-rw-r--r--   0        0        0     3665 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/api_schemas.py
+-rw-r--r--   0        0        0      464 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/compat.py
+-rw-r--r--   0        0        0     1147 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/config.py
+-rw-r--r--   0        0        0      914 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/constants.py
+-rw-r--r--   0        0        0      209 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/exceptions.py
+-rw-r--r--   0        0        0     1754 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/helpers.py
+-rw-r--r--   0        0        0     2858 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/main.py
+-rw-r--r--   0        0        0     1316 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/security.py
+-rw-r--r--   0        0        0     1830 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/storage.py
+-rw-r--r--   0        0        0     2541 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/table_schemas.py
+-rw-r--r--   0        0        0     1099 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/lm_backend/version.py
+-rw-r--r--   0        0        0     2011 2023-06-08 19:49:41.094053 license_manager_backend-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 license_manager_backend-2.3.2/PKG-INFO
```

### Comparing `license_manager_backend-2.3.1/lm_backend/api/booking.py` & `license_manager_backend-2.3.2/lm_backend/api/booking.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/api/config.py` & `license_manager_backend-2.3.2/lm_backend/api/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/api/license.py` & `license_manager_backend-2.3.2/lm_backend/api/license.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/api_schemas.py` & `license_manager_backend-2.3.2/lm_backend/api_schemas.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/config.py` & `license_manager_backend-2.3.2/lm_backend/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/constants.py` & `license_manager_backend-2.3.2/lm_backend/constants.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/helpers.py` & `license_manager_backend-2.3.2/lm_backend/helpers.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/main.py` & `license_manager_backend-2.3.2/lm_backend/main.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/security.py` & `license_manager_backend-2.3.2/lm_backend/security.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/storage.py` & `license_manager_backend-2.3.2/lm_backend/storage.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/table_schemas.py` & `license_manager_backend-2.3.2/lm_backend/table_schemas.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/lm_backend/version.py` & `license_manager_backend-2.3.2/lm_backend/version.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.1/pyproject.toml` & `license_manager_backend-2.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-backend"
-version = "2.3.1"
+version = "2.3.2"
 description = "Provides an API for managing license data"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_backend" }]
```

### Comparing `license_manager_backend-2.3.1/PKG-INFO` & `license_manager_backend-2.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-backend
-Version: 2.3.1
+Version: 2.3.2
 Summary: Provides an API for managing license data
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
```

