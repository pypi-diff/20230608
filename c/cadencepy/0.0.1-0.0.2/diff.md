# Comparing `tmp/cadencepy-0.0.1.tar.gz` & `tmp/cadencepy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cadencepy-0.0.1.tar", last modified: Thu Jun  8 15:43:56 2023, max compression
+gzip compressed data, was "dist/cadencepy-0.0.2.tar", last modified: Thu Jun  8 15:51:53 2023, max compression
```

## Comparing `cadencepy-0.0.1.tar` & `cadencepy-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 15:43:56.000000 cadencepy-0.0.1/
-drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 15:43:56.000000 cadencepy-0.0.1/cadencepy.egg-info/
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 15:43:55.000000 cadencepy-0.0.1/cadencepy.egg-info/PKG-INFO
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      182 2023-06-08 15:43:55.000000 cadencepy-0.0.1/cadencepy.egg-info/SOURCES.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        1 2023-06-08 15:43:55.000000 cadencepy-0.0.1/cadencepy.egg-info/dependency_links.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       15 2023-06-08 15:43:55.000000 cadencepy-0.0.1/cadencepy.egg-info/requires.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        1 2023-06-08 15:43:55.000000 cadencepy-0.0.1/cadencepy.egg-info/top_level.txt
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:43:55.000000 cadencepy-0.0.1/README.md
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      734 2023-06-08 15:43:49.000000 cadencepy-0.0.1/setup.py
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 15:43:56.000000 cadencepy-0.0.1/PKG-INFO
--rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       38 2023-06-08 15:43:56.000000 cadencepy-0.0.1/setup.cfg
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 15:51:53.000000 cadencepy-0.0.2/
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 15:51:53.000000 cadencepy-0.0.2/cadencepy.egg-info/
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 15:51:53.000000 cadencepy-0.0.2/cadencepy.egg-info/PKG-INFO
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      246 2023-06-08 15:51:53.000000 cadencepy-0.0.2/cadencepy.egg-info/SOURCES.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        1 2023-06-08 15:51:53.000000 cadencepy-0.0.2/cadencepy.egg-info/dependency_links.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       15 2023-06-08 15:51:53.000000 cadencepy-0.0.2/cadencepy.egg-info/requires.txt
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       10 2023-06-08 15:51:53.000000 cadencepy-0.0.2/cadencepy.egg-info/top_level.txt
+drwxrwxr-x   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 15:51:53.000000 cadencepy-0.0.2/pycadence/
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:36:21.000000 cadencepy-0.0.2/pycadence/__init__.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)     1490 2023-06-08 14:53:28.000000 cadencepy-0.0.2/pycadence/pycadence.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      814 2023-06-08 14:32:37.000000 cadencepy-0.0.2/pycadence/utils.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)        0 2023-06-08 14:43:55.000000 cadencepy-0.0.2/README.md
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      734 2023-06-08 15:51:30.000000 cadencepy-0.0.2/setup.py
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)      495 2023-06-08 15:51:53.000000 cadencepy-0.0.2/PKG-INFO
+-rw-rw-r--   0 joelthomas  (1017) joelthomas  (1017)       38 2023-06-08 15:51:53.000000 cadencepy-0.0.2/setup.cfg
```

### Comparing `cadencepy-0.0.1/setup.py` & `cadencepy-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readall(path):
     with open(path) as fp:
         return fp.read()
 
 setup(
     name="cadencepy",
-    version="0.0.1",
+    version="0.0.2",
     author="joetho786",
     author_email="thomas.2@iitj.ac.in",
     description="A python SDK for running simulation and reading data from Ocean Cadence",
     long_description=readall("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/user/reponame",
     packages=find_packages(),
```

