# Comparing `tmp/ngm_salam-0.0.5.tar.gz` & `tmp/ngm_salam-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngm_salam-0.0.5.tar", last modified: Thu Jun  8 03:52:18 2023, max compression
+gzip compressed data, was "ngm_salam-0.0.6.tar", last modified: Thu Jun  8 04:01:12 2023, max compression
```

## Comparing `ngm_salam-0.0.5.tar` & `ngm_salam-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 03:52:18.810403 ngm_salam-0.0.5/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      259 2023-06-08 03:52:18.810112 ngm_salam-0.0.5/PKG-INFO
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       88 2023-06-08 03:52:05.000000 ngm_salam-0.0.5/README.md
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 03:52:18.807607 ngm_salam-0.0.5/ngm_salam/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-06-07 17:21:12.000000 ngm_salam-0.0.5/ngm_salam/__init__.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      139 2023-06-07 20:22:06.000000 ngm_salam-0.0.5/ngm_salam/__main__.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       48 2023-06-07 19:10:01.000000 ngm_salam-0.0.5/ngm_salam/message.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      686 2023-06-07 18:49:48.000000 ngm_salam-0.0.5/ngm_salam/sysparams.py
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 03:52:18.809750 ngm_salam-0.0.5/ngm_salam.egg-info/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      259 2023-06-08 03:52:18.000000 ngm_salam-0.0.5/ngm_salam.egg-info/PKG-INFO
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      312 2023-06-08 03:52:18.000000 ngm_salam-0.0.5/ngm_salam.egg-info/SOURCES.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-06-08 03:52:18.000000 ngm_salam-0.0.5/ngm_salam.egg-info/dependency_links.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       50 2023-06-08 03:52:18.000000 ngm_salam-0.0.5/ngm_salam.egg-info/entry_points.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       16 2023-06-08 03:52:18.000000 ngm_salam-0.0.5/ngm_salam.egg-info/requires.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       10 2023-06-08 03:52:18.000000 ngm_salam-0.0.5/ngm_salam.egg-info/top_level.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      348 2023-06-08 03:51:54.000000 ngm_salam-0.0.5/pyproject.toml
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-06-08 03:52:18.810496 ngm_salam-0.0.5/setup.cfg
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 04:01:12.774050 ngm_salam-0.0.6/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      259 2023-06-08 04:01:12.773766 ngm_salam-0.0.6/PKG-INFO
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       88 2023-06-08 03:52:05.000000 ngm_salam-0.0.6/README.md
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 04:01:12.771055 ngm_salam-0.0.6/ngm_salam/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-06-07 17:21:12.000000 ngm_salam-0.0.6/ngm_salam/__init__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      139 2023-06-07 20:22:06.000000 ngm_salam-0.0.6/ngm_salam/__main__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       48 2023-06-07 19:10:01.000000 ngm_salam-0.0.6/ngm_salam/message.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      686 2023-06-07 18:49:48.000000 ngm_salam-0.0.6/ngm_salam/sysparams.py
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 04:01:12.773384 ngm_salam-0.0.6/ngm_salam.egg-info/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      259 2023-06-08 04:01:12.000000 ngm_salam-0.0.6/ngm_salam.egg-info/PKG-INFO
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      312 2023-06-08 04:01:12.000000 ngm_salam-0.0.6/ngm_salam.egg-info/SOURCES.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-06-08 04:01:12.000000 ngm_salam-0.0.6/ngm_salam.egg-info/dependency_links.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       50 2023-06-08 04:01:12.000000 ngm_salam-0.0.6/ngm_salam.egg-info/entry_points.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       16 2023-06-08 04:01:12.000000 ngm_salam-0.0.6/ngm_salam.egg-info/requires.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       10 2023-06-08 04:01:12.000000 ngm_salam-0.0.6/ngm_salam.egg-info/top_level.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      433 2023-06-08 04:00:56.000000 ngm_salam-0.0.6/pyproject.toml
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-06-08 04:01:12.774128 ngm_salam-0.0.6/setup.cfg
```

### Comparing `ngm_salam-0.0.5/ngm_salam/sysparams.py` & `ngm_salam-0.0.6/ngm_salam/sysparams.py`

 * *Files identical despite different names*

