# Comparing `tmp/lts-mpsmqutils-2.0.2a17.tar.gz` & `tmp/lts-mpsmqutils-2.0.2a18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a17.tar", last modified: Thu Jun  8 16:52:04 2023, max compression
+gzip compressed data, was "dist/lts-mpsmqutils-2.0.2a18.tar", last modified: Thu Jun  8 17:09:34 2023, max compression
```

## Comparing `lts-mpsmqutils-2.0.2a17.tar` & `lts-mpsmqutils-2.0.2a18.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:52:04.351858 lts-mpsmqutils-2.0.2a17/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 16:52:04.351182 lts-mpsmqutils-2.0.2a17/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a17/README.md
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:52:04.343789 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/
--rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 16:52:04.000000 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/PKG-INFO
--rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-06-08 16:52:04.000000 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/SOURCES.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-08 16:52:04.000000 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/dependency_links.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-08 16:52:04.000000 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/requires.txt
--rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-08 16:52:04.000000 lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/top_level.txt
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:52:04.347140 lts-mpsmqutils-2.0.2a17/mpsmqutils/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     1004 2023-06-08 16:51:45.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/log_wrapper.py
--rw-r--r--   0 dougsimon   (502) staff       (20)    27237 2023-06-08 16:50:15.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/messagehandler.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     7271 2023-06-08 16:31:48.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/mqutils.py
-drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 16:52:04.349248 lts-mpsmqutils-2.0.2a17/mpsmqutils/tests/
--rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/tests/__init__.py
--rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a17/mpsmqutils/tests/test_mqutils.py
--rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-08 16:52:04.352072 lts-mpsmqutils-2.0.2a17/setup.cfg
--rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-08 16:51:57.000000 lts-mpsmqutils-2.0.2a17/setup.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:09:34.733498 lts-mpsmqutils-2.0.2a18/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 17:09:34.733181 lts-mpsmqutils-2.0.2a18/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)     5103 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a18/README.md
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:09:34.729059 lts-mpsmqutils-2.0.2a18/lts_mpsmqutils.egg-info/
+-rw-r--r--   0 dougsimon   (502) staff       (20)     6652 2023-06-08 17:09:34.000000 lts-mpsmqutils-2.0.2a18/lts_mpsmqutils.egg-info/PKG-INFO
+-rw-r--r--   0 dougsimon   (502) staff       (20)      369 2023-06-08 17:09:34.000000 lts-mpsmqutils-2.0.2a18/lts_mpsmqutils.egg-info/SOURCES.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)        1 2023-06-08 17:09:34.000000 lts-mpsmqutils-2.0.2a18/lts_mpsmqutils.egg-info/dependency_links.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       62 2023-06-08 17:09:34.000000 lts-mpsmqutils-2.0.2a18/lts_mpsmqutils.egg-info/requires.txt
+-rw-r--r--   0 dougsimon   (502) staff       (20)       11 2023-06-08 17:09:34.000000 lts-mpsmqutils-2.0.2a18/lts_mpsmqutils.egg-info/top_level.txt
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:09:34.731165 lts-mpsmqutils-2.0.2a18/mpsmqutils/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a18/mpsmqutils/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)      788 2023-06-08 17:09:20.000000 lts-mpsmqutils-2.0.2a18/mpsmqutils/log_wrapper.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)    27237 2023-06-08 16:50:15.000000 lts-mpsmqutils-2.0.2a18/mpsmqutils/messagehandler.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     7271 2023-06-08 16:31:48.000000 lts-mpsmqutils-2.0.2a18/mpsmqutils/mqutils.py
+drwxr-xr-x   0 dougsimon   (502) staff       (20)        0 2023-06-08 17:09:34.732332 lts-mpsmqutils-2.0.2a18/mpsmqutils/tests/
+-rw-r--r--   0 dougsimon   (502) staff       (20)        0 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a18/mpsmqutils/tests/__init__.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)     4783 2021-10-29 20:43:09.000000 lts-mpsmqutils-2.0.2a18/mpsmqutils/tests/test_mqutils.py
+-rw-r--r--   0 dougsimon   (502) staff       (20)       38 2023-06-08 17:09:34.733599 lts-mpsmqutils-2.0.2a18/setup.cfg
+-rw-r--r--   0 dougsimon   (502) staff       (20)      899 2023-06-08 17:09:26.000000 lts-mpsmqutils-2.0.2a18/setup.py
```

### Comparing `lts-mpsmqutils-2.0.2a17/PKG-INFO` & `lts-mpsmqutils-2.0.2a18/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a17
+Version: 2.0.2a18
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a17/README.md` & `lts-mpsmqutils-2.0.2a18/README.md`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a17/lts_mpsmqutils.egg-info/PKG-INFO` & `lts-mpsmqutils-2.0.2a18/lts_mpsmqutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lts-mpsmqutils
-Version: 2.0.2a17
+Version: 2.0.2a18
 Summary: A set of utilities for communicating with a message queue
 Home-page: https://github.huit.harvard.edu/LTS/mps-mqutils
 License: UNKNOWN
 Description: # mps-mqutils
         
         ## Introduction
         A set of utilities for Media Preservation Services that provides standard methods to communicate with the message queue.
```

### Comparing `lts-mpsmqutils-2.0.2a17/mpsmqutils/messagehandler.py` & `lts-mpsmqutils-2.0.2a18/mpsmqutils/messagehandler.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a17/mpsmqutils/mqutils.py` & `lts-mpsmqutils-2.0.2a18/mpsmqutils/mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a17/mpsmqutils/tests/test_mqutils.py` & `lts-mpsmqutils-2.0.2a18/mpsmqutils/tests/test_mqutils.py`

 * *Files identical despite different names*

### Comparing `lts-mpsmqutils-2.0.2a17/setup.py` & `lts-mpsmqutils-2.0.2a18/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lts-mpsmqutils",
-    version="2.0.2a17",
+    version="2.0.2a18",
     description="A set of utilities for communicating with a message queue",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.huit.harvard.edu/LTS/mps-mqutils",
     packages=setuptools.find_packages(),
     install_requires=[
         'lts-mpsjobtracker-mongo',
```

