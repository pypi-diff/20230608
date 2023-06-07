# Comparing `tmp/progscheduler-2.3.3.tar.gz` & `tmp/progscheduler-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "progscheduler-2.3.3.tar", last modified: Wed Jun  7 21:17:37 2023, max compression
+gzip compressed data, was "progscheduler-2.3.4.tar", last modified: Wed Jun  7 21:57:15 2023, max compression
```

## Comparing `progscheduler-2.3.3.tar` & `progscheduler-2.3.4.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-07 21:17:24.000000 progscheduler-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-06-07 21:17:37.588670 progscheduler-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-06-07 21:17:24.000000 progscheduler-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/progscheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/progscheduler/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/settings/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/settings/generic_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/settings/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/settings/specific_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/progscheduler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/progscheduler/version/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/version/progsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 21:17:24.000000 progscheduler-2.3.3/progscheduler/version/progsettings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:17:37.588670 progscheduler-2.3.3/progscheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 21:17:37.000000 progscheduler-2.3.3/progscheduler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:17:37.588670 progscheduler-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-07 21:17:24.000000 progscheduler-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:57:15.987598 progscheduler-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-07 21:56:58.000000 progscheduler-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-06-07 21:57:15.987598 progscheduler-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-06-07 21:56:58.000000 progscheduler-2.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:57:15.987598 progscheduler-2.3.4/progscheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:57:15.987598 progscheduler-2.3.4/progscheduler/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/settings/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/settings/generic_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/settings/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/settings/specific_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:57:15.987598 progscheduler-2.3.4/progscheduler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/utils/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/utils/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:57:15.987598 progscheduler-2.3.4/progscheduler/version/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/version/progsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 21:56:58.000000 progscheduler-2.3.4/progscheduler/version/progsettings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:57:15.987598 progscheduler-2.3.4/progscheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-06-07 21:57:15.000000 progscheduler-2.3.4/progscheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 21:57:15.000000 progscheduler-2.3.4/progscheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:57:15.000000 progscheduler-2.3.4/progscheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 21:57:15.000000 progscheduler-2.3.4/progscheduler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 21:57:15.000000 progscheduler-2.3.4/progscheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 21:57:15.000000 progscheduler-2.3.4/progscheduler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 21:57:15.987598 progscheduler-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-07 21:56:58.000000 progscheduler-2.3.4/setup.py
```

### Comparing `progscheduler-2.3.3/LICENSE` & `progscheduler-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/PKG-INFO` & `progscheduler-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progscheduler
-Version: 2.3.3
+Version: 2.3.4
 Summary: A simple automated task to schedule files to open in specific days of the week or every day at startup or at specific time of the day.
 Home-page: https://github.com/zaytiri/program-scheduler
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/program-scheduler
 Project-URL: Changelog, https://github.com/zaytiri/program-scheduler/blob/main/CHANGELOG.md
 Keywords: program,schedule,scheduler,startup,days,open,files,folders
 Classifier: Environment :: Console
```

### Comparing `progscheduler-2.3.3/README.md` & `progscheduler-2.3.4/README.md`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/progscheduler/app.py` & `progscheduler-2.3.4/progscheduler/app.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/progscheduler/scheduler.py` & `progscheduler-2.3.4/progscheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/progscheduler/settings/commands.py` & `progscheduler-2.3.4/progscheduler/settings/commands.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/progscheduler/settings/generic_arguments.py` & `progscheduler-2.3.4/progscheduler/settings/generic_arguments.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/progscheduler/settings/manager.py` & `progscheduler-2.3.4/progscheduler/settings/manager.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/progscheduler/settings/specific_arguments.py` & `progscheduler-2.3.4/progscheduler/settings/specific_arguments.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/progscheduler/utils/date.py` & `progscheduler-2.3.4/progscheduler/utils/date.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/progscheduler/utils/directory.py` & `progscheduler-2.3.4/progscheduler/utils/directory.py`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/progscheduler.egg-info/PKG-INFO` & `progscheduler-2.3.4/progscheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: progscheduler
-Version: 2.3.3
+Version: 2.3.4
 Summary: A simple automated task to schedule files to open in specific days of the week or every day at startup or at specific time of the day.
 Home-page: https://github.com/zaytiri/program-scheduler
 Author: zaytiri
 Project-URL: GitHub, https://github.com/zaytiri/program-scheduler
 Project-URL: Changelog, https://github.com/zaytiri/program-scheduler/blob/main/CHANGELOG.md
 Keywords: program,schedule,scheduler,startup,days,open,files,folders
 Classifier: Environment :: Console
```

### Comparing `progscheduler-2.3.3/progscheduler.egg-info/SOURCES.txt` & `progscheduler-2.3.4/progscheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `progscheduler-2.3.3/setup.py` & `progscheduler-2.3.4/setup.py`

 * *Files identical despite different names*

