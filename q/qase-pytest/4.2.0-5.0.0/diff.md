# Comparing `tmp/qase-pytest-4.2.0.tar.gz` & `tmp/qase-pytest-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-pytest-4.2.0.tar", last modified: Mon Apr  3 05:30:41 2023, max compression
+gzip compressed data, was "qase-pytest-5.0.0.tar", last modified: Thu Jun  8 07:33:18 2023, max compression
```

## Comparing `qase-pytest-4.2.0.tar` & `qase-pytest-5.0.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:30:41.113756 qase-pytest-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-04-03 05:30:41.113756 qase-pytest-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:30:41.109756 qase-pytest-4.2.0/example/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/example/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-04-03 05:30:41.113756 qase-pytest-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:30:41.101756 qase-pytest-4.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:30:41.109756 qase-pytest-4.2.0/src/qase_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-04-03 05:30:40.000000 qase-pytest-4.2.0/src/qase_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-03 05:30:41.000000 qase-pytest-4.2.0/src/qase_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 05:30:40.000000 qase-pytest-4.2.0/src/qase_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-03 05:30:40.000000 qase-pytest-4.2.0/src/qase_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-03 05:30:40.000000 qase-pytest-4.2.0/src/qase_pytest.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 05:30:40.000000 qase-pytest-4.2.0/src/qase_pytest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-03 05:30:40.000000 qase-pytest-4.2.0/src/qase_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-03 05:30:40.000000 qase-pytest-4.2.0/src/qase_pytest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:30:41.101756 qase-pytest-4.2.0/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:30:41.109756 qase-pytest-4.2.0/src/qaseio/pytest/
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/src/qaseio/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/src/qaseio/pytest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/src/qaseio/pytest/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 05:30:41.113756 qase-pytest-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-03 05:30:37.000000 qase-pytest-4.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/CONFIGURATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/UPGRADE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.966138 qase-pytest-5.0.0/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/example/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.966138 qase-pytest-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/src/qase_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 07:33:18.000000 qase-pytest-5.0.0/src/qase_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.966138 qase-pytest-5.0.0/src/qaseio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/src/qaseio/pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/src/qaseio/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/src/qaseio/pytest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/src/qaseio/pytest/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/src/qaseio/pytest/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:18.970138 qase-pytest-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-08 07:33:10.000000 qase-pytest-5.0.0/tox.ini
```

### Comparing `qase-pytest-4.2.0/.coveragerc` & `qase-pytest-5.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `qase-pytest-4.2.0/.gitignore` & `qase-pytest-5.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qase-pytest-4.2.0/.pre-commit-config.yaml` & `qase-pytest-5.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qase-pytest-4.2.0/LICENSE.txt` & `qase-pytest-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qase-pytest-4.2.0/PKG-INFO` & `qase-pytest-5.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,111 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 4.2.0
+Version: 5.0.0
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
 # [Qase](https://qase.io) Pytest Plugin
 
 [![License](https://lxgaming.github.io/badges/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
-# Installation
+## Installation
 
 ```
 pip install qase-pytest
 ```
 
-# Usage
+## Upgrade from 4.x to 5.x
+A new version of qase-pytest reporter has breaking changes. Follow these [guide](UPGRADE.md) that will help you to migrate to a new version.
 
-### Command-line arguments
-Configuration could be provided both by `pytest.ini`/`tox.ini` params
-and using command-line arguments:
-
-* Command-line args:
-```
-  --qase-mode           Define mode: `testops` to enable report
-  --qase-environment=QS_ENVIRONMENT
-                        Define execution environment ID
-  --qase-to-api-token=QS_TO_API_TOKEN
-                        Api token for Qase TestOps
-  --qase-to-project=QS_TO_PROJECT
-                        Project code in Qase TestOps
-  --qase-to-run=QS_TO_RUN_ID
-                        Test Run ID in Qase TestOps
-  --qase-to-run-title=QS_TO_RUN_TITLE
-                        Define a custom title for Qase Test Run
-  --qase-to-plan=QS_TO_PLAN_ID
-                        Test Plan ID in Qase TestOps
-  --qase-to-complete-run
-                        Complete run after all tests are finished
-  --qase-to-mode=QS_TO_MODE
-                        You can choose `sync` or `async` mode for results publication. Default: `async`
-  --qase-to-host=QS_TO_HOST
-                        Qase TestOps Enterprise customers can set their own hosts. Default: `qase.io`
-```
-
-* INI file parameters:
-
-```
-  qs_mode (string):     default value for --qase-mode
-  qs_environment (string):
-                        default value for --qase-environment
-  qs_to_api_token (string):
-                        default value for --qase-to-api-token
-  qs_to_project (string):
-                        default value for --qase-to-project
-  qs_to_run_id (string):
-                        default value for --qase-to-run
-  qs_to_run_title (string):
-                        default value for --qase-to-run-title
-  qs_to_plan_id (string):
-                        default value for --qase-to-plan
-  qs_to_complete_run (bool):
-                        default value for --qase-to-complete-run
-  qs_to_mode (string):
-                        default value for --qase-to-mode
-  qs_to_host (string):
-                        default value for --qase-to-host
-    
+## Configuration
+
+Qase Pytest Plugin can be configured in multiple ways:
+ - using a config file `qase.config.json`
+ - using environment variables
+ - using CLI options
+
+All configuration options are listed in the following doc: [Configuration](../README.md#configuration).
+
+
+### Example: qase.config.json
+
+```
+{
+	"mode": "testops", 
+	"fallback": "report",
+	"report": {
+		"driver": "local",
+		"connection": {
+			"local": {
+				"path": "./build/qase-report",
+				"format": "json" 
+			}
+		}
+	},
+	"testops": {
+		"bulk": true,
+		"api": {
+			"token": "YOUR_API_TOKEN",
+			"host": "qase.io"
+		},
+		"run": {
+            "id": 1,
+			"title": "Test run title",
+			"complete": true
+		},
+        "plan": {
+            "id": 1
+        },
+		"defect": true,
+		"project": "YOUR_PROJECT_CODE",
+		"chunk": 200
+	},
+	"framework": {
+		"pytest": {
+			"capture": {
+				"logs": true,
+				"http": true
+			}
+		}
+	},
+	"environment": "local"
+}
 ```
 
-## Link tests with test cases in Qase TestOps
+## Usage
+
+### Link tests with test cases in Qase TestOps
 
 To link tests in code with tests in Qase TestOps you can use predefined decorators:
 
 ```python
 from qaseio.pytest import qase
 
 @qase.id(13)
 @qase.title("My first test")
-@qase.severity("critical")
-@qase.layer("unit")
-@qase.precondition("*Precondition 1*. Markdown is supported.")
-@qase.description("Try to login in Qase TestOps using login and password")
+@qase.fields(
+    ("severity", "critical"),
+    ("priority", "hight"),
+    ("layer", "unit"),
+    ("description", "Try to login in Qase TestOps using login and password"),
+    ("description", "*Precondition 1*. Markdown is supported."),
+)
 def test_example_1():
     pass
 ```
 
 Each unique number can only be assigned once to the class or function being used.
 
 ### Ignore a particular test
@@ -113,24 +122,28 @@
 ### Possible test result statuses
 
 - PASSED - when test passed
 - FAILED - when test failed with AssertionError
 - BLOCKED - when test failed with any other exception
 - SKIPPED - when test has been skipped
 
-## Add attachments to test results
+### Capture network logs
+In order to capture network logs, you need to enable the `http` option in the `capture` section of the `framework` section in the config file.
+
+Qase Pytest reporter will capture all requests and responses and save as a test step automatically.
+
+### Add attachments to test results
 
 When you need to push some additional information to server you could use
 attachments:
 
 ```python
 import pytest
 from qaseio.pytest import qase
 
-
 @pytest.fixture(scope="session")
 def driver():
     driver = webdriver.Chrome()
     yield driver
     logs = "\n".join(str(row) for row in driver.get_log('browser')).encode('utf-8')
     qase.attach((logs, "text/plain", "browser.log"))
     driver.quit()
@@ -153,30 +166,29 @@
 Also you should know, that if no case id is associated with current test in
 pytest - attachment would not be uploaded:
 
 ```python
 import pytest
 from qaseio.pytest import qase
 
-
 @pytest.fixture(scope="session")
 def driver():
     driver = webdriver.Chrome()
     yield driver
     logs = "\n".join(str(row) for row in driver.get_log('browser')).encode('utf-8')
     # This would do nothing, because last test does not have case id link
     qase.attach((logs, "text/plain", "browser.log"))
     driver.quit()
 
 def test_example_2(driver):
     # This would do nothing
     qase.attach((driver.get_screenshot_as_png(), "image/png", "result.png"))
 ```
 
-## Linking code with steps
+### Linking code with steps
 
 It is possible to link test step with function, or using context.
 
 ```python
 from qaseio.pytest import qase
 
 @qase.step("First step") # test step name
@@ -193,56 +205,48 @@
     some_step()
     another_step()
     # test step hash
     with qase.step("Third step"):
         sleep(1)
 ```
 
-## Sending tests to existing testrun
+### Sending tests to existing testrun
 
 Testrun in TestOps will contain only those test results, which are presented in testrun,
 but every test would be executed.
 
 ```bash
 pytest \
     --qase-mode=testops \
-    --qase-to-api-token=<your api token here> \
-    --qase-to-project=PRJCODE \ # project, where your testrun exists in
-    --qase-to-run=3 # testrun id
+    --qase-testops-api-token=<your api token here> \
+    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
+    --qase-testops-run-id=3 # testrun id
 ```
 
-## Creating test run base on test plan
+### Creating test run base on test plan (selective launch)
 
 Create new testrun base on testplan. Testrun in Qase TestOps will contain only those
-test results, which are presented in testrun, but every test would be executed.
+test results. `qase-pytest` supports selective execution
 
 ```bash
 pytest \
     --qase-mode=testops \
-    --qase-to-api-token=<your api token here> \
-    --qase-to-project=PRJCODE \ # project, where your testrun exists in
-    --qase-to-plan=3 # testplan id
+    --qase-testops-api-token=<your api token here> \
+    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
+    --qase-testops-plan-id=3 # testplan id
 ```
 
-## Creating new testrun according to current pytest run
+### Creating new testrun according to current pytest run
 
 If you want to create a new test run in Qase TestOps for each execution, you can simply 
-skip `--qase-to-run`. If you want to provide a custom name for this run, you can add an
-option `--qase-to-run-title` 
+skip `--qase-testops-run` option. If you want to provide a custom name for this run, you can add an
+option `--qase-testops-run-title` 
 
 ```bash
 pytest \
     --qase-mode=testops \
-    --qase-to-api-token=<your api token here> \
-    --qase-to-project=PRJCODE \ # project, where your testrun would be created
-    --qase-to-run-title=My\ First\ Automated\ Run
+    --qase-testops-api-token=<your api token here> \
+    --qase-testops-project=PRJCODE \ # project, where your testrun would be created
+    --qase-testops-run-title=My\ First\ Automated\ Run
 ```
 
-## Qase TestOps submission mode
-
-Qase Pytest plugin for TestOps can work in two different modes: `sync` or `async`. 
-
-*Sync* sends each result to Qase TestOps API right after particular test execution. This mode allows you to see the results in realtime, even before test run is fully executed. 
-
-*Async* mode sends the results of test execution when the test run is complete. It uses bulk method that dramatically reduces reporting time.
-
```

### Comparing `qase-pytest-4.2.0/README.md` & `qase-pytest-5.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,93 @@
 # [Qase](https://qase.io) Pytest Plugin
 
 [![License](https://lxgaming.github.io/badges/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
-# Installation
+## Installation
 
 ```
 pip install qase-pytest
 ```
 
-# Usage
+## Upgrade from 4.x to 5.x
+A new version of qase-pytest reporter has breaking changes. Follow these [guide](UPGRADE.md) that will help you to migrate to a new version.
 
-### Command-line arguments
-Configuration could be provided both by `pytest.ini`/`tox.ini` params
-and using command-line arguments:
-
-* Command-line args:
-```
-  --qase-mode           Define mode: `testops` to enable report
-  --qase-environment=QS_ENVIRONMENT
-                        Define execution environment ID
-  --qase-to-api-token=QS_TO_API_TOKEN
-                        Api token for Qase TestOps
-  --qase-to-project=QS_TO_PROJECT
-                        Project code in Qase TestOps
-  --qase-to-run=QS_TO_RUN_ID
-                        Test Run ID in Qase TestOps
-  --qase-to-run-title=QS_TO_RUN_TITLE
-                        Define a custom title for Qase Test Run
-  --qase-to-plan=QS_TO_PLAN_ID
-                        Test Plan ID in Qase TestOps
-  --qase-to-complete-run
-                        Complete run after all tests are finished
-  --qase-to-mode=QS_TO_MODE
-                        You can choose `sync` or `async` mode for results publication. Default: `async`
-  --qase-to-host=QS_TO_HOST
-                        Qase TestOps Enterprise customers can set their own hosts. Default: `qase.io`
-```
-
-* INI file parameters:
-
-```
-  qs_mode (string):     default value for --qase-mode
-  qs_environment (string):
-                        default value for --qase-environment
-  qs_to_api_token (string):
-                        default value for --qase-to-api-token
-  qs_to_project (string):
-                        default value for --qase-to-project
-  qs_to_run_id (string):
-                        default value for --qase-to-run
-  qs_to_run_title (string):
-                        default value for --qase-to-run-title
-  qs_to_plan_id (string):
-                        default value for --qase-to-plan
-  qs_to_complete_run (bool):
-                        default value for --qase-to-complete-run
-  qs_to_mode (string):
-                        default value for --qase-to-mode
-  qs_to_host (string):
-                        default value for --qase-to-host
-    
+## Configuration
+
+Qase Pytest Plugin can be configured in multiple ways:
+ - using a config file `qase.config.json`
+ - using environment variables
+ - using CLI options
+
+All configuration options are listed in the following doc: [Configuration](../README.md#configuration).
+
+
+### Example: qase.config.json
+
+```
+{
+	"mode": "testops", 
+	"fallback": "report",
+	"report": {
+		"driver": "local",
+		"connection": {
+			"local": {
+				"path": "./build/qase-report",
+				"format": "json" 
+			}
+		}
+	},
+	"testops": {
+		"bulk": true,
+		"api": {
+			"token": "YOUR_API_TOKEN",
+			"host": "qase.io"
+		},
+		"run": {
+            "id": 1,
+			"title": "Test run title",
+			"complete": true
+		},
+        "plan": {
+            "id": 1
+        },
+		"defect": true,
+		"project": "YOUR_PROJECT_CODE",
+		"chunk": 200
+	},
+	"framework": {
+		"pytest": {
+			"capture": {
+				"logs": true,
+				"http": true
+			}
+		}
+	},
+	"environment": "local"
+}
 ```
 
-## Link tests with test cases in Qase TestOps
+## Usage
+
+### Link tests with test cases in Qase TestOps
 
 To link tests in code with tests in Qase TestOps you can use predefined decorators:
 
 ```python
 from qaseio.pytest import qase
 
 @qase.id(13)
 @qase.title("My first test")
-@qase.severity("critical")
-@qase.layer("unit")
-@qase.precondition("*Precondition 1*. Markdown is supported.")
-@qase.description("Try to login in Qase TestOps using login and password")
+@qase.fields(
+    ("severity", "critical"),
+    ("priority", "hight"),
+    ("layer", "unit"),
+    ("description", "Try to login in Qase TestOps using login and password"),
+    ("description", "*Precondition 1*. Markdown is supported."),
+)
 def test_example_1():
     pass
 ```
 
 Each unique number can only be assigned once to the class or function being used.
 
 ### Ignore a particular test
@@ -95,24 +104,28 @@
 ### Possible test result statuses
 
 - PASSED - when test passed
 - FAILED - when test failed with AssertionError
 - BLOCKED - when test failed with any other exception
 - SKIPPED - when test has been skipped
 
-## Add attachments to test results
+### Capture network logs
+In order to capture network logs, you need to enable the `http` option in the `capture` section of the `framework` section in the config file.
+
+Qase Pytest reporter will capture all requests and responses and save as a test step automatically.
+
+### Add attachments to test results
 
 When you need to push some additional information to server you could use
 attachments:
 
 ```python
 import pytest
 from qaseio.pytest import qase
 
-
 @pytest.fixture(scope="session")
 def driver():
     driver = webdriver.Chrome()
     yield driver
     logs = "\n".join(str(row) for row in driver.get_log('browser')).encode('utf-8')
     qase.attach((logs, "text/plain", "browser.log"))
     driver.quit()
@@ -135,30 +148,29 @@
 Also you should know, that if no case id is associated with current test in
 pytest - attachment would not be uploaded:
 
 ```python
 import pytest
 from qaseio.pytest import qase
 
-
 @pytest.fixture(scope="session")
 def driver():
     driver = webdriver.Chrome()
     yield driver
     logs = "\n".join(str(row) for row in driver.get_log('browser')).encode('utf-8')
     # This would do nothing, because last test does not have case id link
     qase.attach((logs, "text/plain", "browser.log"))
     driver.quit()
 
 def test_example_2(driver):
     # This would do nothing
     qase.attach((driver.get_screenshot_as_png(), "image/png", "result.png"))
 ```
 
-## Linking code with steps
+### Linking code with steps
 
 It is possible to link test step with function, or using context.
 
 ```python
 from qaseio.pytest import qase
 
 @qase.step("First step") # test step name
@@ -175,54 +187,46 @@
     some_step()
     another_step()
     # test step hash
     with qase.step("Third step"):
         sleep(1)
 ```
 
-## Sending tests to existing testrun
+### Sending tests to existing testrun
 
 Testrun in TestOps will contain only those test results, which are presented in testrun,
 but every test would be executed.
 
 ```bash
 pytest \
     --qase-mode=testops \
-    --qase-to-api-token=<your api token here> \
-    --qase-to-project=PRJCODE \ # project, where your testrun exists in
-    --qase-to-run=3 # testrun id
+    --qase-testops-api-token=<your api token here> \
+    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
+    --qase-testops-run-id=3 # testrun id
 ```
 
-## Creating test run base on test plan
+### Creating test run base on test plan (selective launch)
 
 Create new testrun base on testplan. Testrun in Qase TestOps will contain only those
-test results, which are presented in testrun, but every test would be executed.
+test results. `qase-pytest` supports selective execution
 
 ```bash
 pytest \
     --qase-mode=testops \
-    --qase-to-api-token=<your api token here> \
-    --qase-to-project=PRJCODE \ # project, where your testrun exists in
-    --qase-to-plan=3 # testplan id
+    --qase-testops-api-token=<your api token here> \
+    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
+    --qase-testops-plan-id=3 # testplan id
 ```
 
-## Creating new testrun according to current pytest run
+### Creating new testrun according to current pytest run
 
 If you want to create a new test run in Qase TestOps for each execution, you can simply 
-skip `--qase-to-run`. If you want to provide a custom name for this run, you can add an
-option `--qase-to-run-title` 
+skip `--qase-testops-run` option. If you want to provide a custom name for this run, you can add an
+option `--qase-testops-run-title` 
 
 ```bash
 pytest \
     --qase-mode=testops \
-    --qase-to-api-token=<your api token here> \
-    --qase-to-project=PRJCODE \ # project, where your testrun would be created
-    --qase-to-run-title=My\ First\ Automated\ Run
+    --qase-testops-api-token=<your api token here> \
+    --qase-testops-project=PRJCODE \ # project, where your testrun would be created
+    --qase-testops-run-title=My\ First\ Automated\ Run
 ```
-
-## Qase TestOps submission mode
-
-Qase Pytest plugin for TestOps can work in two different modes: `sync` or `async`. 
-
-*Sync* sends each result to Qase TestOps API right after particular test execution. This mode allows you to see the results in realtime, even before test run is fully executed. 
-
-*Async* mode sends the results of test execution when the test run is complete. It uses bulk method that dramatically reduces reporting time.
```

### Comparing `qase-pytest-4.2.0/setup.cfg` & `qase-pytest-5.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 author = Qase Team
 author-email = support@qase.io
 license = apache
 long-description = file: README.md
 long-description-content-type = text/markdown; charset=UTF-8; variant=GFM
 url = https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 platforms = any
-version = 4.2.0
+version = 5.0.0
 classifiers = 
-	Development Status :: 4 - Beta
+	Development Status :: 5 - Production/Stable
 	Framework :: Pytest
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
-	qase-python-commons~=1.0.3
+	qase-python-commons>=2.0.0,<2.1.0
 	pytest>=7.2.0
 	filelock~=3.10.7
+	more_itertools
 python_requires = >=3.7
 
 [options.packages.find]
 where = src
 include = qaseio.*
 exclude = 
 	tests
```

### Comparing `qase-pytest-4.2.0/setup.py` & `qase-pytest-5.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     PyScaffold helps you to put up the scaffold of your new Python project.
     Learn more under: https://pyscaffold.org/
 """
 import sys
 from pkg_resources import VersionConflict, require
 from setuptools import setup
 
-VERSION = "4.2.0"
+VERSION = "5.0.0"
 
 try:
     require("setuptools>=38.3")
 except VersionConflict:
     print("Error: version of setuptools is too old (<38.3)!")
     sys.exit(1)
```

### Comparing `qase-pytest-4.2.0/src/qase_pytest.egg-info/PKG-INFO` & `qase-pytest-5.0.0/src/qase_pytest.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,111 @@
 Metadata-Version: 2.1
 Name: qase-pytest
-Version: 4.2.0
+Version: 5.0.0
 Summary: Qase Pytest Plugin for Qase TestOps and Qase Report
 Home-page: https://github.com/qase-tms/qase-python/tree/master/qase-pytest
 Author: Qase Team
 Author-email: support@qase.io
 License: apache
 Platform: any
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
 # [Qase](https://qase.io) Pytest Plugin
 
 [![License](https://lxgaming.github.io/badges/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 
-# Installation
+## Installation
 
 ```
 pip install qase-pytest
 ```
 
-# Usage
+## Upgrade from 4.x to 5.x
+A new version of qase-pytest reporter has breaking changes. Follow these [guide](UPGRADE.md) that will help you to migrate to a new version.
 
-### Command-line arguments
-Configuration could be provided both by `pytest.ini`/`tox.ini` params
-and using command-line arguments:
-
-* Command-line args:
-```
-  --qase-mode           Define mode: `testops` to enable report
-  --qase-environment=QS_ENVIRONMENT
-                        Define execution environment ID
-  --qase-to-api-token=QS_TO_API_TOKEN
-                        Api token for Qase TestOps
-  --qase-to-project=QS_TO_PROJECT
-                        Project code in Qase TestOps
-  --qase-to-run=QS_TO_RUN_ID
-                        Test Run ID in Qase TestOps
-  --qase-to-run-title=QS_TO_RUN_TITLE
-                        Define a custom title for Qase Test Run
-  --qase-to-plan=QS_TO_PLAN_ID
-                        Test Plan ID in Qase TestOps
-  --qase-to-complete-run
-                        Complete run after all tests are finished
-  --qase-to-mode=QS_TO_MODE
-                        You can choose `sync` or `async` mode for results publication. Default: `async`
-  --qase-to-host=QS_TO_HOST
-                        Qase TestOps Enterprise customers can set their own hosts. Default: `qase.io`
-```
-
-* INI file parameters:
-
-```
-  qs_mode (string):     default value for --qase-mode
-  qs_environment (string):
-                        default value for --qase-environment
-  qs_to_api_token (string):
-                        default value for --qase-to-api-token
-  qs_to_project (string):
-                        default value for --qase-to-project
-  qs_to_run_id (string):
-                        default value for --qase-to-run
-  qs_to_run_title (string):
-                        default value for --qase-to-run-title
-  qs_to_plan_id (string):
-                        default value for --qase-to-plan
-  qs_to_complete_run (bool):
-                        default value for --qase-to-complete-run
-  qs_to_mode (string):
-                        default value for --qase-to-mode
-  qs_to_host (string):
-                        default value for --qase-to-host
-    
+## Configuration
+
+Qase Pytest Plugin can be configured in multiple ways:
+ - using a config file `qase.config.json`
+ - using environment variables
+ - using CLI options
+
+All configuration options are listed in the following doc: [Configuration](../README.md#configuration).
+
+
+### Example: qase.config.json
+
+```
+{
+	"mode": "testops", 
+	"fallback": "report",
+	"report": {
+		"driver": "local",
+		"connection": {
+			"local": {
+				"path": "./build/qase-report",
+				"format": "json" 
+			}
+		}
+	},
+	"testops": {
+		"bulk": true,
+		"api": {
+			"token": "YOUR_API_TOKEN",
+			"host": "qase.io"
+		},
+		"run": {
+            "id": 1,
+			"title": "Test run title",
+			"complete": true
+		},
+        "plan": {
+            "id": 1
+        },
+		"defect": true,
+		"project": "YOUR_PROJECT_CODE",
+		"chunk": 200
+	},
+	"framework": {
+		"pytest": {
+			"capture": {
+				"logs": true,
+				"http": true
+			}
+		}
+	},
+	"environment": "local"
+}
 ```
 
-## Link tests with test cases in Qase TestOps
+## Usage
+
+### Link tests with test cases in Qase TestOps
 
 To link tests in code with tests in Qase TestOps you can use predefined decorators:
 
 ```python
 from qaseio.pytest import qase
 
 @qase.id(13)
 @qase.title("My first test")
-@qase.severity("critical")
-@qase.layer("unit")
-@qase.precondition("*Precondition 1*. Markdown is supported.")
-@qase.description("Try to login in Qase TestOps using login and password")
+@qase.fields(
+    ("severity", "critical"),
+    ("priority", "hight"),
+    ("layer", "unit"),
+    ("description", "Try to login in Qase TestOps using login and password"),
+    ("description", "*Precondition 1*. Markdown is supported."),
+)
 def test_example_1():
     pass
 ```
 
 Each unique number can only be assigned once to the class or function being used.
 
 ### Ignore a particular test
@@ -113,24 +122,28 @@
 ### Possible test result statuses
 
 - PASSED - when test passed
 - FAILED - when test failed with AssertionError
 - BLOCKED - when test failed with any other exception
 - SKIPPED - when test has been skipped
 
-## Add attachments to test results
+### Capture network logs
+In order to capture network logs, you need to enable the `http` option in the `capture` section of the `framework` section in the config file.
+
+Qase Pytest reporter will capture all requests and responses and save as a test step automatically.
+
+### Add attachments to test results
 
 When you need to push some additional information to server you could use
 attachments:
 
 ```python
 import pytest
 from qaseio.pytest import qase
 
-
 @pytest.fixture(scope="session")
 def driver():
     driver = webdriver.Chrome()
     yield driver
     logs = "\n".join(str(row) for row in driver.get_log('browser')).encode('utf-8')
     qase.attach((logs, "text/plain", "browser.log"))
     driver.quit()
@@ -153,30 +166,29 @@
 Also you should know, that if no case id is associated with current test in
 pytest - attachment would not be uploaded:
 
 ```python
 import pytest
 from qaseio.pytest import qase
 
-
 @pytest.fixture(scope="session")
 def driver():
     driver = webdriver.Chrome()
     yield driver
     logs = "\n".join(str(row) for row in driver.get_log('browser')).encode('utf-8')
     # This would do nothing, because last test does not have case id link
     qase.attach((logs, "text/plain", "browser.log"))
     driver.quit()
 
 def test_example_2(driver):
     # This would do nothing
     qase.attach((driver.get_screenshot_as_png(), "image/png", "result.png"))
 ```
 
-## Linking code with steps
+### Linking code with steps
 
 It is possible to link test step with function, or using context.
 
 ```python
 from qaseio.pytest import qase
 
 @qase.step("First step") # test step name
@@ -193,56 +205,48 @@
     some_step()
     another_step()
     # test step hash
     with qase.step("Third step"):
         sleep(1)
 ```
 
-## Sending tests to existing testrun
+### Sending tests to existing testrun
 
 Testrun in TestOps will contain only those test results, which are presented in testrun,
 but every test would be executed.
 
 ```bash
 pytest \
     --qase-mode=testops \
-    --qase-to-api-token=<your api token here> \
-    --qase-to-project=PRJCODE \ # project, where your testrun exists in
-    --qase-to-run=3 # testrun id
+    --qase-testops-api-token=<your api token here> \
+    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
+    --qase-testops-run-id=3 # testrun id
 ```
 
-## Creating test run base on test plan
+### Creating test run base on test plan (selective launch)
 
 Create new testrun base on testplan. Testrun in Qase TestOps will contain only those
-test results, which are presented in testrun, but every test would be executed.
+test results. `qase-pytest` supports selective execution
 
 ```bash
 pytest \
     --qase-mode=testops \
-    --qase-to-api-token=<your api token here> \
-    --qase-to-project=PRJCODE \ # project, where your testrun exists in
-    --qase-to-plan=3 # testplan id
+    --qase-testops-api-token=<your api token here> \
+    --qase-testops-project=PRJCODE \ # project, where your testrun exists in
+    --qase-testops-plan-id=3 # testplan id
 ```
 
-## Creating new testrun according to current pytest run
+### Creating new testrun according to current pytest run
 
 If you want to create a new test run in Qase TestOps for each execution, you can simply 
-skip `--qase-to-run`. If you want to provide a custom name for this run, you can add an
-option `--qase-to-run-title` 
+skip `--qase-testops-run` option. If you want to provide a custom name for this run, you can add an
+option `--qase-testops-run-title` 
 
 ```bash
 pytest \
     --qase-mode=testops \
-    --qase-to-api-token=<your api token here> \
-    --qase-to-project=PRJCODE \ # project, where your testrun would be created
-    --qase-to-run-title=My\ First\ Automated\ Run
+    --qase-testops-api-token=<your api token here> \
+    --qase-testops-project=PRJCODE \ # project, where your testrun would be created
+    --qase-testops-run-title=My\ First\ Automated\ Run
 ```
 
-## Qase TestOps submission mode
-
-Qase Pytest plugin for TestOps can work in two different modes: `sync` or `async`. 
-
-*Sync* sends each result to Qase TestOps API right after particular test execution. This mode allows you to see the results in realtime, even before test run is fully executed. 
-
-*Async* mode sends the results of test execution when the test run is complete. It uses bulk method that dramatically reduces reporting time.
-
```

### Comparing `qase-pytest-4.2.0/src/qase_pytest.egg-info/SOURCES.txt` & `qase-pytest-5.0.0/src/qase_pytest.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .coveragerc
 .gitignore
 .isort.cfg
 .pre-commit-config.yaml
 AUTHORS.rst
+CONFIGURATION.md
 LICENSE.txt
 README.md
+UPGRADE.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 example/test_example.py
 src/qase_pytest.egg-info/PKG-INFO
@@ -17,12 +19,13 @@
 src/qase_pytest.egg-info/entry_points.txt
 src/qase_pytest.egg-info/namespace_packages.txt
 src/qase_pytest.egg-info/not-zip-safe
 src/qase_pytest.egg-info/requires.txt
 src/qase_pytest.egg-info/top_level.txt
 src/qaseio/pytest/__init__.py
 src/qaseio/pytest/conftest.py
+src/qaseio/pytest/options.py
 src/qaseio/pytest/plugin.py
 tests/conftest.py
 tests/test_conftest.py
 tests/test_package.py
 tests/test_plugin.py
```

