# Comparing `tmp/mi_libreria-0.2.tar.gz` & `tmp/mi_libreria-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mi_libreria-0.2.tar", last modified: Thu Jun  8 02:22:05 2023, max compression
+gzip compressed data, was "mi_libreria-0.3.tar", last modified: Thu Jun  8 02:26:13 2023, max compression
```

## Comparing `mi_libreria-0.2.tar` & `mi_libreria-0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:22:05.194450 mi_libreria-0.2/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       53 2023-06-08 02:22:05.194450 mi_libreria-0.2/PKG-INFO
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:22:05.194450 mi_libreria-0.2/mi_libreria.egg-info/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       53 2023-06-08 02:22:04.000000 mi_libreria-0.2/mi_libreria.egg-info/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      186 2023-06-08 02:22:05.000000 mi_libreria-0.2/mi_libreria.egg-info/SOURCES.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 02:22:04.000000 mi_libreria-0.2/mi_libreria.egg-info/dependency_links.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       58 2023-06-08 02:22:04.000000 mi_libreria-0.2/mi_libreria.egg-info/entry_points.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       12 2023-06-08 02:22:04.000000 mi_libreria-0.2/mi_libreria.egg-info/top_level.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 02:22:05.194450 mi_libreria-0.2/setup.cfg
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      231 2023-06-08 02:21:48.000000 mi_libreria-0.2/setup.py
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:26:13.541168 mi_libreria-0.3/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       53 2023-06-08 02:26:13.541168 mi_libreria-0.3/PKG-INFO
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:26:13.541168 mi_libreria-0.3/mi_libreria.egg-info/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       53 2023-06-08 02:26:13.000000 mi_libreria-0.3/mi_libreria.egg-info/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      201 2023-06-08 02:26:13.000000 mi_libreria-0.3/mi_libreria.egg-info/SOURCES.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 02:26:13.000000 mi_libreria-0.3/mi_libreria.egg-info/dependency_links.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       58 2023-06-08 02:26:13.000000 mi_libreria-0.3/mi_libreria.egg-info/entry_points.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       12 2023-06-08 02:26:13.000000 mi_libreria-0.3/mi_libreria.egg-info/top_level.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       62 2023-06-08 02:19:49.000000 mi_libreria-0.3/mi_libreria.py
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 02:26:13.541168 mi_libreria-0.3/setup.cfg
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      232 2023-06-08 02:25:07.000000 mi_libreria-0.3/setup.py
```

