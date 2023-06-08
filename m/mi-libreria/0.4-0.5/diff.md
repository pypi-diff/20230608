# Comparing `tmp/mi_libreria-0.4.tar.gz` & `tmp/mi_libreria-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mi_libreria-0.4.tar", last modified: Thu Jun  8 02:31:41 2023, max compression
+gzip compressed data, was "mi_libreria-0.5.tar", last modified: Thu Jun  8 02:35:18 2023, max compression
```

## Comparing `mi_libreria-0.4.tar` & `mi_libreria-0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:31:41.187901 mi_libreria-0.4/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       53 2023-06-08 02:31:41.187901 mi_libreria-0.4/PKG-INFO
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:31:41.187901 mi_libreria-0.4/mi_libreria.egg-info/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       53 2023-06-08 02:31:40.000000 mi_libreria-0.4/mi_libreria.egg-info/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      186 2023-06-08 02:31:41.000000 mi_libreria-0.4/mi_libreria.egg-info/SOURCES.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 02:31:40.000000 mi_libreria-0.4/mi_libreria.egg-info/dependency_links.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       58 2023-06-08 02:31:40.000000 mi_libreria-0.4/mi_libreria.egg-info/entry_points.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       12 2023-06-08 02:31:40.000000 mi_libreria-0.4/mi_libreria.egg-info/top_level.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 02:31:41.187901 mi_libreria-0.4/setup.cfg
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      232 2023-06-08 02:31:25.000000 mi_libreria-0.4/setup.py
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:35:18.381278 mi_libreria-0.5/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       53 2023-06-08 02:35:18.381278 mi_libreria-0.5/PKG-INFO
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:35:18.381278 mi_libreria-0.5/mi_libreria.egg-info/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       53 2023-06-08 02:35:18.000000 mi_libreria-0.5/mi_libreria.egg-info/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      186 2023-06-08 02:35:18.000000 mi_libreria-0.5/mi_libreria.egg-info/SOURCES.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 02:35:18.000000 mi_libreria-0.5/mi_libreria.egg-info/dependency_links.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       58 2023-06-08 02:35:18.000000 mi_libreria-0.5/mi_libreria.egg-info/entry_points.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       12 2023-06-08 02:35:18.000000 mi_libreria-0.5/mi_libreria.egg-info/top_level.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 02:35:18.381278 mi_libreria-0.5/setup.cfg
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      232 2023-06-08 02:35:00.000000 mi_libreria-0.5/setup.py
```

