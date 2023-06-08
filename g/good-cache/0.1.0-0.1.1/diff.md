# Comparing `tmp/good_cache-0.1.0.tar.gz` & `tmp/good_cache-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "good_cache-0.1.0.tar", last modified: Wed Jun  7 19:47:59 2023, max compression
+gzip compressed data, was "good_cache-0.1.1.tar", last modified: Thu Jun  8 01:41:03 2023, max compression
```

## Comparing `good_cache-0.1.0.tar` & `good_cache-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-07 19:47:59.224692 good_cache-0.1.0/
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)    11357 2023-05-04 02:17:26.000000 good_cache-0.1.0/LICENSE
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      324 2023-06-07 19:47:59.224692 good_cache-0.1.0/PKG-INFO
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1373 2023-05-04 02:17:26.000000 good_cache-0.1.0/README.md
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       38 2023-06-07 19:47:59.224692 good_cache-0.1.0/setup.cfg
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      572 2023-06-07 19:42:01.000000 good_cache-0.1.0/setup.py
-drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-07 19:47:59.192693 good_cache-0.1.0/src/
-drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-07 19:47:59.224692 good_cache-0.1.0/src/good_cache.egg-info/
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      324 2023-06-07 19:47:59.000000 good_cache-0.1.0/src/good_cache.egg-info/PKG-INFO
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      215 2023-06-07 19:47:59.000000 good_cache-0.1.0/src/good_cache.egg-info/SOURCES.txt
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)        1 2023-06-07 19:47:59.000000 good_cache-0.1.0/src/good_cache.egg-info/dependency_links.txt
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       11 2023-06-07 19:47:59.000000 good_cache-0.1.0/src/good_cache.egg-info/requires.txt
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)        1 2023-06-07 19:47:59.000000 good_cache-0.1.0/src/good_cache.egg-info/top_level.txt
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 01:41:03.526802 good_cache-0.1.1/
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)    11357 2023-05-04 02:17:26.000000 good_cache-0.1.1/LICENSE
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      324 2023-06-08 01:41:03.526802 good_cache-0.1.1/PKG-INFO
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1370 2023-06-08 01:38:42.000000 good_cache-0.1.1/README.md
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       38 2023-06-08 01:41:03.526802 good_cache-0.1.1/setup.cfg
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      572 2023-06-08 01:40:31.000000 good_cache-0.1.1/setup.py
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 01:41:03.522802 good_cache-0.1.1/src/
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 01:41:03.526802 good_cache-0.1.1/src/good_cache.egg-info/
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      324 2023-06-08 01:41:03.000000 good_cache-0.1.1/src/good_cache.egg-info/PKG-INFO
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      215 2023-06-08 01:41:03.000000 good_cache-0.1.1/src/good_cache.egg-info/SOURCES.txt
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)        1 2023-06-08 01:41:03.000000 good_cache-0.1.1/src/good_cache.egg-info/dependency_links.txt
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       11 2023-06-08 01:41:03.000000 good_cache-0.1.1/src/good_cache.egg-info/requires.txt
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)        1 2023-06-08 01:41:03.000000 good_cache-0.1.1/src/good_cache.egg-info/top_level.txt
```

### Comparing `good_cache-0.1.0/LICENSE` & `good_cache-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `good_cache-0.1.0/README.md` & `good_cache-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,10 +20,7 @@
 ## Here are examples:
 ### You have a file <code>stock-quotes.parquet</code> that looks so:
 | ticker | date | price | 
 |-|-|-|
 |A|1999-01-01|15|
 |AMZN|1999-01-01|24|
 ...
-
-
-
```

### Comparing `good_cache-0.1.0/setup.py` & `good_cache-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='good_cache',
-    version='0.1.0',
+    version='0.1.1',
     url='https://github.com/arunsundaram50/good-cache.git',
     author='Arun Sundaram',
     author_email='arun_co@yahoo.com',
     description='Efficient function caching based on file modifications and function parameters.',
     packages=find_packages(where="src"),  # Specifies the src directory
     package_dir={"": "src"},  # Specifies the package directory
     install_requires=requirements,
```

