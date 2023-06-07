# Comparing `tmp/man_etl-0.0.3.tar.gz` & `tmp/man_etl-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "man_etl-0.0.3.tar", last modified: Wed Jun  7 22:27:06 2023, max compression
+gzip compressed data, was "man_etl-0.0.4.tar", last modified: Wed Jun  7 22:35:56 2023, max compression
```

## Comparing `man_etl-0.0.3.tar` & `man_etl-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:27:06.364629 man_etl-0.0.3/
--rw-r--r--   0 johnphillips   (501) staff       (20)       51 2023-06-07 22:27:06.364386 man_etl-0.0.3/PKG-INFO
--rw-r--r--   0 johnphillips   (501) staff       (20)       22 2023-06-05 19:31:25.000000 man_etl-0.0.3/README.md
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:27:06.360113 man_etl-0.0.3/WM9L8_IMA/
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.3/WM9L8_IMA/__init__.py
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:27:06.361019 man_etl-0.0.3/WM9L8_IMA/etl_pipelines/
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 21:52:42.000000 man_etl-0.0.3/WM9L8_IMA/etl_pipelines/__init__.py
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.3/WM9L8_IMA/etl_pipelines/arctic_transform.py
--rw-r--r--   0 johnphillips   (501) staff       (20)     1499 2023-06-07 22:09:59.000000 man_etl-0.0.3/WM9L8_IMA/etl_pipelines/csv_to_arctic.py
--rw-r--r--   0 johnphillips   (501) staff       (20)      146 2023-06-07 17:47:11.000000 man_etl-0.0.3/WM9L8_IMA/generate_db.py
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:27:06.362480 man_etl-0.0.3/WM9L8_IMA/python/
--rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.3/WM9L8_IMA/python/__init__.py
--rw-r--r--   0 johnphillips   (501) staff       (20)      611 2023-06-07 17:47:11.000000 man_etl-0.0.3/WM9L8_IMA/python/app.py
--rw-r--r--   0 johnphillips   (501) staff       (20)       59 2023-06-07 17:47:11.000000 man_etl-0.0.3/WM9L8_IMA/python/main.py
--rw-r--r--   0 johnphillips   (501) staff       (20)       77 2023-06-07 17:47:11.000000 man_etl-0.0.3/WM9L8_IMA/python/utils.py
-drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:27:06.364024 man_etl-0.0.3/man_etl.egg-info/
--rw-r--r--   0 johnphillips   (501) staff       (20)       51 2023-06-07 22:27:06.000000 man_etl-0.0.3/man_etl.egg-info/PKG-INFO
--rw-r--r--   0 johnphillips   (501) staff       (20)      478 2023-06-07 22:27:06.000000 man_etl-0.0.3/man_etl.egg-info/SOURCES.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)        1 2023-06-07 22:27:06.000000 man_etl-0.0.3/man_etl.egg-info/dependency_links.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       86 2023-06-07 22:27:06.000000 man_etl-0.0.3/man_etl.egg-info/entry_points.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       22 2023-06-07 22:27:06.000000 man_etl-0.0.3/man_etl.egg-info/requires.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       10 2023-06-07 22:27:06.000000 man_etl-0.0.3/man_etl.egg-info/top_level.txt
--rw-r--r--   0 johnphillips   (501) staff       (20)       38 2023-06-07 22:27:06.364716 man_etl-0.0.3/setup.cfg
--rw-r--r--   0 johnphillips   (501) staff       (20)      372 2023-06-07 22:26:10.000000 man_etl-0.0.3/setup.py
+drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:35:56.672844 man_etl-0.0.4/
+-rw-r--r--   0 johnphillips   (501) staff       (20)       51 2023-06-07 22:35:56.672596 man_etl-0.0.4/PKG-INFO
+-rw-r--r--   0 johnphillips   (501) staff       (20)       22 2023-06-05 19:31:25.000000 man_etl-0.0.4/README.md
+drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:35:56.666998 man_etl-0.0.4/WM9L8_IMA/
+-rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/__init__.py
+drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:35:56.668567 man_etl-0.0.4/WM9L8_IMA/etl_pipelines/
+-rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 21:52:42.000000 man_etl-0.0.4/WM9L8_IMA/etl_pipelines/__init__.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/etl_pipelines/arctic_transform.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)     1499 2023-06-07 22:09:59.000000 man_etl-0.0.4/WM9L8_IMA/etl_pipelines/csv_to_arctic.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)      146 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/generate_db.py
+drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:35:56.670339 man_etl-0.0.4/WM9L8_IMA/python/
+-rw-r--r--   0 johnphillips   (501) staff       (20)        0 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/python/__init__.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)      611 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/python/app.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)       59 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/python/main.py
+-rw-r--r--   0 johnphillips   (501) staff       (20)       77 2023-06-07 17:47:11.000000 man_etl-0.0.4/WM9L8_IMA/python/utils.py
+drwxr-xr-x   0 johnphillips   (501) staff       (20)        0 2023-06-07 22:35:56.672156 man_etl-0.0.4/man_etl.egg-info/
+-rw-r--r--   0 johnphillips   (501) staff       (20)       51 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/PKG-INFO
+-rw-r--r--   0 johnphillips   (501) staff       (20)      478 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 johnphillips   (501) staff       (20)        1 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 johnphillips   (501) staff       (20)       86 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/entry_points.txt
+-rw-r--r--   0 johnphillips   (501) staff       (20)       29 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/requires.txt
+-rw-r--r--   0 johnphillips   (501) staff       (20)       10 2023-06-07 22:35:56.000000 man_etl-0.0.4/man_etl.egg-info/top_level.txt
+-rw-r--r--   0 johnphillips   (501) staff       (20)       38 2023-06-07 22:35:56.673209 man_etl-0.0.4/setup.cfg
+-rw-r--r--   0 johnphillips   (501) staff       (20)      379 2023-06-07 22:35:47.000000 man_etl-0.0.4/setup.py
```

### Comparing `man_etl-0.0.3/WM9L8_IMA/etl_pipelines/csv_to_arctic.py` & `man_etl-0.0.4/WM9L8_IMA/etl_pipelines/csv_to_arctic.py`

 * *Files identical despite different names*

### Comparing `man_etl-0.0.3/WM9L8_IMA/python/app.py` & `man_etl-0.0.4/WM9L8_IMA/python/app.py`

 * *Files identical despite different names*

