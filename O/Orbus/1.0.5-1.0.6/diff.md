# Comparing `tmp/Orbus-1.0.5.tar.gz` & `tmp/Orbus-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orbus-1.0.5.tar", last modified: Thu Jun  8 03:22:26 2023, max compression
+gzip compressed data, was "Orbus-1.0.6.tar", last modified: Thu Jun  8 03:30:44 2023, max compression
```

## Comparing `Orbus-1.0.5.tar` & `Orbus-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:22:26.215722 Orbus-1.0.5/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 02:54:32.000000 Orbus-1.0.5/LICENSE
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:22:26.215722 Orbus-1.0.5/Orbus.egg-info/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      423 2023-06-08 03:22:26.000000 Orbus-1.0.5/Orbus.egg-info/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      174 2023-06-08 03:22:26.000000 Orbus-1.0.5/Orbus.egg-info/SOURCES.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 03:22:26.000000 Orbus-1.0.5/Orbus.egg-info/dependency_links.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       56 2023-06-08 03:22:26.000000 Orbus-1.0.5/Orbus.egg-info/entry_points.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       11 2023-06-08 03:22:26.000000 Orbus-1.0.5/Orbus.egg-info/top_level.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      423 2023-06-08 03:22:26.215722 Orbus-1.0.5/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        8 2023-06-08 02:53:32.000000 Orbus-1.0.5/README.md
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 03:22:26.215722 Orbus-1.0.5/setup.cfg
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1696 2023-06-08 03:22:06.000000 Orbus-1.0.5/setup.py
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:30:44.324264 Orbus-1.0.6/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 02:54:32.000000 Orbus-1.0.6/LICENSE
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:30:44.324264 Orbus-1.0.6/Orbus.egg-info/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      423 2023-06-08 03:30:44.000000 Orbus-1.0.6/Orbus.egg-info/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      174 2023-06-08 03:30:44.000000 Orbus-1.0.6/Orbus.egg-info/SOURCES.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 03:30:44.000000 Orbus-1.0.6/Orbus.egg-info/dependency_links.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       70 2023-06-08 03:30:44.000000 Orbus-1.0.6/Orbus.egg-info/entry_points.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       11 2023-06-08 03:30:44.000000 Orbus-1.0.6/Orbus.egg-info/top_level.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      423 2023-06-08 03:30:44.324264 Orbus-1.0.6/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        8 2023-06-08 02:53:32.000000 Orbus-1.0.6/README.md
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 03:30:44.324264 Orbus-1.0.6/setup.cfg
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      823 2023-06-08 03:30:31.000000 Orbus-1.0.6/setup.py
```

### Comparing `Orbus-1.0.5/LICENSE` & `Orbus-1.0.6/LICENSE`

 * *Files identical despite different names*

