# Comparing `tmp/Orbus-1.0.4.tar.gz` & `tmp/Orbus-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orbus-1.0.4.tar", last modified: Thu Jun  8 03:15:16 2023, max compression
+gzip compressed data, was "Orbus-1.0.5.tar", last modified: Thu Jun  8 03:22:26 2023, max compression
```

## Comparing `Orbus-1.0.4.tar` & `Orbus-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:15:16.602194 Orbus-1.0.4/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 02:54:32.000000 Orbus-1.0.4/LICENSE
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      446 2023-06-08 03:15:16.602194 Orbus-1.0.4/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        8 2023-06-08 02:53:32.000000 Orbus-1.0.4/README.md
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 03:15:16.602194 Orbus-1.0.4/setup.cfg
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      958 2023-06-08 03:14:55.000000 Orbus-1.0.4/setup.py
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:15:16.602194 Orbus-1.0.4/src/
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:15:16.602194 Orbus-1.0.4/src/Orbus.egg-info/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      446 2023-06-08 03:15:16.000000 Orbus-1.0.4/src/Orbus.egg-info/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      212 2023-06-08 03:15:16.000000 Orbus-1.0.4/src/Orbus.egg-info/SOURCES.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 03:15:16.000000 Orbus-1.0.4/src/Orbus.egg-info/dependency_links.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       56 2023-06-08 03:15:16.000000 Orbus-1.0.4/src/Orbus.egg-info/entry_points.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       11 2023-06-08 03:15:16.000000 Orbus-1.0.4/src/Orbus.egg-info/top_level.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       35 2023-06-08 03:01:30.000000 Orbus-1.0.4/src/orbusmaker.py
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:22:26.215722 Orbus-1.0.5/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 02:54:32.000000 Orbus-1.0.5/LICENSE
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:22:26.215722 Orbus-1.0.5/Orbus.egg-info/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      423 2023-06-08 03:22:26.000000 Orbus-1.0.5/Orbus.egg-info/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      174 2023-06-08 03:22:26.000000 Orbus-1.0.5/Orbus.egg-info/SOURCES.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 03:22:26.000000 Orbus-1.0.5/Orbus.egg-info/dependency_links.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       56 2023-06-08 03:22:26.000000 Orbus-1.0.5/Orbus.egg-info/entry_points.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       11 2023-06-08 03:22:26.000000 Orbus-1.0.5/Orbus.egg-info/top_level.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      423 2023-06-08 03:22:26.215722 Orbus-1.0.5/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        8 2023-06-08 02:53:32.000000 Orbus-1.0.5/README.md
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 03:22:26.215722 Orbus-1.0.5/setup.cfg
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1696 2023-06-08 03:22:06.000000 Orbus-1.0.5/setup.py
```

### Comparing `Orbus-1.0.4/LICENSE` & `Orbus-1.0.5/LICENSE`

 * *Files identical despite different names*

