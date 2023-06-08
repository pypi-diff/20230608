# Comparing `tmp/lspsp-1.0.2.post2.tar.gz` & `tmp/lspsp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lspsp-1.0.2.post2.tar", last modified: Tue May  9 04:44:49 2023, max compression
+gzip compressed data, was "lspsp-1.0.3.tar", last modified: Thu Jun  8 10:24:30 2023, max compression
```

## Comparing `lspsp-1.0.2.post2.tar` & `lspsp-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:49.828255 lspsp-1.0.2.post2/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-09 04:44:49.828255 lspsp-1.0.2.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/config.json.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:49.828255 lspsp-1.0.2.post2/lspsp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/lspmon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/lspnotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/lspsp.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/mailbuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/monexec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:49.828255 lspsp-1.0.2.post2/lspsp/resource/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/resource/mail.html
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/lspsp/resource/test.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 04:44:49.828255 lspsp-1.0.2.post2/lspsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-09 04:44:49.000000 lspsp-1.0.2.post2/lspsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 04:44:49.832255 lspsp-1.0.2.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-09 04:44:32.000000 lspsp-1.0.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:30.439299 lspsp-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 10:24:20.000000 lspsp-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 10:24:30.439299 lspsp-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 10:24:20.000000 lspsp-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-08 10:24:20.000000 lspsp-1.0.3/config.json.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:30.435299 lspsp-1.0.3/lspsp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/lspmon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/lspnotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/lspsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/mailbuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/monexec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:30.439299 lspsp-1.0.3/lspsp/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/resource/mail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 10:24:20.000000 lspsp-1.0.3/lspsp/resource/test.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:30.439299 lspsp-1.0.3/lspsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 10:24:30.000000 lspsp-1.0.3/lspsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:24:30.439299 lspsp-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-08 10:24:20.000000 lspsp-1.0.3/setup.py
```

### Comparing `lspsp-1.0.2.post2/lspsp/lspmon.py` & `lspsp-1.0.3/lspsp/lspmon.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,16 @@
         self._interval = data['interval']
         self._api = Lspsp(data['loginuser'])
         logging.basicConfig(
             level=logging.INFO, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')
         self._logger = logging.getLogger(__name__)
         self._mode = mode
         self._notifier = LspNotify(mode)
+        logging.getLogger('apscheduler.executors.default').setLevel(
+            logging.WARNING)
 
     def diff(self, data):
         diff = {}
         for key in data.keys():
             if self._current.get(key) == None:
                 diff[key] = data[key]
         return diff
```

### Comparing `lspsp-1.0.2.post2/lspsp/lspnotify.py` & `lspsp-1.0.3/lspsp/lspnotify.py`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.2.post2/lspsp/lspsp.py` & `lspsp-1.0.3/lspsp/lspsp.py`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.2.post2/lspsp/mailbuilder.py` & `lspsp-1.0.3/lspsp/mailbuilder.py`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.2.post2/lspsp/monexec.py` & `lspsp-1.0.3/lspsp/monexec.py`

 * *Files identical despite different names*

### Comparing `lspsp-1.0.2.post2/setup.py` & `lspsp-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="lspsp",
-    version="1.0.2-2",
+    version="1.0.3",
     license='GPL',
     description='LSPSP.ME Monitor',
     long_description='LSPSP.ME Monitor Service',
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
     install_requires=[
```

