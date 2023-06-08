# Comparing `tmp/ngm_salam-0.0.3.tar.gz` & `tmp/ngm_salam-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngm_salam-0.0.3.tar", last modified: Thu Jun  8 03:23:03 2023, max compression
+gzip compressed data, was "ngm_salam-0.0.4.tar", last modified: Thu Jun  8 03:31:55 2023, max compression
```

## Comparing `ngm_salam-0.0.3.tar` & `ngm_salam-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 03:23:03.492004 ngm_salam-0.0.3/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      177 2023-06-08 03:23:03.491594 ngm_salam-0.0.3/PKG-INFO
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       54 2023-06-08 02:58:19.000000 ngm_salam-0.0.3/README.md
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 03:23:03.487667 ngm_salam-0.0.3/ngm_salam/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-06-07 17:21:12.000000 ngm_salam-0.0.3/ngm_salam/__init__.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      139 2023-06-07 20:22:06.000000 ngm_salam-0.0.3/ngm_salam/__main__.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       48 2023-06-07 19:10:01.000000 ngm_salam-0.0.3/ngm_salam/message.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      686 2023-06-07 18:49:48.000000 ngm_salam-0.0.3/ngm_salam/sysparams.py
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 03:23:03.491112 ngm_salam-0.0.3/ngm_salam.egg-info/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      177 2023-06-08 03:23:03.000000 ngm_salam-0.0.3/ngm_salam.egg-info/PKG-INFO
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      312 2023-06-08 03:23:03.000000 ngm_salam-0.0.3/ngm_salam.egg-info/SOURCES.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-06-08 03:23:03.000000 ngm_salam-0.0.3/ngm_salam.egg-info/dependency_links.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       50 2023-06-08 03:23:03.000000 ngm_salam-0.0.3/ngm_salam.egg-info/entry_points.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       16 2023-06-08 03:23:03.000000 ngm_salam-0.0.3/ngm_salam.egg-info/requires.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       10 2023-06-08 03:23:03.000000 ngm_salam-0.0.3/ngm_salam.egg-info/top_level.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      289 2023-06-08 03:22:44.000000 ngm_salam-0.0.3/pyproject.toml
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-06-08 03:23:03.492080 ngm_salam-0.0.3/setup.cfg
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 03:31:55.816063 ngm_salam-0.0.4/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      211 2023-06-08 03:31:55.815789 ngm_salam-0.0.4/PKG-INFO
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       88 2023-06-08 03:31:24.000000 ngm_salam-0.0.4/README.md
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 03:31:55.813685 ngm_salam-0.0.4/ngm_salam/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-06-07 17:21:12.000000 ngm_salam-0.0.4/ngm_salam/__init__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      139 2023-06-07 20:22:06.000000 ngm_salam-0.0.4/ngm_salam/__main__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       48 2023-06-07 19:10:01.000000 ngm_salam-0.0.4/ngm_salam/message.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      686 2023-06-07 18:49:48.000000 ngm_salam-0.0.4/ngm_salam/sysparams.py
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 03:31:55.815445 ngm_salam-0.0.4/ngm_salam.egg-info/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      211 2023-06-08 03:31:55.000000 ngm_salam-0.0.4/ngm_salam.egg-info/PKG-INFO
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      312 2023-06-08 03:31:55.000000 ngm_salam-0.0.4/ngm_salam.egg-info/SOURCES.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-06-08 03:31:55.000000 ngm_salam-0.0.4/ngm_salam.egg-info/dependency_links.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       50 2023-06-08 03:31:55.000000 ngm_salam-0.0.4/ngm_salam.egg-info/entry_points.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       16 2023-06-08 03:31:55.000000 ngm_salam-0.0.4/ngm_salam.egg-info/requires.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       10 2023-06-08 03:31:55.000000 ngm_salam-0.0.4/ngm_salam.egg-info/top_level.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      289 2023-06-08 03:31:40.000000 ngm_salam-0.0.4/pyproject.toml
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-06-08 03:31:55.816146 ngm_salam-0.0.4/setup.cfg
```

### Comparing `ngm_salam-0.0.3/ngm_salam/sysparams.py` & `ngm_salam-0.0.4/ngm_salam/sysparams.py`

 * *Files identical despite different names*

