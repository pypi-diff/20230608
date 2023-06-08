# Comparing `tmp/fofamap-1.1.4.tar.gz` & `tmp/fofamap-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fofamap-1.1.4.tar", last modified: Thu Jun  8 09:59:48 2023, max compression
+gzip compressed data, was "fofamap-1.1.5.tar", last modified: Thu Jun  8 10:11:24 2023, max compression
```

## Comparing `fofamap-1.1.4.tar` & `fofamap-1.1.5.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 qiuan      (501) staff       (20)        0 2023-06-08 09:59:48.586524 fofamap-1.1.4/
--rw-r--r--   0 qiuan      (501) staff       (20)      285 2023-06-08 09:59:48.586397 fofamap-1.1.4/PKG-INFO
-drwxr-xr-x   0 qiuan      (501) staff       (20)        0 2023-06-08 09:59:48.586222 fofamap-1.1.4/fofamap.egg-info/
--rw-r--r--   0 qiuan      (501) staff       (20)      285 2023-06-08 09:59:48.000000 fofamap-1.1.4/fofamap.egg-info/PKG-INFO
--rw-r--r--   0 qiuan      (501) staff       (20)      196 2023-06-08 09:59:48.000000 fofamap-1.1.4/fofamap.egg-info/SOURCES.txt
--rw-r--r--   0 qiuan      (501) staff       (20)        1 2023-06-08 09:59:48.000000 fofamap-1.1.4/fofamap.egg-info/dependency_links.txt
--rw-r--r--   0 qiuan      (501) staff       (20)       49 2023-06-08 09:59:48.000000 fofamap-1.1.4/fofamap.egg-info/entry_points.txt
--rw-r--r--   0 qiuan      (501) staff       (20)       67 2023-06-08 09:59:48.000000 fofamap-1.1.4/fofamap.egg-info/requires.txt
--rw-r--r--   0 qiuan      (501) staff       (20)        1 2023-06-08 09:59:48.000000 fofamap-1.1.4/fofamap.egg-info/top_level.txt
--rw-r--r--   0 qiuan      (501) staff       (20)       38 2023-06-08 09:59:48.586567 fofamap-1.1.4/setup.cfg
--rw-r--r--   0 qiuan      (501) staff       (20)      701 2023-06-08 09:56:41.000000 fofamap-1.1.4/setup.py
+drwxr-xr-x   0 qiuan      (501) staff       (20)        0 2023-06-08 10:11:24.832316 fofamap-1.1.5/
+-rw-r--r--   0 qiuan      (501) staff       (20)      285 2023-06-08 10:11:24.832190 fofamap-1.1.5/PKG-INFO
+-rw-r--r--   0 qiuan      (501) staff       (20)    19618 2023-05-24 23:40:52.000000 fofamap-1.1.5/README.md
+drwxr-xr-x   0 qiuan      (501) staff       (20)        0 2023-06-08 10:11:24.832018 fofamap-1.1.5/fofamap.egg-info/
+-rw-r--r--   0 qiuan      (501) staff       (20)      285 2023-06-08 10:11:24.000000 fofamap-1.1.5/fofamap.egg-info/PKG-INFO
+-rw-r--r--   0 qiuan      (501) staff       (20)      206 2023-06-08 10:11:24.000000 fofamap-1.1.5/fofamap.egg-info/SOURCES.txt
+-rw-r--r--   0 qiuan      (501) staff       (20)        1 2023-06-08 10:11:24.000000 fofamap-1.1.5/fofamap.egg-info/dependency_links.txt
+-rw-r--r--   0 qiuan      (501) staff       (20)       49 2023-06-08 10:11:24.000000 fofamap-1.1.5/fofamap.egg-info/entry_points.txt
+-rw-r--r--   0 qiuan      (501) staff       (20)       67 2023-06-08 10:11:24.000000 fofamap-1.1.5/fofamap.egg-info/requires.txt
+-rw-r--r--   0 qiuan      (501) staff       (20)        1 2023-06-08 10:11:24.000000 fofamap-1.1.5/fofamap.egg-info/top_level.txt
+-rw-r--r--   0 qiuan      (501) staff       (20)       38 2023-06-08 10:11:24.832356 fofamap-1.1.5/setup.cfg
+-rw-r--r--   0 qiuan      (501) staff       (20)      701 2023-06-08 10:11:12.000000 fofamap-1.1.5/setup.py
```

### Comparing `fofamap-1.1.4/setup.py` & `fofamap-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fofamap',
-    version='1.1.4',
+    version='1.1.5',
     packages=find_packages(),
     url='https://github.com/asaotomo/FofaMap',
     keywords='Fofa,FofaMap,nuclei',
     license='',
     author='asaotomo',
     author_email='asaotomo@qq.com',
     platforms=['any'],
```

