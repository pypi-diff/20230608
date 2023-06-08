# Comparing `tmp/qase-python-commons-2.0.0.tar.gz` & `tmp/qase-python-commons-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-python-commons-2.0.0.tar", last modified: Thu Jun  8 05:35:47 2023, max compression
+gzip compressed data, was "qase-python-commons-2.0.1.tar", last modified: Thu Jun  8 07:29:00 2023, max compression
```

## Comparing `qase-python-commons-2.0.0.tar` & `qase-python-commons-2.0.1.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.417632 qase-python-commons-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-08 05:35:47.417632 qase-python-commons-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-08 05:35:47.417632 qase-python-commons-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.409632 qase-python-commons-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.413632 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.409632 qase-python-commons-2.0.0/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.413632 qase-python-commons-2.0.0/src/qaseio/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.413632 qase-python-commons-2.0.0/src/qaseio/commons/models/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/testops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.413632 qase-python-commons-2.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.413632 qase-python-commons-2.0.0/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tests/models/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tests/test_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.415452 qase-python-commons-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.415452 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 07:29:00.000000 qase-python-commons-2.0.1/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.415452 qase-python-commons-2.0.1/src/qaseio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.415452 qase-python-commons-2.0.1/src/qaseio/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/src/qaseio/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/models/suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/testops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/src/qaseio/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:29:00.419452 qase-python-commons-2.0.1/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/tests/models/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-08 07:28:51.000000 qase-python-commons-2.0.1/tox.ini
```

### Comparing `qase-python-commons-2.0.0/.gitignore` & `qase-python-commons-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/.pre-commit-config.yaml` & `qase-python-commons-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/PKG-INFO` & `qase-python-commons-2.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 2.0.0
+Version: 2.0.1
 Summary: A library for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: AUTHORS.rst
 
 # Qase Python Commons
```

### Comparing `qase-python-commons-2.0.0/license.txt` & `qase-python-commons-2.0.1/license.txt`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/setup.cfg` & `qase-python-commons-2.0.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -6,50 +6,53 @@
 license = apache
 long-description = file: README.md
 long-description-content-type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 platforms = any
 version = 2.0.0
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Programming Language :: Python
 
 [options]
 zip_safe = False
 packages = find_namespace:
 namespace_packages = qaseio
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
 	certifi>=2022.12.7
 	qaseio>=3.2.1
 	attrs>=19.3.0
+	more_itertools
 python_requires = >=3.7
 
 [options.packages.find]
 where = src
 include = qaseio.*
 exclude = 
 	tests
 
 [options.extras_require]
 testing = 
 	pytest
 	pytest-cov
 	mock
 	more_itertools
+	requests
+	urllib3
 
 [test]
 extras = True
 
 [tool:pytest]
 addopts = 
-	--cov qaseio.commons --cov-report term-missing
+	--cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
 	build
 	.tox
 testpaths = tests
```

### Comparing `qase-python-commons-2.0.0/setup.py` & `qase-python-commons-2.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/src/qase_python_commons.egg-info/PKG-INFO` & `qase-python-commons-2.0.1/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 2.0.0
+Version: 2.0.1
 Summary: A library for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: AUTHORS.rst
 
 # Qase Python Commons
```

### Comparing `qase-python-commons-2.0.0/src/qase_python_commons.egg-info/SOURCES.txt` & `qase-python-commons-2.0.1/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,11 +29,10 @@
 src/qaseio/commons/models/relation.py
 src/qaseio/commons/models/result.py
 src/qaseio/commons/models/run.py
 src/qaseio/commons/models/runtime.py
 src/qaseio/commons/models/step.py
 src/qaseio/commons/models/suite.py
 tests/test_config.py
-tests/test_interceptor.py
 tests/test_report.py
 tests/test_utils.py
 tests/models/test_run.py
```

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/config.py` & `qase-python-commons-2.0.1/src/qaseio/commons/config.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/interceptor.py` & `qase-python-commons-2.0.1/src/qaseio/commons/interceptor.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/loader.py` & `qase-python-commons-2.0.1/src/qaseio/commons/loader.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/models/attachment.py` & `qase-python-commons-2.0.1/src/qaseio/commons/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/models/result.py` & `qase-python-commons-2.0.1/src/qaseio/commons/models/result.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Type, Optional, Union
+from typing import Type, Optional, Union, Dict, List
 import time
 import uuid
 import json
 from qaseio.commons.models.step import Step
 from qaseio.commons.models.relation import Relation
 from qaseio.commons.models.attachment import Attachment
 from qaseio.commons.utils import QaseUtils
@@ -43,17 +43,17 @@
         self.duration = (int)((self.end_time - self.start_time) * 1000)
 
 class Request(object):
     def __init__(self,
             method: str,
             url: str,
             status: int,
-            request_headers: dict[str, str],
+            request_headers: Dict[str, str],
             request_body: str,
-            response_headers: dict[str, str],
+            response_headers: Dict[str, str],
             response_body: str):
         self.method = method
         self.url = url
         self.status = status
         self.request_headers = request_headers
         self.request_body = request_body
         self.response_headers = response_headers
@@ -63,31 +63,31 @@
     def __init__(self, title: str, signature: str) -> None:
         self.id: str = str(uuid.uuid4())
         self.title: str = title
         self.signature: str = signature
         self.run_id: Optional[str] = None
         self.testops_id: Optional[int] = None
         self.execution: Type[Execution] = Execution()
-        self.fields: dict[Type[Field]] = {}
-        self.attachments: list[Attachment] = []
-        self.steps: list[Type[Step]] = []
+        self.fields: Dict[Type[Field]] = {}
+        self.attachments: List[Attachment] = []
+        self.steps: List[Type[Step]] = []
         self.params: Optional[dict] = {}
         self.author: Optional[str] = None
-        self.relations: list[Type[Relation]] = []
+        self.relations: List[Type[Relation]] = []
         self.muted: bool = False
         self.message: Optional[str] = None
         QaseUtils.get_host_data()
 
     def add_message(self, message: str) -> None:
         self.message = message
     
     def add_field(self, field: Type[Field]) -> None:
         self.fields[field.name] = field.value
 
-    def add_steps(self, steps: list[Type[Step]]) -> None:
+    def add_steps(self, steps: List[Type[Step]]) -> None:
         self.steps = QaseUtils().build_tree(steps)
 
     def add_attachment(self, attachment: Attachment) -> None:
         self.attachments.append(attachment)
 
     def add_relation(self, relation: Type[Relation]) -> None:
         self.relations.append(relation)
```

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/models/run.py` & `qase-python-commons-2.0.1/src/qaseio/commons/models/run.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from typing import Optional
+from typing import Optional, List
 
 class RunExecution(object):
     def __init__(self,
                  start_time: float,
                  end_time: float,
                  cumulative_duration: int = 0,
                  ) -> None:
@@ -21,36 +21,36 @@
         self.failed = 0
         self.skipped = 0
         self.broken = 0
         self.muted = 0
         self.total = 0
         
     def track(self, result: dict):
-        match result["execution"]["status"]:
-            case "passed":
-                self.passed += 1
-            case "failed":
-                self.failed += 1
-            case "skipped":
-                self.skipped += 1
-            case "broken":
-                self.broken += 1
+        status = result["execution"]["status"]
+        if status == "passed":
+            self.passed += 1
+        elif status == "failed":
+            self.failed += 1
+        elif status == "skipped":
+            self.skipped += 1
+        elif status == "broken":
+            self.broken += 1
         self.total += 1
         if result.get('muted', False):
             self.muted += 1
             
 
 class Run(object):
     def __init__(self, 
                  title: str,
                  start_time: float,
                  end_time: float,
-                 results: list[str] = [],
-                 threads: list[str] = [],
-                 suites: list[str] = [],
+                 results: List[str] = [],
+                 threads: List[str] = [],
+                 suites: List[str] = [],
                  environment: Optional[str] = None
                  ):
         self.title = title
         self.execution = RunExecution(start_time=start_time, end_time=end_time)
         self.stats = RunStats()
         self.results = results
         self.threads = threads
```

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/models/runtime.py` & `qase-python-commons-2.0.1/src/qaseio/commons/models/runtime.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/models/step.py` & `qase-python-commons-2.0.1/src/qaseio/commons/models/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union
+from typing import Optional, Union, Dict, List, Type
 import time
 import uuid
 from qaseio.commons.models.attachment import Attachment
 
 class StepTextData(object):
     def __init__(self, action: str, expected_result: Optional[str] = None):
         self.action = action
@@ -17,27 +17,27 @@
 class StepGherkinData(object):
     def __init__(self, keyword: str, name: str, line: int):
         self.keyword = keyword
         self.name = name
         self.line = line
 
 class StepRequestData(object):
-    def __init__(self, request_body: str, request_headers: dict[str, str], request_method: str, request_url: str):
+    def __init__(self, request_body: str, request_headers: Dict[str, str], request_method: str, request_url: str):
         if (isinstance(request_body, bytes)):
             request_body = request_body.decode('utf-8')
         self.request_body = request_body
         if (isinstance(request_headers, bytes)):
             request_headers = request_headers.decode('utf-8')
         self.request_headers = request_headers
         self.request_method = request_method
         self.request_url = request_url
 
-    def add_response(self, status_code: int, response_body: Optional[str] = None, response_headers: Optional[dict[str, str]] = None):
+    def add_response(self, status_code: int, response_body: Optional[str] = None, response_headers: Optional[Dict[str, str]] = None):
         self.status_code = status_code
-        
+
         if (isinstance(response_body, bytes)):
             response_body = response_body.decode('utf-8')
         self.response_body = response_body
         if (isinstance(response_headers, bytes)):
             response_headers = response_headers.decode('utf-8')
         self.response_headers = response_headers
 
@@ -100,15 +100,15 @@
             return {step.id: step for step in self.steps}
         else:
             return self.steps
 
     def set_data(self, data: Union[StepTextData, StepAssertData, StepGherkinData, StepRequestData]):
         self.data = data
 
-    def add_step(self, step: type['Step']):
+    def add_step(self, step: Type['Step']):
         self.steps.append(step)
 
-    def set_steps(self, steps: list[type['Step']]):
+    def set_steps(self, steps: List[Type['Step']]):
         self.steps = steps
 
     def add_attachment(self, attachment: Attachment):
         self.attachments.append(attachment)
```

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/report.py` & `qase-python-commons-2.0.1/src/qaseio/commons/report.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/testops.py` & `qase-python-commons-2.0.1/src/qaseio/commons/testops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from qaseio.api_client import ApiClient
 from qaseio.configuration import Configuration
 from qaseio.api.attachments_api import AttachmentsApi
-from qaseio.api.environments_api import EnvironmentsApi
 from qaseio.api.projects_api import ProjectsApi
 from qaseio.api.results_api import ResultsApi
 from qaseio.api.runs_api import RunsApi
 from qaseio.model.run_create import RunCreate
 from qaseio.model.result_create_bulk import ResultCreateBulk
 from qaseio.model.result_create import ResultCreate
 from qaseio.model.result_create_case import ResultCreateCase
```

### Comparing `qase-python-commons-2.0.0/src/qaseio/commons/utils.py` & `qase-python-commons-2.0.1/src/qaseio/commons/utils.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.0/tests/models/test_run.py` & `qase-python-commons-2.0.1/tests/models/test_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-import pytest
 from mock import Mock
 import json
 import time
 
-from qaseio.commons.models.run import RunExecution, RunStats, Run  # Replace with the actual import
+from qaseio.commons.models.run import RunExecution, RunStats, Run
 
 def test_run_execution():
     start_time = time.time()
     end_time = start_time + 1  # 1 second later
     execution = RunExecution(start_time, end_time)
 
     assert execution.start_time == start_time
```

### Comparing `qase-python-commons-2.0.0/tests/test_config.py` & `qase-python-commons-2.0.1/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import json
 import unittest
 from unittest.mock import patch, mock_open
-from qaseio.commons.config import ConfigManager  # replace 'your_module' with the actual module name
+from qaseio.commons.config import ConfigManager
 
 class TestConfigManager(unittest.TestCase):
     def setUp(self):
         self.config_manager = ConfigManager()
         self.mock_config_data = json.dumps({
             "database": {
                 "host": "localhost",
```

### Comparing `qase-python-commons-2.0.0/tests/test_report.py` & `qase-python-commons-2.0.1/tests/test_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import pytest
-import os
 from unittest.mock import MagicMock, patch
-from qaseio.commons import QaseReport
+from qaseio.commons.report import QaseReport
 
 def test_QaseReport_init():
     report = QaseReport(report_path="custom_path", format="json", environment="env1")
     assert report.report_path == "custom_path"
     assert report.format == "json"
     assert report.environment == "env1"
```

### Comparing `qase-python-commons-2.0.0/tests/test_utils.py` & `qase-python-commons-2.0.1/tests/test_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-import pytest
 from mock import Mock
 import os
 import threading
 import sys
 import pip
 
-from qaseio.commons import QaseUtils  # Replace with the actual import
+from qaseio.commons import QaseUtils
 
 def test_build_tree():
     # Mocking item objects
     item1 = Mock()
     item1.id = 1
     item1.parent_id = None
     item1.steps = []
```

