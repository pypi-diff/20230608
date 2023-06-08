# Comparing `tmp/localize-1.2.1.tar.gz` & `tmp/localize-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localize-1.2.1.tar", last modified: Mon Jan  9 19:13:12 2023, max compression
+gzip compressed data, was "localize-1.2.2.tar", last modified: Thu Jun  8 17:46:01 2023, max compression
```

## Comparing `localize-1.2.1.tar` & `localize-1.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-01-09 19:13:12.811942 localize-1.2.1/
--rw-r--r--   0 derek      (501) staff       (20)     1075 2022-11-14 18:53:35.000000 localize-1.2.1/LICENSE.txt
--rw-r--r--   0 derek      (501) staff       (20)       38 2022-11-14 18:53:35.000000 localize-1.2.1/MANIFEST.in
--rw-r--r--   0 derek      (501) staff       (20)     1188 2023-01-09 19:13:12.812055 localize-1.2.1/PKG-INFO
--rw-r--r--   0 derek      (501) staff       (20)      627 2022-11-14 18:53:35.000000 localize-1.2.1/README.rst
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-01-09 19:13:12.805088 localize-1.2.1/localize/
--rw-r--r--   0 derek      (501) staff       (20)        0 2022-11-14 18:53:35.000000 localize-1.2.1/localize/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)     7372 2023-01-09 18:47:42.000000 localize-1.2.1/localize/commands.py
--rw-r--r--   0 derek      (501) staff       (20)     1811 2022-12-16 15:23:27.000000 localize-1.2.1/localize/localize.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-01-09 19:13:12.807431 localize-1.2.1/localize.egg-info/
--rw-r--r--   0 derek      (501) staff       (20)     1188 2023-01-09 19:13:12.000000 localize-1.2.1/localize.egg-info/PKG-INFO
--rw-r--r--   0 derek      (501) staff       (20)      527 2023-01-09 19:13:12.000000 localize-1.2.1/localize.egg-info/SOURCES.txt
--rw-r--r--   0 derek      (501) staff       (20)        1 2023-01-09 19:13:12.000000 localize-1.2.1/localize.egg-info/dependency_links.txt
--rw-r--r--   0 derek      (501) staff       (20)       53 2023-01-09 19:13:12.000000 localize-1.2.1/localize.egg-info/entry_points.txt
--rw-r--r--   0 derek      (501) staff       (20)       47 2023-01-09 19:13:12.000000 localize-1.2.1/localize.egg-info/requires.txt
--rw-r--r--   0 derek      (501) staff       (20)       15 2023-01-09 19:13:12.000000 localize-1.2.1/localize.egg-info/top_level.txt
--rw-r--r--   0 derek      (501) staff       (20)      146 2023-01-09 19:13:12.812498 localize-1.2.1/setup.cfg
--rw-r--r--   0 derek      (501) staff       (20)      939 2023-01-09 19:12:55.000000 localize-1.2.1/setup.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-01-09 19:13:12.807993 localize-1.2.1/tests/
--rw-r--r--   0 derek      (501) staff       (20)        0 2022-11-14 18:53:35.000000 localize-1.2.1/tests/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)      581 2022-12-16 15:23:27.000000 localize-1.2.1/tests/bootstrap.py
-drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-01-09 19:13:12.811538 localize-1.2.1/tests/unit/
--rw-r--r--   0 derek      (501) staff       (20)        0 2022-11-14 18:53:35.000000 localize-1.2.1/tests/unit/__init__.py
--rw-r--r--   0 derek      (501) staff       (20)      110 2022-12-12 16:38:20.000000 localize-1.2.1/tests/unit/test_config.py
--rw-r--r--   0 derek      (501) staff       (20)      994 2022-12-16 15:23:27.000000 localize-1.2.1/tests/unit/test_get_url.py
--rw-r--r--   0 derek      (501) staff       (20)      583 2022-11-14 18:53:35.000000 localize-1.2.1/tests/unit/test_lang_format.py
--rw-r--r--   0 derek      (501) staff       (20)     7758 2022-12-16 15:23:27.000000 localize-1.2.1/tests/unit/test_pull.py
--rw-r--r--   0 derek      (501) staff       (20)     8720 2022-12-16 15:23:27.000000 localize-1.2.1/tests/unit/test_push.py
--rw-r--r--   0 derek      (501) staff       (20)      304 2022-12-16 15:23:27.000000 localize-1.2.1/tests/unit/test_utils.py
+drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-06-08 17:46:01.557108 localize-1.2.2/
+-rw-r--r--   0 derek      (501) staff       (20)     1075 2022-11-14 18:53:35.000000 localize-1.2.2/LICENSE.txt
+-rw-r--r--   0 derek      (501) staff       (20)       38 2022-11-14 18:53:35.000000 localize-1.2.2/MANIFEST.in
+-rw-r--r--   0 derek      (501) staff       (20)     1188 2023-06-08 17:46:01.557302 localize-1.2.2/PKG-INFO
+-rw-r--r--   0 derek      (501) staff       (20)      627 2022-11-14 18:53:35.000000 localize-1.2.2/README.rst
+drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-06-08 17:46:01.549999 localize-1.2.2/localize/
+-rw-r--r--   0 derek      (501) staff       (20)        0 2022-11-14 18:53:35.000000 localize-1.2.2/localize/__init__.py
+-rw-r--r--   0 derek      (501) staff       (20)     7372 2023-01-09 18:47:42.000000 localize-1.2.2/localize/commands.py
+-rw-r--r--   0 derek      (501) staff       (20)     1811 2022-12-16 15:23:27.000000 localize-1.2.2/localize/localize.py
+drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-06-08 17:46:01.552305 localize-1.2.2/localize.egg-info/
+-rw-r--r--   0 derek      (501) staff       (20)     1188 2023-06-08 17:46:01.000000 localize-1.2.2/localize.egg-info/PKG-INFO
+-rw-r--r--   0 derek      (501) staff       (20)      527 2023-06-08 17:46:01.000000 localize-1.2.2/localize.egg-info/SOURCES.txt
+-rw-r--r--   0 derek      (501) staff       (20)        1 2023-06-08 17:46:01.000000 localize-1.2.2/localize.egg-info/dependency_links.txt
+-rw-r--r--   0 derek      (501) staff       (20)       53 2023-06-08 17:46:01.000000 localize-1.2.2/localize.egg-info/entry_points.txt
+-rw-r--r--   0 derek      (501) staff       (20)       47 2023-06-08 17:46:01.000000 localize-1.2.2/localize.egg-info/requires.txt
+-rw-r--r--   0 derek      (501) staff       (20)       15 2023-06-08 17:46:01.000000 localize-1.2.2/localize.egg-info/top_level.txt
+-rw-r--r--   0 derek      (501) staff       (20)      146 2023-06-08 17:46:01.558033 localize-1.2.2/setup.cfg
+-rw-r--r--   0 derek      (501) staff       (20)      939 2023-06-08 17:39:46.000000 localize-1.2.2/setup.py
+drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-06-08 17:46:01.552957 localize-1.2.2/tests/
+-rw-r--r--   0 derek      (501) staff       (20)        0 2022-11-14 18:53:35.000000 localize-1.2.2/tests/__init__.py
+-rw-r--r--   0 derek      (501) staff       (20)      581 2022-12-16 15:23:27.000000 localize-1.2.2/tests/bootstrap.py
+drwxr-xr-x   0 derek      (501) staff       (20)        0 2023-06-08 17:46:01.556573 localize-1.2.2/tests/unit/
+-rw-r--r--   0 derek      (501) staff       (20)        0 2022-11-14 18:53:35.000000 localize-1.2.2/tests/unit/__init__.py
+-rw-r--r--   0 derek      (501) staff       (20)      110 2022-12-12 16:38:20.000000 localize-1.2.2/tests/unit/test_config.py
+-rw-r--r--   0 derek      (501) staff       (20)      994 2022-12-16 15:23:27.000000 localize-1.2.2/tests/unit/test_get_url.py
+-rw-r--r--   0 derek      (501) staff       (20)      583 2022-11-14 18:53:35.000000 localize-1.2.2/tests/unit/test_lang_format.py
+-rw-r--r--   0 derek      (501) staff       (20)     7758 2022-12-16 15:23:27.000000 localize-1.2.2/tests/unit/test_pull.py
+-rw-r--r--   0 derek      (501) staff       (20)     8720 2022-12-16 15:23:27.000000 localize-1.2.2/tests/unit/test_push.py
+-rw-r--r--   0 derek      (501) staff       (20)      304 2022-12-16 15:23:27.000000 localize-1.2.2/tests/unit/test_utils.py
```

### Comparing `localize-1.2.1/LICENSE.txt` & `localize-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localize-1.2.1/PKG-INFO` & `localize-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localize
-Version: 1.2.1
+Version: 1.2.2
 Summary: Command line utility for Localize.
 Home-page: https://help.localizejs.com/docs/localize-cli
 Author: Localize
 Author-email: support@localizejs.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `localize-1.2.1/README.rst` & `localize-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `localize-1.2.1/localize/commands.py` & `localize-1.2.2/localize/commands.py`

 * *Files identical despite different names*

### Comparing `localize-1.2.1/localize/localize.py` & `localize-1.2.2/localize/localize.py`

 * *Files identical despite different names*

### Comparing `localize-1.2.1/localize.egg-info/PKG-INFO` & `localize-1.2.2/localize.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localize
-Version: 1.2.1
+Version: 1.2.2
 Summary: Command line utility for Localize.
 Home-page: https://help.localizejs.com/docs/localize-cli
 Author: Localize
 Author-email: support@localizejs.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `localize-1.2.1/localize.egg-info/SOURCES.txt` & `localize-1.2.2/localize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localize-1.2.1/setup.py` & `localize-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # read the contents of your README file
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
   name="localize",
-  version="1.2.1",
+  version="1.2.2",
   author='Localize',
   author_email='support@localizejs.com',
   url='https://help.localizejs.com/docs/localize-cli',
   packages=find_packages(),
   description='Command line utility for Localize.',
   long_description=readme(),
   install_requires=[
-    "requests==2.25.0",
+    "requests==2.31.0",
     "colorama==0.4.4",
     "pyyaml==5.4.1"
   ],
   entry_points={
     'console_scripts': [
       'localize = localize.localize:main',
     ]
```

### Comparing `localize-1.2.1/tests/bootstrap.py` & `localize-1.2.2/tests/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localize-1.2.1/tests/unit/test_get_url.py` & `localize-1.2.2/tests/unit/test_get_url.py`

 * *Files identical despite different names*

### Comparing `localize-1.2.1/tests/unit/test_lang_format.py` & `localize-1.2.2/tests/unit/test_lang_format.py`

 * *Files identical despite different names*

### Comparing `localize-1.2.1/tests/unit/test_pull.py` & `localize-1.2.2/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `localize-1.2.1/tests/unit/test_push.py` & `localize-1.2.2/tests/unit/test_push.py`

 * *Files identical despite different names*

