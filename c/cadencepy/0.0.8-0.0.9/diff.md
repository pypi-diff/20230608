# Comparing `tmp/cadencepy-0.0.8.tar.gz` & `tmp/cadencepy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cadencepy-0.0.8.tar", last modified: Thu Jun  8 18:29:00 2023, max compression
+gzip compressed data, was "dist/cadencepy-0.0.9.tar", last modified: Thu Jun  8 18:33:22 2023, max compression
```

## Comparing `cadencepy-0.0.8.tar` & `cadencepy-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 18:29:00.000000 cadencepy-0.0.8/
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 18:29:00.000000 cadencepy-0.0.8/cadencepy.egg-info/
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     3581 2023-06-08 18:29:00.000000 cadencepy-0.0.8/cadencepy.egg-info/PKG-INFO
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      321 2023-06-08 18:29:00.000000 cadencepy-0.0.8/cadencepy.egg-info/SOURCES.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        1 2023-06-08 18:29:00.000000 cadencepy-0.0.8/cadencepy.egg-info/dependency_links.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       15 2023-06-08 18:29:00.000000 cadencepy-0.0.8/cadencepy.egg-info/requires.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       10 2023-06-08 18:29:00.000000 cadencepy-0.0.8/cadencepy.egg-info/top_level.txt
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 18:29:00.000000 cadencepy-0.0.8/pycadence/
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:36:21.000000 cadencepy-0.0.8/pycadence/__init__.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      172 2023-06-08 16:34:41.000000 cadencepy-0.0.8/pycadence/connect.sh
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       99 2023-06-08 14:52:30.000000 cadencepy-0.0.8/pycadence/disconnect.sh
--rwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)       87 2023-06-08 14:51:23.000000 cadencepy-0.0.8/pycadence/ocean_simulation.sh
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     1610 2023-06-08 16:15:56.000000 cadencepy-0.0.8/pycadence/pycadence.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      814 2023-06-08 14:32:37.000000 cadencepy-0.0.8/pycadence/utils.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     2661 2023-06-08 18:28:08.000000 cadencepy-0.0.8/README.md
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      776 2023-06-08 18:28:26.000000 cadencepy-0.0.8/setup.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     3581 2023-06-08 18:29:00.000000 cadencepy-0.0.8/PKG-INFO
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       38 2023-06-08 18:29:00.000000 cadencepy-0.0.8/setup.cfg
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 18:33:22.000000 cadencepy-0.0.9/
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 18:33:22.000000 cadencepy-0.0.9/cadencepy.egg-info/
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     3581 2023-06-08 18:33:22.000000 cadencepy-0.0.9/cadencepy.egg-info/PKG-INFO
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      321 2023-06-08 18:33:22.000000 cadencepy-0.0.9/cadencepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        1 2023-06-08 18:33:22.000000 cadencepy-0.0.9/cadencepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       15 2023-06-08 18:33:22.000000 cadencepy-0.0.9/cadencepy.egg-info/requires.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       10 2023-06-08 18:33:22.000000 cadencepy-0.0.9/cadencepy.egg-info/top_level.txt
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 18:33:22.000000 cadencepy-0.0.9/pycadence/
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:36:21.000000 cadencepy-0.0.9/pycadence/__init__.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      172 2023-06-08 16:34:41.000000 cadencepy-0.0.9/pycadence/connect.sh
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       99 2023-06-08 14:52:30.000000 cadencepy-0.0.9/pycadence/disconnect.sh
+-rwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)       87 2023-06-08 14:51:23.000000 cadencepy-0.0.9/pycadence/ocean_simulation.sh
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     1610 2023-06-08 16:15:56.000000 cadencepy-0.0.9/pycadence/pycadence.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      814 2023-06-08 14:32:37.000000 cadencepy-0.0.9/pycadence/utils.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     2661 2023-06-08 18:28:08.000000 cadencepy-0.0.9/README.md
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      776 2023-06-08 18:33:17.000000 cadencepy-0.0.9/setup.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     3581 2023-06-08 18:33:22.000000 cadencepy-0.0.9/PKG-INFO
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       38 2023-06-08 18:33:22.000000 cadencepy-0.0.9/setup.cfg
```

### Comparing `cadencepy-0.0.8/cadencepy.egg-info/PKG-INFO` & `cadencepy-0.0.9/cadencepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadencepy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python SDK for running simulation and reading data from Ocean Cadence
 Home-page: https://github.com/user/reponame
 Author: joetho786
 Author-email: thomas.2@iitj.ac.in
 License: UNKNOWN
 Description: # PyCadence
          A Python wrapper for running Cadence simulations
```

### Comparing `cadencepy-0.0.8/pycadence/pycadence.py` & `cadencepy-0.0.9/pycadence/pycadence.py`

 * *Files identical despite different names*

### Comparing `cadencepy-0.0.8/pycadence/utils.py` & `cadencepy-0.0.9/pycadence/utils.py`

 * *Files identical despite different names*

### Comparing `cadencepy-0.0.8/README.md` & `cadencepy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cadencepy-0.0.8/setup.py` & `cadencepy-0.0.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readall(path):
     with open(path) as fp:
         return fp.read()
 
 setup(
     name="cadencepy",
-    version="0.0.8",
+    version="0.0.9",
     author="joetho786",
     author_email="thomas.2@iitj.ac.in",
     description="A python SDK for running simulation and reading data from Ocean Cadence",
     long_description=readall("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/user/reponame",
     packages=find_packages(),
```

### Comparing `cadencepy-0.0.8/PKG-INFO` & `cadencepy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cadencepy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python SDK for running simulation and reading data from Ocean Cadence
 Home-page: https://github.com/user/reponame
 Author: joetho786
 Author-email: thomas.2@iitj.ac.in
 License: UNKNOWN
 Description: # PyCadence
          A Python wrapper for running Cadence simulations
```

