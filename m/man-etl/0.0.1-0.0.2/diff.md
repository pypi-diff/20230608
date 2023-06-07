# Comparing `tmp/man_etl-0.0.1.tar.gz` & `tmp/man_etl-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "man_etl-0.0.1.tar", last modified: Wed Jun  7 22:07:30 2023, max compression
+gzip compressed data, was "man_etl-0.0.2.tar", last modified: Wed Jun  7 22:16:31 2023, max compression
```

## Comparing `man_etl-0.0.1.tar` & `man_etl-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:07:30.471419 man_etl-0.0.1/
--rw-r--r--   0 johnphillips   (501) staff       (20)       51 2023-06-07 22:07:30.471172 man_etl-0.0.1/PKG-INFO
--rw-r--r--   0 johnphillips   (501) staff       (20)       22 2023-06-05 19:31:25.000000 man_etl-0.0.1/README.md
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:07:30.466868 man_etl-0.0.1/WM9L8_IMA/
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.1/WM9L8_IMA/__init__.py
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:07:30.467783 man_etl-0.0.1/WM9L8_IMA/etl_pipelines/
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 21:52:42.000000 man_etl-0.0.1/WM9L8_IMA/etl_pipelines/__init__.py
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.1/WM9L8_IMA/etl_pipelines/arctic_transform.py
--rw-r--r--   0 johnphillips   (501) staff       (20)     1498 2023-06-07 17:47:11.000000 man_etl-0.0.1/WM9L8_IMA/etl_pipelines/csv_to_arctic.py
--rw-r--r--   0 johnphillips   (501) staff       (20)      146 2023-06-07 17:47:11.000000 man_etl-0.0.1/WM9L8_IMA/generate_db.py
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:07:30.469059 man_etl-0.0.1/WM9L8_IMA/python/
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.1/WM9L8_IMA/python/__init__.py
--rw-r--r--   0 johnphillips   (501) staff       (20)      611 2023-06-07 17:47:11.000000 man_etl-0.0.1/WM9L8_IMA/python/app.py
--rw-r--r--   0 johnphillips   (501) staff       (20)       59 2023-06-07 17:47:11.000000 man_etl-0.0.1/WM9L8_IMA/python/main.py
--rw-r--r--   0 johnphillips   (501) staff       (20)       77 2023-06-07 17:47:11.000000 man_etl-0.0.1/WM9L8_IMA/python/utils.py
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:07:30.470755 man_etl-0.0.1/man_etl.egg-info/
--rw-r--r--   0 johnphillips   (501) staff       (20)       51 2023-06-07 22:07:30.000000 man_etl-0.0.1/man_etl.egg-info/PKG-INFO
--rw-r--r--   0 johnphillips   (501) staff       (20)      478 2023-06-07 22:07:30.000000 man_etl-0.0.1/man_etl.egg-info/SOURCES.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)        1 2023-06-07 22:07:30.000000 man_etl-0.0.1/man_etl.egg-info/dependency_links.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       86 2023-06-07 22:07:30.000000 man_etl-0.0.1/man_etl.egg-info/entry_points.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)        6 2023-06-07 22:07:30.000000 man_etl-0.0.1/man_etl.egg-info/requires.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       10 2023-06-07 22:07:30.000000 man_etl-0.0.1/man_etl.egg-info/top_level.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       38 2023-06-07 22:07:30.471514 man_etl-0.0.1/setup.cfg
--rw-r--r--   0 johnphillips   (501) staff       (20)      334 2023-06-07 22:07:29.000000 man_etl-0.0.1/setup.py
+drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:16:31.908652 man_etl-0.0.2/
+-rw-r--r--   0 johnphillips   (501) staff       (20)       51 2023-06-07 22:16:31.908376 man_etl-0.0.2/PKG-INFO
+-rw-r--r--   0 johnphillips   (501) staff       (20)       22 2023-06-05 19:31:25.000000 man_etl-0.0.2/README.md
+drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:16:31.903812 man_etl-0.0.2/WM9L8_IMA/
+-rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.2/WM9L8_IMA/__init__.py
+drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:16:31.904725 man_etl-0.0.2/WM9L8_IMA/etl_pipelines/
+-rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 21:52:42.000000 man_etl-0.0.2/WM9L8_IMA/etl_pipelines/__init__.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.2/WM9L8_IMA/etl_pipelines/arctic_transform.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)     1499 2023-06-07 22:09:59.000000 man_etl-0.0.2/WM9L8_IMA/etl_pipelines/csv_to_arctic.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)      146 2023-06-07 17:47:11.000000 man_etl-0.0.2/WM9L8_IMA/generate_db.py
+drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:16:31.906348 man_etl-0.0.2/WM9L8_IMA/python/
+-rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.2/WM9L8_IMA/python/__init__.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)      611 2023-06-07 17:47:11.000000 man_etl-0.0.2/WM9L8_IMA/python/app.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)       59 2023-06-07 17:47:11.000000 man_etl-0.0.2/WM9L8_IMA/python/main.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)       77 2023-06-07 17:47:11.000000 man_etl-0.0.2/WM9L8_IMA/python/utils.py
+drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:16:31.907947 man_etl-0.0.2/man_etl.egg-info/
+-rw-r--r--   0 johnphillips   (501) staff       (20)       51 2023-06-07 22:16:31.000000 man_etl-0.0.2/man_etl.egg-info/PKG-INFO
+-rw-r--r--   0 johnphillips   (501) staff       (20)      478 2023-06-07 22:16:31.000000 man_etl-0.0.2/man_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 johnphillips   (501) staff       (20)        1 2023-06-07 22:16:31.000000 man_etl-0.0.2/man_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 johnphillips   (501) staff       (20)       86 2023-06-07 22:16:31.000000 man_etl-0.0.2/man_etl.egg-info/entry_points.txt
+-rw-r--r--   0 johnphillips   (501) staff       (20)        6 2023-06-07 22:16:31.000000 man_etl-0.0.2/man_etl.egg-info/requires.txt
+-rw-r--r--   0 johnphillips   (501) staff       (20)       10 2023-06-07 22:16:31.000000 man_etl-0.0.2/man_etl.egg-info/top_level.txt
+-rw-r--r--   0 johnphillips   (501) staff       (20)       38 2023-06-07 22:16:31.908750 man_etl-0.0.2/setup.cfg
+-rw-r--r--   0 johnphillips   (501) staff       (20)      334 2023-06-07 22:16:28.000000 man_etl-0.0.2/setup.py
```

### Comparing `man_etl-0.0.1/WM9L8_IMA/etl_pipelines/csv_to_arctic.py` & `man_etl-0.0.2/WM9L8_IMA/etl_pipelines/csv_to_arctic.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import List, Dict
 from arcticdb import Arctic
 from logging import getLogger
 import click
 
 CSV_PATH = '../data/'
 DB_PATH = 'lmdb:////mnt/c/Users/sharl/repos/DTS/BigData/WM9L8-IMA/astore'
-S3_PATH = "s3://s3.eu-west-2.amazonaws.com:manstocks?region=eu-west-2&access=AKIAVHAD6ZB4RYHDPBWA&secret=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
+S3_PATH = "s3://s3.eu-west-2.amazonaws.com:manstocks?region=eu-west-2&access=AKIAVHAD6ZB4RYHDPBWA&secret=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"
 
 class ArcticInitializer:
     def __init__(self, dbpath:str, libname:str):
         self.dbpath = dbpath
         self.libname = libname
 
     def get_db(self):
```

### Comparing `man_etl-0.0.1/WM9L8_IMA/python/app.py` & `man_etl-0.0.2/WM9L8_IMA/python/app.py`

 * *Files identical despite different names*

