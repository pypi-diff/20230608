# Comparing `tmp/galaxy-job-execution-22.1.1.tar.gz` & `tmp/galaxy-job-execution-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-job-execution-22.1.1.tar", last modified: Mon Aug 22 19:45:51 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/job_execution/dist/.tmp-zc_1j6wx/galaxy-job-execution-23.0.1.tar", last modified: Thu Jun  8 17:43:33 2023, max compression
```

## Comparing `galaxy-job-execution-22.1.1.tar` & `galaxy-job-execution-23.0.1.tar`

### file list

```diff
@@ -1,48 +1,36 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:51.047204 galaxy-job-execution-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      332 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-job-execution-22.1.1/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       29 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1695 2022-08-22 19:45:51.047334 galaxy-job-execution-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      323 2022-03-24 19:47:11.000000 galaxy-job-execution-22.1.1/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:51.040428 galaxy-job-execution-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/galaxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:51.041731 galaxy-job-execution-22.1.1/galaxy/job_execution/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:10.000000 galaxy-job-execution-22.1.1/galaxy/job_execution/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:51.042259 galaxy-job-execution-22.1.1/galaxy/job_execution/actions/
--rw-r--r--   0 mvandenb   (501) staff       (20)       51 2022-08-18 15:49:02.000000 galaxy-job-execution-22.1.1/galaxy/job_execution/actions/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    24276 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/galaxy/job_execution/actions/post.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4618 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/galaxy/job_execution/compute_environment.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4541 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/galaxy/job_execution/datasets.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    31359 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/galaxy/job_execution/output_collect.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:51.042832 galaxy-job-execution-22.1.1/galaxy/job_execution/ports/
--rw-r--r--   0 mvandenb   (501) staff       (20)       61 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/galaxy/job_execution/ports/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1623 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/galaxy/job_execution/ports/view.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    10325 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/galaxy/job_execution/setup.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:51.043357 galaxy-job-execution-22.1.1/galaxy/metadata/
--rw-r--r--   0 mvandenb   (501) staff       (20)    13439 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/galaxy/metadata/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    23284 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/galaxy/metadata/set_metadata.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      440 2022-08-22 19:45:29.000000 galaxy-job-execution-22.1.1/galaxy/project_galaxy_job_execution.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:51.045171 galaxy-job-execution-22.1.1/galaxy_job_execution.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1695 2022-08-22 19:45:50.000000 galaxy-job-execution-22.1.1/galaxy_job_execution.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     1096 2022-08-22 19:45:50.000000 galaxy-job-execution-22.1.1/galaxy_job_execution.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:50.000000 galaxy-job-execution-22.1.1/galaxy_job_execution.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       97 2022-08-22 19:45:50.000000 galaxy-job-execution-22.1.1/galaxy_job_execution.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:50.000000 galaxy-job-execution-22.1.1/galaxy_job_execution.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)       12 2022-08-22 19:45:50.000000 galaxy-job-execution-22.1.1/galaxy_job_execution.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-08-22 19:45:50.000000 galaxy-job-execution-22.1.1/galaxy_job_execution.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       12 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:51.045955 galaxy-job-execution-22.1.1/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:45:51.054194 galaxy-job-execution-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2866 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-03-24 19:47:11.000000 galaxy-job-execution-22.1.1/test-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:51.046245 galaxy-job-execution-22.1.1/tests/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-08-18 15:49:03.000000 galaxy-job-execution-22.1.1/tests/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:51.046913 galaxy-job-execution-22.1.1/tests/job_execution/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-08-18 15:49:03.000000 galaxy-job-execution-22.1.1/tests/job_execution/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      879 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/tests/job_execution/test_datasets.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2794 2022-08-22 19:45:28.000000 galaxy-job-execution-22.1.1/tests/job_execution/test_job_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-job-execution-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25169 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/actions/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/compute_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/container_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32009 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/output_collect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/ports/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/ports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/ports/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/job_execution/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26492 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/metadata/set_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy_job_execution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy_job_execution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy_job_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy_job_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy_job_execution.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy_job_execution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/galaxy_job_execution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-08 17:43:33.000000 galaxy-job-execution-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:37:04.000000 galaxy-job-execution-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-job-execution-22.1.1/LICENSE` & `galaxy-job-execution-23.0.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,61 @@
-Copyright (c) 2005-2016 Galaxy Contributors (see CONTRIBUTORS.md)
+Copyright (c) 2005-2022 Galaxy Contributors (see CONTRIBUTORS.md)
+
+Work contributed from 2021-04-07 onwards is licensed under the MIT License.
+Work contributed before this date is licensed under the Academic Free License
+version 3.0.
+See https://github.com/galaxyproject/galaxy/ for the contribution history.
+See below for the full text of both licenses.
+
+
+Some icons found in Galaxy are from the Silk Icons set, available under
+the Creative Commons Attribution 2.5 License, from:
+
+http://www.famfamfam.com/lab/icons/silk/
+
+
+Other images and documentation are licensed under the Creative Commons
+Attribution 3.0 (CC BY 3.0) License. See:
+
+http://creativecommons.org/licenses/by/3.0/
+
+
+--------------------------------------------------------------------------------
+
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+--------------------------------------------------------------------------------
+
+
+Academic Free License ("AFL") v. 3.0
+
+This Academic Free License (the "License") applies to any original work of
+authorship (the "Original Work") whose owner (the "Licensor") has placed the
+following licensing notice adjacent to the copyright notice for the Original
+Work:
 
 Licensed under the Academic Free License version 3.0
 
  1) Grant of Copyright License. Licensor grants You a worldwide, royalty-free, 
     non-exclusive, sublicensable license, for the duration of the copyright, to 
     do the following:
 
@@ -169,18 +222,7 @@
     replace the notice specified in the first paragraph above with the 
     notice "Licensed under <insert your license name here>" or with a notice 
     of your own that is not confusingly similar to the notice in this 
     License; and (iii) You may not claim that your original works are open 
     source software unless your Modified License has been approved by Open 
     Source Initiative (OSI) and You comply with its license review and 
     certification process.
-
-
-Some icons found in Galaxy are from the Silk Icons set, available under
-the Creative Commons Attribution 2.5 License, from:
-
-http://www.famfamfam.com/lab/icons/silk/
-
-
-Other images and documentation are licensed under the Creative Commons Attribution 3.0 (CC BY 3.0) License.   See 
-
-http://creativecommons.org/licenses/by/3.0/
```

### Comparing `galaxy-job-execution-22.1.1/PKG-INFO` & `galaxy-job-execution-23.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,64 @@
 Metadata-Version: 2.1
 Name: galaxy-job-execution
-Version: 22.1.1
-Summary: Galaxy Job Execution Runtime Utilities
+Version: 23.0.1
+Summary: Galaxy job execution runtime utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-job-execution.svg
    :target: https://pypi.org/project/galaxy-job-execution/
 
 
 Overview
 --------
 
 The Galaxy_ job execution runtime module.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
-
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
+No recorded changes since last release
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
-
-
```

### Comparing `galaxy-job-execution-22.1.1/galaxy/job_execution/actions/post.py` & `galaxy-job-execution-23.0.1/galaxy/job_execution/actions/post.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,72 +16,87 @@
 log = get_logger(__name__)
 
 
 class DefaultJobAction:
     """
     Base job action.
     """
+
     name = "DefaultJobAction"
     verbose_name = "Default Job"
 
     @classmethod
     def execute(cls, app, sa_session, action, job, replacement_dict=None, final_job_state=None):
         pass
 
     @classmethod
-    def execute_on_mapped_over(cls, trans, sa_session, action, step_inputs, step_outputs, replacement_dict, final_job_state=None):
+    def execute_on_mapped_over(
+        cls, trans, sa_session, action, step_inputs, step_outputs, replacement_dict, final_job_state=None
+    ):
         pass
 
     @classmethod
     def get_short_str(cls, pja):
         if pja.action_arguments:
             return f"{pja.action_type} -> {escape(pja.action_arguments)}"
         else:
             return f"{pja.action_type}"
 
 
 class EmailAction(DefaultJobAction):
     """
     This action sends an email to the galaxy user responsible for a job.
     """
+
     name = "EmailAction"
     verbose_name = "Email Notification"
 
     @classmethod
     def execute(cls, app, sa_session, action, job, replacement_dict, final_job_state=None):
         try:
             frm = app.config.email_from
             history_id_encoded = app.security.encode_id(job.history_id)
+            link_invocation = None
+            if job.workflow_invocation_step:
+                invocation_id_encoded = app.security.encode_id(job.workflow_invocation_step.workflow_invocation_id)
+                link_invocation = (
+                    f"{app.config.galaxy_infrastructure_url}/workflows/invocations/report?id={invocation_id_encoded}"
+                )
             link = f"{app.config.galaxy_infrastructure_url}/histories/view?id={history_id_encoded}"
             if frm is None:
-                if action.action_arguments and 'host' in action.action_arguments:
-                    host = action.action_arguments['host']
+                if action.action_arguments and "host" in action.action_arguments:
+                    host = action.action_arguments["host"]
                 else:
                     host = socket.getfqdn()
-                frm = f'galaxy-no-reply@{host}'
+                frm = f"galaxy-no-reply@{host}"
             to = job.get_user_email()
             subject = f"Galaxy job completion notification from history '{job.history.name}'"
-            outdata = ',\n'.join(ds.dataset.display_name() for ds in job.output_datasets)
+            outdata = ",\n".join(ds.dataset.display_name() for ds in job.output_datasets)
             body = f"Your Galaxy job generating dataset(s):\n\n{outdata}\n\nis complete as of {datetime.datetime.now().strftime('%I:%M')}. Click the link below to access your data: \n{link}"
+            if link_invocation:
+                body += f"\n\nWorkflow Invocation Report:\n{link_invocation}"
             send_mail(frm, to, subject, body, app.config)
         except Exception as e:
             log.error("EmailAction PJA Failed, exception: %s", unicodify(e))
 
     @classmethod
     def get_short_str(cls, pja):
-        if pja.action_arguments and 'host' in pja.action_arguments:
-            return f"Email the current user from server {escape(pja.action_arguments['host'])} when this job is complete."
+        if pja.action_arguments and "host" in pja.action_arguments:
+            return (
+                f"Email the current user from server {escape(pja.action_arguments['host'])} when this job is complete."
+            )
         else:
             return "Email the current user when this job is complete."
 
 
 class ValidateOutputsAction(DefaultJobAction):
     """
     This action validates the produced outputs against the expected datatype.
     """
+
     name = "ValidateOutputsAction"
     verbose_name = "Validate Tool Outputs"
 
     @classmethod
     def execute(cls, app, sa_session, action, job, replacement_dict, final_job_state=None):
         # no-op: needs to inject metadata handling parameters ahead of time.
         pass
@@ -93,55 +108,61 @@
 
 class ChangeDatatypeAction(DefaultJobAction):
     name = "ChangeDatatypeAction"
     verbose_name = "Change Datatype"
 
     @classmethod
     def execute(cls, app, sa_session, action, job, replacement_dict, final_job_state=None):
+        if job.state == job.states.SKIPPED:
+            # Don't change datatype, must remain expression.json
+            return
         for dataset_assoc in job.output_datasets:
-            if action.output_name == '' or dataset_assoc.name == action.output_name:
-                app.datatypes_registry.change_datatype(dataset_assoc.dataset, action.action_arguments['newtype'])
+            if action.output_name == "" or dataset_assoc.name == action.output_name:
+                app.datatypes_registry.change_datatype(dataset_assoc.dataset, action.action_arguments["newtype"])
         for dataset_collection_assoc in job.output_dataset_collection_instances:
-            if action.output_name == '' or dataset_collection_assoc.name == action.output_name:
+            if action.output_name == "" or dataset_collection_assoc.name == action.output_name:
                 for dataset_instance in dataset_collection_assoc.dataset_collection_instance.dataset_instances:
                     if dataset_instance:
-                        app.datatypes_registry.change_datatype(dataset_instance, action.action_arguments['newtype'])
+                        app.datatypes_registry.change_datatype(dataset_instance, action.action_arguments["newtype"])
 
     @classmethod
     def get_short_str(cls, pja):
-        return "Set the datatype of output '{}' to '{}'".format(escape(pja.output_name),
-                                                            escape(pja.action_arguments['newtype']))
+        return "Set the datatype of output '{}' to '{}'".format(
+            escape(pja.output_name), escape(pja.action_arguments["newtype"])
+        )
 
 
 class RenameDatasetAction(DefaultJobAction):
     name = "RenameDatasetAction"
     verbose_name = "Rename Dataset"
 
     @classmethod
-    def execute_on_mapped_over(cls, trans, sa_session, action, step_inputs, step_outputs, replacement_dict, final_job_state=None):
+    def execute_on_mapped_over(
+        cls, trans, sa_session, action, step_inputs, step_outputs, replacement_dict, final_job_state=None
+    ):
         # Prevent renaming a dataset to the empty string.
         input_names = {}
         #  Lookp through inputs find one with "to_be_replaced" input
         #  variable name, and get the replacement name
         for input_key, step_input in step_inputs.items():
             if step_input and hasattr(step_input, "name"):
                 input_names[input_key] = step_input.name
 
         new_name = cls._gen_new_name(action, input_names, replacement_dict)
         if new_name:
             for name, step_output in step_outputs.items():
-                if action.output_name == '' or name == action.output_name:
+                if action.output_name == "" or name == action.output_name:
                     step_output.name = new_name
 
     @classmethod
     def _gen_new_name(self, action, input_names, replacement_dict):
         new_name = None
 
-        if action.action_arguments and action.action_arguments.get('newname', ''):
-            new_name = action.action_arguments['newname']
+        if action.action_arguments and action.action_arguments.get("newname", ""):
+            new_name = action.action_arguments["newname"]
             #  TODO: Unify and simplify replacement options.
             #      Add interface through workflow editor UI
 
             #  The following if statement will process a request to rename
             #  using an input file name.
             #  TODO: Replace all matching code with regex
             #  Proper syntax is #{input_file_variable | option 1 | option n}
@@ -179,15 +200,15 @@
                 # to allow access to repeat elements, for instance first
                 # repeat in cat1 would be something like queries_0.input2.
                 input_file_var = input_file_var.replace(".", "|")
 
                 replacement = input_names.get(input_file_var, "")
 
                 # In case name was None.
-                replacement = replacement or ''
+                replacement = replacement or ""
                 #  Do operations on replacement
                 #  Any control that is not defined will be ignored.
                 #  This should be moved out to a class or module function
                 for operation in operations:
                     # Basename returns everything prior to the final '.'
                     if operation == "basename":
                         fields = replacement.split(".")
@@ -225,46 +246,49 @@
             has_collection = input_assoc.dataset_collection
             if has_collection and hasattr(has_collection, "name"):
                 input_names[input_assoc.name] = has_collection.name
 
         new_name = cls._gen_new_name(action, input_names, replacement_dict)
         if new_name:
             for dataset_assoc in job.output_datasets:
-                if action.output_name == '' or dataset_assoc.name == action.output_name:
+                if action.output_name == "" or dataset_assoc.name == action.output_name:
                     dataset_assoc.dataset.name = new_name
 
             for dataset_collection_assoc in job.output_dataset_collection_instances:
-                if action.output_name == '' or dataset_collection_assoc.name == action.output_name:
+                if action.output_name == "" or dataset_collection_assoc.name == action.output_name:
                     dataset_collection_assoc.dataset_collection_instance.name = new_name
 
     @classmethod
     def get_short_str(cls, pja):
         # Prevent renaming a dataset to the empty string.
-        if pja.action_arguments and pja.action_arguments.get('newname', ''):
-            return "Rename output '{}' to '{}'.".format(escape(pja.output_name),
-                                                    escape(pja.action_arguments['newname']))
+        if pja.action_arguments and pja.action_arguments.get("newname", ""):
+            return "Rename output '{}' to '{}'.".format(
+                escape(pja.output_name), escape(pja.action_arguments["newname"])
+            )
         else:
             return "Rename action used without a new name specified.  Output name will be unchanged."
 
 
 class HideDatasetAction(DefaultJobAction):
     name = "HideDatasetAction"
     verbose_name = "Hide Dataset"
 
     @classmethod
     def execute(cls, app, sa_session, action, job, replacement_dict, final_job_state=None):
         if final_job_state != job.states.ERROR:
             for output_association in job.output_datasets + job.output_dataset_collection_instances:
-                if action.output_name == '' or output_association.name == action.output_name:
+                if action.output_name == "" or output_association.name == action.output_name:
                     output_association.item.visible = False
 
     @classmethod
-    def execute_on_mapped_over(cls, trans, sa_session, action, step_inputs, step_outputs, replacement_dict, final_job_state=None):
+    def execute_on_mapped_over(
+        cls, trans, sa_session, action, step_inputs, step_outputs, replacement_dict, final_job_state=None
+    ):
         for name, step_output in step_outputs.items():
-            if action.output_name == '' or name == action.output_name:
+            if action.output_name == "" or name == action.output_name:
                 step_output.visible = False
 
     @classmethod
     def get_short_str(cls, pja):
         return f"Hide output '{escape(pja.output_name)}'."
 
 
@@ -272,59 +296,61 @@
     # This is disabled for right now.  Deleting a dataset in the middle of a workflow causes errors (obviously) for the subsequent steps using the data.
     name = "DeleteDatasetAction"
     verbose_name = "Delete Dataset"
 
     @classmethod
     def execute(cls, app, sa_session, action, job, replacement_dict, final_job_state=None):
         for output_association in job.output_datasets + job.output_dataset_collection_instances:
-            if action.output_name == '' or output_association.name == action.output_name:
+            if action.output_name == "" or output_association.name == action.output_name:
                 output_association.item.deleted = True
 
     @classmethod
-    def execute_on_mapped_over(cls, trans, sa_session, action, step_inputs, step_outputs, replacement_dict, final_job_state=None):
+    def execute_on_mapped_over(
+        cls, trans, sa_session, action, step_inputs, step_outputs, replacement_dict, final_job_state=None
+    ):
         for name, step_output in step_outputs.items():
-            if action.output_name == '' or name == action.output_name:
+            if action.output_name == "" or name == action.output_name:
                 step_output.deleted = True
 
     @classmethod
     def get_short_str(cls, pja):
         return "Delete this dataset after creation."
 
 
 class ColumnSetAction(DefaultJobAction):
     name = "ColumnSetAction"
     verbose_name = "Assign Columns"
 
     @classmethod
     def execute(cls, app, sa_session, action, job, replacement_dict, final_job_state=None):
         for dataset_assoc in job.output_datasets:
-            if action.output_name == '' or dataset_assoc.name == action.output_name:
+            if action.output_name == "" or dataset_assoc.name == action.output_name:
                 for k, v in action.action_arguments.items():
                     if v:
                         # Try to use both pure integer and 'cX' format.
                         if not isinstance(v, int):
-                            if v[0] == 'c':
+                            if v[0] == "c":
                                 v = v[1:]
                             v = int(v)
                         if v != 0:
                             setattr(dataset_assoc.dataset.metadata, k, v)
 
     @classmethod
     def get_short_str(cls, pja):
-        return f"Set the following metadata values:<br/>{'<br/>'.join('{} : {}'.format(escape(k), escape(v)) for k, v in pja.action_arguments.items())}"
+        return f"Set the following metadata values:<br/>{'<br/>'.join(f'{escape(k)} : {escape(v)}' for k, v in pja.action_arguments.items())}"
 
 
 class SetMetadataAction(DefaultJobAction):
     name = "SetMetadataAction"
     # DBTODO Setting of Metadata is currently broken and disabled.  It should not be used (yet).
 
     @classmethod
     def execute(cls, app, sa_session, action, job, replacement_dict, final_job_state=None):
         for data in job.output_datasets:
-            data.set_metadata(action.action_arguments['newtype'])
+            data.set_metadata(action.action_arguments["newtype"])
 
 
 class DeleteIntermediatesAction(DefaultJobAction):
     name = "DeleteIntermediatesAction"
     verbose_name = "Delete Non-Output Completed Intermediate Steps"
 
     @classmethod
@@ -349,42 +375,57 @@
         if wfi.active:
             log.debug("Workflow still scheduling so new jobs may appear, skipping deletion of intermediate files.")
             # Still evaluating workflow so we don't yet have all workflow invocation
             # steps to start looking at.
             return
         outputs_defined = wfi.workflow.has_outputs_defined()
         if outputs_defined:
-            wfi_steps = [wfistep for wfistep in wfi.steps if not wfistep.workflow_step.workflow_outputs and wfistep.workflow_step.type == "tool"]
+            wfi_steps = [
+                wfistep
+                for wfistep in wfi.steps
+                if not wfistep.workflow_step.workflow_outputs and wfistep.workflow_step.type == "tool"
+            ]
             jobs_to_check = []
             for wfi_step in wfi_steps:
                 sa_session.refresh(wfi_step)
                 wfi_step_job = wfi_step.job
                 if wfi_step_job:
                     jobs_to_check.append(wfi_step_job)
                 else:
                     log.debug(f"No job found yet for wfi_step {wfi_step}, (step {wfi_step.workflow_step})")
             for j2c in jobs_to_check:
                 creating_jobs = []
                 for input_dataset in j2c.input_datasets:
                     if not input_dataset.dataset:
-                        log.debug(f"PJA Async Issue: No dataset attached to input_dataset {input_dataset.id} during handling of workflow invocation {wfi}")
+                        log.debug(
+                            f"PJA Async Issue: No dataset attached to input_dataset {input_dataset.id} during handling of workflow invocation {wfi}"
+                        )
                     elif not input_dataset.dataset.creating_job:
-                        log.debug(f"PJA Async Issue: No creating job attached to dataset {input_dataset.dataset.id} during handling of workflow invocation {wfi}")
+                        log.debug(
+                            f"PJA Async Issue: No creating job attached to dataset {input_dataset.dataset.id} during handling of workflow invocation {wfi}"
+                        )
                     else:
                         creating_jobs.append((input_dataset, input_dataset.dataset.creating_job))
-                for (input_dataset, creating_job) in creating_jobs:
+                for input_dataset, creating_job in creating_jobs:
                     sa_session.refresh(creating_job)
                     sa_session.refresh(input_dataset)
-                for input_dataset in [x.dataset for (x, creating_job) in creating_jobs if creating_job.workflow_invocation_step and creating_job.workflow_invocation_step.workflow_invocation == wfi]:
+                for input_dataset in [
+                    x.dataset
+                    for (x, creating_job) in creating_jobs
+                    if creating_job.workflow_invocation_step
+                    and creating_job.workflow_invocation_step.workflow_invocation == wfi
+                ]:
                     # note that the above input_dataset is a reference to a
                     # job.input_dataset.dataset at this point
                     safe_to_delete = True
                     for job_to_check in [d_j.job for d_j in input_dataset.dependent_jobs]:
                         if job_to_check != job and job_to_check.state not in [job.states.OK, job.states.DELETED]:
-                            log.trace(f"Workflow Intermediates cleanup attempted, but non-terminal state '{job_to_check.state}' detected for job {job_to_check.id}")
+                            log.trace(
+                                f"Workflow Intermediates cleanup attempted, but non-terminal state '{job_to_check.state}' detected for job {job_to_check.id}"
+                            )
                             safe_to_delete = False
                     if safe_to_delete:
                         # Support purging here too.
                         input_dataset.mark_deleted()
         else:
             # No workflow outputs defined, so we can't know what to delete.
             # We could make this work differently in the future
@@ -398,48 +439,55 @@
 class TagDatasetAction(DefaultJobAction):
     name = "TagDatasetAction"
     verbose_name = "Add tag to dataset"
     action = "Add"
     direction = "to"
 
     @classmethod
-    def execute_on_mapped_over(cls, trans, sa_session, action, step_inputs, step_outputs, replacement_dict, final_job_state=None):
+    def execute_on_mapped_over(
+        cls, trans, sa_session, action, step_inputs, step_outputs, replacement_dict, final_job_state=None
+    ):
         tag_handler = trans.app.tag_handler.create_tag_handler_session()
         if action.action_arguments:
-            tags = [t.replace('#', 'name:') if t.startswith('#') else t for t in [t.strip() for t in action.action_arguments.get('tags', '').split(',') if t.strip()]]
+            tags = [
+                t.replace("#", "name:") if t.startswith("#") else t
+                for t in [t.strip() for t in action.action_arguments.get("tags", "").split(",") if t.strip()]
+            ]
             if tags:
                 for name, step_output in step_outputs.items():
-                    if action.output_name == '' or name == action.output_name:
+                    if action.output_name == "" or name == action.output_name:
                         cls._execute(tag_handler, trans.user, step_output, tags)
 
     @classmethod
     def execute(cls, app, sa_session, action, job, replacement_dict, final_job_state=None):
         if action.action_arguments:
             tag_handler = app.tag_handler.create_tag_handler_session()
-            tags = [t.replace('#', 'name:') if t.startswith('#') else t for t in [t.strip() for t in action.action_arguments.get('tags', '').split(',') if t.strip()]]
+            tags = [
+                t.replace("#", "name:") if t.startswith("#") else t
+                for t in [t.strip() for t in action.action_arguments.get("tags", "").split(",") if t.strip()]
+            ]
             if tags:
                 for dataset_assoc in job.output_datasets:
-                    if action.output_name == '' or dataset_assoc.name == action.output_name:
+                    if action.output_name == "" or dataset_assoc.name == action.output_name:
                         cls._execute(tag_handler, job.user, dataset_assoc.dataset, tags)
 
                 for dataset_collection_assoc in job.output_dataset_collection_instances:
-                    if action.output_name == '' or dataset_collection_assoc.name == action.output_name:
+                    if action.output_name == "" or dataset_collection_assoc.name == action.output_name:
                         cls._execute(tag_handler, job.user, dataset_collection_assoc.dataset_collection_instance, tags)
 
     @classmethod
     def _execute(cls, tag_handler, user, output, tags):
         tag_handler.add_tags_from_list(user, output, tags, flush=False)
 
     @classmethod
     def get_short_str(cls, pja):
-        if pja.action_arguments and pja.action_arguments.get('tags', ''):
-            return "{} tag(s) '{}' {} '{}'.".format(cls.action,
-                                                escape(pja.action_arguments['tags']),
-                                                cls.direction,
-                                                escape(pja.output_name))
+        if pja.action_arguments and pja.action_arguments.get("tags", ""):
+            return "{} tag(s) '{}' {} '{}'.".format(
+                cls.action, escape(pja.action_arguments["tags"]), cls.direction, escape(pja.output_name)
+            )
         else:
             return f"{cls.action} Tag action used without a tag specified.  No tag will be added."
 
 
 class RemoveTagDatasetAction(TagDatasetAction):
     name = "RemoveTagDatasetAction"
     verbose_name = "Remove tag from dataset"
@@ -448,67 +496,80 @@
 
     @classmethod
     def _execute(cls, tag_handler, user, output, tags):
         tag_handler.remove_tags_from_list(user, output, tags)
 
 
 class ActionBox:
-
-    actions = {"RenameDatasetAction": RenameDatasetAction,
-               "HideDatasetAction": HideDatasetAction,
-               "ChangeDatatypeAction": ChangeDatatypeAction,
-               "ColumnSetAction": ColumnSetAction,
-               "EmailAction": EmailAction,
-               "DeleteIntermediatesAction": DeleteIntermediatesAction,
-               "TagDatasetAction": TagDatasetAction,
-               "RemoveTagDatasetAction": RemoveTagDatasetAction}
-    public_actions = ['RenameDatasetAction', 'ChangeDatatypeAction',
-                      'ColumnSetAction', 'EmailAction',
-                      'DeleteIntermediatesAction', 'TagDatasetAction',
-                      'RemoveTagDatasetAction']
+    actions = {
+        "RenameDatasetAction": RenameDatasetAction,
+        "HideDatasetAction": HideDatasetAction,
+        "ChangeDatatypeAction": ChangeDatatypeAction,
+        "ColumnSetAction": ColumnSetAction,
+        "EmailAction": EmailAction,
+        "DeleteIntermediatesAction": DeleteIntermediatesAction,
+        "TagDatasetAction": TagDatasetAction,
+        "RemoveTagDatasetAction": RemoveTagDatasetAction,
+    }
+    public_actions = [
+        "RenameDatasetAction",
+        "ChangeDatatypeAction",
+        "ColumnSetAction",
+        "EmailAction",
+        "DeleteIntermediatesAction",
+        "TagDatasetAction",
+        "RemoveTagDatasetAction",
+    ]
     # Actions that can be applied ahead of the job execution while workflow is still
     # being scheduled and jobs created.
-    immediate_actions = ['ChangeDatatypeAction', 'RenameDatasetAction',
-                         'TagDatasetAction', 'RemoveTagDatasetAction']
+    immediate_actions = ["ChangeDatatypeAction", "RenameDatasetAction", "TagDatasetAction", "RemoveTagDatasetAction"]
     # Actions that will be applied to implicit mapped over collection outputs and not
     # just individual outputs when steps include mapped over tools and implicit collection outputs.
-    mapped_over_output_actions = ['RenameDatasetAction', 'HideDatasetAction',
-                                  'TagDatasetAction', 'RemoveTagDatasetAction']
+    mapped_over_output_actions = [
+        "RenameDatasetAction",
+        "HideDatasetAction",
+        "TagDatasetAction",
+        "RemoveTagDatasetAction",
+    ]
 
     @classmethod
     def get_short_str(cls, action):
         if action.action_type in ActionBox.actions:
             return ActionBox.actions[action.action_type].get_short_str(action)
         else:
             return "Unknown Action"
 
     @classmethod
     def handle_incoming(cls, incoming):
         npd = {}
         for key, val in incoming.items():
-            if key.startswith('pja'):
-                sp = key.split('__')
+            if key.startswith("pja"):
+                sp = key.split("__")
                 ao_key = sp[2] + sp[1]
                 # flag / output_name / pjatype / desc
                 if ao_key not in npd:
-                    npd[ao_key] = {'action_type': sp[2],
-                                   'output_name': sp[1],
-                                   'action_arguments': {}}
+                    npd[ao_key] = {"action_type": sp[2], "output_name": sp[1], "action_arguments": {}}
                 if len(sp) > 3:
-                    if sp[3] == 'output_name':
-                        npd[ao_key]['output_name'] = val
+                    if sp[3] == "output_name":
+                        npd[ao_key]["output_name"] = val
                     else:
-                        npd[ao_key]['action_arguments'][sp[3]] = val
+                        npd[ao_key]["action_arguments"][sp[3]] = val
             else:
                 # Not pja stuff.
                 pass
         return npd
 
     @classmethod
-    def execute_on_mapped_over(cls, trans, sa_session, pja, step_inputs, step_outputs, replacement_dict=None, final_job_state=None):
+    def execute_on_mapped_over(
+        cls, trans, sa_session, pja, step_inputs, step_outputs, replacement_dict=None, final_job_state=None
+    ):
         if pja.action_type in ActionBox.actions:
-            ActionBox.actions[pja.action_type].execute_on_mapped_over(trans, sa_session, pja, step_inputs, step_outputs, replacement_dict, final_job_state=final_job_state)
+            ActionBox.actions[pja.action_type].execute_on_mapped_over(
+                trans, sa_session, pja, step_inputs, step_outputs, replacement_dict, final_job_state=final_job_state
+            )
 
     @classmethod
     def execute(cls, app, sa_session, pja, job, replacement_dict=None, final_job_state=None):
         if pja.action_type in ActionBox.actions:
-            ActionBox.actions[pja.action_type].execute(app, sa_session, pja, job, replacement_dict, final_job_state=final_job_state)
+            ActionBox.actions[pja.action_type].execute(
+                app, sa_session, pja, job, replacement_dict, final_job_state=final_job_state
+            )
```

### Comparing `galaxy-job-execution-22.1.1/galaxy/job_execution/compute_environment.py` & `galaxy-job-execution-23.0.1/galaxy/job_execution/compute_environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import os
 from abc import (
     ABCMeta,
     abstractmethod,
 )
+from typing import (
+    Any,
+    Dict,
+)
 
 from galaxy.job_execution.setup import JobIO
 from galaxy.model import Job
 
 
 class ComputeEnvironment(metaclass=ABCMeta):
-    """ Definition of the job as it will be run on the (potentially) remote
+    """Definition of the job as it will be run on the (potentially) remote
     compute server.
     """
 
     @abstractmethod
     def output_names(self):
-        """ Output unqualified filenames defined by job. """
+        """Output unqualified filenames defined by job."""
 
     @abstractmethod
     def input_path_rewrite(self, dataset):
         """Input path for specified dataset."""
 
     @abstractmethod
     def output_path_rewrite(self, dataset):
@@ -39,78 +43,79 @@
 
     @abstractmethod
     def unstructured_path_rewrite(self, path):
         """Rewrite loc file paths, etc.."""
 
     @abstractmethod
     def working_directory(self):
-        """ Job working directory (potentially remote) """
+        """Job working directory (potentially remote)"""
 
     @abstractmethod
     def config_directory(self):
-        """ Directory containing config files (potentially remote) """
+        """Directory containing config files (potentially remote)"""
 
     @abstractmethod
     def env_config_directory(self):
         """Working directory (possibly as environment variable evaluation)."""
 
     @abstractmethod
     def sep(self):
-        """ os.path.sep for the platform this job will execute in.
-        """
+        """os.path.sep for the platform this job will execute in."""
 
     @abstractmethod
     def new_file_path(self):
-        """ Absolute path to dump new files for this job on compute server. """
+        """Absolute path to dump new files for this job on compute server."""
 
     @abstractmethod
     def tool_directory(self):
-        """ Absolute path to tool files for this job on compute server. """
+        """Absolute path to tool files for this job on compute server."""
 
     @abstractmethod
     def version_path(self):
-        """ Location of the version file for the underlying tool. """
+        """Location of the version file for the underlying tool."""
 
     @abstractmethod
     def home_directory(self):
         """Home directory of target job - none if HOME should not be set."""
 
     @abstractmethod
     def tmp_directory(self):
         """Temp directory of target job - none if HOME should not be set."""
 
     @abstractmethod
     def galaxy_url(self):
         """URL to access Galaxy API from for this compute environment."""
 
     @abstractmethod
-    def get_file_sources_dict(self):
+    def get_file_sources_dict(self) -> Dict[str, Any]:
         """Return file sources dict for current user."""
 
 
 class SimpleComputeEnvironment:
-
     def config_directory(self):
         return os.path.join(self.working_directory(), "configs")  # type: ignore[attr-defined]
 
     def sep(self):
         return os.path.sep
 
 
 class SharedComputeEnvironment(SimpleComputeEnvironment, ComputeEnvironment):
-    """ Default ComputeEnvironment for job and task wrapper to pass
+    """Default ComputeEnvironment for job and task wrapper to pass
     to ToolEvaluator - valid when Galaxy and compute share all the relevant
     file systems.
     """
 
+    job_id: JobIO
+    job: Job
+
     def __init__(self, job_io: JobIO, job: Job):
         self.job_io = job_io
         self.job = job
 
-    def get_file_sources_dict(self):
+    def get_file_sources_dict(self) -> Dict[str, Any]:
         return self.job_io.file_sources_dict
 
     def output_names(self):
         return self.job_io.get_output_basenames()
 
     def output_paths(self):
         return self.job_io.get_output_fnames()
```

### Comparing `galaxy-job-execution-22.1.1/galaxy/job_execution/datasets.py` & `galaxy-job-execution-23.0.1/galaxy/job_execution/datasets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """
 Utility classes allowing Job interface to reason about datasets.
 """
 import os.path
 from abc import (
     ABCMeta,
-    abstractmethod
+    abstractmethod,
 )
 
 
 def dataset_path_rewrites(dataset_paths):
     dataset_paths_with_rewrites = [path for path in dataset_paths if getattr(path, "false_path", None)]
     return {dp.real_path: dp for dp in dataset_paths_with_rewrites}
 
 
 class DatasetPath:
-
     def __init__(
         self,
         dataset_id,
         real_path,
         false_path=None,
         false_extra_files_path=None,
         false_metadata_path=None,
@@ -55,75 +54,77 @@
                 false_metadata_path=false_metadata_path,
                 mutable=self.mutable,
             )
         return dataset_path
 
 
 class DatasetPathRewriter(metaclass=ABCMeta):
-    """ Used by runner to rewrite paths. """
+    """Used by runner to rewrite paths."""
 
     @abstractmethod
     def rewrite_dataset_path(self, dataset, dataset_type):
         """
         Dataset type is 'input' or 'output'.
         Return None to indicate not to rewrite this path.
         """
 
 
-class NullDatasetPathRewriter:
-    """ Used by default for jobwrapper, do not rewrite anything.
-    """
+class NullDatasetPathRewriter(DatasetPathRewriter):
+    """Used by default for jobwrapper, do not rewrite anything."""
 
     def rewrite_dataset_path(self, dataset, dataset_type):
-        """ Keep path the same.
-        """
+        """Keep path the same."""
         return None
 
 
-class OutputsToWorkingDirectoryPathRewriter:
-    """ Rewrites all paths to place them in the specified working
+class OutputsToWorkingDirectoryPathRewriter(DatasetPathRewriter):
+    """Rewrites all paths to place them in the specified working
     directory for normal jobs when Galaxy is configured with
     app.config.outputs_to_working_directory. Job runner base class
     is responsible for copying these out after job is complete.
     """
 
     def __init__(self, working_directory, outputs_directory_name):
         self.working_directory = working_directory
         self.outputs_directory_name = outputs_directory_name
 
     def rewrite_dataset_path(self, dataset, dataset_type):
-        """ Keep path the same.
-        """
-        if dataset_type == 'output':
+        """Keep path the same."""
+        if dataset_type == "output":
             base_output_directory = os.path.abspath(self.working_directory)
             if self.outputs_directory_name is not None:
                 base_output_directory = os.path.join(base_output_directory, self.outputs_directory_name)
             # set false_path to uuid, no harm even if object store uses id
             false_path = os.path.join(base_output_directory, f"galaxy_dataset_{dataset.dataset.uuid}.dat")
             return false_path
         else:
             return None
 
 
-class TaskPathRewriter:
-    """ Rewrites all paths to place them in the specified working
+class TaskPathRewriter(DatasetPathRewriter):
+    """Rewrites all paths to place them in the specified working
     directory for TaskWrapper. TaskWrapper is responsible for putting
     them there and pulling them out.
     """
 
     def __init__(self, working_directory, job_dataset_path_rewriter):
         self.working_directory = working_directory
         self.job_dataset_path_rewriter = job_dataset_path_rewriter
 
     def rewrite_dataset_path(self, dataset, dataset_type):
-        """
-        """
+        """ """
         dataset_file_name = dataset.file_name
         job_file_name = self.job_dataset_path_rewriter.rewrite_dataset_path(dataset, dataset_type) or dataset_file_name
         return os.path.join(self.working_directory, os.path.basename(job_file_name))
 
 
-def get_path_rewriter(outputs_to_working_directory, working_directory, outputs_directory, is_task):
-    job_dataset_path_rewriter = OutputsToWorkingDirectoryPathRewriter(working_directory, outputs_directory) if outputs_to_working_directory else NullDatasetPathRewriter()
+def get_path_rewriter(
+    outputs_to_working_directory, working_directory, outputs_directory, is_task
+) -> DatasetPathRewriter:
+    job_dataset_path_rewriter: DatasetPathRewriter = (
+        OutputsToWorkingDirectoryPathRewriter(working_directory, outputs_directory)
+        if outputs_to_working_directory
+        else NullDatasetPathRewriter()
+    )
     if is_task:
         return TaskPathRewriter(working_directory, job_dataset_path_rewriter=job_dataset_path_rewriter)
     return job_dataset_path_rewriter
```

### Comparing `galaxy-job-execution-22.1.1/galaxy/job_execution/output_collect.py` & `galaxy-job-execution-23.0.1/galaxy/job_execution/output_collect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 """ Code allowing tools to define extra files associated with an output datset.
 """
 import logging
 import operator
 import os
 import re
 from tempfile import NamedTemporaryFile
-from typing import Callable, Dict, List, Optional, Union
+from typing import (
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Union,
+)
 
 from sqlalchemy.orm.scoping import ScopedSession
 
 from galaxy.model import (
     HistoryDatasetAssociation,
     HistoryDatasetCollectionAssociation,
     Job,
@@ -39,28 +45,28 @@
     INPUT_DBKEY_TOKEN,
     ToolProvidedMetadataDatasetCollection,
 )
 from galaxy.tool_util.parser.output_objects import (
     ToolOutput,
     ToolOutputCollection,
 )
+from galaxy.tool_util.provided_metadata import BaseToolProvidedMetadata
 from galaxy.util import (
     shrink_and_unicodify,
     unicodify,
 )
 
 DATASET_ID_TOKEN = "DATASET_ID"
 
 log = logging.getLogger(__name__)
 
 
 # PermissionProvider and MetadataSourceProvider are abstractions over input data used to
 # collect and produce dynamic outputs.
 class PermissionProvider(AbstractPermissionProvider):
-
     def __init__(self, inp_data, security_agent, job):
         self._job = job
         self._security_agent = security_agent
         self._inp_data = inp_data
         self._user = job.user
         self._permissions = None
 
@@ -84,15 +90,14 @@
             self._security_agent.set_all_dataset_permissions(primary_data.dataset, permissions, new=True, flush=False)
 
     def copy_dataset_permissions(self, init_from, primary_data):
         self._security_agent.copy_dataset_permissions(init_from.dataset, primary_data.dataset)
 
 
 class MetadataSourceProvider(AbstractMetadataSourceProvider):
-
     def __init__(self, inp_data):
         self._inp_data = inp_data
 
     def get_metadata_source(self, input_name):
         return self._inp_data[input_name]
 
 
@@ -158,15 +163,17 @@
             collection = has_collection
 
         # We are adding dynamic collections, which may be precreated, but their actually state is still new!
         collection.populated_state = collection.populated_states.NEW
 
         try:
             collection_builder = builder.BoundCollectionBuilder(collection)
-            dataset_collectors = [dataset_collector(description) for description in output_collection_def.dataset_collector_descriptions]
+            dataset_collectors = [
+                dataset_collector(description) for description in output_collection_def.dataset_collector_descriptions
+            ]
             output_name = output_collection_def.name
             filenames = job_context.find_files(output_name, collection, dataset_collectors)
             job_context.populate_collection_elements(
                 collection,
                 collection_builder,
                 filenames,
                 name=output_collection_def.name,
@@ -177,73 +184,76 @@
         except Exception:
             log.exception("Problem gathering output collection.")
             collection.handle_population_failed("Problem building datasets for collection.")
 
         job_context.add_dataset_collection(has_collection)
 
 
-class BaseJobContext:
-
+class BaseJobContext(ModelPersistenceContext):
     max_discovered_files: Union[int, float]
+    tool_provided_metadata: BaseToolProvidedMetadata
+    job_working_directory: str
 
     def add_dataset_collection(self, collection):
         pass
 
-    def find_files(self, output_name, collection, dataset_collectors):
-        filenames = {}
-        for discovered_file in discover_files(output_name, self.tool_provided_metadata, dataset_collectors, self.job_working_directory, collection):
+    def find_files(self, output_name, collection, dataset_collectors) -> list:
+        discovered_files = []
+        for discovered_file in discover_files(
+            output_name, self.tool_provided_metadata, dataset_collectors, self.job_working_directory, collection
+        ):
             self.increment_discovered_file_count()
-            filenames[discovered_file.path] = discovered_file
-        return filenames
+            discovered_files.append(discovered_file)
+        return discovered_files
 
     def get_job_id(self):
         return None  # overwritten in subclasses
 
 
-class JobContext(ModelPersistenceContext, BaseJobContext):
-
+class JobContext(BaseJobContext):
     def __init__(
-            self,
-            tool,
-            tool_provided_metadata,
-            job,
-            job_working_directory,
-            permission_provider,
-            metadata_source_provider,
-            input_dbkey,
-            object_store,
-            final_job_state,
-            max_discovered_files: Optional[int],
-            flush_per_n_datasets=None,
+        self,
+        tool,
+        tool_provided_metadata: BaseToolProvidedMetadata,
+        job,
+        job_working_directory,
+        permission_provider,
+        metadata_source_provider,
+        input_dbkey,
+        object_store,
+        final_job_state,
+        max_discovered_files: Optional[int],
+        flush_per_n_datasets=None,
     ):
         self.tool = tool
         self._metadata_source_provider = metadata_source_provider
         self._permission_provider = permission_provider
         self._input_dbkey = input_dbkey
         self.app = tool.app
         self._sa_session = tool.sa_session
         self._job = job
         self.job_working_directory = job_working_directory
         self.tool_provided_metadata = tool_provided_metadata
         self._object_store = object_store
         self.final_job_state = final_job_state
         self._flush_per_n_datasets = flush_per_n_datasets
-        self.max_discovered_files = float('inf') if max_discovered_files is None else max_discovered_files
+        self.max_discovered_files = float("inf") if max_discovered_files is None else max_discovered_files
         self.discovered_file_count = 0
         self._tag_handler = None
 
     @property
     def tag_handler(self):
         if self._tag_handler is None:
             self._tag_handler = self.app.tag_handler.create_tag_handler_session()
         return self._tag_handler
 
     @property
     def work_context(self):
         from galaxy.work.context import WorkRequestContext
+
         return WorkRequestContext(self.app, user=self.user)
 
     @property
     def sa_session(self) -> ScopedSession:
         return self._sa_session
 
     @property
@@ -283,15 +293,17 @@
 
     def flush(self):
         self.sa_session.flush()
 
     def get_library_folder(self, destination):
         app = self.app
         library_folder_manager = app.library_folder_manager
-        library_folder = library_folder_manager.get(self.work_context, app.security.decode_id(destination.get("library_folder_id")))
+        folder_id = destination.get("library_folder_id")
+        decoded_folder_id = app.security.decode_id(folder_id) if isinstance(folder_id, str) else folder_id
+        library_folder = library_folder_manager.get(self.work_context, decoded_folder_id)
         return library_folder
 
     def get_hdca(self, object_id):
         hdca = self.sa_session.query(HistoryDatasetCollectionAssociation).get(int(object_id))
         return hdca
 
     def create_library_folder(self, parent_folder, name, description):
@@ -300,17 +312,15 @@
         nested_folder = library_folder_manager.create(self.work_context, parent_folder.id, name, description)
         return nested_folder
 
     def create_hdca(self, name, structure):
         history = self.job.history
         trans = self.work_context
         collection_manager = self.app.dataset_collection_manager
-        hdca = collection_manager.precreate_dataset_collection_instance(
-            trans, history, name, structure=structure
-        )
+        hdca = collection_manager.precreate_dataset_collection_instance(trans, history, name, structure=structure)
         return hdca
 
     def add_output_dataset_association(self, name, dataset):
         assoc = JobToOutputDatasetAssociation(name, dataset)
         assoc.job = self.job
         self.sa_session.add(assoc)
 
@@ -323,15 +333,17 @@
         trans.app.security_agent.copy_library_permissions(trans, library_folder, ld)
         trans.sa_session.add(ld)
         trans.sa_session.flush()
 
         # Permissions must be the same on the LibraryDatasetDatasetAssociation and the associated LibraryDataset
         trans.app.security_agent.copy_library_permissions(trans, ld, ldda)
         # Copy the current user's DefaultUserPermissions to the new LibraryDatasetDatasetAssociation.dataset
-        trans.app.security_agent.set_all_dataset_permissions(ldda.dataset, trans.app.security_agent.user_get_default_permissions(trans.user))
+        trans.app.security_agent.set_all_dataset_permissions(
+            ldda.dataset, trans.app.security_agent.user_get_default_permissions(trans.user)
+        )
         library_folder.add_library_dataset(ld, genome_build=ldda.dbkey)
         trans.sa_session.add(library_folder)
         trans.sa_session.flush()
 
         trans.sa_session.add(ld)
         trans.sa_session.flush()
 
@@ -374,23 +386,32 @@
         return self.job.id
 
     def get_implicit_collection_jobs_association_id(self):
         return self.job.implicit_collection_jobs_association and self.job.implicit_collection_jobs_association.id
 
 
 class SessionlessJobContext(SessionlessModelPersistenceContext, BaseJobContext):
-
-    def __init__(self, metadata_params, tool_provided_metadata, object_store, export_store, import_store, working_directory, final_job_state, max_discovered_files: Optional[int]):
+    def __init__(
+        self,
+        metadata_params,
+        tool_provided_metadata: BaseToolProvidedMetadata,
+        object_store,
+        export_store,
+        import_store,
+        working_directory,
+        final_job_state,
+        max_discovered_files: Optional[int],
+    ):
         # TODO: use a metadata source provider... (pop from inputs and add parameter)
         super().__init__(object_store, export_store, working_directory)
         self.metadata_params = metadata_params
         self.tool_provided_metadata = tool_provided_metadata
         self.import_store = import_store
         self.final_job_state = final_job_state
-        self.max_discovered_files = float('inf') if max_discovered_files is None else max_discovered_files
+        self.max_discovered_files = float("inf") if max_discovered_files is None else max_discovered_files
         self.discovered_file_count = 0
 
     def output_collection_def(self, name):
         tool_as_dict = self.metadata_params["tool"]
         output_collection_defs = tool_as_dict["output_collections"]
         if name not in output_collection_defs:
             return False
@@ -415,24 +436,24 @@
     def get_hdca(self, object_id):
         hdca = self.import_store.sa_session.query(HistoryDatasetCollectionAssociation).find(int(object_id))
         if hdca:
             self.export_store.add_dataset_collection(hdca)
             for collection_dataset in hdca.dataset_instances:
                 include_files = True
                 self.export_store.add_dataset(collection_dataset, include_files=include_files)
-                self.export_store.collection_datasets[collection_dataset.id] = True
+                self.export_store.collection_datasets.add(collection_dataset.id)
 
         return hdca
 
     def add_dataset_collection(self, collection):
         self.export_store.add_dataset_collection(collection)
         for collection_dataset in collection.dataset_instances:
             include_files = True
             self.export_store.add_dataset(collection_dataset, include_files=include_files)
-            self.export_store.collection_datasets[collection_dataset.id] = True
+            self.export_store.collection_datasets.add(collection_dataset.id)
 
     def add_output_dataset_association(self, name, dataset_instance):
         self.export_store.add_job_output_dataset_associations(self.get_job_id(), name, dataset_instance)
 
     def get_job_id(self):
         return self.metadata_params["job_id_tag"]
 
@@ -449,17 +470,21 @@
     new_outdata_name = None
     primary_datasets: Dict[str, Dict[str, Union[HistoryDatasetAssociation, LibraryDatasetDatasetAssociation]]] = {}
     storage_callbacks: List[Callable] = []
     for output_index, (name, outdata) in enumerate(output.items()):
         dataset_collectors = [DEFAULT_DATASET_COLLECTOR]
         output_def = job_context.output_def(name)
         if output_def is not None:
-            dataset_collectors = [dataset_collector(description) for description in output_def.dataset_collector_descriptions]
+            dataset_collectors = [
+                dataset_collector(description) for description in output_def.dataset_collector_descriptions
+            ]
         filenames = {}
-        for discovered_file in discover_files(name, job_context.tool_provided_metadata, dataset_collectors, job_working_directory, outdata):
+        for discovered_file in discover_files(
+            name, job_context.tool_provided_metadata, dataset_collectors, job_working_directory, outdata
+        ):
             job_context.increment_discovered_file_count()
             filenames[discovered_file.path] = discovered_file
         for filename_index, (filename, discovered_file) in enumerate(filenames.items()):
             extra_file_collector = discovered_file.collector
             fields_match = discovered_file.match
             if not fields_match:
                 # Before I guess pop() would just have thrown an IndexError
@@ -486,44 +511,47 @@
             visible = fields_match.visible
             # Create new primary dataset
             new_primary_name = fields_match.name or f"{outdata.name} ({designation})"
             info = outdata.info
 
             # TODO: should be able to disambiguate files in different directories...
             new_primary_filename = os.path.split(filename)[-1]
-            new_primary_datasets_attributes = job_context.tool_provided_metadata.get_new_dataset_meta_by_basename(name, new_primary_filename)
+            new_primary_datasets_attributes = job_context.tool_provided_metadata.get_new_dataset_meta_by_basename(
+                name, new_primary_filename
+            )
             extra_files = None
             if new_primary_datasets_attributes:
-                extra_files_path = new_primary_datasets_attributes.get('extra_files', None)
+                extra_files_path = new_primary_datasets_attributes.get("extra_files", None)
                 if extra_files_path:
                     extra_files = os.path.join(job_working_directory, extra_files_path)
             primary_data = job_context.create_dataset(
                 ext,
                 designation,
                 visible,
                 dbkey,
                 new_primary_name,
                 filename,
                 extra_files=extra_files,
                 info=info,
                 init_from=outdata,
                 dataset_attributes=new_primary_datasets_attributes,
                 creating_job_id=job_context.get_job_id() if job_context else None,
-                storage_callbacks=storage_callbacks
+                storage_callbacks=storage_callbacks,
             )
             # Associate new dataset with job
-            job_context.add_output_dataset_association(f'__new_primary_file_{name}|{designation}__', primary_data)
+            job_context.add_output_dataset_association(f"__new_primary_file_{name}|{designation}__", primary_data)
             job_context.add_datasets_to_history([primary_data], for_output_dataset=outdata)
             # Add dataset to return dict
             primary_datasets[name][designation] = primary_data
         if primary_output_assigned:
             outdata.name = new_outdata_name
             outdata.init_meta()
             outdata.set_meta()
             outdata.set_peek()
+            outdata.discovered = True
             sa_session = job_context.sa_session
             if sa_session:
                 sa_session.add(outdata)
 
     # Move discovered outputs to storage and set metdata / peeks
     for callback in storage_callbacks:
         callback()
@@ -536,24 +564,30 @@
         # just load entries from tool provided metadata...
         assert len(extra_file_collectors) == 1
         extra_file_collector = extra_file_collectors[0]
         target_directory = discover_target_directory(extra_file_collector.directory, job_working_directory)
         for dataset in tool_provided_metadata.get_new_datasets(output_name):
             filename = dataset["filename"]
             path = os.path.join(target_directory, filename)
-            yield DiscoveredFile(path, extra_file_collector, JsonCollectedDatasetMatch(dataset, extra_file_collector, filename, path=path))
+            yield DiscoveredFile(
+                path,
+                extra_file_collector,
+                JsonCollectedDatasetMatch(dataset, extra_file_collector, filename, path=path),
+            )
     else:
-        for (match, collector) in walk_over_file_collectors(extra_file_collectors, job_working_directory, matchable):
+        for match, collector in walk_over_file_collectors(extra_file_collectors, job_working_directory, matchable):
             yield DiscoveredFile(match.path, collector, match)
 
 
 def walk_over_file_collectors(extra_file_collectors, job_working_directory, matchable):
     for extra_file_collector in extra_file_collectors:
         assert extra_file_collector.discover_via == "pattern"
-        for match in walk_over_extra_files(extra_file_collector.directory, extra_file_collector, job_working_directory, matchable):
+        for match in walk_over_extra_files(
+            extra_file_collector.directory, extra_file_collector, job_working_directory, matchable
+        ):
             yield match, extra_file_collector
 
 
 def walk_over_extra_files(target_dir, extra_file_collector, job_working_directory, matchable, parent_paths=None):
     """
     Walks through all files in a given directory, and returns all files that
     match the given collector's match criteria. If the collector has the
@@ -575,18 +609,17 @@
                             filename, extra_file_collector, directory, matchable, parent_paths=new_parent_paths
                         )
                 else:
                     match = extra_file_collector.match(matchable, filename, path=path, parent_paths=parent_paths)
                     if match:
                         yield match
 
-    for match in extra_file_collector.sort(
+    yield from extra_file_collector.sort(
         _walk(target_dir, extra_file_collector, job_working_directory, matchable, parent_paths)
-    ):
-        yield match
+    )
 
 
 def dataset_collector(dataset_collection_description):
     if dataset_collection_description is DEFAULT_DATASET_COLLECTOR_DESCRIPTION:
         # Use 'is' and 'in' operators, so lets ensure this is
         # treated like a singleton.
         return DEFAULT_DATASET_COLLECTOR
@@ -594,44 +627,42 @@
         if dataset_collection_description.discover_via == "pattern":
             return DatasetCollector(dataset_collection_description)
         else:
             return ToolMetadataDatasetCollector(dataset_collection_description)
 
 
 class ToolMetadataDatasetCollector:
-
     def __init__(self, dataset_collection_description):
         self.discover_via = dataset_collection_description.discover_via
         self.default_dbkey = dataset_collection_description.default_dbkey
         self.default_ext = dataset_collection_description.default_ext
         self.default_visible = dataset_collection_description.default_visible
         self.directory = dataset_collection_description.directory
         self.assign_primary_output = dataset_collection_description.assign_primary_output
 
 
 class DatasetCollector:
-
     def __init__(self, dataset_collection_description):
         self.discover_via = dataset_collection_description.discover_via
         # dataset_collection_description is an abstract description
-        # built from the tool parsing module - see galaxy.tool_util.parser.output_colleciton_def
+        # built from the tool parsing module - see galaxy.tool_util.parser.output_collection_def
         self.sort_key = dataset_collection_description.sort_key
         self.sort_reverse = dataset_collection_description.sort_reverse
         self.sort_comp = dataset_collection_description.sort_comp
         self.pattern = dataset_collection_description.pattern
         self.default_dbkey = dataset_collection_description.default_dbkey
         self.default_ext = dataset_collection_description.default_ext
         self.default_visible = dataset_collection_description.default_visible
         self.directory = dataset_collection_description.directory
         self.assign_primary_output = dataset_collection_description.assign_primary_output
         self.recurse = dataset_collection_description.recurse
         self.match_relative_path = dataset_collection_description.match_relative_path
 
     def _pattern_for_dataset(self, dataset_instance=None):
-        token_replacement = r'\d+'
+        token_replacement = r"\d+"
         if dataset_instance:
             token_replacement = str(dataset_instance.id)
         return self.pattern.replace(DATASET_ID_TOKEN, token_replacement)
 
     def match(self, dataset_instance, filename, path=None, parent_paths=None):
         pattern = self._pattern_for_dataset(dataset_instance)
         if self.match_relative_path and parent_paths:
@@ -680,51 +711,53 @@
         log.warning(f"({galaxy_id_tag}) Exit code '{exit_code_str}' invalid. Using 0.")
         exit_code = 0
 
     return exit_code
 
 
 def default_exit_code_file(files_dir, id_tag):
-    return os.path.join(files_dir, f'galaxy_{id_tag}.ec')
+    return os.path.join(files_dir, f"galaxy_{id_tag}.ec")
 
 
 def collect_extra_files(object_store, dataset, job_working_directory):
     file_name = dataset.dataset.extra_files_path_name_from(object_store)
     temp_file_path = os.path.join(job_working_directory, "working", file_name)
     extra_dir = None
     try:
         # This skips creation of directories - object store
         # automatically creates them.  However, empty directories will
         # not be created in the object store at all, which might be a
         # problem.
         for root, _dirs, files in os.walk(temp_file_path):
-            extra_dir = root.replace(os.path.join(job_working_directory, "working"), '', 1).lstrip(os.path.sep)
+            extra_dir = root.replace(os.path.join(job_working_directory, "working"), "", 1).lstrip(os.path.sep)
             for f in files:
                 object_store.update_from_file(
                     dataset.dataset,
                     extra_dir=extra_dir,
                     alt_name=f,
                     file_name=os.path.join(root, f),
                     create=True,
-                    preserve_symlinks=True
+                    preserve_symlinks=True,
                 )
     except Exception as e:
         log.debug("Error in collect_associated_files: %s", unicodify(e))
 
     # Handle composite datatypes of auto_primary_file type
-    if dataset.datatype.composite_type == 'auto_primary_file' and not dataset.has_data():
+    if dataset.datatype.composite_type == "auto_primary_file" and not dataset.has_data():
         try:
-            with NamedTemporaryFile(mode='w') as temp_fh:
+            with NamedTemporaryFile(mode="w") as temp_fh:
                 temp_fh.write(dataset.datatype.generate_primary_file(dataset))
                 temp_fh.flush()
                 object_store.update_from_file(dataset.dataset, file_name=temp_fh.name, create=True)
                 dataset.set_size()
         except Exception as e:
-            log.warning('Unable to generate primary composite file automatically for %s: %s', dataset.dataset.id, unicodify(e))
+            log.warning(
+                "Unable to generate primary composite file automatically for %s: %s", dataset.dataset.id, unicodify(e)
+            )
 
 
 def collect_shrinked_content_from_path(path):
     try:
-        with open(path, 'rb') as fh:
+        with open(path, "rb") as fh:
             return shrink_and_unicodify(fh.read().strip())
     except FileNotFoundError:
         return None
```

### Comparing `galaxy-job-execution-22.1.1/galaxy/job_execution/ports/view.py` & `galaxy-job-execution-23.0.1/galaxy/job_execution/ports/view.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import logging
 
 from galaxy import (
     model,
-    util
+    util,
+)
+from galaxy.exceptions import (
+    ItemAccessibilityException,
+    ObjectAttributeMissingException,
 )
-from galaxy.exceptions import ItemAccessibilityException, ObjectAttributeMissingException
 
 log = logging.getLogger(__name__)
 
 
 class JobPortsView:
-
     def __init__(self, app):
         self._app = app
 
     def register_container_information(self, job_id, **kwd):
         job = self.__authorize_job_access(job_id, **kwd)
         container_runtime = kwd.get("container_runtime")
         log.info(kwd)
```

### Comparing `galaxy-job-execution-22.1.1/galaxy/job_execution/setup.py` & `galaxy-job-execution-23.0.1/galaxy/job_execution/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,100 @@
 """Utilities to help job and tool code setup jobs."""
 import json
 import os
-from typing import Any, cast, Dict, List, Optional, Tuple, Union
+from typing import (
+    Any,
+    cast,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
 
 from galaxy.files import (
     ConfiguredFileSources,
     DictFileSourcesUserContext,
     ProvidesUserFileSourcesUserContext,
 )
 from galaxy.job_execution.datasets import (
     DatasetPath,
+    DatasetPathRewriter,
     get_path_rewriter,
 )
 from galaxy.model import (
     DatasetInstance,
     Job,
     JobExportHistoryArchive,
     MetadataFile,
 )
 from galaxy.util import safe_makedirs
 from galaxy.util.dictifiable import Dictifiable
 
-TOOL_PROVIDED_JOB_METADATA_FILE = 'galaxy.json'
-TOOL_PROVIDED_JOB_METADATA_KEYS = ['name', 'info', 'dbkey', 'created_from_basename']
+TOOL_PROVIDED_JOB_METADATA_FILE = "galaxy.json"
+TOOL_PROVIDED_JOB_METADATA_KEYS = ["name", "info", "dbkey", "created_from_basename"]
 
 
 OutputHdasAndType = Dict[str, Tuple[DatasetInstance, DatasetPath]]
 OutputPaths = List[DatasetPath]
 
 
 class JobIO(Dictifiable):
     dict_collection_visible_keys = (
-        'job_id',
-        'working_directory',
-        'outputs_directory',
-        'outputs_to_working_directory',
-        'galaxy_url',
-        'version_path',
-        'tool_directory',
-        'home_directory',
-        'tmp_directory',
-        'tool_data_path',
-        'galaxy_data_manager_data_path',
-        'new_file_path',
-        'len_file_path',
-        'builds_file_path',
-        'file_sources_dict',
-        'check_job_script_integrity',
-        'check_job_script_integrity_count',
-        'check_job_script_integrity_sleep',
-        'tool_source',
-        'tool_source_class',
-        'tool_dir',
-        'is_task',
+        "job_id",
+        "working_directory",
+        "outputs_directory",
+        "outputs_to_working_directory",
+        "galaxy_url",
+        "version_path",
+        "tool_directory",
+        "home_directory",
+        "tmp_directory",
+        "tool_data_path",
+        "galaxy_data_manager_data_path",
+        "new_file_path",
+        "len_file_path",
+        "builds_file_path",
+        "file_sources_dict",
+        "check_job_script_integrity",
+        "check_job_script_integrity_count",
+        "check_job_script_integrity_sleep",
+        "tool_source",
+        "tool_source_class",
+        "tool_dir",
+        "is_task",
     )
 
     def __init__(
-            self,
-            sa_session,
-            job: Job,
-            working_directory: str,
-            outputs_directory: str,
-            outputs_to_working_directory: bool,
-            galaxy_url: str,
-            version_path: str,
-            tool_directory: str,
-            home_directory: str,
-            tmp_directory: str,
-            tool_data_path: str,
-            galaxy_data_manager_data_path: str,
-            new_file_path: str,
-            len_file_path: str,
-            builds_file_path: str,
-            check_job_script_integrity: bool,
-            check_job_script_integrity_count: int,
-            check_job_script_integrity_sleep: float,
-            file_sources_dict: Dict[str, Any],
-            user_context: Union[ProvidesUserFileSourcesUserContext, Dict['str', Any]],
-            tool_source: Optional[str] = None,
-            tool_source_class: Optional['str'] = 'XmlToolSource',
-            tool_dir: Optional[str] = None,
-            is_task: bool = False):
+        self,
+        sa_session,
+        job: Job,
+        working_directory: str,
+        outputs_directory: str,
+        outputs_to_working_directory: bool,
+        galaxy_url: str,
+        version_path: str,
+        tool_directory: str,
+        home_directory: str,
+        tmp_directory: str,
+        tool_data_path: str,
+        galaxy_data_manager_data_path: str,
+        new_file_path: str,
+        len_file_path: str,
+        builds_file_path: str,
+        check_job_script_integrity: bool,
+        check_job_script_integrity_count: int,
+        check_job_script_integrity_sleep: float,
+        file_sources_dict: Dict[str, Any],
+        user_context: Union[ProvidesUserFileSourcesUserContext, Dict["str", Any]],
+        tool_source: Optional[str] = None,
+        tool_source_class: Optional["str"] = "XmlToolSource",
+        tool_dir: Optional[str] = None,
+        is_task: bool = False,
+    ):
         user_context_instance: Union[ProvidesUserFileSourcesUserContext, DictFileSourcesUserContext]
         if isinstance(user_context, dict):
             user_context_instance = DictFileSourcesUserContext(**user_context)
         else:
             user_context_instance = user_context
         self.file_sources_dict = file_sources_dict
         self.user_context = user_context_instance
@@ -109,161 +119,162 @@
         self.check_job_script_integrity_sleep = check_job_script_integrity_sleep
         self.tool_dir = tool_dir
         self.is_task = is_task
         self.tool_source = tool_source
         self.tool_source_class = tool_source_class
         self._output_paths: Optional[OutputPaths] = None
         self._output_hdas_and_paths: Optional[OutputHdasAndType] = None
-        self._dataset_path_rewriter = None
+        self._dataset_path_rewriter: Optional[DatasetPathRewriter] = None
 
     @classmethod
     def from_json(cls, path, sa_session):
         with open(path) as job_io_serialized:
             io_dict = json.load(job_io_serialized)
         return cls.from_dict(io_dict=io_dict, sa_session=sa_session)
 
     @classmethod
     def from_dict(cls, io_dict, sa_session):
-        io_dict.pop('model_class')
-        job_id = io_dict.pop('job_id')
+        io_dict.pop("model_class")
+        job_id = io_dict.pop("job_id")
         job = sa_session.query(Job).get(job_id)
         return cls(sa_session=sa_session, job=job, **io_dict)
 
     def to_dict(self):
         io_dict = super().to_dict()
-        io_dict['user_context'] = self.user_context.to_dict()
+        io_dict["user_context"] = self.user_context.to_dict()
         return io_dict
 
     def to_json(self, path):
-        with open(path, 'w') as out:
+        with open(path, "w") as out:
             out.write(json.dumps(self.to_dict()))
 
     @property
     def file_sources(self) -> ConfiguredFileSources:
         return ConfiguredFileSources.from_dict(self.file_sources_dict)
 
     @property
-    def dataset_path_rewriter(self):
+    def dataset_path_rewriter(self) -> DatasetPathRewriter:
         if self._dataset_path_rewriter is None:
             self._dataset_path_rewriter = get_path_rewriter(
                 outputs_to_working_directory=self.outputs_to_working_directory,
                 working_directory=self.working_directory,
                 outputs_directory=self.outputs_directory,
                 is_task=self.is_task,
             )
+        assert self._dataset_path_rewriter is not None
         return self._dataset_path_rewriter
 
     @property
     def output_paths(self) -> OutputPaths:
         if self._output_paths is None:
             self.compute_outputs()
         return cast(OutputPaths, self._output_paths)
 
     @property
     def output_hdas_and_paths(self) -> OutputHdasAndType:
         if self._output_hdas_and_paths is None:
             self.compute_outputs()
         return cast(OutputHdasAndType, self._output_hdas_and_paths)
 
-    def get_input_dataset_fnames(self, ds: DatasetInstance):
+    def get_input_dataset_fnames(self, ds: DatasetInstance) -> List[str]:
         filenames = [ds.file_name]
         # we will need to stage in metadata file names also
         # TODO: would be better to only stage in metadata files that are actually needed (found in command line, referenced in config files, etc.)
         for value in ds.metadata.values():
             if isinstance(value, MetadataFile):
                 filenames.append(value.file_name)
         return filenames
 
-    def get_input_fnames(self):
+    def get_input_fnames(self) -> List[str]:
         job = self.job
         filenames = []
         for da in job.input_datasets + job.input_library_datasets:  # da is JobToInputDatasetAssociation object
             if da.dataset:
                 filenames.extend(self.get_input_dataset_fnames(da.dataset))
         return filenames
 
-    def get_input_paths(self):
+    def get_input_paths(self) -> List[DatasetPath]:
         job = self.job
         paths = []
         for da in job.input_datasets + job.input_library_datasets:  # da is JobToInputDatasetAssociation object
             if da.dataset:
                 paths.append(self.get_input_path(da.dataset))
         return paths
 
-    def get_input_path(self, dataset: DatasetInstance):
+    def get_input_path(self, dataset: DatasetInstance) -> DatasetPath:
         real_path = dataset.file_name
-        false_path = self.dataset_path_rewriter.rewrite_dataset_path(dataset, 'input')
+        false_path = self.dataset_path_rewriter.rewrite_dataset_path(dataset, "input")
         return DatasetPath(
             dataset.dataset.id,
             real_path=real_path,
             false_path=false_path,
             mutable=False,
             dataset_uuid=dataset.dataset.uuid,
             object_store_id=dataset.dataset.object_store_id,
         )
 
-    def get_output_basenames(self):
+    def get_output_basenames(self) -> List[str]:
         return [os.path.basename(str(fname)) for fname in self.get_output_fnames()]
 
-    def get_output_fnames(self):
+    def get_output_fnames(self) -> OutputPaths:
         return self.output_paths
 
     def get_output_path(self, dataset):
         if getattr(dataset, "fake_dataset_association", False):
             return dataset.file_name
         assert dataset.id is not None, f"{dataset} needs to be flushed to find output path"
-        for (hda, dataset_path) in self.output_hdas_and_paths.values():
+        for hda, dataset_path in self.output_hdas_and_paths.values():
             if hda.id == dataset.id:
                 return dataset_path
         raise KeyError(f"Couldn't find job output for [{dataset}] in [{self.output_hdas_and_paths.values()}]")
 
     def get_mutable_output_fnames(self):
         return [dsp for dsp in self.output_paths if dsp.mutable]
 
-    def get_output_hdas_and_fnames(self):
+    def get_output_hdas_and_fnames(self) -> OutputHdasAndType:
         return self.output_hdas_and_paths
 
-    def compute_outputs(self):
+    def compute_outputs(self) -> None:
         dataset_path_rewriter = self.dataset_path_rewriter
 
         job = self.job
         # Job output datasets are combination of history, library, and jeha datasets.
         special = self.sa_session.query(JobExportHistoryArchive).filter_by(job=job).first()
         false_path = None
 
         results = []
         for da in job.output_datasets + job.output_library_datasets:
-            da_false_path = dataset_path_rewriter.rewrite_dataset_path(da.dataset, 'output')
+            da_false_path = dataset_path_rewriter.rewrite_dataset_path(da.dataset, "output")
             mutable = da.dataset.dataset.external_filename is None
-            dataset_path = DatasetPath(da.dataset.dataset.id, da.dataset.file_name, false_path=da_false_path, mutable=mutable)
+            dataset_path = DatasetPath(
+                da.dataset.dataset.id, da.dataset.file_name, false_path=da_false_path, mutable=mutable
+            )
             results.append((da.name, da.dataset, dataset_path))
 
         self._output_paths = [t[2] for t in results]
         self._output_hdas_and_paths = {t[0]: t[1:] for t in results}
         if special:
-            false_path = dataset_path_rewriter.rewrite_dataset_path(special, 'output')
+            false_path = dataset_path_rewriter.rewrite_dataset_path(special, "output")
             dsp = DatasetPath(special.dataset.id, special.dataset.file_name, false_path)
             self._output_paths.append(dsp)
             self._output_hdas_and_paths["output_file"] = (special.fda, dsp)
 
-    def get_output_file_id(self, file):
+    def get_output_file_id(self, file: str) -> Optional[int]:
         for dp in self.output_paths:
             if self.outputs_to_working_directory and os.path.basename(dp.false_path) == file:
                 return dp.dataset_id
             elif os.path.basename(dp.real_path) == file:
                 return dp.dataset_id
         return None
 
 
-def ensure_configs_directory(work_dir):
+def ensure_configs_directory(work_dir: str) -> str:
     configs_dir = os.path.join(work_dir, "configs")
     if not os.path.exists(configs_dir):
         safe_makedirs(configs_dir)
     return configs_dir
 
 
-def create_working_directory_for_job(object_store, job):
-    object_store.create(
-        job, base_dir='job_work', dir_only=True, obj_dir=True)
-    working_directory = object_store.get_filename(
-        job, base_dir='job_work', dir_only=True, obj_dir=True)
+def create_working_directory_for_job(object_store, job) -> str:
+    object_store.create(job, base_dir="job_work", dir_only=True, obj_dir=True)
+    working_directory = object_store.get_filename(job, base_dir="job_work", dir_only=True, obj_dir=True)
     return working_directory
```

### Comparing `galaxy-job-execution-22.1.1/galaxy/metadata/__init__.py` & `galaxy-job-execution-23.0.1/galaxy/metadata/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,56 +4,83 @@
 import json
 import os
 import shutil
 from logging import getLogger
 
 import galaxy.model
 from galaxy.model import store
-from galaxy.model.metadata import FileParameter, MetadataTempFile
+from galaxy.model.metadata import (
+    FileParameter,
+    MetadataTempFile,
+)
 from galaxy.model.store import DirectoryModelExportStore
 from galaxy.util import safe_makedirs
 
 log = getLogger(__name__)
 
-SET_METADATA_SCRIPT = 'from galaxy_ext.metadata.set_metadata import set_metadata; set_metadata()'
+SET_METADATA_SCRIPT = """
+import os
+import traceback
+try:
+    from galaxy_ext.metadata.set_metadata import set_metadata; set_metadata()
+except Exception:
+    WORKING_DIRECTORY = os.getcwd()
+    WORKING_PARENT = os.path.join(WORKING_DIRECTORY, os.path.pardir)
+    if not os.path.isdir("working") and os.path.isdir(os.path.join(WORKING_PARENT, "working")):
+        # We're probably in pulsar
+        WORKING_DIRECTORY = WORKING_PARENT
+    METADATA_DIRECTORY = os.path.join(WORKING_DIRECTORY, "metadata")
+    EXPORT_STORE_DIRECTORY = os.path.join(METADATA_DIRECTORY, "outputs_populated")
+    os.makedirs(EXPORT_STORE_DIRECTORY, exist_ok=True)
+    with open(os.path.join(EXPORT_STORE_DIRECTORY, "traceback.txt"), "w") as out:
+        out.write(traceback.format_exc())
+    raise
+"""
 
 
 def get_metadata_compute_strategy(config, job_id, metadata_strategy_override=None, tool_id=None):
     metadata_strategy = metadata_strategy_override or config.metadata_strategy
     if metadata_strategy == "legacy":
-        raise Exception('legacy metadata_strategy has been removed')
-    elif metadata_strategy == "extended" and tool_id != "__SET_METADATA__":
+        raise Exception("legacy metadata_strategy has been removed")
+    elif "extended" in metadata_strategy and tool_id != "__SET_METADATA__":
         return ExtendedDirectoryMetadataGenerator(job_id)
     else:
         return PortableDirectoryMetadataGenerator(job_id)
 
 
 class MetadataCollectionStrategy(metaclass=abc.ABCMeta):
-    """Interface describing the abstract process of writing out and collecting output metadata.
-    """
-    extended = False
-
-    def invalidate_external_metadata(self, datasets, sa_session):
-        """Invalidate written files."""
-
-    def set_job_runner_external_pid(self, pid, sa_session):
-        pass
+    """Interface describing the abstract process of writing out and collecting output metadata."""
 
-    def cleanup_external_metadata(self, sa_session):
-        pass
+    extended = False
 
     @abc.abstractmethod
-    def setup_external_metadata(self, datasets_dict, out_collections, sa_session, exec_dir=None,
-                                tmp_dir=None, dataset_files_path=None,
-                                output_fnames=None, config_root=None, use_bin=False,
-                                config_file=None, datatypes_config=None,
-                                job_metadata=None, provided_metadata_style=None, compute_tmp_dir=None,
-                                include_command=True, max_metadata_value_size=0, max_discovered_files=None,
-                                object_store_conf=None, tool=None, job=None,
-                                kwds=None):
+    def setup_external_metadata(
+        self,
+        datasets_dict,
+        out_collections,
+        sa_session,
+        exec_dir=None,
+        tmp_dir=None,
+        dataset_files_path=None,
+        output_fnames=None,
+        config_root=None,
+        use_bin=False,
+        config_file=None,
+        datatypes_config=None,
+        job_metadata=None,
+        provided_metadata_style=None,
+        compute_tmp_dir=None,
+        include_command=True,
+        max_metadata_value_size=0,
+        max_discovered_files=None,
+        object_store_conf=None,
+        tool=None,
+        job=None,
+        kwds=None,
+    ):
         """Setup files needed for external metadata collection.
 
         If include_command is True, return full Python command to externally compute metadata
         otherwise just the arguments to galaxy_ext.metadata.set_metadata required to build.
         """
 
     @abc.abstractmethod
@@ -61,19 +88,20 @@
         """Return boolean indicating if metadata for specified dataset was written properly."""
 
     @abc.abstractmethod
     def load_metadata(self, dataset, name, sa_session, working_directory, remote_metadata_directory=None):
         """Load metadata calculated externally into specified dataset."""
 
     def _load_metadata_from_path(self, dataset, metadata_output_path, working_directory, remote_metadata_directory):
-
         def path_rewriter(path):
             if not path:
                 return path
-            normalized_remote_metadata_directory = remote_metadata_directory and os.path.normpath(remote_metadata_directory)
+            normalized_remote_metadata_directory = remote_metadata_directory and os.path.normpath(
+                remote_metadata_directory
+            )
             normalized_path = os.path.normpath(path)
             if remote_metadata_directory and normalized_path.startswith(normalized_remote_metadata_directory):
                 if self.portable:
                     target_directory = os.path.join(working_directory, "metadata")
                 else:
                     target_directory = working_directory
                 return normalized_path.replace(normalized_remote_metadata_directory, target_directory, 1)
@@ -86,34 +114,52 @@
             with open(filename_results_code) as f:
                 rval, rstring = json.load(f)
         except OSError:
             rval = False
             rstring = f"Metadata results could not be read from '{filename_results_code}'"
 
         if not rval:
-            log.debug(f'setting metadata externally failed for {dataset.__class__.__name__} {dataset.id}: {rstring}')
+            log.debug(f"setting metadata externally failed for {dataset.__class__.__name__} {dataset.id}: {rstring}")
         return rval
 
 
 class PortableDirectoryMetadataGenerator(MetadataCollectionStrategy):
     portable = True
     write_object_store_conf = False
 
     def __init__(self, job_id):
         self.job_id = job_id
 
-    def setup_external_metadata(self, datasets_dict, out_collections, sa_session, exec_dir=None,
-                                tmp_dir=None, dataset_files_path=None,
-                                output_fnames=None, config_root=None, use_bin=False,
-                                config_file=None, datatypes_config=None,
-                                job_metadata=None, provided_metadata_style=None, compute_tmp_dir=None,
-                                include_command=True, max_metadata_value_size=0, max_discovered_files=None,
-                                validate_outputs=False,
-                                object_store_conf=None, tool=None, job=None, link_data_only=False,
-                                kwds=None):
+    def setup_external_metadata(
+        self,
+        datasets_dict,
+        out_collections,
+        sa_session,
+        exec_dir=None,
+        tmp_dir=None,
+        dataset_files_path=None,
+        output_fnames=None,
+        config_root=None,
+        use_bin=False,
+        config_file=None,
+        datatypes_config=None,
+        job_metadata=None,
+        provided_metadata_style=None,
+        compute_tmp_dir=None,
+        compute_version_path=None,
+        include_command=True,
+        max_metadata_value_size=0,
+        max_discovered_files=None,
+        validate_outputs=False,
+        object_store_conf=None,
+        tool=None,
+        job=None,
+        link_data_only=False,
+        kwds=None,
+    ):
         assert job_metadata, "setup_external_metadata must be supplied with job_metadata path"
         kwds = kwds or {}
         if not job:
             job = sa_session.query(galaxy.model.Job).get(self.job_id)
         tmp_dir = _init_tmp_dir(tmp_dir)
 
         metadata_dir = os.path.join(tmp_dir, "metadata")
@@ -129,86 +175,102 @@
 
         for name, dataset in datasets_dict.items():
             assert name is not None
             assert name not in outputs
             key = name
 
             def _metadata_path(what):
-                return os.path.join(metadata_dir, f"metadata_{what}_{key}")
+                return os.path.join(metadata_dir, f"metadata_{what}_{key}")  # noqa: B023
 
-            _initialize_metadata_inputs(dataset, _metadata_path, tmp_dir, kwds, real_metadata_object=self.write_object_store_conf)
+            _initialize_metadata_inputs(
+                dataset, _metadata_path, tmp_dir, kwds, real_metadata_object=self.write_object_store_conf
+            )
 
             outputs[name] = {
                 "filename_override": _get_filename_override(output_fnames, dataset.file_name),
                 "validate": validate_outputs,
                 "object_store_store_by": dataset.dataset.store_by,
-                'id': dataset.id,
-                'model_class': 'LibraryDatasetDatasetAssociation' if isinstance(dataset, galaxy.model.LibraryDatasetDatasetAssociation) else 'HistoryDatasetAssociation'
+                "id": dataset.id,
+                "model_class": "LibraryDatasetDatasetAssociation"
+                if isinstance(dataset, galaxy.model.LibraryDatasetDatasetAssociation)
+                else "HistoryDatasetAssociation",
             }
 
         metadata_params_path = os.path.join(metadata_dir, "params.json")
-        datatypes_config = os.path.relpath(datatypes_config, tmp_dir)
+        datatypes_config = os.path.relpath(datatypes_config, tmp_dir) if datatypes_config else None
         metadata_params = {
             "job_metadata": job_relative_path(job_metadata),
             "provided_metadata_style": provided_metadata_style,
             "datatypes_config": datatypes_config,
             "max_metadata_value_size": max_metadata_value_size,
             "max_discovered_files": max_discovered_files,
             "outputs": outputs,
         }
 
         # export model objects and object store configuration for extended metadata also.
         export_directory = os.path.join(metadata_dir, "outputs_new")
-        with DirectoryModelExportStore(export_directory, for_edit=True, strip_metadata_files=False, serialize_dataset_objects=True, serialize_jobs=False) as export_store:
+        with DirectoryModelExportStore(
+            export_directory,
+            for_edit=True,
+            strip_metadata_files=False,
+            serialize_dataset_objects=True,
+            serialize_jobs=False,
+        ) as export_store:
             export_store.export_job(job, tool=tool)
             for dataset in datasets_dict.values():
                 export_store.add_dataset(dataset)
 
             for name, dataset_collection in out_collections.items():
                 export_store.export_collection(dataset_collection)
                 output_collections[name] = {
-                    'id': dataset_collection.id,
-                    'model_class': dataset_collection.__class__.__name__
+                    "id": dataset_collection.id,
+                    "model_class": dataset_collection.__class__.__name__,
                 }
 
         if self.write_object_store_conf:
             with open(os.path.join(metadata_dir, "object_store_conf.json"), "w") as f:
                 json.dump(object_store_conf, f)
 
             # setup tool
             tool_as_dict = {}
             tool_as_dict["stdio_exit_codes"] = [e.to_dict() for e in tool.stdio_exit_codes]
             tool_as_dict["stdio_regexes"] = [r.to_dict() for r in tool.stdio_regexes]
             tool_as_dict["outputs"] = {name: output.to_dict() for name, output in tool.outputs.items()}
-            tool_as_dict["output_collections"] = {name: output.to_dict() for name, output in tool.output_collections.items()}
+            tool_as_dict["output_collections"] = {
+                name: output.to_dict() for name, output in tool.output_collections.items()
+            }
 
             # setup the rest
             metadata_params["tool"] = tool_as_dict
             metadata_params["link_data_only"] = link_data_only
             metadata_params["tool_path"] = tool.config_file
             metadata_params["job_id_tag"] = job.get_id_tag()
-            metadata_params["implicit_collection_jobs_association_id"] = job.implicit_collection_jobs_association and job.implicit_collection_jobs_association.id
+            metadata_params["implicit_collection_jobs_association_id"] = (
+                job.implicit_collection_jobs_association and job.implicit_collection_jobs_association.id
+            )
             metadata_params["job_params"] = job.raw_param_dict()
             metadata_params["output_collections"] = output_collections
+            if compute_version_path:
+                metadata_params["compute_version_path"] = compute_version_path
 
         with open(metadata_params_path, "w") as f:
             json.dump(metadata_params, f)
 
         if include_command:
             # return command required to build
             if use_bin:
                 return "galaxy-set-metadata"
             else:
                 script_path = os.path.join(metadata_dir, "set.py")
                 with open(script_path, "w") as f:
                     f.write(SET_METADATA_SCRIPT)
-                return 'python "metadata/set.py"'
+                return "python metadata/set.py"
         else:
             # return args to galaxy_ext.metadata.set_metadata required to build
-            return ''
+            return ""
 
     def load_metadata(self, dataset, name, sa_session, working_directory, remote_metadata_directory=None):
         metadata_output_path = os.path.join(working_directory, "metadata", f"metadata_out_{name}")
         self._load_metadata_from_path(dataset, metadata_output_path, working_directory, remote_metadata_directory)
 
     def external_metadata_set_successfully(self, dataset, name, sa_session, working_directory):
         metadata_results_path = os.path.join(working_directory, "metadata", f"metadata_results_{name}")
@@ -232,41 +294,43 @@
 
     def load_metadata(self, dataset, name, sa_session, working_directory, remote_metadata_directory=None):
         # This method shouldn't really be called one-at-a-time dataset-wise like this and
         # isn't in job_wrapper.finish, instead finish just executes perform_import() on
         # the target model store within the context of a session to bring in all the changed objects.
         # However, this method is part of the metadata interface and is used by unit tests,
         # so we allow a sessionless import and loading of individual dataset as below.
-        import_model_store = store.imported_store_for_metadata(os.path.join(working_directory, 'metadata', 'outputs_populated'))
+        import_model_store = store.imported_store_for_metadata(
+            os.path.join(working_directory, "metadata", "outputs_populated")
+        )
         imported_dataset = import_model_store.sa_session.query(galaxy.model.HistoryDatasetAssociation).find(dataset.id)
         dataset.metadata = imported_dataset.metadata
         return dataset
 
 
 def _initialize_metadata_inputs(dataset, path_for_part, tmp_dir, kwds, real_metadata_object=True):
     filename_out = path_for_part("out")
     filename_results_code = path_for_part("results")
     filename_kwds = path_for_part("kwds")
     filename_override_metadata = path_for_part("override")
 
-    open(filename_out, 'wt+')  # create the file on disk, so it cannot be reused by tempfile (unlikely, but possible)
+    open(filename_out, "wt+")  # create the file on disk, so it cannot be reused by tempfile (unlikely, but possible)
     # create the file on disk, so it cannot be reused by tempfile (unlikely, but possible)
-    json.dump((False, 'External set_meta() not called'), open(filename_results_code, 'wt+'))
-    json.dump(kwds, open(filename_kwds, 'wt+'), ensure_ascii=True)
+    json.dump((False, "External set_meta() not called"), open(filename_results_code, "wt+"))
+    json.dump(kwds, open(filename_kwds, "wt+"), ensure_ascii=True)
 
     override_metadata = []
     for meta_key, spec_value in dataset.metadata.spec.items():
         if isinstance(spec_value.param, FileParameter) and dataset.metadata.get(meta_key, None) is not None:
             if not real_metadata_object:
                 metadata_temp = MetadataTempFile()
                 metadata_temp.tmp_dir = tmp_dir
                 shutil.copy(dataset.metadata.get(meta_key, None).file_name, metadata_temp.file_name)
                 override_metadata.append((meta_key, metadata_temp.to_JSON()))
 
-    json.dump(override_metadata, open(filename_override_metadata, 'wt+'))
+    json.dump(override_metadata, open(filename_override_metadata, "wt+"))
 
     return filename_out, filename_results_code, filename_kwds, filename_override_metadata
 
 
 def _get_filename_override(output_fnames, file_name):
     if output_fnames:
         for dataset_path in output_fnames:
```

### Comparing `galaxy-job-execution-22.1.1/galaxy/metadata/set_metadata.py` & `galaxy-job-execution-23.0.1/galaxy/metadata/set_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 import glob
 import json
 import logging
 import os
 import sys
 import traceback
 from pathlib import Path
+from typing import Optional
 
 try:
     from pulsar.client.staging import COMMAND_VERSION_FILENAME
 except ImportError:
     # Package unit tests
-    COMMAND_VERSION_FILENAME = 'COMMAND_VERSION'
+    COMMAND_VERSION_FILENAME = "COMMAND_VERSION"
 
 import galaxy.datatypes.registry
 import galaxy.model.mapping
 from galaxy.datatypes import sniff
 from galaxy.datatypes.data import validate
 from galaxy.job_execution.output_collect import (
     collect_dynamic_outputs,
@@ -43,15 +44,18 @@
     HistoryDatasetAssociation,
     Job,
     store,
 )
 from galaxy.model.custom_types import total_size
 from galaxy.model.metadata import MetadataTempFile
 from galaxy.model.store.discover import MaxDiscoveredFilesExceededError
-from galaxy.objectstore import build_object_store_from_config
+from galaxy.objectstore import (
+    build_object_store_from_config,
+    ObjectStore,
+)
 from galaxy.tool_util.output_checker import (
     check_output,
     DETECTED_JOB_STATE,
 )
 from galaxy.tool_util.parser.stdio import (
     ToolStdioExitCode,
     ToolStdioRegex,
@@ -63,51 +67,60 @@
 )
 from galaxy.util.expressions import ExpressionContext
 
 logging.basicConfig()
 log = logging.getLogger(__name__)
 
 
-MAX_STDIO_READ_BYTES = 100 * 10 ** 6  # 100 MB
+MAX_STDIO_READ_BYTES = 100 * 10**6  # 100 MB
 
 
 def set_validated_state(dataset_instance):
     datatype_validation = validate(dataset_instance)
 
     dataset_instance.validated_state = datatype_validation.state
     dataset_instance.validated_state_message = datatype_validation.message
 
     # Set special metadata property that will reload this on server side.
     dataset_instance.metadata.__validated_state__ = datatype_validation.state
     dataset_instance.metadata.__validated_state_message__ = datatype_validation.message
 
 
-def set_meta_with_tool_provided(dataset_instance, file_dict, set_meta_kwds, datatypes_registry, max_metadata_value_size):
+def set_meta_with_tool_provided(
+    dataset_instance,
+    file_dict,
+    set_meta_kwds,
+    datatypes_registry,
+    max_metadata_value_size,
+):
     # This method is somewhat odd, in that we set the metadata attributes from tool,
     # then call set_meta, then set metadata attributes from tool again.
     # This is intentional due to interplay of overwrite kwd, the fact that some metadata
     # parameters may rely on the values of others, and that we are accepting the
     # values provided by the tool as Truth.
     extension = dataset_instance.extension
     if extension == "_sniff_":
         try:
-            extension = sniff.handle_uploaded_dataset_file(dataset_instance.dataset.external_filename, datatypes_registry)
+            extension = sniff.handle_uploaded_dataset_file(
+                dataset_instance.dataset.external_filename, datatypes_registry
+            )
             # We need to both set the extension so it is available to set_meta
             # and record it in the metadata so it can be reloaded on the server
             # side and the model updated (see MetadataCollection.{from,to}_JSON_dict)
             dataset_instance.extension = extension
             # Set special metadata property that will reload this on server side.
             dataset_instance.metadata.__extension__ = extension
         except Exception:
             log.exception("Problem sniffing datatype.")
 
-    for metadata_name, metadata_value in file_dict.get('metadata', {}).items():
+    for metadata_name, metadata_value in file_dict.get("metadata", {}).items():
         setattr(dataset_instance.metadata, metadata_name, metadata_value)
-    dataset_instance.datatype.set_meta(dataset_instance, **set_meta_kwds)
-    for metadata_name, metadata_value in file_dict.get('metadata', {}).items():
+    if not dataset_instance.metadata_deferred:
+        dataset_instance.datatype.set_meta(dataset_instance, **set_meta_kwds)
+    for metadata_name, metadata_value in file_dict.get("metadata", {}).items():
         setattr(dataset_instance.metadata, metadata_name, metadata_value)
 
     if max_metadata_value_size:
         for k, v in list(dataset_instance.metadata.items()):
             if total_size(v) > max_metadata_value_size:
                 log.info(f"Key {k} too large for metadata, discarding")
                 dataset_instance.metadata.remove_key(k)
@@ -122,48 +135,68 @@
     try:
         with open(metadata_params_path) as f:
             return json.load(f)
     except OSError:
         raise Exception(f"Failed to find metadata/params.json from cwd [{tool_job_working_directory}]")
 
 
-def get_object_store(tool_job_working_directory):
-    object_store_conf_path = os.path.join(tool_job_working_directory, "metadata", "object_store_conf.json")
-    with open(object_store_conf_path) as f:
-        config_dict = json.load(f)
-    assert config_dict is not None
-    object_store = build_object_store_from_config(None, config_dict=config_dict)
+def get_object_store(tool_job_working_directory, object_store=None):
+    if not object_store:
+        object_store_conf_path = os.path.join(tool_job_working_directory, "metadata", "object_store_conf.json")
+        with open(object_store_conf_path) as f:
+            config_dict = json.load(f)
+        assert config_dict is not None
+        object_store = build_object_store_from_config(None, config_dict=config_dict)
     Dataset.object_store = object_store
     return object_store
 
 
-def set_metadata_portable():
-    tool_job_working_directory = os.path.abspath(os.getcwd())
+def set_metadata_portable(
+    tool_job_working_directory=None,
+    object_store: Optional[ObjectStore] = None,
+    extended_metadata_collection: Optional[bool] = None,
+):
+    is_celery_task = tool_job_working_directory is not None
+    tool_job_working_directory = Path(tool_job_working_directory or os.path.abspath(os.getcwd()))
     metadata_tmp_files_dir = os.path.join(tool_job_working_directory, "metadata")
-    MetadataTempFile.tmp_dir = metadata_tmp_files_dir
-
     metadata_params = get_metadata_params(tool_job_working_directory)
-    datatypes_config = metadata_params["datatypes_config"]
-    job_metadata = metadata_params["job_metadata"]
+    if not is_celery_task:
+        if not extended_metadata_collection:
+            # Legacy handling for datatypes that don't pass metadata_tmp_files_dir from set_meta kwargs
+            # to MetadataTempFile constructor. Remove if we ever remove TS datatypes.
+            MetadataTempFile.tmp_dir = metadata_tmp_files_dir
+    datatypes_config = tool_job_working_directory / metadata_params["datatypes_config"]
+    datatypes_registry = validate_and_load_datatypes_config(datatypes_config)
+    job_metadata = tool_job_working_directory / metadata_params["job_metadata"]
     provided_metadata_style = metadata_params.get("provided_metadata_style")
     max_metadata_value_size = metadata_params.get("max_metadata_value_size") or 0
     max_discovered_files = metadata_params.get("max_discovered_files")
     outputs = metadata_params["outputs"]
 
-    datatypes_registry = validate_and_load_datatypes_config(datatypes_config)
     tool_provided_metadata = load_job_metadata(job_metadata, provided_metadata_style)
 
     def set_meta(new_dataset_instance, file_dict):
-        set_meta_with_tool_provided(new_dataset_instance, file_dict, set_meta_kwds, datatypes_registry, max_metadata_value_size)
+        if not extended_metadata_collection:
+            set_meta_kwds["metadata_tmp_files_dir"] = metadata_tmp_files_dir
+        set_meta_with_tool_provided(
+            new_dataset_instance,
+            file_dict,
+            set_meta_kwds,
+            datatypes_registry,
+            max_metadata_value_size,
+        )
 
     try:
-        object_store = get_object_store(tool_job_working_directory=tool_job_working_directory)
+        object_store = get_object_store(
+            tool_job_working_directory=tool_job_working_directory, object_store=object_store
+        )
     except (FileNotFoundError, AssertionError):
         object_store = None
-    extended_metadata_collection = bool(object_store)
+    if extended_metadata_collection is None:
+        extended_metadata_collection = bool(object_store)
     job_context = None
     version_string = None
 
     export_store = None
     final_job_state = Job.states.OK
     job_messages = []
     if extended_metadata_collection:
@@ -171,281 +204,338 @@
         stdio_exit_code_dicts, stdio_regex_dicts = tool_dict["stdio_exit_codes"], tool_dict["stdio_regexes"]
         stdio_exit_codes = list(map(ToolStdioExitCode, stdio_exit_code_dicts))
         stdio_regexes = list(map(ToolStdioRegex, stdio_regex_dicts))
 
         outputs_directory = os.path.join(tool_job_working_directory, "outputs")
         if not os.path.exists(outputs_directory):
             outputs_directory = tool_job_working_directory
+        metadata_directory = os.path.join(tool_job_working_directory, "metadata")
 
         # TODO: constants...
         locations = [
-            (outputs_directory, 'tool_'),
-            (tool_job_working_directory, ''),
-            (outputs_directory, ''),  # # Pulsar style output directory? Was this ever used - did this ever work?
+            (metadata_directory, "tool_"),
+            (outputs_directory, "tool_"),
+            (tool_job_working_directory, ""),
         ]
         for directory, prefix in locations:
-            if os.path.exists(os.path.join(directory, f"{prefix}stdout")):
-                with open(os.path.join(directory, f"{prefix}stdout"), 'rb') as f:
+            if directory and os.path.exists(os.path.join(directory, f"{prefix}stdout")):
+                with open(os.path.join(directory, f"{prefix}stdout"), "rb") as f:
                     tool_stdout = f.read(MAX_STDIO_READ_BYTES)
-                with open(os.path.join(directory, f"{prefix}stderr"), 'rb') as f:
+                with open(os.path.join(directory, f"{prefix}stderr"), "rb") as f:
                     tool_stderr = f.read(MAX_STDIO_READ_BYTES)
                 break
         else:
-            if os.path.exists(os.path.join(tool_job_working_directory, 'task_0')):
+            if os.path.exists(os.path.join(tool_job_working_directory, "task_0")):
                 # We have a task splitting job
-                tool_stdout = b''
-                tool_stderr = b''
-                paths = Path(tool_job_working_directory).glob('task_*')
+                tool_stdout = b""
+                tool_stderr = b""
+                paths = tool_job_working_directory.glob("task_*")
                 for path in paths:
-                    with open(path / 'outputs' / 'tool_stdout', 'rb') as f:
+                    with open(path / "outputs" / "tool_stdout", "rb") as f:
                         task_stdout = f.read(MAX_STDIO_READ_BYTES)
                         if task_stdout:
                             tool_stdout = b"%s[%s stdout]\n%s\n" % (tool_stdout, path.name.encode(), task_stdout)
-                    with open(path / 'outputs' / 'tool_stderr', 'rb') as f:
+                    with open(path / "outputs" / "tool_stderr", "rb") as f:
                         task_stderr = f.read(MAX_STDIO_READ_BYTES)
                         if task_stderr:
                             tool_stderr = b"%s[%s stdout]\n%s\n" % (tool_stderr, path.name.encode(), task_stderr)
             else:
                 wdc = os.listdir(tool_job_working_directory)
                 odc = os.listdir(outputs_directory)
-                error_desc = "Failed to find tool_stdout or tool_stderr for this job, cannot collect metadata"
-                error_extra = f"Working dir contents [{wdc}], output directory contents [{odc}]"
-                log.warn(f"{error_desc}. {error_extra}")
-                raise Exception(error_desc)
+                if not is_celery_task:
+                    error_desc = "Failed to find tool_stdout or tool_stderr for this job, cannot collect metadata"
+                    error_extra = f"Working dir contents [{wdc}], output directory contents [{odc}]"
+                    log.warn(f"{error_desc}. {error_extra}")
+                    raise Exception(error_desc)
+                else:
+                    tool_stdout = tool_stderr = b""
 
         job_id_tag = metadata_params["job_id_tag"]
 
         exit_code_file = default_exit_code_file(".", job_id_tag)
         tool_exit_code = read_exit_code_from(exit_code_file, job_id_tag)
 
-        check_output_detected_state, tool_stdout, tool_stderr, job_messages = check_output(stdio_regexes, stdio_exit_codes, tool_stdout, tool_stderr, tool_exit_code, job_id_tag)
+        check_output_detected_state, tool_stdout, tool_stderr, job_messages = check_output(
+            stdio_regexes, stdio_exit_codes, tool_stdout, tool_stderr, tool_exit_code, job_id_tag
+        )
         if check_output_detected_state == DETECTED_JOB_STATE.OK and not tool_provided_metadata.has_failed_outputs():
             final_job_state = Job.states.OK
         else:
             final_job_state = Job.states.ERROR
 
-        version_string_path = os.path.join('outputs', COMMAND_VERSION_FILENAME)
+        default_version_string_path = os.path.join("outputs", COMMAND_VERSION_FILENAME)
+        version_string_path = metadata_params.get("compute_version_path", default_version_string_path)
         version_string = collect_shrinked_content_from_path(version_string_path)
-
         expression_context = ExpressionContext(dict(stdout=tool_stdout[:255], stderr=tool_stderr[:255]))
 
         # Load outputs.
-        export_store = store.DirectoryModelExportStore('metadata/outputs_populated', serialize_dataset_objects=True, for_edit=True, strip_metadata_files=False, serialize_jobs=True)
-    try:
-        import_model_store = store.imported_store_for_metadata('metadata/outputs_new', object_store=object_store)
-    except AssertionError:
-        # Remove in 21.09, this should only happen for jobs that started on <= 20.09 and finish now
-        import_model_store = None
-
-    tool_script_file = os.path.join(tool_job_working_directory, 'tool_script.sh')
-    job = None
-    if import_model_store and export_store:
+        export_store = store.DirectoryModelExportStore(
+            tool_job_working_directory / "metadata/outputs_populated",
+            serialize_dataset_objects=True,
+            for_edit=True,
+            strip_metadata_files=False,
+            serialize_jobs=True,
+        )
+    import_model_store = store.imported_store_for_metadata(
+        tool_job_working_directory / "metadata/outputs_new", object_store=object_store
+    )
+
+    tool_script_file = tool_job_working_directory / "tool_script.sh"
+    job: Optional[Job] = None
+    if export_store:
         job = next(iter(import_model_store.sa_session.objects[Job].values()))
 
     job_context = SessionlessJobContext(
         metadata_params,
         tool_provided_metadata,
         object_store,
         export_store,
         import_model_store,
-        os.path.join(tool_job_working_directory, "working"),
+        tool_job_working_directory / "working",
         final_job_state=final_job_state,
         max_discovered_files=max_discovered_files,
     )
 
     if extended_metadata_collection:
+        if not export_store:
+            # Can't happen, but type system doesn't know
+            raise Exception("export_store not built")
         # discover extra outputs...
         output_collections = {}
         for name, output_collection in metadata_params["output_collections"].items():
             # TODO: remove HistoryDatasetCollectionAssociation fallback on 22.01, model_class used to not be serialized prior to 21.09
-            model_class = output_collection.get('model_class', 'HistoryDatasetCollectionAssociation')
-            collection = import_model_store.sa_session.query(getattr(galaxy.model, model_class)).find(output_collection["id"])
+            model_class = output_collection.get("model_class", "HistoryDatasetCollectionAssociation")
+            collection = import_model_store.sa_session.query(getattr(galaxy.model, model_class)).find(
+                output_collection["id"]
+            )
             output_collections[name] = collection
         output_instances = {}
         for name, output in metadata_params["outputs"].items():
-            klass = getattr(galaxy.model, output.get('model_class', 'HistoryDatasetAssociation'))
+            klass = getattr(galaxy.model, output.get("model_class", "HistoryDatasetAssociation"))
             output_instances[name] = import_model_store.sa_session.query(klass).find(output["id"])
 
         input_ext = json.loads(metadata_params["job_params"].get("__input_ext") or '"data"')
         try:
             collect_primary_datasets(
                 job_context,
                 output_instances,
                 input_ext=input_ext,
             )
             collect_dynamic_outputs(job_context, output_collections)
         except MaxDiscoveredFilesExceededError as e:
             final_job_state = Job.states.ERROR
             job_messages.append(str(e))
         if job:
-            job.job_messages = job_messages
+            job.set_streams(tool_stdout=tool_stdout, tool_stderr=tool_stderr, job_messages=job_messages)
             job.state = final_job_state
-        if os.path.exists(tool_script_file):
-            with open(tool_script_file) as command_fh:
-                command_line_lines = []
-                for i, line in enumerate(command_fh):
-                    if i == 0 and line.endswith('COMMAND_VERSION 2>&1;'):
-                        # Don't record version command as part of command line
-                        continue
-                    command_line_lines.append(line)
-                job.command_line = "".join(command_line_lines).strip()
-                export_store.export_job(job, include_job_data=False)
+            if os.path.exists(tool_script_file):
+                with open(tool_script_file) as command_fh:
+                    command_line_lines = []
+                    for i, line in enumerate(command_fh):
+                        if i == 0 and line.endswith("COMMAND_VERSION 2>&1;"):
+                            # Don't record version command as part of command line
+                            continue
+                        command_line_lines.append(line)
+                    job.command_line = "".join(command_line_lines).strip()
+                    export_store.export_job(job, include_job_data=False)
 
     unnamed_id_to_path = {}
+    unnamed_is_deferred = {}
     for unnamed_output_dict in job_context.tool_provided_metadata.get_unnamed_outputs():
         destination = unnamed_output_dict["destination"]
         elements = unnamed_output_dict["elements"]
         destination_type = destination["type"]
-        if destination_type == 'hdas':
+        if destination_type == "hdas":
             for element in elements:
-                filename = element.get('filename')
-                object_id = element.get('object_id')
+                object_id = element.get("object_id")
+                if element.get("state") == "deferred":
+                    unnamed_is_deferred[object_id] = True
+                    continue
+                filename = element.get("filename")
                 if filename and object_id:
                     unnamed_id_to_path[object_id] = os.path.join(job_context.job_working_directory, filename)
 
     for output_name, output_dict in outputs.items():
         dataset_instance_id = output_dict["id"]
-        klass = getattr(galaxy.model, output_dict.get('model_class', 'HistoryDatasetAssociation'))
-        dataset = None
-        if import_model_store:
-            dataset = import_model_store.sa_session.query(klass).find(dataset_instance_id)
-        if dataset is None:
-            # legacy check for jobs that started before 21.01, remove on 21.05
-            filename_in = os.path.join(f"metadata/metadata_in_{output_name}")
-            import pickle
-            dataset = pickle.load(open(filename_in, 'rb'))  # load DatasetInstance
+        klass = getattr(galaxy.model, output_dict.get("model_class", "HistoryDatasetAssociation"))
+        dataset = import_model_store.sa_session.query(klass).find(dataset_instance_id)
         assert dataset is not None
 
-        filename_kwds = os.path.join(f"metadata/metadata_kwds_{output_name}")
-        filename_out = os.path.join(f"metadata/metadata_out_{output_name}")
-        filename_results_code = os.path.join(f"metadata/metadata_results_{output_name}")
-        override_metadata = os.path.join(f"metadata/metadata_override_{output_name}")
+        filename_kwds = tool_job_working_directory / f"metadata/metadata_kwds_{output_name}"
+        filename_out = tool_job_working_directory / f"metadata/metadata_out_{output_name}"
+        filename_results_code = tool_job_working_directory / f"metadata/metadata_results_{output_name}"
+        override_metadata = tool_job_working_directory / f"metadata/metadata_override_{output_name}"
         dataset_filename_override = output_dict["filename_override"]
-        # pre-20.05 this was a per job parameter and not a per dataset parameter, drop in 21.XX
-        legacy_object_store_store_by = metadata_params.get("object_store_store_by", "id")
-
         # Same block as below...
-        set_meta_kwds = stringify_dictionary_keys(json.load(open(filename_kwds)))  # load kwds; need to ensure our keywords are not unicode
+        set_meta_kwds = stringify_dictionary_keys(
+            json.load(open(filename_kwds))
+        )  # load kwds; need to ensure our keywords are not unicode
         try:
-            external_filename = unnamed_id_to_path.get(dataset_instance_id, dataset_filename_override)
-            if not os.path.exists(external_filename):
-                matches = glob.glob(external_filename)
-                assert len(matches) == 1, f"More than one file matched by output glob '{external_filename}'"
-                external_filename = matches[0]
-                assert safe_contains(tool_job_working_directory, external_filename), f"Cannot collect output '{external_filename}' from outside of working directory"
-                created_from_basename = os.path.relpath(external_filename, os.path.join(tool_job_working_directory, 'working'))
-                dataset.dataset.created_from_basename = created_from_basename
-            # override filename if we're dealing with outputs to working directory and dataset is not linked to
-            link_data_only = metadata_params.get("link_data_only")
-            if not link_data_only:
-                # Only set external filename if we're dealing with files in job working directory.
-                # Fixes link_data_only uploads
-                dataset.dataset.external_filename = external_filename
-                store_by = output_dict.get("object_store_store_by", legacy_object_store_store_by)
-                extra_files_dir_name = f"dataset_{getattr(dataset.dataset, store_by)}_files"
-                files_path = os.path.abspath(os.path.join(tool_job_working_directory, "working", extra_files_dir_name))
-                dataset.dataset.external_extra_files_path = files_path
+            is_deferred = bool(unnamed_is_deferred.get(dataset_instance_id))
+            dataset.metadata_deferred = is_deferred
+            if not is_deferred:
+                external_filename = unnamed_id_to_path.get(dataset_instance_id, dataset_filename_override)
+                if not os.path.exists(external_filename):
+                    matches = glob.glob(external_filename)
+                    assert len(matches) == 1, f"{len(matches)} file(s) matched by output glob '{external_filename}'"
+                    external_filename = matches[0]
+                    assert safe_contains(
+                        tool_job_working_directory, external_filename
+                    ), f"Cannot collect output '{external_filename}' from outside of working directory"
+                    created_from_basename = os.path.relpath(
+                        external_filename, os.path.join(tool_job_working_directory, "working")
+                    )
+                    dataset.dataset.created_from_basename = created_from_basename
+                # override filename if we're dealing with outputs to working directory and dataset is not linked to
+                link_data_only = metadata_params.get("link_data_only")
+                if not link_data_only:
+                    # Only set external filename if we're dealing with files in job working directory.
+                    # Fixes link_data_only uploads
+                    dataset.dataset.external_filename = external_filename
+                    store_by = output_dict.get("object_store_store_by", "id")
+                    extra_files_dir_name = f"dataset_{getattr(dataset.dataset, store_by)}_files"
+                    files_path = os.path.abspath(
+                        os.path.join(tool_job_working_directory, "working", extra_files_dir_name)
+                    )
+                    if os.path.exists(files_path):
+                        dataset.dataset.external_extra_files_path = files_path
+                    else:
+                        # could be pulsar, stores extra files in outputs directory
+                        pulsar_extra_files_path = os.path.join(
+                            tool_job_working_directory, "outputs", extra_files_dir_name
+                        )
+                        if os.path.exists(pulsar_extra_files_path):
+                            dataset.dataset.external_extra_files_path = pulsar_extra_files_path
+                        elif dataset_filename_override and not object_store:
+                            # pulsar, no remote metadata and no extended metadata
+                            dataset.dataset.external_extra_files_path = os.path.join(
+                                os.path.dirname(dataset_filename_override), extra_files_dir_name
+                            )
+
             file_dict = tool_provided_metadata.get_dataset_meta(output_name, dataset.dataset.id, dataset.dataset.uuid)
-            if 'ext' in file_dict:
-                dataset.extension = file_dict['ext']
+            if "ext" in file_dict:
+                dataset.extension = file_dict["ext"]
             # Metadata FileParameter types may not be writable on a cluster node, and are therefore temporarily substituted with MetadataTempFiles
             override_metadata = json.load(open(override_metadata))
             for metadata_name, metadata_file_override in override_metadata:
                 if MetadataTempFile.is_JSONified_value(metadata_file_override):
                     metadata_file_override = MetadataTempFile.from_JSON(metadata_file_override)
                 setattr(dataset.metadata, metadata_name, metadata_file_override)
             if output_dict.get("validate", False):
                 set_validated_state(dataset)
             if dataset_instance_id not in unnamed_id_to_path:
                 # We're going to run through set_metadata in collect_dynamic_outputs with more contextual metadata,
                 # so skip set_meta here.
                 set_meta(dataset, file_dict)
                 if extended_metadata_collection:
                     collect_extra_files(object_store, dataset, ".")
-                    dataset.state = dataset.dataset.state = final_job_state
+                    dataset_state = "deferred" if (is_deferred and final_job_state == "ok") else final_job_state
+                    if not dataset.state == dataset.states.ERROR:
+                        # Don't overwrite failed state (for invalid content) here
+                        dataset.state = dataset.dataset.state = dataset_state
 
             if extended_metadata_collection:
-                if not link_data_only and os.path.getsize(external_filename):
+                if not object_store or not export_store:
+                    # Can't happen, but type system doesn't know
+                    raise Exception("object_store not built")
+                if not is_deferred and not link_data_only and os.path.getsize(external_filename):
                     # Here we might be updating a disk based objectstore when outputs_to_working_directory is used,
                     # or a remote object store from its cache path.
                     object_store.update_from_file(dataset.dataset, file_name=external_filename, create=True)
                 # TODO: merge expression_context into tool_provided_metadata so we don't have to special case this (here and in _finish_dataset)
                 meta = tool_provided_metadata.get_dataset_meta(output_name, dataset.dataset.id, dataset.dataset.uuid)
                 if meta:
                     context = ExpressionContext(meta, expression_context)
                 else:
                     context = expression_context
-                dataset.blurb = 'done'
-                dataset.peek = 'no peek'
-                dataset.info = (dataset.info or '')
-                if context['stdout'].strip():
+                dataset.blurb = "done"
+                dataset.peek = "no peek"
+                dataset.info = dataset.info or ""
+                if context["stdout"].strip():
                     # Ensure white space between entries
                     dataset.info = f"{dataset.info.rstrip()}\n{context['stdout'].strip()}"
-                if context['stderr'].strip():
+                if context["stderr"].strip():
                     # Ensure white space between entries
                     dataset.info = f"{dataset.info.rstrip()}\n{context['stderr'].strip()}"
                 dataset.tool_version = version_string
-                if 'uuid' in context:
-                    dataset.dataset.uuid = context['uuid']
+                if "uuid" in context:
+                    dataset.dataset.uuid = context["uuid"]
                 if not final_job_state == Job.states.ERROR:
-                    line_count = context.get('line_count', None)
+                    line_count = context.get("line_count", None)
                     try:
                         # Certain datatype's set_peek methods contain a line_count argument
                         dataset.set_peek(line_count=line_count)
                     except TypeError:
                         # ... and others don't
                         dataset.set_peek()
                 for context_key in TOOL_PROVIDED_JOB_METADATA_KEYS:
                     if context_key in context:
                         context_value = context[context_key]
                         setattr(dataset, context_key, context_value)
                 # We only want to persist the external_filename if the dataset has been linked in.
-                if not link_data_only:
+                if not is_deferred and not link_data_only:
                     dataset.dataset.external_filename = None
                     dataset.dataset.extra_files_path = None
                 export_store.add_dataset(dataset)
             else:
                 dataset.metadata.to_JSON_dict(filename_out)  # write out results of set_meta
 
-            json.dump((True, 'Metadata has been set successfully'), open(filename_results_code, 'wt+'))  # setting metadata has succeeded
+            json.dump(
+                (True, "Metadata has been set successfully"), open(filename_results_code, "wt+")
+            )  # setting metadata has succeeded
         except Exception:
-            json.dump((False, traceback.format_exc()), open(filename_results_code, 'wt+'))  # setting metadata has failed somehow
+            json.dump(
+                (False, traceback.format_exc()), open(filename_results_code, "wt+")
+            )  # setting metadata has failed somehow
 
     if export_store:
+        export_store.push_metadata_files()
         export_store._finalize()
     write_job_metadata(tool_job_working_directory, job_metadata, set_meta, tool_provided_metadata)
 
 
 def validate_and_load_datatypes_config(datatypes_config):
     galaxy_root = os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, os.pardir, os.pardir))
 
     if not os.path.exists(datatypes_config):
         # Hack for Pulsar on usegalaxy.org, drop ASAP.
         datatypes_config = "configs/registry.xml"
 
     if not os.path.exists(datatypes_config):
-        print(f"Metadata setting failed because registry.xml [{datatypes_config}] could not be found. You may retry setting metadata.")
+        print(
+            f"Metadata setting failed because registry.xml [{datatypes_config}] could not be found. You may retry setting metadata."
+        )
         sys.exit(1)
     datatypes_registry = galaxy.datatypes.registry.Registry()
-    datatypes_registry.load_datatypes(root_dir=galaxy_root, config=datatypes_config, use_build_sites=False, use_converters=False, use_display_applications=False)
+    datatypes_registry.load_datatypes(
+        root_dir=galaxy_root,
+        config=datatypes_config,
+        use_build_sites=False,
+        use_converters=False,
+        use_display_applications=False,
+    )
     galaxy.model.set_datatypes_registry(datatypes_registry)
     return datatypes_registry
 
 
 def load_job_metadata(job_metadata, provided_metadata_style):
     return parse_tool_provided_metadata(job_metadata, provided_metadata_style=provided_metadata_style)
 
 
 def write_job_metadata(tool_job_working_directory, job_metadata, set_meta, tool_provided_metadata):
     for i, file_dict in enumerate(tool_provided_metadata.get_new_datasets_for_metadata_collection(), start=1):
         filename = file_dict["filename"]
         new_dataset_filename = os.path.join(tool_job_working_directory, "working", filename)
         new_dataset = Dataset(id=-i, external_filename=new_dataset_filename)
-        extra_files = file_dict.get('extra_files', None)
+        extra_files = file_dict.get("extra_files", None)
         if extra_files is not None:
             new_dataset._extra_files_path = os.path.join(tool_job_working_directory, "working", extra_files)
         new_dataset.state = new_dataset.states.OK
-        new_dataset_instance = HistoryDatasetAssociation(id=-i, dataset=new_dataset, extension=file_dict.get('ext', 'data'))
+        new_dataset_instance = HistoryDatasetAssociation(
+            id=-i, dataset=new_dataset, extension=file_dict.get("ext", "data")
+        )
         set_meta(new_dataset_instance, file_dict)
-        file_dict['metadata'] = json.loads(new_dataset_instance.metadata.to_JSON_dict())  # storing metadata in external form, need to turn back into dict, then later jsonify
+        file_dict["metadata"] = json.loads(
+            new_dataset_instance.metadata.to_JSON_dict()
+        )  # storing metadata in external form, need to turn back into dict, then later jsonify
 
     tool_provided_metadata.rewrite()
```

### Comparing `galaxy-job-execution-22.1.1/galaxy_job_execution.egg-info/PKG-INFO` & `galaxy-job-execution-23.0.1/galaxy_job_execution.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,69 +1,64 @@
 Metadata-Version: 2.1
 Name: galaxy-job-execution
-Version: 22.1.1
-Summary: Galaxy Job Execution Runtime Utilities
+Version: 23.0.1
+Summary: Galaxy job execution runtime utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-job-execution.svg
    :target: https://pypi.org/project/galaxy-job-execution/
 
 
 Overview
 --------
 
 The Galaxy_ job execution runtime module.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
-
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
+No recorded changes since last release
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
-
-
```

### Comparing `galaxy-job-execution-22.1.1/galaxy_job_execution.egg-info/SOURCES.txt` & `galaxy-job-execution-23.0.1/galaxy_job_execution.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
-Makefile
 README.rst
 dev-requirements.txt
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 test-requirements.txt
 galaxy/__init__.py
-galaxy/project_galaxy_job_execution.py
+galaxy/py.typed
 galaxy/job_execution/__init__.py
 galaxy/job_execution/compute_environment.py
+galaxy/job_execution/container_monitor.py
 galaxy/job_execution/datasets.py
 galaxy/job_execution/output_collect.py
 galaxy/job_execution/setup.py
 galaxy/job_execution/actions/__init__.py
 galaxy/job_execution/actions/post.py
 galaxy/job_execution/ports/__init__.py
 galaxy/job_execution/ports/view.py
 galaxy/metadata/__init__.py
 galaxy/metadata/set_metadata.py
 galaxy_job_execution.egg-info/PKG-INFO
 galaxy_job_execution.egg-info/SOURCES.txt
 galaxy_job_execution.egg-info/dependency_links.txt
 galaxy_job_execution.egg-info/entry_points.txt
-galaxy_job_execution.egg-info/not-zip-safe
 galaxy_job_execution.egg-info/requires.txt
-galaxy_job_execution.egg-info/top_level.txt
-scripts/commit_version.py
-scripts/new_version.py
-scripts/print_version_for_release.py
-tests/__init__.py
-tests/job_execution/__init__.py
-tests/job_execution/test_datasets.py
-tests/job_execution/test_job_io.py
+galaxy_job_execution.egg-info/top_level.txt
```

