# Comparing `tmp/gaohn-common-utils-0.0.25.tar.gz` & `tmp/gaohn-common-utils-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.25.tar", last modified: Thu Jun  8 11:35:43 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.26.tar", last modified: Thu Jun  8 11:37:45 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.25.tar` & `gaohn-common-utils-0.0.26.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:43.220607 gaohn-common-utils-0.0.25/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 11:35:43.216607 gaohn-common-utils-0.0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:43.212607 gaohn-common-utils-0.0.25/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:43.212607 gaohn-common-utils-0.0.25/common_utils/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/cloud/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:43.212607 gaohn-common-utils-0.0.25/common_utils/cloud/gcp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:43.212607 gaohn-common-utils-0.0.25/common_utils/cloud/gcp/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:43.216607 gaohn-common-utils-0.0.25/common_utils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/core/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/core/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/core/file_system_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:43.212607 gaohn-common-utils-0.0.25/common_utils/versioning/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:43.216607 gaohn-common-utils-0.0.25/common_utils/versioning/dvc/
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:35:43.216607 gaohn-common-utils-0.0.25/gaohn_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 11:35:43.000000 gaohn-common-utils-0.0.25/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-08 11:35:43.000000 gaohn-common-utils-0.0.25/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:35:43.000000 gaohn-common-utils-0.0.25/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-08 11:35:43.000000 gaohn-common-utils-0.0.25/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 11:35:43.000000 gaohn-common-utils-0.0.25/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-08 11:35:24.000000 gaohn-common-utils-0.0.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:35:43.220607 gaohn-common-utils-0.0.25/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:45.695347 gaohn-common-utils-0.0.26/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 11:37:45.695347 gaohn-common-utils-0.0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:45.691347 gaohn-common-utils-0.0.26/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:45.695347 gaohn-common-utils-0.0.26/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:45.691347 gaohn-common-utils-0.0.26/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:45.695347 gaohn-common-utils-0.0.26/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:45.695347 gaohn-common-utils-0.0.26/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:45.691347 gaohn-common-utils-0.0.26/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:45.695347 gaohn-common-utils-0.0.26/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:37:45.695347 gaohn-common-utils-0.0.26/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 11:37:45.000000 gaohn-common-utils-0.0.26/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-08 11:37:45.000000 gaohn-common-utils-0.0.26/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:37:45.000000 gaohn-common-utils-0.0.26/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-08 11:37:45.000000 gaohn-common-utils-0.0.26/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 11:37:45.000000 gaohn-common-utils-0.0.26/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-08 11:37:24.000000 gaohn-common-utils-0.0.26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:37:45.695347 gaohn-common-utils-0.0.26/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.25/LICENSE` & `gaohn-common-utils-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.25/PKG-INFO` & `gaohn-common-utils-0.0.26/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.25
+Version: 0.0.26
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.25/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.26/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.25/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.26/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.25/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.26/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.25/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.26/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.25/common_utils/core/common.py` & `gaohn-common-utils-0.0.26/common_utils/core/common.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.25/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.26/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.25/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.26/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.25/common_utils/core/logger.py` & `gaohn-common-utils-0.0.26/common_utils/core/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         return log_output_dir
 
     def _init_logger(self) -> logging.Logger:
         if self.log_dir is not None:
             log_output_dir = self._create_log_output_dir()
             log_file_path = log_output_dir / self.log_file if self.log_file else None
             self.log_output_dir = log_output_dir
+        else:
+            log_file_path = None
 
         if self.module_name is None:
             logger = logging.getLogger(__name__)
         else:
             # get module name, useful for multi-module logging
             logger = logging.getLogger(self.module_name)
```

### Comparing `gaohn-common-utils-0.0.25/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.26/common_utils/versioning/dvc/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.25/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.26/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.25
+Version: 0.0.26
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.25/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.26/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.25/pyproject.toml` & `gaohn-common-utils-0.0.26/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gaohn-common-utils"
-version = "0.0.25"
+version = "0.0.26"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "A small utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

