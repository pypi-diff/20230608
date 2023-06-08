# Comparing `tmp/cadencepy-0.0.6.tar.gz` & `tmp/cadencepy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cadencepy-0.0.6.tar", last modified: Thu Jun  8 16:27:40 2023, max compression
+gzip compressed data, was "dist/cadencepy-0.0.7.tar", last modified: Thu Jun  8 16:30:38 2023, max compression
```

## Comparing `cadencepy-0.0.6.tar` & `cadencepy-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:27:40.000000 cadencepy-0.0.6/
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:27:40.000000 cadencepy-0.0.6/cadencepy.egg-info/
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 16:27:39.000000 cadencepy-0.0.6/cadencepy.egg-info/PKG-INFO
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      246 2023-06-08 16:27:39.000000 cadencepy-0.0.6/cadencepy.egg-info/SOURCES.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        1 2023-06-08 16:27:39.000000 cadencepy-0.0.6/cadencepy.egg-info/dependency_links.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       15 2023-06-08 16:27:39.000000 cadencepy-0.0.6/cadencepy.egg-info/requires.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       10 2023-06-08 16:27:39.000000 cadencepy-0.0.6/cadencepy.egg-info/top_level.txt
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:27:40.000000 cadencepy-0.0.6/pycadence/
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:36:21.000000 cadencepy-0.0.6/pycadence/__init__.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     1610 2023-06-08 16:15:56.000000 cadencepy-0.0.6/pycadence/pycadence.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      814 2023-06-08 14:32:37.000000 cadencepy-0.0.6/pycadence/utils.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:43:55.000000 cadencepy-0.0.6/README.md
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      734 2023-06-08 16:27:11.000000 cadencepy-0.0.6/setup.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 16:27:40.000000 cadencepy-0.0.6/PKG-INFO
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       38 2023-06-08 16:27:40.000000 cadencepy-0.0.6/setup.cfg
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:30:38.000000 cadencepy-0.0.7/
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:30:38.000000 cadencepy-0.0.7/cadencepy.egg-info/
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 16:30:38.000000 cadencepy-0.0.7/cadencepy.egg-info/PKG-INFO
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      321 2023-06-08 16:30:38.000000 cadencepy-0.0.7/cadencepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        1 2023-06-08 16:30:38.000000 cadencepy-0.0.7/cadencepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       15 2023-06-08 16:30:38.000000 cadencepy-0.0.7/cadencepy.egg-info/requires.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       10 2023-06-08 16:30:38.000000 cadencepy-0.0.7/cadencepy.egg-info/top_level.txt
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 16:30:38.000000 cadencepy-0.0.7/pycadence/
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:36:21.000000 cadencepy-0.0.7/pycadence/__init__.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      166 2023-06-08 16:12:09.000000 cadencepy-0.0.7/pycadence/connect.sh
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       99 2023-06-08 14:52:30.000000 cadencepy-0.0.7/pycadence/disconnect.sh
+-rwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)       87 2023-06-08 14:51:23.000000 cadencepy-0.0.7/pycadence/ocean_simulation.sh
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     1610 2023-06-08 16:15:56.000000 cadencepy-0.0.7/pycadence/pycadence.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      814 2023-06-08 14:32:37.000000 cadencepy-0.0.7/pycadence/utils.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:43:55.000000 cadencepy-0.0.7/README.md
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      776 2023-06-08 16:30:35.000000 cadencepy-0.0.7/setup.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 16:30:38.000000 cadencepy-0.0.7/PKG-INFO
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       38 2023-06-08 16:30:38.000000 cadencepy-0.0.7/setup.cfg
```

### Comparing `cadencepy-0.0.6/pycadence/pycadence.py` & `cadencepy-0.0.7/pycadence/pycadence.py`

 * *Files identical despite different names*

### Comparing `cadencepy-0.0.6/pycadence/utils.py` & `cadencepy-0.0.7/pycadence/utils.py`

 * *Files identical despite different names*

### Comparing `cadencepy-0.0.6/setup.py` & `cadencepy-0.0.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 
 def readall(path):
     with open(path) as fp:
         return fp.read()
 
 setup(
     name="cadencepy",
-    version="0.0.6",
+    version="0.0.7",
     author="joetho786",
     author_email="thomas.2@iitj.ac.in",
     description="A python SDK for running simulation and reading data from Ocean Cadence",
     long_description=readall("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/user/reponame",
     packages=find_packages(),
+    package_data={'pycadence': ['*.sh']},
     install_requires=["requests","numpy"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
```

