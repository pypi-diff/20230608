# Comparing `tmp/galaxy-job-metrics-22.1.1.tar.gz` & `tmp/galaxy-job-metrics-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-job-metrics-22.1.1.tar", last modified: Mon Aug 22 19:45:52 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/job_metrics/dist/.tmp-k82uluf6/galaxy-job-metrics-23.0.1.tar", last modified: Thu Jun  8 17:39:12 2023, max compression
```

## Comparing `galaxy-job-metrics-22.1.1.tar` & `galaxy-job-metrics-23.0.1.tar`

### file list

```diff
@@ -1,51 +1,32 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:52.560481 galaxy-job-metrics-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      473 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-job-metrics-22.1.1/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       28 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1823 2022-08-22 19:45:52.560592 galaxy-job-metrics-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      332 2022-03-24 19:47:11.000000 galaxy-job-metrics-22.1.1/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:52.553004 galaxy-job-metrics-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:52.553537 galaxy-job-metrics-22.1.1/galaxy/job_metrics/
--rw-r--r--   0 mvandenb   (501) staff       (20)     5503 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:52.554853 galaxy-job-metrics-22.1.1/galaxy/job_metrics/collectl/
--rw-r--r--   0 mvandenb   (501) staff       (20)      163 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/collectl/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5445 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/collectl/cli.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     8975 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/collectl/processes.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      610 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/collectl/stats.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1572 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/collectl/subsystems.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      704 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/formatting.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:52.557201 galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1871 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5808 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/cgroup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     9196 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/collectl.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     3870 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/core.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2083 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/cpuinfo.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2389 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/env.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      951 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/hostname.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2055 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/meminfo.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1066 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/uname.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      418 2022-08-22 19:45:29.000000 galaxy-job-metrics-22.1.1/galaxy/project_galaxy_job_metrics.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:52.558904 galaxy-job-metrics-22.1.1/galaxy_job_metrics.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1823 2022-08-22 19:45:51.000000 galaxy-job-metrics-22.1.1/galaxy_job_metrics.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     1301 2022-08-22 19:45:52.000000 galaxy-job-metrics-22.1.1/galaxy_job_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:51.000000 galaxy-job-metrics-22.1.1/galaxy_job_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       27 2022-08-22 19:45:51.000000 galaxy-job-metrics-22.1.1/galaxy_job_metrics.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:45:51.000000 galaxy-job-metrics-22.1.1/galaxy_job_metrics.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)       12 2022-08-22 19:45:51.000000 galaxy-job-metrics-22.1.1/galaxy_job_metrics.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-08-22 19:45:51.000000 galaxy-job-metrics-22.1.1/galaxy_job_metrics.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       12 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:52.559626 galaxy-job-metrics-22.1.1/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:45:52.566188 galaxy-job-metrics-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2751 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-03-24 19:47:11.000000 galaxy-job-metrics-22.1.1/test-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:52.559906 galaxy-job-metrics-22.1.1/tests/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-08-18 15:49:03.000000 galaxy-job-metrics-22.1.1/tests/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:45:52.560287 galaxy-job-metrics-22.1.1/tests/job_metrics/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-08-18 15:49:03.000000 galaxy-job-metrics-22.1.1/tests/job_metrics/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1435 2022-08-22 19:45:28.000000 galaxy-job-metrics-22.1.1/tests/job_metrics/test_job_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-job-metrics-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/cgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/hostname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/meminfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/uname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/job_metrics/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-08 17:39:12.000000 galaxy-job-metrics-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:37:04.000000 galaxy-job-metrics-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-job-metrics-22.1.1/LICENSE` & `galaxy-job-metrics-23.0.1/LICENSE`

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

### Comparing `galaxy-job-metrics-22.1.1/PKG-INFO` & `galaxy-job-metrics-23.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,70 @@
 Metadata-Version: 2.1
 Name: galaxy-job-metrics
-Version: 22.1.1
-Summary: Galaxy Job Metrics
+Version: 23.0.1
+Summary: Galaxy job metrics
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
 
 
 .. image:: https://badge.fury.io/py/galaxy-job-metrics.svg
    :target: https://pypi.org/project/galaxy-job-metrics/
 
 
 Overview
 --------
 
 The Galaxy_ job metrics framework and default plugins.
 
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
 
----------------------
+-------------------
 19.9.0 (2019-12-16)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 19.09 development cycle.
-
-
```

### Comparing `galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/cgroup.py` & `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/cgroup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,117 +1,132 @@
 """The module describes the ``cgroup`` job metrics plugin."""
 import logging
 import numbers
 from collections import namedtuple
-
-from galaxy.util import asbool, nice_size
+from typing import (
+    Any,
+    Dict,
+    List,
+)
+
+from galaxy.util import (
+    asbool,
+    nice_size,
+)
 from . import InstrumentPlugin
 from .. import formatting
 
 log = logging.getLogger(__name__)
 
 TITLES = {
     "memory.memsw.max_usage_in_bytes": "Max memory usage (MEM+SWP)",
     "memory.max_usage_in_bytes": "Max memory usage (MEM)",
     "memory.limit_in_bytes": "Memory limit on cgroup (MEM)",
     "memory.memsw.limit_in_bytes": "Memory limit on cgroup (MEM+SWP)",
     "memory.soft_limit_in_bytes": "Memory softlimit on cgroup",
     "memory.failcnt": "Failed to allocate memory count",
     "memory.oom_control.oom_kill_disable": "OOM Control enabled",
     "memory.oom_control.under_oom": "Was OOM Killer active?",
-    "cpuacct.usage": "CPU Time"
+    "cpuacct.usage": "CPU Time",
 }
 CONVERSION = {
     "memory.oom_control.oom_kill_disable": lambda x: "No" if x == 1 else "Yes",
     "memory.oom_control.under_oom": lambda x: "Yes" if x == 1 else "No",
-    "cpuacct.usage": lambda x: formatting.seconds_to_str(x / 10**9)  # convert nanoseconds
+    "cpuacct.usage": lambda x: formatting.seconds_to_str(x / 10**9),  # convert nanoseconds
 }
 CPU_USAGE_TEMPLATE = r"""
 if [ -e "/proc/$$/cgroup" -a -d "{cgroup_mount}" ]; then
     cgroup_path=$(cat "/proc/$$/cgroup" | awk -F':' '($2=="cpuacct,cpu") || ($2=="cpu,cpuacct") {{print $3}}');
     if [ ! -e "{cgroup_mount}/cpu$cgroup_path/cpuacct.usage" ]; then
         cgroup_path="";
     fi;
     for f in {cgroup_mount}/{{cpu\,cpuacct,cpuacct\,cpu}}$cgroup_path/{{cpu,cpuacct}}.*; do
         if [ -f "$f" ]; then
             echo "__$(basename $f)__" >> {metrics}; cat "$f" >> {metrics} 2>/dev/null;
         fi;
     done;
 fi
-""".replace("\n", " ").strip()
+""".replace(
+    "\n", " "
+).strip()
 MEMORY_USAGE_TEMPLATE = """
 if [ -e "/proc/$$/cgroup" -a -d "{cgroup_mount}" ]; then
     cgroup_path=$(cat "/proc/$$/cgroup" | awk -F':' '$2=="memory"{{print $3}}');
     if [ ! -e "{cgroup_mount}/memory$cgroup_path/memory.max_usage_in_bytes" ]; then
         cgroup_path="";
     fi;
     for f in {cgroup_mount}/memory$cgroup_path/memory.*; do
         echo "__$(basename $f)__" >> {metrics}; cat "$f" >> {metrics} 2>/dev/null;
     done;
 fi
-""".replace("\n", " ").strip()
+""".replace(
+    "\n", " "
+).strip()
 
 
 Metric = namedtuple("Metric", ("key", "subkey", "value"))
 
 
 class CgroupPluginFormatter(formatting.JobMetricFormatter):
-
     def format(self, key, value):
         title = TITLES.get(key, key)
         if key in CONVERSION:
             return title, CONVERSION[key](value)
         elif key.endswith("_bytes"):
             try:
                 return title, nice_size(value)
             except ValueError:
                 pass
-        elif isinstance(value, numbers.Number) and value == int(value):
+        elif isinstance(value, (numbers.Integral, numbers.Real)) and value == int(value):
             value = int(value)
         return title, value
 
 
 class CgroupPlugin(InstrumentPlugin):
-    """ Plugin that collects memory and cpu utilization from within a cgroup.
-    """
+    """Plugin that collects memory and cpu utilization from within a cgroup."""
+
     plugin_type = "cgroup"
     formatter = CgroupPluginFormatter()
 
     def __init__(self, **kwargs):
         self.verbose = asbool(kwargs.get("verbose", False))
         self.cgroup_mount = kwargs.get("cgroup_mount", "/sys/fs/cgroup")
         params_str = kwargs.get("params", None)
         if params_str:
             params = [v.strip() for v in params_str.split(",")]
         else:
-            params = TITLES.keys()
+            params = list(TITLES.keys())
         self.params = params
 
-    def post_execute_instrument(self, job_directory):
-        commands = []
+    def post_execute_instrument(self, job_directory: str) -> List[str]:
+        commands: List[str] = []
         commands.append(self.__record_cgroup_cpu_usage(job_directory))
         commands.append(self.__record_cgroup_memory_usage(job_directory))
         return commands
 
-    def job_properties(self, job_id, job_directory):
+    def job_properties(self, job_id, job_directory: str) -> Dict[str, Any]:
         metrics = self.__read_metrics(self.__cgroup_metrics_file(job_directory))
         return metrics
 
-    def __record_cgroup_cpu_usage(self, job_directory):
+    def __record_cgroup_cpu_usage(self, job_directory: str) -> str:
         # comounted cgroups (which cpu and cpuacct are on the supported Linux distros) can appear in any order (cpu,cpuacct or cpuacct,cpu)
-        return CPU_USAGE_TEMPLATE.format(metrics=self.__cgroup_metrics_file(job_directory), cgroup_mount=self.cgroup_mount)
-
-    def __record_cgroup_memory_usage(self, job_directory):
-        return MEMORY_USAGE_TEMPLATE.format(metrics=self.__cgroup_metrics_file(job_directory), cgroup_mount=self.cgroup_mount)
+        return CPU_USAGE_TEMPLATE.format(
+            metrics=self.__cgroup_metrics_file(job_directory), cgroup_mount=self.cgroup_mount
+        )
+
+    def __record_cgroup_memory_usage(self, job_directory: str) -> str:
+        return MEMORY_USAGE_TEMPLATE.format(
+            metrics=self.__cgroup_metrics_file(job_directory), cgroup_mount=self.cgroup_mount
+        )
 
     def __cgroup_metrics_file(self, job_directory):
         return self._instrument_file_path(job_directory, "_metrics")
 
     def __read_metrics(self, path):
-        metrics = {}
+        metrics: Dict[str, str] = {}
         key = None
         with open(path) as infile:
             for line in infile:
                 try:
                     metric, key = self.__read_key_value(line.strip(), key)
                 except Exception:
                     log.exception("Caught exception attempting to read metric from cgroup line: %s", line)
@@ -122,15 +137,15 @@
         return metrics
 
     def __add_metric(self, metrics, metric):
         if metric and (metric.subkey in self.params or self.verbose):
             metrics[metric.subkey] = metric.value
 
     def __read_key_value(self, line, key):
-        if line.startswith('__') and line.endswith('__'):
+        if line.startswith("__") and line.endswith("__"):
             # line is the beginning of a new param
             key = line[2:][:-2]
             return (None, key)
         elif line.count(" ") == 1:
             # line has a subkey
             subkey, value = line.split(" ", 1)
             subkey = ".".join((key, subkey))
@@ -147,8 +162,8 @@
                 return int(value)
             except ValueError:
                 return float(value)
         except ValueError:
             return value
 
 
-__all__ = ('CgroupPlugin', )
+__all__ = ("CgroupPlugin",)
```

### Comparing `galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/cpuinfo.py` & `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/cpuinfo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 """The module describes the ``cpuinfo`` job metrics plugin."""
 import logging
 import re
+from typing import Any
 
 from galaxy import util
 from . import InstrumentPlugin
-from .. import formatting
+from ..formatting import (
+    FormattedMetric,
+    JobMetricFormatter,
+)
 
 log = logging.getLogger(__name__)
 
 PROCESSOR_LINE = re.compile(r"processor\s*\:\s*(\d+)")
 
 
-class CpuInfoFormatter(formatting.JobMetricFormatter):
-
-    def format(self, key, value):
+class CpuInfoFormatter(JobMetricFormatter):
+    def format(self, key: str, value: Any) -> FormattedMetric:
         if key == "processor_count":
-            return "Processor Count", f"{int(value)}"
+            return FormattedMetric("Processor Count", f"{int(value)}")
         else:
-            return key, value
+            return super().format(key, value)
 
 
 class CpuInfoPlugin(InstrumentPlugin):
-    """ Gather information about processor configuration from /proc/cpuinfo.
+    """Gather information about processor configuration from /proc/cpuinfo.
     Linux only.
     """
+
     plugin_type = "cpuinfo"
     formatter = CpuInfoFormatter()
 
     def __init__(self, **kwargs):
         self.verbose = util.asbool(kwargs.get("verbose", False))
 
     def pre_execute_instrument(self, job_directory):
@@ -56,8 +60,8 @@
         properties["processor_count"] = processor_count
         return properties
 
     def __instrument_cpuinfo_path(self, job_directory):
         return self._instrument_file_path(job_directory, "cpuinfo")
 
 
-__all__ = ('CpuInfoPlugin', )
+__all__ = ("CpuInfoPlugin",)
```

### Comparing `galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/env.py` & `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/env.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,77 @@
 """The module describes the ``env`` job metrics plugin."""
 import logging
 import re
+from typing import (
+    List,
+    Optional,
+)
 
 from . import InstrumentPlugin
-from .. import formatting
+from ..formatting import JobMetricFormatter
+from ..safety import Safety
 
 log = logging.getLogger(__name__)
 
 
-class EnvFormatter(formatting.JobMetricFormatter):
+class EnvFormatter(JobMetricFormatter):
     pass
 
 
 class EnvPlugin(InstrumentPlugin):
-    """ Instrumentation plugin capable of recording all or specific environment
+    """Instrumentation plugin capable of recording all or specific environment
     variables for a job at runtime.
     """
+
     plugin_type = "env"
     formatter = EnvFormatter()
+    variables: Optional[List[str]]
+    default_safety = Safety.UNSAFE
 
     def __init__(self, **kwargs):
         variables_str = kwargs.get("variables", None)
         if variables_str:
-            variables = [v.strip() for v in variables_str.split(",")]
+            self.variables = [v.strip() for v in variables_str.split(",")]
         else:
-            variables = None
-        self.variables = variables
+            self.variables = None
 
-    def pre_execute_instrument(self, job_directory):
-        """ Use env to dump all environment variables to a file.
-        """
+    def pre_execute_instrument(self, job_directory: str):
+        """Use env to dump all environment variables to a file."""
         return f"env > '{self.__env_file(job_directory)}'"
 
     def post_execute_instrument(self, job_directory):
         return None
 
     def job_properties(self, job_id, job_directory):
-        """ Recover environment variables dumped out on compute server and filter
+        """Recover environment variables dumped out on compute server and filter
         out specific variables if needed.
         """
         variables = self.variables
 
         properties = {}
-        env_string = ''.join(open(self.__env_file(job_directory)).readlines())
+        env_string = "".join(open(self.__env_file(job_directory)).readlines())
         while env_string:
             # Check if the next lines contain a shell function.
             # We use '\n\}\n' as regex termination because shell
             # functions can be nested.
             # We use the non-greedy '.+?' because of re.DOTALL .
-            m = re.match(r'([^=]+)=(\(\) \{.+?\n\})\n', env_string, re.DOTALL)
+            m = re.match(r"([^=]+)=(\(\) \{.+?\n\})\n", env_string, re.DOTALL)
             if m is None:
-                m = re.match('([^=]+)=(.*)\n', env_string)
+                m = re.match("([^=]+)=(.*)\n", env_string)
             if m is None:
                 # Some problem recording or reading back env output.
                 message_template = "Problem parsing env metric output for job %s - properties will be incomplete"
                 message = message_template % job_id
                 log.debug(message)
                 break
             (var, value) = m.groups()
             if not variables or var in variables:
                 properties[var] = value
-            env_string = env_string[m.end():]
+            env_string = env_string[m.end() :]
 
         return properties
 
     def __env_file(self, job_directory):
         return self._instrument_file_path(job_directory, "vars")
 
 
-__all__ = ('EnvPlugin', )
+__all__ = ("EnvPlugin",)
```

### Comparing `galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/hostname.py` & `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/hostname.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,33 +4,32 @@
 from . import InstrumentPlugin
 from .. import formatting
 
 log = logging.getLogger(__name__)
 
 
 class HostnameFormatter(formatting.JobMetricFormatter):
-
     def format(self, key, value):
         return key, value
 
 
 class HostnamePlugin(InstrumentPlugin):
-    """ Gather hostname
-    """
+    """Gather hostname"""
+
     plugin_type = "hostname"
     formatter = HostnameFormatter()
 
     def __init__(self, **kwargs):
         pass
 
     def pre_execute_instrument(self, job_directory):
         return f"hostname -f > '{self.__instrument_hostname_path(job_directory)}'"
 
     def job_properties(self, job_id, job_directory):
         with open(self.__instrument_hostname_path(job_directory)) as f:
-            return {'hostname': f.read().strip()}
+            return {"hostname": f.read().strip()}
 
     def __instrument_hostname_path(self, job_directory):
         return self._instrument_file_path(job_directory, "hostname")
 
 
-__all__ = ('HostnamePlugin', )
+__all__ = ("HostnamePlugin",)
```

### Comparing `galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/meminfo.py` & `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/meminfo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 """The module describes the ``meminfo`` job metrics plugin."""
 import re
 
 from galaxy import util
 from . import InstrumentPlugin
 from .. import formatting
-
+from ..safety import Safety
 
 MEMINFO_LINE = re.compile(r"(\w+)\s*\:\s*(\d+) kB")
 
 # Important (non-verbose) meminfo property titles.
-MEMINFO_TITLES = {
-    "memtotal": "Total System Memory",
-    "swaptotal": "Total System Swap"
-}
+MEMINFO_TITLES = {"memtotal": "Total System Memory", "swaptotal": "Total System Swap"}
 
 
 class MemInfoFormatter(formatting.JobMetricFormatter):
-
     def format(self, key, value):
         title = MEMINFO_TITLES.get(key, key)
         return title, util.nice_size(value * 1000)  # kB = *1000, KB = *1024 - wikipedia
 
 
 class MemInfoPlugin(InstrumentPlugin):
-    """ Gather information about processor configuration from /proc/cpuinfo.
+    """Gather information about processor configuration from /proc/cpuinfo.
     Linux only.
     """
+
     plugin_type = "meminfo"
     formatter = MemInfoFormatter()
+    default_safety = Safety.SAFE
 
     def __init__(self, **kwargs):
         self.verbose = util.asbool(kwargs.get("verbose", False))
 
     def pre_execute_instrument(self, job_directory):
         return f"cat /proc/meminfo > '{self.__instrument_meminfo_path(job_directory)}'"
 
@@ -54,8 +52,8 @@
                     properties[key] = value
         return properties
 
     def __instrument_meminfo_path(self, job_directory):
         return self._instrument_file_path(job_directory, "meminfo")
 
 
-__all__ = ('MemInfoPlugin', )
+__all__ = ("MemInfoPlugin",)
```

### Comparing `galaxy-job-metrics-22.1.1/galaxy/job_metrics/instrumenters/uname.py` & `galaxy-job-metrics-23.0.1/galaxy/job_metrics/instrumenters/uname.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """The module describes the ``uname`` job metrics plugin."""
 from . import InstrumentPlugin
 from .. import formatting
 
 
 class UnameFormatter(formatting.JobMetricFormatter):
-
     def format(self, key, value):
         return "Operating System", value
 
 
 class UnamePlugin(InstrumentPlugin):
-    """ Use uname to gather operating system information about remote system
+    """Use uname to gather operating system information about remote system
     job is running on. Linux only.
     """
+
     plugin_type = "uname"
     formatter = UnameFormatter()
 
     def __init__(self, **kwargs):
         self.uname_args = kwargs.get("args", "-a")
 
     def pre_execute_instrument(self, job_directory):
@@ -28,8 +28,8 @@
             properties["uname"] = f.read()
         return properties
 
     def __instrument_uname_path(self, job_directory):
         return self._instrument_file_path(job_directory, "uname")
 
 
-__all__ = ('UnamePlugin', )
+__all__ = ("UnamePlugin",)
```

### Comparing `galaxy-job-metrics-22.1.1/galaxy_job_metrics.egg-info/PKG-INFO` & `galaxy-job-metrics-23.0.1/galaxy_job_metrics.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,70 @@
 Metadata-Version: 2.1
 Name: galaxy-job-metrics
-Version: 22.1.1
-Summary: Galaxy Job Metrics
+Version: 23.0.1
+Summary: Galaxy job metrics
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
 
 
 .. image:: https://badge.fury.io/py/galaxy-job-metrics.svg
    :target: https://pypi.org/project/galaxy-job-metrics/
 
 
 Overview
 --------
 
 The Galaxy_ job metrics framework and default plugins.
 
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
 
----------------------
+-------------------
 19.9.0 (2019-12-16)
----------------------
+-------------------
 
 * Initial import from dev branch of Galaxy during 19.09 development cycle.
-
-
```

