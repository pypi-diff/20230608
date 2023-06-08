# Comparing `tmp/arvados-cwl-runner-2.6.3.tar.gz` & `tmp/arvados-cwl-runner-2.6.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.6.3.tar", last modified: Thu Jun  8 21:55:14 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-cwl-runner-2.6.3rc1.tar", last modified: Thu Jun  1 21:38:17 2023, max compression
```

## Comparing `arvados-cwl-runner-2.6.3.tar` & `arvados-cwl-runner-2.6.3rc1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/arvados_cwl/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21157 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/arvados_cwl/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/arv-cwl-schema-v1.0.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/arv-cwl-schema-v1.1.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12840 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/arv-cwl-schema-v1.2.yml
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35231 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/arvcontainer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/arvdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5438 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/arvtool.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31521 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/arvworkflow.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2155 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/context.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3935 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/done.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    44529 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/executor.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17994 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/perf.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    39139 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/runner.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1810 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_cwl/util.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/arvados_cwl_runner.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      558 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/arvados_cwl_runner.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/arvados_cwl_runner.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/arvados_cwl_runner.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/arvados_cwl_runner.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      174 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/arvados_cwl_runner.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/arvados_cwl_runner.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.6.3/arvados_cwl_runner.egg-info/zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/bin/arvados-cwl-runner
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/bin/cwl-runner
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2072 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:14.000000 arvados-cwl-runner-2.6.3/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/hw.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/matcher.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/mock_discovery.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73382 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/test_container.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/test_copy_deps.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/test_fsaccess.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/test_make_output.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/test_pathmapper.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/test_set_output_prop.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87484 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/test_submit.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/test_tq.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/test_urljoin.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3439 2023-06-08 21:55:03.000000 arvados-cwl-runner-2.6.3/tests/test_util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      149 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    20500 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14343 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.0.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12837 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.1.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12840 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.2.yml
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    35160 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvcontainer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6934 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5438 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvtool.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    31521 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvworkflow.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2155 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/context.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3986 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/done.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    44529 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/executor.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12495 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17991 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      560 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/perf.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    39024 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/runner.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1810 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl/util.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      561 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1135 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       87 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      177 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       18 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2174 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/bin/arvados-cwl-runner
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      217 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/bin/cwl-runner
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2073 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:17.000000 arvados-cwl-runner-2.6.3rc1/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      100 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      158 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/hw.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1049 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/matcher.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      416 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/mock_discovery.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    73382 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_container.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7275 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_copy_deps.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     5236 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_fsaccess.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7098 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_make_output.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10597 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_pathmapper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1299 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_set_output_prop.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    87484 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_submit.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1434 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_tq.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2503 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_urljoin.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3439 2023-06-01 21:38:09.000000 arvados-cwl-runner-2.6.3rc1/tests/test_util.py
```

### Comparing `arvados-cwl-runner-2.6.3/LICENSE-2.0.txt` & `arvados-cwl-runner-2.6.3rc1/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/PKG-INFO` & `arvados-cwl-runner-2.6.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.6.3
+Version: 2.6.3rc1
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/__init__.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 import cwltool.argparser
 from cwltool.errors import WorkflowException
 from cwltool.process import shortname, UnsupportedRequirement, use_custom_schema
 from cwltool.utils import adjustFileObjs, adjustDirObjs, get_listing
 
 import arvados
 import arvados.config
-import arvados.logging
 from arvados.keep import KeepClient
 from arvados.errors import ApiError
 import arvados.commands._util as arv_cmd
 from arvados.api import OrderedJsonModel
 
 from .perf import Perf
 from ._version import __version__
@@ -374,28 +373,18 @@
     # Note that unless in debug mode, some stack traces related to user
     # workflow errors may be suppressed.
 
     # Set the logging on most modules INFO (instead of default which is WARNING)
     logger.setLevel(logging.INFO)
     logging.getLogger('arvados').setLevel(logging.INFO)
     logging.getLogger('arvados.keep').setLevel(logging.WARNING)
-    # API retries are filtered to the INFO level and can be noisy, but as long as
-    # they succeed we don't need to see warnings about it.
-    googleapiclient_http_logger = logging.getLogger('googleapiclient.http')
-    googleapiclient_http_logger.addFilter(arvados.logging.GoogleHTTPClientFilter())
-    googleapiclient_http_logger.setLevel(logging.WARNING)
 
     if arvargs.debug:
         logger.setLevel(logging.DEBUG)
         logging.getLogger('arvados').setLevel(logging.DEBUG)
-        # In debug mode show logs about retries, but we arn't
-        # debugging the google client so we don't need to see
-        # everything.
-        googleapiclient_http_logger.setLevel(logging.NOTSET)
-        logging.getLogger('googleapiclient').setLevel(logging.INFO)
 
     if arvargs.quiet:
         logger.setLevel(logging.WARN)
         logging.getLogger('arvados').setLevel(logging.WARN)
         logging.getLogger('arvados.arv-run').setLevel(logging.WARN)
 
     if arvargs.metrics:
```

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/arv-cwl-schema-v1.0.yml` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.0.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/arv-cwl-schema-v1.1.yml` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.1.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/arv-cwl-schema-v1.2.yml` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arv-cwl-schema-v1.2.yml`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/arvcontainer.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvcontainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -455,15 +455,14 @@
             return True
 
         return False
 
     def done(self, record):
         outputs = {}
         retried = False
-        rcode = None
         try:
             container = self.arvrunner.api.containers().get(
                 uuid=record["container_uuid"]
             ).execute(num_retries=self.arvrunner.num_retries)
             if container["state"] == "Complete":
                 rcode = container["exit_code"]
                 if self.successCodes and rcode in self.successCodes:
@@ -496,15 +495,15 @@
                 logc = arvados.collection.CollectionReader(record["log_uuid"],
                                                            api_client=self.arvrunner.api,
                                                            keep_client=self.arvrunner.keep_client,
                                                            num_retries=self.arvrunner.num_retries)
                 label = self.arvrunner.label(self)
                 done.logtail(
                     logc, logger.error,
-                    "%s (%s) error log:" % (label, record["uuid"]), maxlen=40, include_crunchrun=(rcode is None or rcode > 127))
+                    "%s (%s) error log:" % (label, record["uuid"]), maxlen=40)
 
             if record["output_uuid"]:
                 if self.arvrunner.trash_intermediate or self.arvrunner.intermediate_output_ttl:
                     # Compute the trash time to avoid requesting the collection record.
                     trash_at = ciso8601.parse_datetime_as_naive(record["modified_at"]) + datetime.timedelta(0, self.arvrunner.intermediate_output_ttl)
                     aftertime = " at %s" % trash_at.strftime("%Y-%m-%d %H:%M:%S UTC") if self.arvrunner.intermediate_output_ttl else ""
                     orpart = ", or" if self.arvrunner.trash_intermediate and self.arvrunner.intermediate_output_ttl else ""
```

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/arvdocker.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/arvtool.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvtool.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/arvworkflow.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/arvworkflow.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/context.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/context.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/done.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/done.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,49 +53,47 @@
     self.builder.outdir = outdir
     self.builder.pathmapper.keepdir = keepdir
     return self.collect_outputs("keep:" + record["output"], record["exit_code"])
 
 crunchstat_re = re.compile(r"^\d{4}-\d\d-\d\d_\d\d:\d\d:\d\d [a-z0-9]{5}-8i9sb-[a-z0-9]{15} \d+ \d+ stderr crunchstat:")
 timestamp_re = re.compile(r"^(\d{4}-\d\d-\d\dT\d\d:\d\d:\d\d\.\d+Z) (.*)")
 
-def logtail(logcollection, logfunc, header, maxlen=25, include_crunchrun=True):
+def logtail(logcollection, logfunc, header, maxlen=25):
     if len(logcollection) == 0:
         logfunc("%s\n%s", header, "  ** log is empty **")
         return
 
+    containersapi = ("crunch-run.txt" in logcollection)
     mergelogs = {}
-    logfiles = ["stdout.txt", "stderr.txt"]
 
-    if include_crunchrun:
-        logfiles.append("crunch-run.txt")
-
-    for log in logfiles:
-        if log not in logcollection:
-            continue
-        logname = log[:-4]  # trim off the .txt
-        logt = deque([], maxlen)
-        mergelogs[logname] = logt
-        with logcollection.open(log, encoding="utf-8") as f:
-            for l in f:
-                g = timestamp_re.match(l)
-                logt.append((g.group(1), g.group(2)))
-
-    keys = list(mergelogs)
-    loglines = []
-
-    # we assume the log lines are all in order so this this is a
-    # straight linear merge where we look at the next timestamp of
-    # each log and take whichever one is earliest.
-    while True:
-        earliest = None
-        for k in keys:
-            if mergelogs[k]:
-                if earliest is None or mergelogs[k][0][0] < mergelogs[earliest][0][0]:
-                    earliest = k
-        if earliest is None:
-            break
-        ts, msg = mergelogs[earliest].popleft()
-        loglines.append("%s %s %s" % (ts, earliest, msg))
-    loglines = loglines[-maxlen:]
+    for log in list(logcollection):
+        if not containersapi or log in ("crunch-run.txt", "stdout.txt", "stderr.txt"):
+            logname = log[:-4]
+            logt = deque([], maxlen)
+            mergelogs[logname] = logt
+            with logcollection.open(log, encoding="utf-8") as f:
+                for l in f:
+                    if containersapi:
+                        g = timestamp_re.match(l)
+                        logt.append((g.group(1), g.group(2)))
+                    elif not crunchstat_re.match(l):
+                        logt.append(l)
+
+    if containersapi:
+        keys = list(mergelogs)
+        loglines = []
+        while True:
+            earliest = None
+            for k in keys:
+                if mergelogs[k]:
+                    if earliest is None or mergelogs[k][0][0] < mergelogs[earliest][0][0]:
+                        earliest = k
+            if earliest is None:
+                break
+            ts, msg = mergelogs[earliest].popleft()
+            loglines.append("%s %s %s" % (ts, earliest, msg))
+        loglines = loglines[-maxlen:]
+    else:
+        loglines = mergelogs[list(mergelogs)[0]]
 
     logtxt = "\n  ".join(l.strip() for l in loglines)
-    logfunc("%s\n\n  %s\n", header, logtxt)
+    logfunc("%s\n\n  %s", header, logtxt)
```

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/executor.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/executor.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/fsaccess.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/pathmapper.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/pathmapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
                     else:
                         keepref = "keep:%s/%s" % http_to_keep(self.arvrunner.api, self.arvrunner.project_uuid, src,
                                                               varying_url_params=self.arvrunner.toplevel_runtimeContext.varying_url_params,
                                                               prefer_cached_downloads=self.arvrunner.toplevel_runtimeContext.prefer_cached_downloads)
                         logger.info("%s is %s", src, keepref)
                         self._pathmap[src] = MapperEnt(keepref, keepref, srcobj["class"], True)
                 except Exception as e:
-                    logger.warning("Download error: %s", e)
+                    logger.warning(str(e))
             else:
                 self._pathmap[src] = MapperEnt(src, src, srcobj["class"], True)
 
         with SourceLine(srcobj, "secondaryFiles", WorkflowException, debug):
             for l in srcobj.get("secondaryFiles", []):
                 self.visit(l, uploadfiles)
         with SourceLine(srcobj, "listing", WorkflowException, debug):
@@ -143,15 +143,15 @@
             with c.open(path + "/" + obj["basename"], "w") as f:
                 f.write(obj["contents"])
             remap.append((obj["location"], path + "/" + obj["basename"]))
         else:
             for opt in self.optional_deps:
                 if obj["location"] == opt["location"]:
                     return
-            raise SourceLine(obj, "location", WorkflowException).makeError("Can't handle '%s'" % obj["location"])
+            raise SourceLine(obj, "location", WorkflowException).makeError("Don't know what to do with '%s'" % obj["location"])
 
     def needs_new_collection(self, srcobj, prefix=""):
         """Check if files need to be staged into a new collection.
 
         If all the files are in the same collection and in the same
         paths they would be staged to, return False.  Otherwise, a new
         collection is needed with files copied/created in the
```

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/perf.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/perf.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/runner.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -919,16 +919,15 @@
             outputs = {}
 
             if processStatus == "permanentFail":
                 logc = arvados.collection.CollectionReader(record["log"],
                                                            api_client=self.arvrunner.api,
                                                            keep_client=self.arvrunner.keep_client,
                                                            num_retries=self.arvrunner.num_retries)
-                done.logtail(logc, logger.error, "%s (%s) error log:" % (self.arvrunner.label(self), record["uuid"]), maxlen=40,
-                             include_crunchrun=(record.get("exit_code") is None or record.get("exit_code") > 127))
+                done.logtail(logc, logger.error, "%s (%s) error log:" % (self.arvrunner.label(self), record["uuid"]), maxlen=40)
 
             self.final_output = record["output"]
             outc = arvados.collection.CollectionReader(self.final_output,
                                                        api_client=self.arvrunner.api,
                                                        keep_client=self.arvrunner.keep_client,
                                                        num_retries=self.arvrunner.num_retries)
             if "cwl.output.json" in outc:
```

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl/util.py` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl/util.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl_runner.egg-info/PKG-INFO` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arvados-cwl-runner
-Version: 2.6.3
+Version: 2.6.3rc1
 Summary: Arvados Common Workflow Language runner
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-cwl-runner-2.6.3/arvados_cwl_runner.egg-info/SOURCES.txt` & `arvados-cwl-runner-2.6.3rc1/arvados_cwl_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/arvados_version.py` & `arvados-cwl-runner-2.6.3rc1/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/setup.py` & `arvados-cwl-runner-2.6.3rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,22 +32,22 @@
       packages=find_packages(),
       package_data={'arvados_cwl': ['arv-cwl-schema-v1.0.yml', 'arv-cwl-schema-v1.1.yml', 'arv-cwl-schema-v1.2.yml']},
       entry_points={"console_scripts": ["cwl-runner=arvados_cwl:main", "arvados-cwl-runner=arvados_cwl:main"]},
       # Note that arvados/build/run-build-packages.sh looks at this
       # file to determine what version of cwltool and schema-salad to
       # build.
       install_requires=[
-          'cwltool==3.1.20230601100705',
-          'schema-salad==8.4.20230601112322',
+          'cwltool==3.1.20230127121939',
+          'schema-salad==8.4.20230127112827',
           'arvados-python-client{}'.format(pysdk_dep),
           'ciso8601 >= 2.0.0',
           'networkx < 2.6',
           'msgpack==1.0.3',
           'importlib-metadata<5',
-          'setuptools>=40.3.0'
+          'setuptools>=40.3.0',
       ],
       data_files=[
           ('share/doc/arvados-cwl-runner', ['LICENSE-2.0.txt', 'README.rst']),
       ],
       python_requires=">=3.5, <4",
       classifiers=[
           'Programming Language :: Python :: 3',
```

### Comparing `arvados-cwl-runner-2.6.3/tests/matcher.py` & `arvados-cwl-runner-2.6.3rc1/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/tests/test_container.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/tests/test_copy_deps.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_copy_deps.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/tests/test_fsaccess.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_fsaccess.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/tests/test_make_output.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_make_output.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/tests/test_pathmapper.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_pathmapper.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/tests/test_set_output_prop.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_set_output_prop.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/tests/test_submit.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_submit.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/tests/test_tq.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_tq.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/tests/test_urljoin.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_urljoin.py`

 * *Files identical despite different names*

### Comparing `arvados-cwl-runner-2.6.3/tests/test_util.py` & `arvados-cwl-runner-2.6.3rc1/tests/test_util.py`

 * *Files identical despite different names*

