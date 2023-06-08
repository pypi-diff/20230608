# Comparing `tmp/pytest-reportportal-5.1.8.tar.gz` & `tmp/pytest-reportportal-5.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-reportportal-5.1.8.tar", last modified: Wed May 24 15:16:41 2023, max compression
+gzip compressed data, was "pytest-reportportal-5.1.9.tar", last modified: Thu Jun  8 11:22:11 2023, max compression
```

## Comparing `pytest-reportportal-5.1.8.tar` & `pytest-reportportal-5.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:41.027979 pytest-reportportal-5.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-05-24 15:16:41.027979 pytest-reportportal-5.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9742 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:41.023979 pytest-reportportal-5.1.8/pytest_reportportal/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/config.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/rp_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    31887 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/pytest_reportportal/service.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 15:16:41.027979 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10467 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-24 15:16:41.000000 pytest-reportportal-5.1.8/pytest_reportportal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-24 15:16:41.027979 pytest-reportportal-5.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-24 15:16:33.000000 pytest-reportportal-5.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:22:11.452448 pytest-reportportal-5.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-06-08 11:22:11.452448 pytest-reportportal-5.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9858 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:22:11.452448 pytest-reportportal-5.1.9/pytest_reportportal/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/rp_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31902 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/pytest_reportportal/service.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:22:11.452448 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 11:22:11.000000 pytest-reportportal-5.1.9/pytest_reportportal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 11:22:11.452448 pytest-reportportal-5.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-08 11:21:54.000000 pytest-reportportal-5.1.9/setup.py
```

### Comparing `pytest-reportportal-5.1.8/CONTRIBUTING.rst` & `pytest-reportportal-5.1.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.8/LICENSE` & `pytest-reportportal-5.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.8/PKG-INFO` & `pytest-reportportal-5.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reportportal
-Version: 5.1.8
+Version: 5.1.9
 Summary: Agent for Reporting results of tests to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-pytest
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,pytest,agent
 Classifier: Framework :: Pytest
@@ -75,60 +75,58 @@
 .. code-block:: bash
 
     py.test -c config.cfg
 
 
 The :code:`pytest.ini` file should have next mandatory fields:
 
-- :code:`rp_uuid` - value could be found in the User Profile section
+- :code:`rp_api_key` - value could be found in the User Profile section
 - :code:`rp_project` - name of project in Report Portal
 - :code:`rp_endpoint` - address of Report Portal Server
 
 Example of :code:`pytest.ini`:
 
 .. code-block:: text
 
     [pytest]
-    rp_uuid = fb586627-32be-47dd-93c1-678873458a5f
+    rp_api_key = fb586627-32be-47dd-93c1-678873458a5f
     rp_endpoint = http://192.168.1.10:8080
     rp_project = user_personal
     rp_launch = AnyLaunchName
     rp_launch_attributes = 'PyTest' 'Smoke'
     rp_launch_description = 'Smoke test'
     rp_ignore_attributes = 'xfail' 'usefixture'
 
-- The :code:`rp_uuid` can also be set with the environment variable `RP_UUID`. This will override the value set for :code:`rp_uuid` in pytest.ini
+- The :code:`rp_api_key` can also be set with the environment variable `RP_API_KEY`. This will override the value set for :code:`rp_api_key` in pytest.ini
 
 The following parameters are optional:
 
-- :code:`rp_launch = AnyLaunchName` - launch name (could be overridden
-  by pytest --rp-launch option, default value is 'Pytest Launch')
-- :code:`rp_launch_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing launch (the session will not handle the lifecycle of the given launch)
-- :code:`rp_launch_attributes = 'PyTest' 'Smoke' 'Env:Python3'` - list of attributes for launch
-- :code:`rp_parent_item_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing test item for session to use as parent item for the tests (the session will not handle the lifecycle of the given test item)
-- :code:`rp_tests_attributes = 'PyTest' 'Smoke'` - list of attributes that will be added for each item in the launch
-- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden
-  by pytest --rp-launch-description option, default value is '')
-
-- :code:`rp_log_batch_size = 20` - size of batch log request
-- :code:`rp_log_batch_payload_size = 65000000` - maximum payload size in bytes of async batch log requests
-- :code:`rp_log_level = INFO` - The log level that will be reported
+- :code:`rp_launch = AnyLaunchName` - launch name (could be overridden by pytest --rp-launch option, default value is 'Pytest Launch').
+- :code:`rp_launch_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing launch (the session will not handle the lifecycle of the given launch).
+- :code:`rp_launch_attributes = 'PyTest' 'Smoke' 'Env:Python3'` - list of attributes for launch.
+- :code:`rp_parent_item_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing test item for session to use as parent item for the tests (the session will not handle the lifecycle of the given test item).
+- :code:`rp_tests_attributes = 'PyTest' 'Smoke'` - list of attributes that will be added for each item in the launch.
+- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden by pytest --rp-launch-description option, default value is '').
+- :code:`rp_log_batch_size = 20` - size of batch log request.
+- :code:`rp_log_batch_payload_size = 65000000` - maximum payload size in bytes of async batch log requests.
+- :code:`rp_log_level = INFO` - The log level that will be reported.
 - :code:`rp_log_format = [%(levelname)7s] (%(name)s) %(message)s (%(filename)s:%(lineno)s)` - Format string to be used for logs sent to the service.
-- :code:`rp_ignore_attributes = 'xfail' 'usefixture'` - Ignore specified pytest markers
+- :code:`rp_ignore_attributes = 'xfail' 'usefixture'` - Ignore specified pytest markers.
 - :code:`rp_is_skipped_an_issue = False` - Treat skipped tests as required investigation. Default is True.
-- :code:`rp_hierarchy_dirs_level = 0` - Directory starting hierarchy level (from pytest.ini level) (default `0`)
+- :code:`rp_hierarchy_dirs_level = 0` - Directory starting hierarchy level (from pytest.ini level) (default `0`).
 - :code:`rp_hierarchy_dirs = True` - Enables hierarchy for tests directories, default `False`. Doesn't support 'xdist' plugin.
-- :code:`rp_hierarchy_dir_path_separator` - Path separator to display directories in test hierarchy. In case of empty value current system path separator will be used (os.path.sep)
+- :code:`rp_hierarchy_dir_path_separator` - Path separator to display directories in test hierarchy. In case of empty value current system path separator will be used (os.path.sep).
 - :code:`rp_hierarchy_code` - Enables hierarchy for inner classes and parametrized tests, default `False`. Doesn't support 'xdist' plugin.
-- :code:`rp_issue_system_url = https://bugzilla.some.com/show_bug.cgi?id={issue_id}` - issue URL (issue_id will be filled by parameter from pytest mark)
-- :code:`rp_issue_id_marks = True` - Enables adding marks for issue ids (e.g. "issue:123456")
-- :code:`rp_verify_ssl = True` - Verify SSL when connecting to the server
-- :code:`rp_mode = DEFAULT` - DEBUG or DEFAULT launch mode. DEBUG launches are displayed in a separate tab and not visible to anyone except owner
+- :code:`rp_issue_system_url = https://bugzilla.some.com/show_bug.cgi?id={issue_id}` - issue URL (issue_id will be filled by parameter from pytest mark).
+- :code:`rp_issue_id_marks = True` - Enables adding marks for issue ids (e.g. "issue:123456").
+- :code:`rp_verify_ssl = True` - Verify SSL when connecting to the server.
+- :code:`rp_mode = DEFAULT` - DEBUG or DEFAULT launch mode. DEBUG launches are displayed in a separate tab and not visible to anyone except owner.
 - :code:`rp_thread_logging` - EXPERIMENTAL - Enables support for reporting logs from threads by patching the builtin Thread class. Use with caution.
-- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day)
+- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day).
+- :code:`rp_api_retries = 0` - Amount of retries for performing REST calls to RP server.
 
 
 
 If you like to override the above parameters from command line, or from CI environment based on your build, then pass
 - :code:`-o "rp_launch_attributes=Smoke Tests"` during invocation.
 
 Examples
```

### Comparing `pytest-reportportal-5.1.8/README.rst` & `pytest-reportportal-5.1.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -56,60 +56,58 @@
 .. code-block:: bash
 
     py.test -c config.cfg
 
 
 The :code:`pytest.ini` file should have next mandatory fields:
 
-- :code:`rp_uuid` - value could be found in the User Profile section
+- :code:`rp_api_key` - value could be found in the User Profile section
 - :code:`rp_project` - name of project in Report Portal
 - :code:`rp_endpoint` - address of Report Portal Server
 
 Example of :code:`pytest.ini`:
 
 .. code-block:: text
 
     [pytest]
-    rp_uuid = fb586627-32be-47dd-93c1-678873458a5f
+    rp_api_key = fb586627-32be-47dd-93c1-678873458a5f
     rp_endpoint = http://192.168.1.10:8080
     rp_project = user_personal
     rp_launch = AnyLaunchName
     rp_launch_attributes = 'PyTest' 'Smoke'
     rp_launch_description = 'Smoke test'
     rp_ignore_attributes = 'xfail' 'usefixture'
 
-- The :code:`rp_uuid` can also be set with the environment variable `RP_UUID`. This will override the value set for :code:`rp_uuid` in pytest.ini
+- The :code:`rp_api_key` can also be set with the environment variable `RP_API_KEY`. This will override the value set for :code:`rp_api_key` in pytest.ini
 
 The following parameters are optional:
 
-- :code:`rp_launch = AnyLaunchName` - launch name (could be overridden
-  by pytest --rp-launch option, default value is 'Pytest Launch')
-- :code:`rp_launch_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing launch (the session will not handle the lifecycle of the given launch)
-- :code:`rp_launch_attributes = 'PyTest' 'Smoke' 'Env:Python3'` - list of attributes for launch
-- :code:`rp_parent_item_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing test item for session to use as parent item for the tests (the session will not handle the lifecycle of the given test item)
-- :code:`rp_tests_attributes = 'PyTest' 'Smoke'` - list of attributes that will be added for each item in the launch
-- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden
-  by pytest --rp-launch-description option, default value is '')
-
-- :code:`rp_log_batch_size = 20` - size of batch log request
-- :code:`rp_log_batch_payload_size = 65000000` - maximum payload size in bytes of async batch log requests
-- :code:`rp_log_level = INFO` - The log level that will be reported
+- :code:`rp_launch = AnyLaunchName` - launch name (could be overridden by pytest --rp-launch option, default value is 'Pytest Launch').
+- :code:`rp_launch_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing launch (the session will not handle the lifecycle of the given launch).
+- :code:`rp_launch_attributes = 'PyTest' 'Smoke' 'Env:Python3'` - list of attributes for launch.
+- :code:`rp_parent_item_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing test item for session to use as parent item for the tests (the session will not handle the lifecycle of the given test item).
+- :code:`rp_tests_attributes = 'PyTest' 'Smoke'` - list of attributes that will be added for each item in the launch.
+- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden by pytest --rp-launch-description option, default value is '').
+- :code:`rp_log_batch_size = 20` - size of batch log request.
+- :code:`rp_log_batch_payload_size = 65000000` - maximum payload size in bytes of async batch log requests.
+- :code:`rp_log_level = INFO` - The log level that will be reported.
 - :code:`rp_log_format = [%(levelname)7s] (%(name)s) %(message)s (%(filename)s:%(lineno)s)` - Format string to be used for logs sent to the service.
-- :code:`rp_ignore_attributes = 'xfail' 'usefixture'` - Ignore specified pytest markers
+- :code:`rp_ignore_attributes = 'xfail' 'usefixture'` - Ignore specified pytest markers.
 - :code:`rp_is_skipped_an_issue = False` - Treat skipped tests as required investigation. Default is True.
-- :code:`rp_hierarchy_dirs_level = 0` - Directory starting hierarchy level (from pytest.ini level) (default `0`)
+- :code:`rp_hierarchy_dirs_level = 0` - Directory starting hierarchy level (from pytest.ini level) (default `0`).
 - :code:`rp_hierarchy_dirs = True` - Enables hierarchy for tests directories, default `False`. Doesn't support 'xdist' plugin.
-- :code:`rp_hierarchy_dir_path_separator` - Path separator to display directories in test hierarchy. In case of empty value current system path separator will be used (os.path.sep)
+- :code:`rp_hierarchy_dir_path_separator` - Path separator to display directories in test hierarchy. In case of empty value current system path separator will be used (os.path.sep).
 - :code:`rp_hierarchy_code` - Enables hierarchy for inner classes and parametrized tests, default `False`. Doesn't support 'xdist' plugin.
-- :code:`rp_issue_system_url = https://bugzilla.some.com/show_bug.cgi?id={issue_id}` - issue URL (issue_id will be filled by parameter from pytest mark)
-- :code:`rp_issue_id_marks = True` - Enables adding marks for issue ids (e.g. "issue:123456")
-- :code:`rp_verify_ssl = True` - Verify SSL when connecting to the server
-- :code:`rp_mode = DEFAULT` - DEBUG or DEFAULT launch mode. DEBUG launches are displayed in a separate tab and not visible to anyone except owner
+- :code:`rp_issue_system_url = https://bugzilla.some.com/show_bug.cgi?id={issue_id}` - issue URL (issue_id will be filled by parameter from pytest mark).
+- :code:`rp_issue_id_marks = True` - Enables adding marks for issue ids (e.g. "issue:123456").
+- :code:`rp_verify_ssl = True` - Verify SSL when connecting to the server.
+- :code:`rp_mode = DEFAULT` - DEBUG or DEFAULT launch mode. DEBUG launches are displayed in a separate tab and not visible to anyone except owner.
 - :code:`rp_thread_logging` - EXPERIMENTAL - Enables support for reporting logs from threads by patching the builtin Thread class. Use with caution.
-- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day)
+- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day).
+- :code:`rp_api_retries = 0` - Amount of retries for performing REST calls to RP server.
 
 
 
 If you like to override the above parameters from command line, or from CI environment based on your build, then pass
 - :code:`-o "rp_launch_attributes=Smoke Tests"` during invocation.
 
 Examples
```

### Comparing `pytest-reportportal-5.1.8/pytest_reportportal/config.py` & `pytest-reportportal-5.1.9/pytest_reportportal/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module contains class that stores RP agent configuration data."""
+import warnings
 
 from distutils.util import strtobool
 from os import getenv
 
 from reportportal_client.logs.log_manager import MAX_LOG_BATCH_PAYLOAD_SIZE
 
 try:
@@ -65,22 +66,63 @@
         self.rp_mode = self.find_option(pytest_config, 'rp_mode')
         self.rp_parent_item_id = self.find_option(pytest_config,
                                                   'rp_parent_item_id')
         self.rp_project = self.find_option(pytest_config,
                                            'rp_project')
         self.rp_rerun_of = self.find_option(pytest_config,
                                             'rp_rerun_of')
-        self.rp_retries = int(self.find_option(pytest_config,
-                                               'retries'))
         self.rp_skip_connection_test = str(
             self.find_option(pytest_config,
                              'rp_skip_connection_test')).lower() in (
                                            'true', '1', 'yes', 'y')
-        self.rp_uuid = getenv('RP_UUID') or self.find_option(pytest_config,
-                                                             'rp_uuid')
+
+        rp_api_retries_str = self.find_option(pytest_config, 'rp_api_retries')
+        rp_api_retries = rp_api_retries_str and int(rp_api_retries_str)
+        if rp_api_retries and rp_api_retries > 0:
+            self.rp_api_retries = rp_api_retries
+        else:
+            rp_api_retries_str = self.find_option(pytest_config, 'retries')
+            rp_api_retries = rp_api_retries_str and int(rp_api_retries_str)
+            if rp_api_retries and rp_api_retries > 0:
+                self.rp_api_retries = rp_api_retries
+                warnings.warn(
+                    'Parameter `retries` is deprecated since 5.1.9 '
+                    'and will be subject for removing in the next '
+                    'major version. Use `rp_api_retries` argument '
+                    'instead.',
+                    DeprecationWarning,
+                    2
+                )
+            else:
+                self.rp_api_retries = 0
+
+        self.rp_api_key = getenv(
+            'RP_API_KEY') or self.find_option(pytest_config, 'rp_api_key')
+        if not self.rp_api_key:
+            self.rp_api_key = getenv(
+                'RP_UUID') or self.find_option(pytest_config, 'rp_uuid')
+            if self.rp_api_key:
+                warnings.warn(
+                    'Parameter `rp_uuid` is deprecated since 5.1.9 '
+                    'and will be subject for removing in the next '
+                    'major version. Use `rp_api_key` argument '
+                    'instead.',
+                    DeprecationWarning,
+                    2
+                )
+            else:
+                warnings.warn(
+                    'Argument `rp_api_key` is `None` or empty string, '
+                    'that is not supposed to happen because Report '
+                    'Portal is usually requires an authorization key. '
+                    'Please check your configuration.',
+                    RuntimeWarning,
+                    2
+                )
+
         rp_verify_ssl = self.find_option(pytest_config, 'rp_verify_ssl', True)
         try:
             self.rp_verify_ssl = bool(strtobool(rp_verify_ssl))
         except (ValueError, AttributeError):
             self.rp_verify_ssl = rp_verify_ssl
         self.rp_launch_timeout = int(
             self.find_option(pytest_config, 'rp_launch_timeout'))
```

### Comparing `pytest-reportportal-5.1.8/pytest_reportportal/config.pyi` & `pytest-reportportal-5.1.9/pytest_reportportal/config.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     rp_log_batch_payload_size: int
     rp_log_level: Optional[int]
     rp_log_format: Optional[Text]
     rp_mode: Text
     rp_parent_item_id: Optional[Text]
     rp_project: Text
     rp_rerun_of: Optional[Text]
-    rp_retries: int
+    rp_api_retries: int
     rp_skip_connection_test: bool
-    rp_uuid: Text
+    rp_api_key: Text
     rp_verify_ssl: Union[bool, Text]
     rp_launch_timeout: int
 
     def __init__(self, pytest_config: Config) -> None: ...
 
     def find_option(self, pytest_config, param: Text,
                     default: Any = ...) -> Union[Text, bool, list]: ...
```

### Comparing `pytest-reportportal-5.1.8/pytest_reportportal/plugin.py` & `pytest-reportportal-5.1.9/pytest_reportportal/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 log = logging.getLogger(__name__)
 
 MANDATORY_PARAMETER_MISSED_PATTERN = \
     'One of the following mandatory parameters is unset: ' + \
     'rp_project: {}, ' + \
     'rp_endpoint: {}, ' + \
-    'rp_uuid: {}'
+    'rp_api_key: {}'
 
 FAILED_LAUNCH_WAIT = 'Failed to initialize reportportal-client service. ' \
                      + 'Waiting for Launch start timed out. ' \
                      + 'Reporting is disabled.'
 
 
 @pytest.hookimpl(optionalhook=True)
@@ -168,15 +168,15 @@
 
     If connection is successful returns True either False.
     :param agent_config: Instance of the AgentConfig class
     :return True on successful connection check, either False
     """
     url = '{0}/api/v1/project/{1}'.format(agent_config.rp_endpoint,
                                           agent_config.rp_project)
-    headers = {'Authorization': 'bearer {0}'.format(agent_config.rp_uuid)}
+    headers = {'Authorization': 'bearer {0}'.format(agent_config.rp_api_key)}
     try:
         resp = requests.get(url, headers=headers,
                             verify=agent_config.rp_verify_ssl)
         resp.raise_for_status()
         return True
     except requests.exceptions.RequestException as exc:
         log.exception(exc)
@@ -199,15 +199,15 @@
             not config.option.rp_enabled)
     if not config._rp_enabled:
         return
 
     agent_config = AgentConfig(config)
 
     cond = (agent_config.rp_project, agent_config.rp_endpoint,
-            agent_config.rp_uuid)
+            agent_config.rp_api_key)
     config._rp_enabled = all(cond)
     if not config._rp_enabled:
         log.debug(MANDATORY_PARAMETER_MISSED_PATTERN.format(*cond))
         log.debug('Disabling reporting to RP.')
         return
 
     if not agent_config.rp_skip_connection_test:
@@ -375,15 +375,21 @@
         default='',
     )
     add_shared_option(
         name='rp_parent_item_id',
         help_str='Create all test item as child items of the given (already '
                  'existing) item.',
     )
-    add_shared_option(name='rp_uuid', help_str='UUID')
+    add_shared_option(name='rp_uuid', help_str='Deprecated: use `rp_api_key` '
+                      'instead.')
+    add_shared_option(
+        name='rp_api_key',
+        help_str='API key of Report Portal. Usually located on UI profile '
+                 'page.'
+    )
     add_shared_option(name='rp_endpoint', help_str='Server endpoint')
     add_shared_option(
         name='rp_mode',
         help_str='Visibility of current launch [DEFAULT, DEBUG]',
         default='DEFAULT'
     )
     add_shared_option(
@@ -464,14 +470,18 @@
         'rp_issue_id_marks',
         type='bool',
         default=True,
         help='Add tag with issue id to the test')
     parser.addini(
         'retries',
         default='0',
+        help='Deprecated: use `rp_api_retries` instead')
+    parser.addini(
+        'rp_api_retries',
+        default='0',
         help='Amount of retries for performing REST calls to RP server')
     parser.addini(
         'rp_skip_connection_test',
         default=False,
         type='bool',
         help='Skip Report Portal connection test')
     parser.addini(
```

### Comparing `pytest-reportportal-5.1.8/pytest_reportportal/plugin.pyi` & `pytest-reportportal-5.1.9/pytest_reportportal/plugin.pyi`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.8/pytest_reportportal/rp_logging.py` & `pytest-reportportal-5.1.9/pytest_reportportal/rp_logging.py`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.8/pytest_reportportal/service.py` & `pytest-reportportal-5.1.9/pytest_reportportal/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -855,26 +855,26 @@
         self.parent_item_id = self._config.rp_parent_item_id
         self.ignored_attributes = list(
             set(
                 self._config.rp_ignore_attributes or []
             ).union({'parametrize'})
         )
         log.debug('ReportPortal - Init service: endpoint=%s, '
-                  'project=%s, uuid=%s', self._config.rp_endpoint,
-                  self._config.rp_project, self._config.rp_uuid)
+                  'project=%s, api_key=%s', self._config.rp_endpoint,
+                  self._config.rp_project, self._config.rp_api_key)
         launch_id = self._launch_id
         if self._config.rp_launch_id:
             launch_id = self._config.rp_launch_id
         self.rp = RPClient(
             endpoint=self._config.rp_endpoint,
             project=self._config.rp_project,
-            token=self._config.rp_uuid,
+            api_key=self._config.rp_api_key,
             is_skipped_an_issue=self._config.rp_is_skipped_an_issue,
             log_batch_size=self._config.rp_log_batch_size,
-            retries=self._config.rp_retries,
+            retries=self._config.rp_api_retries,
             verify_ssl=self._config.rp_verify_ssl,
             launch_id=launch_id,
             log_batch_payload_size=self._config.rp_log_batch_payload_size
         )
         if hasattr(self.rp, "get_project_settings"):
             self.project_settings = self.rp.get_project_settings()
         self.rp.start()
```

### Comparing `pytest-reportportal-5.1.8/pytest_reportportal/service.pyi` & `pytest-reportportal-5.1.9/pytest_reportportal/service.pyi`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.8/pytest_reportportal.egg-info/PKG-INFO` & `pytest-reportportal-5.1.9/pytest_reportportal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-reportportal
-Version: 5.1.8
+Version: 5.1.9
 Summary: Agent for Reporting results of tests to the Report Portal
 Home-page: https://github.com/reportportal/agent-python-pytest
 Author: Report Portal Team
 Author-email: support@reportportal.io
 License: Apache 2.0
 Keywords: testing,reporting,reportportal,pytest,agent
 Classifier: Framework :: Pytest
@@ -75,60 +75,58 @@
 .. code-block:: bash
 
     py.test -c config.cfg
 
 
 The :code:`pytest.ini` file should have next mandatory fields:
 
-- :code:`rp_uuid` - value could be found in the User Profile section
+- :code:`rp_api_key` - value could be found in the User Profile section
 - :code:`rp_project` - name of project in Report Portal
 - :code:`rp_endpoint` - address of Report Portal Server
 
 Example of :code:`pytest.ini`:
 
 .. code-block:: text
 
     [pytest]
-    rp_uuid = fb586627-32be-47dd-93c1-678873458a5f
+    rp_api_key = fb586627-32be-47dd-93c1-678873458a5f
     rp_endpoint = http://192.168.1.10:8080
     rp_project = user_personal
     rp_launch = AnyLaunchName
     rp_launch_attributes = 'PyTest' 'Smoke'
     rp_launch_description = 'Smoke test'
     rp_ignore_attributes = 'xfail' 'usefixture'
 
-- The :code:`rp_uuid` can also be set with the environment variable `RP_UUID`. This will override the value set for :code:`rp_uuid` in pytest.ini
+- The :code:`rp_api_key` can also be set with the environment variable `RP_API_KEY`. This will override the value set for :code:`rp_api_key` in pytest.ini
 
 The following parameters are optional:
 
-- :code:`rp_launch = AnyLaunchName` - launch name (could be overridden
-  by pytest --rp-launch option, default value is 'Pytest Launch')
-- :code:`rp_launch_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing launch (the session will not handle the lifecycle of the given launch)
-- :code:`rp_launch_attributes = 'PyTest' 'Smoke' 'Env:Python3'` - list of attributes for launch
-- :code:`rp_parent_item_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing test item for session to use as parent item for the tests (the session will not handle the lifecycle of the given test item)
-- :code:`rp_tests_attributes = 'PyTest' 'Smoke'` - list of attributes that will be added for each item in the launch
-- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden
-  by pytest --rp-launch-description option, default value is '')
-
-- :code:`rp_log_batch_size = 20` - size of batch log request
-- :code:`rp_log_batch_payload_size = 65000000` - maximum payload size in bytes of async batch log requests
-- :code:`rp_log_level = INFO` - The log level that will be reported
+- :code:`rp_launch = AnyLaunchName` - launch name (could be overridden by pytest --rp-launch option, default value is 'Pytest Launch').
+- :code:`rp_launch_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing launch (the session will not handle the lifecycle of the given launch).
+- :code:`rp_launch_attributes = 'PyTest' 'Smoke' 'Env:Python3'` - list of attributes for launch.
+- :code:`rp_parent_item_id = xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx` - id of the existing test item for session to use as parent item for the tests (the session will not handle the lifecycle of the given test item).
+- :code:`rp_tests_attributes = 'PyTest' 'Smoke'` - list of attributes that will be added for each item in the launch.
+- :code:`rp_launch_description = 'Smoke test'` - launch description (could be overridden by pytest --rp-launch-description option, default value is '').
+- :code:`rp_log_batch_size = 20` - size of batch log request.
+- :code:`rp_log_batch_payload_size = 65000000` - maximum payload size in bytes of async batch log requests.
+- :code:`rp_log_level = INFO` - The log level that will be reported.
 - :code:`rp_log_format = [%(levelname)7s] (%(name)s) %(message)s (%(filename)s:%(lineno)s)` - Format string to be used for logs sent to the service.
-- :code:`rp_ignore_attributes = 'xfail' 'usefixture'` - Ignore specified pytest markers
+- :code:`rp_ignore_attributes = 'xfail' 'usefixture'` - Ignore specified pytest markers.
 - :code:`rp_is_skipped_an_issue = False` - Treat skipped tests as required investigation. Default is True.
-- :code:`rp_hierarchy_dirs_level = 0` - Directory starting hierarchy level (from pytest.ini level) (default `0`)
+- :code:`rp_hierarchy_dirs_level = 0` - Directory starting hierarchy level (from pytest.ini level) (default `0`).
 - :code:`rp_hierarchy_dirs = True` - Enables hierarchy for tests directories, default `False`. Doesn't support 'xdist' plugin.
-- :code:`rp_hierarchy_dir_path_separator` - Path separator to display directories in test hierarchy. In case of empty value current system path separator will be used (os.path.sep)
+- :code:`rp_hierarchy_dir_path_separator` - Path separator to display directories in test hierarchy. In case of empty value current system path separator will be used (os.path.sep).
 - :code:`rp_hierarchy_code` - Enables hierarchy for inner classes and parametrized tests, default `False`. Doesn't support 'xdist' plugin.
-- :code:`rp_issue_system_url = https://bugzilla.some.com/show_bug.cgi?id={issue_id}` - issue URL (issue_id will be filled by parameter from pytest mark)
-- :code:`rp_issue_id_marks = True` - Enables adding marks for issue ids (e.g. "issue:123456")
-- :code:`rp_verify_ssl = True` - Verify SSL when connecting to the server
-- :code:`rp_mode = DEFAULT` - DEBUG or DEFAULT launch mode. DEBUG launches are displayed in a separate tab and not visible to anyone except owner
+- :code:`rp_issue_system_url = https://bugzilla.some.com/show_bug.cgi?id={issue_id}` - issue URL (issue_id will be filled by parameter from pytest mark).
+- :code:`rp_issue_id_marks = True` - Enables adding marks for issue ids (e.g. "issue:123456").
+- :code:`rp_verify_ssl = True` - Verify SSL when connecting to the server.
+- :code:`rp_mode = DEFAULT` - DEBUG or DEFAULT launch mode. DEBUG launches are displayed in a separate tab and not visible to anyone except owner.
 - :code:`rp_thread_logging` - EXPERIMENTAL - Enables support for reporting logs from threads by patching the builtin Thread class. Use with caution.
-- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day)
+- :code:`rp_launch_timeout = 86400` - Maximum time to wait for child processes finish, default value: 86400 seconds (1 day).
+- :code:`rp_api_retries = 0` - Amount of retries for performing REST calls to RP server.
 
 
 
 If you like to override the above parameters from command line, or from CI environment based on your build, then pass
 - :code:`-o "rp_launch_attributes=Smoke Tests"` during invocation.
 
 Examples
```

### Comparing `pytest-reportportal-5.1.8/pytest_reportportal.egg-info/SOURCES.txt` & `pytest-reportportal-5.1.9/pytest_reportportal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-reportportal-5.1.8/setup.py` & `pytest-reportportal-5.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Config for setup package pytest agent."""
 
 import os
 
 from setuptools import setup
 
 
-__version__ = '5.1.8'
+__version__ = '5.1.9'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Filename to be read
     :return:      File content
```

