# Comparing `tmp/acellera-envlicenses-0.0.1.tar.gz` & `tmp/acellera-envlicenses-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acellera-envlicenses-0.0.1.tar", last modified: Wed Jun  8 13:18:54 2022, max compression
+gzip compressed data, was "acellera-envlicenses-0.0.2.tar", last modified: Thu Jun  8 14:15:23 2023, max compression
```

## Comparing `acellera-envlicenses-0.0.1.tar` & `acellera-envlicenses-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 13:18:54.024006 acellera-envlicenses-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-06-08 13:18:54.024006 acellera-envlicenses-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-06-08 13:18:44.000000 acellera-envlicenses-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 13:18:54.024006 acellera-envlicenses-0.0.1/acellera_envlicenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-06-08 13:18:53.000000 acellera-envlicenses-0.0.1/acellera_envlicenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-06-08 13:18:53.000000 acellera-envlicenses-0.0.1/acellera_envlicenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 13:18:53.000000 acellera-envlicenses-0.0.1/acellera_envlicenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-08 13:18:53.000000 acellera-envlicenses-0.0.1/acellera_envlicenses.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-08 13:18:53.000000 acellera-envlicenses-0.0.1/acellera_envlicenses.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-08 13:18:53.000000 acellera-envlicenses-0.0.1/acellera_envlicenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-08 13:18:54.024006 acellera-envlicenses-0.0.1/envlicenses/
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-06-08 13:18:44.000000 acellera-envlicenses-0.0.1/envlicenses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-06-08 13:18:44.000000 acellera-envlicenses-0.0.1/envlicenses/permissive.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-08 13:18:54.024006 acellera-envlicenses-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-06-08 13:18:44.000000 acellera-envlicenses-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:15:23.432448 acellera-envlicenses-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-08 14:15:23.432448 acellera-envlicenses-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-08 14:15:11.000000 acellera-envlicenses-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:15:23.432448 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:15:23.432448 acellera-envlicenses-0.0.2/envlicenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-08 14:15:11.000000 acellera-envlicenses-0.0.2/envlicenses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-08 14:15:11.000000 acellera-envlicenses-0.0.2/envlicenses/permissive.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:15:23.432448 acellera-envlicenses-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-08 14:15:11.000000 acellera-envlicenses-0.0.2/setup.py
```

### Comparing `acellera-envlicenses-0.0.1/envlicenses/__init__.py` & `acellera-envlicenses-0.0.2/envlicenses/__init__.py`

 * *Files identical despite different names*

### Comparing `acellera-envlicenses-0.0.1/envlicenses/permissive.txt` & `acellera-envlicenses-0.0.2/envlicenses/permissive.txt`

 * *Files 11% similar despite different names*

```diff
@@ -48,17 +48,26 @@
 LGPL-2.0-only
 LGPL-3.0
 LGPL-3.0+
 LGPL 2.1 or MPL 1.1
 LGPL-2.1
 LGPL-2.1-only
 LGPL2
+LGPLv2
+LGPLv3
+LGPL-2.0-or-later
 BSD-3-Clause AND PSF-2.0
 BSD Like
 BSD
 CC0
 CC0-1.0
 NetCDF
 Tcl/Tk
 MPL-2.0 AND MIT
 Public-Domain AND BSD-3-clause
-bzip2
+bzip2
+HPND
+LicenseRef-PSF-2.0 and CC0-1.0
+JasPer-2.0
+zlib-acknowledgement
+PostgreSQL
+BSD-2-Clause AND BSD-3-Clause
```

### Comparing `acellera-envlicenses-0.0.1/setup.py` & `acellera-envlicenses-0.0.2/setup.py`

 * *Files identical despite different names*

