# Comparing `tmp/ProxyMan-0.0.3.tar.gz` & `tmp/ProxyMan-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProxyMan-0.0.3.tar", last modified: Thu Jun  8 15:30:36 2023, max compression
+gzip compressed data, was "ProxyMan-0.0.4.tar", last modified: Thu Jun  8 15:34:31 2023, max compression
```

## Comparing `ProxyMan-0.0.3.tar` & `ProxyMan-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:30:36.995657 ProxyMan-0.0.3/
--rw-r--r--   0 rawandahmad   (501) staff       (20)     3294 2023-06-08 15:30:36.995534 ProxyMan-0.0.3/PKG-INFO
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:30:36.994673 ProxyMan-0.0.3/ProxyMan/
--rw-r--r--   0 rawandahmad   (501) staff       (20)      126 2023-06-08 15:30:32.000000 ProxyMan-0.0.3/ProxyMan/__init__.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)     6274 2023-06-08 15:19:36.000000 ProxyMan-0.0.3/ProxyMan/proxyman.py
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:30:36.995350 ProxyMan-0.0.3/ProxyMan.egg-info/
--rw-r--r--   0 rawandahmad   (501) staff       (20)     3294 2023-06-08 15:30:36.000000 ProxyMan-0.0.3/ProxyMan.egg-info/PKG-INFO
--rw-r--r--   0 rawandahmad   (501) staff       (20)      209 2023-06-08 15:30:36.000000 ProxyMan-0.0.3/ProxyMan.egg-info/SOURCES.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        1 2023-06-08 15:30:36.000000 ProxyMan-0.0.3/ProxyMan.egg-info/dependency_links.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        8 2023-06-08 15:30:36.000000 ProxyMan-0.0.3/ProxyMan.egg-info/requires.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        9 2023-06-08 15:30:36.000000 ProxyMan-0.0.3/ProxyMan.egg-info/top_level.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)       38 2023-06-08 15:30:36.995710 ProxyMan-0.0.3/setup.cfg
--rw-r--r--   0 rawandahmad   (501) staff       (20)      913 2023-06-08 15:30:32.000000 ProxyMan-0.0.3/setup.py
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:34:31.194939 ProxyMan-0.0.4/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)     3294 2023-06-08 15:34:31.194800 ProxyMan-0.0.4/PKG-INFO
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:34:31.193862 ProxyMan-0.0.4/ProxyMan/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      126 2023-06-08 15:34:26.000000 ProxyMan-0.0.4/ProxyMan/__init__.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)     6274 2023-06-08 15:19:36.000000 ProxyMan-0.0.4/ProxyMan/proxyman.py
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:34:31.194591 ProxyMan-0.0.4/ProxyMan.egg-info/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)     3294 2023-06-08 15:34:31.000000 ProxyMan-0.0.4/ProxyMan.egg-info/PKG-INFO
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      209 2023-06-08 15:34:31.000000 ProxyMan-0.0.4/ProxyMan.egg-info/SOURCES.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        1 2023-06-08 15:34:31.000000 ProxyMan-0.0.4/ProxyMan.egg-info/dependency_links.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        8 2023-06-08 15:34:31.000000 ProxyMan-0.0.4/ProxyMan.egg-info/requires.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        9 2023-06-08 15:34:31.000000 ProxyMan-0.0.4/ProxyMan.egg-info/top_level.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       38 2023-06-08 15:34:31.194986 ProxyMan-0.0.4/setup.cfg
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      913 2023-06-08 15:34:26.000000 ProxyMan-0.0.4/setup.py
```

### Comparing `ProxyMan-0.0.3/PKG-INFO` & `ProxyMan-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProxyMan
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple proxy manager for Python with WebShare API support
 Home-page: https://github.com/rawandahmad698/ProxyMan
 Author: Rawand Ahmed Shaswar
 Author-email: rawa@rawa.dev
 License: BSD 3-Clause License
 Description: # ProxyMan 🌐
```

### Comparing `ProxyMan-0.0.3/ProxyMan/proxyman.py` & `ProxyMan-0.0.4/ProxyMan/proxyman.py`

 * *Files identical despite different names*

### Comparing `ProxyMan-0.0.3/ProxyMan.egg-info/PKG-INFO` & `ProxyMan-0.0.4/ProxyMan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProxyMan
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple proxy manager for Python with WebShare API support
 Home-page: https://github.com/rawandahmad698/ProxyMan
 Author: Rawand Ahmed Shaswar
 Author-email: rawa@rawa.dev
 License: BSD 3-Clause License
 Description: # ProxyMan 🌐
```

### Comparing `ProxyMan-0.0.3/setup.py` & `ProxyMan-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 
 from setuptools import setup
 
 # Get root dir
 main_dir = os.path.dirname(os.path.realpath(__file__))
-with open(main_dir + "/README.md", "r", encoding="utf-8") as f:
+with open(main_dir + "/Readme.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name='ProxyMan',
-    version='0.0.3',
+    version='0.0.4',
     description='A simple proxy manager for Python with WebShare API support',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/rawandahmad698/ProxyMan',
     author='Rawand Ahmed Shaswar',
     author_email='rawa@rawa.dev',
     license='BSD 3-Clause License',
```

