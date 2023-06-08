# Comparing `tmp/license_manager_cli-2.3.1.tar.gz` & `tmp/license_manager_cli-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_cli-2.3.1.tar", max compression
+gzip compressed data, was "license_manager_cli-2.3.2.tar", max compression
```

## Comparing `license_manager_cli-2.3.1.tar` & `license_manager_cli-2.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1082 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/LICENSE
--rw-r--r--   0        0        0     7574 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/README.rst
--rw-r--r--   0        0        0        0 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/__init__.py
--rw-r--r--   0        0        0    10990 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/auth.py
--rw-r--r--   0        0        0     2937 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/config.py
--rw-r--r--   0        0        0      299 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/constants.py
--rw-r--r--   0        0        0     2569 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/exceptions.py
--rw-r--r--   0        0        0      675 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/logs.py
--rw-r--r--   0        0        0     5684 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/main.py
--rw-r--r--   0        0        0     4560 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/render.py
--rw-r--r--   0        0        0     7100 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/requests.py
--rw-r--r--   0        0        0     3716 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/schemas.py
--rw-r--r--   0        0        0        0 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/subapps/__init__.py
--rw-r--r--   0        0        0     1734 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/subapps/bookings.py
--rw-r--r--   0        0        0     5971 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/subapps/configurations.py
--rw-r--r--   0        0        0     1680 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/subapps/licenses.py
--rw-r--r--   0        0        0     1147 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/text_tools.py
--rw-r--r--   0        0        0     3516 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/lm_cli/time_loop.py
--rw-r--r--   0        0        0     1833 2023-05-22 18:46:08.656125 license_manager_cli-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     8868 1970-01-01 00:00:00.000000 license_manager_cli-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/LICENSE
+-rw-r--r--   0        0        0     7574 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/README.rst
+-rw-r--r--   0        0        0        0 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/__init__.py
+-rw-r--r--   0        0        0    10990 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/auth.py
+-rw-r--r--   0        0        0     2937 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/config.py
+-rw-r--r--   0        0        0      299 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/constants.py
+-rw-r--r--   0        0        0     2569 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/exceptions.py
+-rw-r--r--   0        0        0      675 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/logs.py
+-rw-r--r--   0        0        0     5684 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/main.py
+-rw-r--r--   0        0        0     4560 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/render.py
+-rw-r--r--   0        0        0     7100 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/requests.py
+-rw-r--r--   0        0        0     3716 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/schemas.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/subapps/__init__.py
+-rw-r--r--   0        0        0     1734 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/subapps/bookings.py
+-rw-r--r--   0        0        0     5971 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/subapps/configurations.py
+-rw-r--r--   0        0        0     1680 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/subapps/licenses.py
+-rw-r--r--   0        0        0     1147 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/text_tools.py
+-rw-r--r--   0        0        0     3516 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/lm_cli/time_loop.py
+-rw-r--r--   0        0        0     1833 2023-06-08 19:49:40.001621 license_manager_cli-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8868 1970-01-01 00:00:00.000000 license_manager_cli-2.3.2/PKG-INFO
```

### Comparing `license_manager_cli-2.3.1/LICENSE` & `license_manager_cli-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/README.rst` & `license_manager_cli-2.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/auth.py` & `license_manager_cli-2.3.2/lm_cli/auth.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/config.py` & `license_manager_cli-2.3.2/lm_cli/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/exceptions.py` & `license_manager_cli-2.3.2/lm_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/logs.py` & `license_manager_cli-2.3.2/lm_cli/logs.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/main.py` & `license_manager_cli-2.3.2/lm_cli/main.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/render.py` & `license_manager_cli-2.3.2/lm_cli/render.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/requests.py` & `license_manager_cli-2.3.2/lm_cli/requests.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/schemas.py` & `license_manager_cli-2.3.2/lm_cli/schemas.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/subapps/bookings.py` & `license_manager_cli-2.3.2/lm_cli/subapps/bookings.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/subapps/configurations.py` & `license_manager_cli-2.3.2/lm_cli/subapps/configurations.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/subapps/licenses.py` & `license_manager_cli-2.3.2/lm_cli/subapps/licenses.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/text_tools.py` & `license_manager_cli-2.3.2/lm_cli/text_tools.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/lm_cli/time_loop.py` & `license_manager_cli-2.3.2/lm_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `license_manager_cli-2.3.1/pyproject.toml` & `license_manager_cli-2.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-cli"
-version = "2.3.1"
+version = "2.3.2"
 description = "License Manager CLI Client"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [ { include = "lm_cli" } ]
```

### Comparing `license_manager_cli-2.3.1/PKG-INFO` & `license_manager_cli-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-cli
-Version: 2.3.1
+Version: 2.3.2
 Summary: License Manager CLI Client
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

