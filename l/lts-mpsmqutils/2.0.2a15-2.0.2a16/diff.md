# Comparing `tmp/lts-mpsmqutils-2.0.2a15.tar.gz` & `tmp/lts-mpsmqutils-2.0.2a16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a15.tar", last modified: Thu Jun  8 16:22:54 2023, max compression
+gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a16.tar", last modified: Thu Jun  8 16:32:39 2023, max compression
```

## Comparing `lts-mpsmqutils-2.0.2a15.tar` & `lts-mpsmqutils-2.0.2a16.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:22:54.832483 lts-mpsmqutils-2.0.2a15/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 16:22:54.832135 lts-mpsmqutils-2.0.2a15/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a15/README.md
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:22:54.828395 lts-mpsmqutils-2.0.2a15/lts_mpsmqutils.egg-info/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 16:22:54.000000 lts-mpsmqutils-2.0.2a15/lts_mpsmqutils.egg-info/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-06-08 16:22:54.000000 lts-mpsmqutils-2.0.2a15/lts_mpsmqutils.egg-info/SOURCES.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-08 16:22:54.000000 lts-mpsmqutils-2.0.2a15/lts_mpsmqutils.egg-info/dependency_links.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-08 16:22:54.000000 lts-mpsmqutils-2.0.2a15/lts_mpsmqutils.egg-info/requires.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-08 16:22:54.000000 lts-mpsmqutils-2.0.2a15/lts_mpsmqutils.egg-info/top_level.txt
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:22:54.830890 lts-mpsmqutils-2.0.2a15/mpsmqutils/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a15/mpsmqutils/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)      784 2023-06-08 14:50:09.000000 lts-mpsmqutils-2.0.2a15/mpsmqutils/log_wrapper.py
--rw-r--r--   0 dougsimon   (502) staff       (20)    27023 2023-06-08 15:18:02.000000 lts-mpsmqutils-2.0.2a15/mpsmqutils/messagehandler.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     7250 2023-06-08 15:22:46.000000 lts-mpsmqutils-2.0.2a15/mpsmqutils/mqutils.py
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:22:54.831586 lts-mpsmqutils-2.0.2a15/mpsmqutils/tests/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a15/mpsmqutils/tests/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a15/mpsmqutils/tests/test_mqutils.py
--rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-08 16:22:54.832570 lts-mpsmqutils-2.0.2a15/setup.cfg
--rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-08 16:22:45.000000 lts-mpsmqutils-2.0.2a15/setup.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:32:39.194702 lts-mpsmqutils-2.0.2a16/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 16:32:39.194423 lts-mpsmqutils-2.0.2a16/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a16/README.md
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:32:39.189529 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 16:32:39.000000 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-06-08 16:32:39.000000 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/SOURCES.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-08 16:32:39.000000 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/dependency_links.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-08 16:32:39.000000 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/requires.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-08 16:32:39.000000 lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/top_level.txt
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:32:39.192261 lts-mpsmqutils-2.0.2a16/mpsmqutils/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)      784 2023-06-08 14:50:09.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/log_wrapper.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)    27044 2023-06-08 16:32:22.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/messagehandler.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     7271 2023-06-08 16:31:48.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/mqutils.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:32:39.193500 lts-mpsmqutils-2.0.2a16/mpsmqutils/tests/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/tests/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a16/mpsmqutils/tests/test_mqutils.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-08 16:32:39.194794 lts-mpsmqutils-2.0.2a16/setup.cfg
+-rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-08 16:31:58.000000 lts-mpsmqutils-2.0.2a16/setup.py
```

### Comparing `lts-mpsmqutils-2.0.2a15/PKG-INFO` & `lts-mpsmqutils-2.0.2a16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a15
+Version: 2.0.2a16
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a15/README.md` & `lts-mpsmqutils-2.0.2a16/README.md`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a15/lts_mpsmqutils.egg-info/PKG-INFO` & `lts-mpsmqutils-2.0.2a16/lts_mpsmqutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a15
+Version: 2.0.2a16
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a15/mpsmqutils/log_wrapper.py` & `lts-mpsmqutils-2.0.2a16/mpsmqutils/log_wrapper.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a15/mpsmqutils/messagehandler.py` & `lts-mpsmqutils-2.0.2a16/mpsmqutils/messagehandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import mpsjobtracker.trackers.jobtracker as jobtracker
 job_tracker = jobtracker.JobTracker()
 
 import requests
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry
 
-from .log_wrapper import LogWrapper
-logger = LogWrapper()
+import mpsmqutils.log_wrapper as log_wrapper
+logger = log_wrapper.LogWrapper()
 
 retry_strategy = Retry(
     total=3,
     status_forcelist=[429, 500, 502, 503, 504],
     backoff_factor=1
 )
 adapter = HTTPAdapter(max_retries=retry_strategy)
```

### Comparing `lts-mpsmqutils-2.0.2a15/mpsmqutils/mqutils.py` & `lts-mpsmqutils-2.0.2a16/mpsmqutils/mqutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os, json, time, datetime
 from contextlib import contextmanager
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 from traceback import format_exc
 # Job tracker module
 import mpsjobtracker.trackers.jobtracker as jobtracker
 
-from .log_wrapper import LogWrapper
-logger = LogWrapper()
+import mpsmqutils.log_wrapper as log_wrapper
+logger = log_wrapper.LogWrapper()
 
 jt = None
 def get_jt():
     global jt
     if not jt:
         jt = jobtracker.JobTracker()
     return jt
```

### Comparing `lts-mpsmqutils-2.0.2a15/mpsmqutils/tests/test_mqutils.py` & `lts-mpsmqutils-2.0.2a16/mpsmqutils/tests/test_mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a15/setup.py` & `lts-mpsmqutils-2.0.2a16/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lts-mpsmqutils",
-    version="2.0.2a15",
+    version="2.0.2a16",
     description="A set of utilities for communicating with a message queue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.huit.harvard.edu/LTS/mps-mqutils",
     packages=setuptools.find_packages(),
     install_requires=[
         'lts-mpsjobtracker-mongo',
```

