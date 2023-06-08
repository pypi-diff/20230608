# Comparing `tmp/qase-python-commons-1.0.4.tar.gz` & `tmp/qase-python-commons-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-python-commons-1.0.4.tar", last modified: Mon Apr  3 05:25:38 2023, max compression
+gzip compressed data, was "qase-python-commons-2.0.0.tar", last modified: Thu Jun  8 05:35:47 2023, max compression
```

## Comparing `qase-python-commons-1.0.4.tar` & `qase-python-commons-2.0.0.tar`

### file list

```diff
@@ -1,33 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:25:38.211017 qase-python-commons-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-03 05:25:38.211017 qase-python-commons-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-03 05:25:38.211017 qase-python-commons-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:25:38.203018 qase-python-commons-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:25:38.207018 qase-python-commons-1.0.4/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-03 05:25:38.000000 qase-python-commons-1.0.4/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-03 05:25:38.000000 qase-python-commons-1.0.4/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 05:25:38.000000 qase-python-commons-1.0.4/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-03 05:25:38.000000 qase-python-commons-1.0.4/src/qase_python_commons.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 05:25:38.000000 qase-python-commons-1.0.4/src/qase_python_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-03 05:25:38.000000 qase-python-commons-1.0.4/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-03 05:25:38.000000 qase-python-commons-1.0.4/src/qase_python_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:25:38.203018 qase-python-commons-1.0.4/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:25:38.207018 qase-python-commons-1.0.4/src/qaseio/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/src/qaseio/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/src/qaseio/commons/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/src/qaseio/commons/testops.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/src/qaseio/commons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:25:38.211017 qase-python-commons-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/tests/test_testops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-03 05:25:34.000000 qase-python-commons-1.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.417632 qase-python-commons-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-08 05:35:47.417632 qase-python-commons-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22714 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-08 05:35:47.417632 qase-python-commons-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.409632 qase-python-commons-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.413632 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 05:35:47.000000 qase-python-commons-2.0.0/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.409632 qase-python-commons-2.0.0/src/qaseio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.413632 qase-python-commons-2.0.0/src/qaseio/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.413632 qase-python-commons-2.0.0/src/qaseio/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/models/suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/testops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/src/qaseio/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.413632 qase-python-commons-2.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:35:47.413632 qase-python-commons-2.0.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tests/models/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tests/test_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-08 05:35:43.000000 qase-python-commons-2.0.0/tox.ini
```

### Comparing `qase-python-commons-1.0.4/.gitignore` & `qase-python-commons-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qase-python-commons-1.0.4/.pre-commit-config.yaml` & `qase-python-commons-2.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qase-python-commons-1.0.4/PKG-INFO` & `qase-python-commons-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 1.0.4
+Version: 2.0.0
 Summary: A library for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qase-python-commons-1.0.4/license.txt` & `qase-python-commons-2.0.0/license.txt`

 * *Files identical despite different names*

### Comparing `qase-python-commons-1.0.4/setup.cfg` & `qase-python-commons-2.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 author = Qase Team
 author-email = support@qase.io
 license = apache
 long-description = file: README.md
 long-description-content-type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 platforms = any
-version = 1.0.4
+version = 2.0.0
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
 packages = find_namespace:
@@ -33,14 +33,16 @@
 exclude = 
 	tests
 
 [options.extras_require]
 testing = 
 	pytest
 	pytest-cov
+	mock
+	more_itertools
 
 [test]
 extras = True
 
 [tool:pytest]
 addopts = 
 	--cov qaseio.commons --cov-report term-missing
```

### Comparing `qase-python-commons-1.0.4/setup.py` & `qase-python-commons-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-1.0.4/src/qase_python_commons.egg-info/PKG-INFO` & `qase-python-commons-2.0.0/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 1.0.4
+Version: 2.0.0
 Summary: A library for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `qase-python-commons-1.0.4/src/qase_python_commons.egg-info/SOURCES.txt` & `qase-python-commons-2.0.0/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -14,13 +14,26 @@
 src/qase_python_commons.egg-info/SOURCES.txt
 src/qase_python_commons.egg-info/dependency_links.txt
 src/qase_python_commons.egg-info/namespace_packages.txt
 src/qase_python_commons.egg-info/not-zip-safe
 src/qase_python_commons.egg-info/requires.txt
 src/qase_python_commons.egg-info/top_level.txt
 src/qaseio/commons/__init__.py
+src/qaseio/commons/config.py
+src/qaseio/commons/interceptor.py
+src/qaseio/commons/loader.py
 src/qaseio/commons/report.py
 src/qaseio/commons/testops.py
 src/qaseio/commons/utils.py
+src/qaseio/commons/models/__init__.py
+src/qaseio/commons/models/attachment.py
+src/qaseio/commons/models/relation.py
+src/qaseio/commons/models/result.py
+src/qaseio/commons/models/run.py
+src/qaseio/commons/models/runtime.py
+src/qaseio/commons/models/step.py
+src/qaseio/commons/models/suite.py
+tests/test_config.py
+tests/test_interceptor.py
 tests/test_report.py
-tests/test_testops.py
-tests/test_utils.py
+tests/test_utils.py
+tests/models/test_run.py
```

### Comparing `qase-python-commons-1.0.4/src/qaseio/commons/testops.py` & `qase-python-commons-2.0.0/src/qaseio/commons/testops.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from qaseio.api_client import ApiClient
 from qaseio.configuration import Configuration
 from qaseio.api.attachments_api import AttachmentsApi
-from qaseio.api.plans_api import PlansApi
+from qaseio.api.environments_api import EnvironmentsApi
 from qaseio.api.projects_api import ProjectsApi
 from qaseio.api.results_api import ResultsApi
 from qaseio.api.runs_api import RunsApi
 from qaseio.model.run_create import RunCreate
 from qaseio.model.result_create_bulk import ResultCreateBulk
 from qaseio.model.result_create import ResultCreate
 from qaseio.model.result_create_case import ResultCreateCase
 from qaseio.rest import ApiException
+from qaseio.commons.models.attachment import Attachment
+from qaseio.commons.models.step import Step
+
+from qaseio.commons.models.result import Result
 
 from datetime import datetime
-from typing import Tuple, Union
-import mimetypes
-import ntpath
+import more_itertools
 import certifi
 
-from io import BytesIO
-
 from pkg_resources import DistributionNotFound, get_distribution
 
 def package_version(name):
     try:
         version = get_distribution(name).version
     except DistributionNotFound:
         version = "unknown"
@@ -34,35 +34,45 @@
 class QaseTestOps:
 
     def __init__(self,
             api_token,
             project_code,
             run_id=None,
             plan_id=None,
-            mode="async",
+            bulk=True,
             run_title=None,
             environment=None,
             host="qase.io",
-            complete_run=False) -> None:
+            complete_run=False,
+            defect=False,
+            chunk_size=200) -> None:
 
         configuration = Configuration()
         configuration.api_key['TokenAuth'] = api_token
         configuration.host = f'https://api.{host}/v1'
         configuration.ssl_ca_cert = certifi.where()
 
         self.client = ApiClient(configuration)
 
         self.project_code = project_code
         self.run_id = int(run_id) if run_id else run_id
         self.plan_id = plan_id
-        self.mode = mode
+        self.bulk = bulk
+        self.defect = defect
         self.complete_after_run = complete_run
-        self.environment = int(environment) if environment else environment
+        if environment:
+            if isinstance(environment, str):
+                self.environment = self._get_environment(environment)
+            elif isinstance(environment, int):
+                self.environment_id = environment
         self.host = host
         self.enabled = True
+        if (chunk_size > 2000):
+            chunk_size = 2000
+        self.chunk_size = chunk_size
 
         if run_title and run_title != '':
             self.run_title = run_title
         else:
             self.run_title = "Automated Run {}".format(str(datetime.now()))
 
         self.run = None
@@ -79,80 +89,108 @@
             try:
                 response = api_instance.get_project(code=project)
                 if hasattr(response, 'result'):
                     return response.result
                 raise ValueError("Unable to find given project code")
             except ApiException as e:
                 self.enabled = False
-                print("Disabling Qase TestOps reporter. Exception when calling ProjectApi->get_project: %s\n" % e)
+                print("[Qase] ⚠️  Disabling Qase TestOps reporter. Exception when calling ProjectApi->get_project: %s\n" % e)
+
+    # Method loads environment by name and returns environment id
+    def _get_environment(self, environment: str):
+        # TODO: Add support for environment lookup by name
+        return None
 
     def _send_bulk_results(self):
         if self.enabled and self.results:
             print()
-            print(f"Uploading attachments for Run ID: {self.run_id}...")
+            print(f"[Qase] Uploading attachments for Run ID: {self.run_id}...")
             results = []
             for result in self.results:
                 attached = []
-                for files in result.get('attachments', []):
-                    attached.extend(self._upload(self.project_code, files))
-                    result['attachments'] = [attach.hash for attach in attached]
+                if result.attachments:
+                    for attachment in result.attachments:
+                        attached.extend(self._upload(attachment))
 
                 steps = []
-                for step in result['steps']:
+                for step in result.steps:
                     prepared = self._prepare_step(step)
                     steps.append(prepared)
 
-                result['steps'] = steps
-
-                results.append(result)
+                case_data = {
+                    "title": result.get_title(),
+                    "description": result.get_field('description'),
+                    "precondtions": result.get_field('precondtions'),
+                    "postconditions": result.get_field('postconditions'),
+                }
+
+                for key, param in result.params.items():
+                    # Hack to match old TestOps API
+                    if param == "": result.params[key] = "empty"
+
+                if (result.get_field('severity')):
+                    case_data["severity"] = result.get_field('severity')
+
+                if (result.get_field('priority')):
+                    case_data["priority"] = result.get_field('priority')
+
+                if (result.get_field('layer')):
+                    case_data["layer"] = result.get_field('layer')
+
+                results.append({
+                    "case_id": result.get_testops_id(),
+                    "status": result.execution.status,
+                    "stacktrace": result.execution.stacktrace,
+                    "time_ms": result.execution.duration,
+                    "comment": result.message,
+                    "attachments": [attach.hash for attach in attached],
+                    "case": case_data,
+                    "steps": steps,
+                    "param": result.params,
+                    "defect": self.defect
+                })
 
             api_results = ResultsApi(self.client)
-            print()
-            print(f"Sending results to test run {self.run_id}...")
-            try:
-                api_results.create_result_bulk(
-                    code=self.project_code,
-                    id=self.run_id,
-                    result_create_bulk=ResultCreateBulk(
-                        results=results
+            print(f"[Qase] Sending results to test run {self.run_id}. Total results: {len(results)}. Results in a chunk: {self.chunk_size}.")
+
+            i = 1
+
+            for chunk in more_itertools.chunked(results, self.chunk_size):
+                try:
+                    print(f"[Qase] Sending chunk #{i}. Chunk size: {len(chunk)}... ")
+                    api_results.create_result_bulk(
+                        code=self.project_code,
+                        id=self.run_id,
+                        result_create_bulk=ResultCreateBulk(
+                            results=chunk
+                        )
                     )
-                )
-                print(f"Results of run {self.run_id} are sent")
-            except Exception as e:
-                print(f"Error at sending results for run {self.run_id}: {e}")
+                    print(f"[Qase] Chunk #{i} was sent successfully.")
+                    i = i+1
+                except Exception as e:
+                    print(f"[Qase] ⚠️  Error at sending results for run {self.run_id} (Chunk #{i}): {e}")
+                    raise e
 
     def _complete_run(self):
         if self.enabled:
             api_runs = RunsApi(self.client)
-            print()
-            print(f"Completing run {self.run_id}")
+            print(f"[Qase] Completing run {self.run_id}")
             res = api_runs.get_run(self.project_code, self.run_id).result
             if res.status == 1:
-                print(f"Run ID:{self.run_id} already finished")
+                print(f"[Qase] Run ID:{self.run_id} already finished")
                 return
             try:
                 api_runs.complete_run(self.project_code, self.run_id)
-                print(f"Run ID:{self.run_id} was finished successfully")
+                print(f"[Qase] Run ID:{self.run_id} was completed successfully")
             except Exception as e:
-                print(f"Run ID:{self.run_id} was finished with error: {e}")
+                print(f"[Qase] ⚠️  Run ID:{self.run_id} was completed with error: {e}")
 
     def _check_run(self):
         if self.enabled:
-            if self.run_id and self.plan_id:
-                raise ValueError(
-                    "You should provide either use test run or test plan"
-                )
-            if self.plan_id:
-                api_plans = PlansApi(self.client)
-                plan = api_plans.get_plan(
-                    code=self.project_code,
-                    id=int(self.plan_id)
-                )
-                if not plan:
-                    raise ValueError("Could not find test plan")
+            if self.plan_id and not self.run_id:
                 self._create_run(plan_id=self.plan_id, environment_id=self.environment)
             if not self.run_id and not self.plan_id:
                 self._create_run(environment_id=self.environment)
                 pass
             if not self.run and not self._load_run:
                 raise TestOpsRunNotFoundException(
                     "Unable to find given test run."
@@ -189,143 +227,145 @@
                     run_create=RunCreate(**{k: v for k, v in kwargs.items() if v is not None})
                 )
                 self.run_id = result.result.id
                 self.run = result.result
 
                 print()
                 print(
-                    "Qase TestOps: created test run "
+                    "[Qase] TestOps: created test run "
                     "https://app.{}/run/{}/dashboard/{}".format(
                         self.host, self.project_code, self.run_id
                     )
                 )
             except Exception as e:
                 self.enabled = False
                 print()
-                print(f"Disabling Qase TestOps reporter. Unable to create test run: {e}")
+                print(f"[Qase] ⚠️  Disabling Qase TestOps reporter. Unable to create test run: {e}")
 
-    def _upload(
-        self,
-        code: str,
-        *file_infos: Union[str, Tuple[str, str], Tuple[bytes, str, str]],
-    ):
+    def _upload(self, attachment: Attachment):
         api_attachments = AttachmentsApi(self.client)
-        for _id, file in enumerate(file_infos):
-            filename = None
-            if isinstance(file, tuple):
-                if len(file) == 2:
-                    path, mime = file
-                else:
-                    path, mime, filename = file
-            else:
-                path = file
-                mime = mimetypes.guess_type(file)[0]
-            if isinstance(path, bytes):
-                content = BytesIO(path)
-                content.name = filename or ntpath.basename(path)
-                content.mime = mime
-            else:
-                content = open(path, "rb")
 
-            return api_attachments.upload_attachment(
-                self.project_code, file=[content],
+        return api_attachments.upload_attachment(
+                self.project_code, file=[attachment.get_for_upload()],
             ).result
+    
+    # This method contains a lot of hacks to match old TestOps API.
+    def _prepare_step(self, step: Step):
+        prepared_children = []
+
+        prepared_step = {
+            "time": step.execution.duration,
+        }
+        
+        prepared_step["status"] = step.execution.status
+        if step.execution.status == 'untested':
+            prepared_step["status"] = 'passed'
+        
+        if step.step_type == "text":
+            prepared_step['action'] = step.data.action
+            if step.data.expected_result:
+                prepared_step['expected_result'] = step.data.expected_result
+        
+        if step.step_type == "request":
+            prepared_step['action'] = step.data.request_method + " " + step.data.request_url
+            if (step.data.request_body):
+                step.attachments.append(Attachment(file_name='request_body.txt', content=step.data.request_body, mime_type='text/plain'))
+            if (step.data.request_headers):
+                step.attachments.append(Attachment(file_name='request_headers.txt', content=step.data.request_headers, mime_type='text/plain'))
+            if (step.data.response_body):
+                step.attachments.append(Attachment(file_name='response_body.txt', content=step.data.response_body, mime_type='text/plain'))
+            if (step.data.response_headers):
+                step.attachments.append(Attachment(file_name='response_headers.txt', content=step.data.response_headers, mime_type='text/plain'))
+
+        if step.attachments:
+            uploaded_attachments = []
+            for file in step.attachments:
+                uploaded_attachments.extend(self._upload(file))
+            prepared_step['attachments'] = [attach.hash for attach in uploaded_attachments]
+
+        if step.steps:
+            for substep in step.steps:
+                prepared_children.append(self._prepare_step(substep))
+            prepared_step["steps"] = prepared_children
+        return prepared_step
 
-    def _prepare_step(self, step):
-        if step['attachments']:
-            attached_step = []
-            for files in step['attachments']:
-                attached_step.extend(self._upload(self.project_code, files))
-            step["attachments"] = [attach.hash for attach in attached_step]
-        if step['steps']:
-            prepared = []
-            for substep in step['steps']:
-                prepared.append(self._prepare_step(substep))
-            step['steps'] = prepared
-        return step
-
-    def _send_result(self, result):
+    def _send_result(self, result: Result):
         if self.enabled:
             api_results = ResultsApi(self.client)
             print()
-            print(f"Sending a result to test run {self.run_id}...")
+            print(f"[Qase] Sending a result to test run {self.run_id}...")
 
-            attachments = result.get("attachments", [])
             attached = []
-            if attachments:
-                for files in attachments:
-                    attached.extend(self._upload(self.project_code, files))
+            if result.attachments:
+                for attachment in result.attachments:
+                    attached.extend(self._upload(attachment))
 
             steps = []
-            for step in result['steps']:
+            for step in result.steps:
                 prepared = self._prepare_step(step)
                 steps.append(prepared)
 
             case_data = {
-                "title": result.get('case').get('title'),
-                "description": result.get('case').get('description', ''),
-                "precondtions": result.get('case').get('precondtions', ''),
-                "postconditions": result.get('case').get('postconditions', ''),
+                "title": result.get_title(),
+                "description": result.get_field('description'),
+                "precondtions": result.get_field('precondtions'),
+                "postconditions": result.get_field('postconditions'),
             }
 
-            if (result.get('case').get('severity', None)):
-                case_data["severity"] = result.get('case').get('severity')
+            for key, param in result.params.items():
+                # Hack to match old TestOps API
+                if param == "":
+                    result.params[key] = "empty"
+
+            if (result.get_field('severity')):
+                case_data["severity"] = result.get_field('severity')
 
-            if (result.get('case').get('layer', None)):
-                case_data["layer"] = result.get('case').get('layer')
+            if (result.get_field('priority')):
+                case_data["priority"] = result.get_field('priority')
+
+            if (result.get_field('layer')):
+                case_data["layer"] = result.get_field('layer')
 
             try:
                 api_results.create_result(
                     code=self.project_code,
                     id=self.run_id,
                     result_create=ResultCreate(
-                        case_id=result.get('case_id', 0),
-                        status=result.get('status'),
-                        stacktrace=result.get('stacktrace'),
-                        time_ms=result.get('time_ms'),
-                        comment=result.get('comment', ''),
+                        case_id=result.get_testops_id(),
+                        status=result.execution.status,
+                        stacktrace=result.execution.stacktrace,
+                        time_ms=result.execution.duration,
+                        comment=result.message,
                         attachments = [attach.hash for attach in attached],
+                        defect=self.defect,
                         case=ResultCreateCase(
                             **{k: v for k, v in case_data.items() if v is not None}
                         ),
                         steps=steps,
-                        param=result.get('param', {})
+                        param=result.params
                     )
                 )
-                print(f"Results of run {self.run_id} was sent")
+                print(f"[Qase] Results of run {self.run_id} was sent")
             except Exception as e:
-                print(f"Error dat sending results for run {self.run_id}: {e}")
-            pass
+                print(f"[Qase] ⚠️  Error at sending results for run {self.run_id}: {e}")
+                raise e
 
     # Lifecycle methods
     def start_run(self):
         if self.enabled:
             """Verify test run"""
             self._check_run()
             return self.run_id
 
     def complete_run(self, is_main=True, exit_code=None):
         if self.enabled:
-            if self.mode == "async":
+            if self.bulk:
                 self._send_bulk_results()
             if self.complete_after_run and is_main:
                 self._complete_run()
 
-    def add_result(self, result, steps):
+    def add_result(self, result: Result):
         if self.enabled:
-            result['steps'] = self._get_steps(steps)
-            if self.mode == "sync":
-                self._send_result(result)
-                pass
-            else:
+            if self.bulk:
                 self.results.append(result)
-                pass
-
-    def _get_steps(self, steps):
-        tree = []
-        for uuid in steps:
-            branch = []
-            if steps[uuid].get('steps', []):
-                branch = self._get_steps(steps[uuid].get('steps', {}))
-            steps[uuid]['steps'] = branch
-            tree.append({**steps[uuid]})
-        return tree
+            else:
+                self._send_result(result)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

