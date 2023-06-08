# Comparing `tmp/ngm_salam-0.0.7.tar.gz` & `tmp/ngm_salam-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngm_salam-0.0.7.tar", last modified: Thu Jun  8 04:06:45 2023, max compression
+gzip compressed data, was "ngm_salam-0.0.8.tar", last modified: Thu Jun  8 04:24:51 2023, max compression
```

## Comparing `ngm_salam-0.0.7.tar` & `ngm_salam-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 04:06:45.884531 ngm_salam-0.0.7/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      467 2023-06-08 04:06:45.884207 ngm_salam-0.0.7/PKG-INFO
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       88 2023-06-08 03:52:05.000000 ngm_salam-0.0.7/README.md
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 04:06:45.882070 ngm_salam-0.0.7/ngm_salam/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-06-07 17:21:12.000000 ngm_salam-0.0.7/ngm_salam/__init__.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      139 2023-06-07 20:22:06.000000 ngm_salam-0.0.7/ngm_salam/__main__.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       48 2023-06-07 19:10:01.000000 ngm_salam-0.0.7/ngm_salam/message.py
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      686 2023-06-07 18:49:48.000000 ngm_salam-0.0.7/ngm_salam/sysparams.py
-drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 04:06:45.883839 ngm_salam-0.0.7/ngm_salam.egg-info/
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      467 2023-06-08 04:06:45.000000 ngm_salam-0.0.7/ngm_salam.egg-info/PKG-INFO
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      312 2023-06-08 04:06:45.000000 ngm_salam-0.0.7/ngm_salam.egg-info/SOURCES.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-06-08 04:06:45.000000 ngm_salam-0.0.7/ngm_salam.egg-info/dependency_links.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       50 2023-06-08 04:06:45.000000 ngm_salam-0.0.7/ngm_salam.egg-info/entry_points.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       16 2023-06-08 04:06:45.000000 ngm_salam-0.0.7/ngm_salam.egg-info/requires.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       10 2023-06-08 04:06:45.000000 ngm_salam-0.0.7/ngm_salam.egg-info/top_level.txt
--rw-r--r--   0 ngmaibulat   (502) staff       (20)      540 2023-06-08 04:06:32.000000 ngm_salam-0.0.7/pyproject.toml
--rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-06-08 04:06:45.884623 ngm_salam-0.0.7/setup.cfg
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 04:24:51.355964 ngm_salam-0.0.8/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      501 2023-06-08 04:24:51.355612 ngm_salam-0.0.8/PKG-INFO
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       88 2023-06-08 03:52:05.000000 ngm_salam-0.0.8/README.md
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 04:24:51.351816 ngm_salam-0.0.8/ngm_salam/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        0 2023-06-07 17:21:12.000000 ngm_salam-0.0.8/ngm_salam/__init__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      139 2023-06-07 20:22:06.000000 ngm_salam-0.0.8/ngm_salam/__main__.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       48 2023-06-07 19:10:01.000000 ngm_salam-0.0.8/ngm_salam/message.py
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      686 2023-06-07 18:49:48.000000 ngm_salam-0.0.8/ngm_salam/sysparams.py
+drwxr-xr-x   0 ngmaibulat   (502) staff       (20)        0 2023-06-08 04:24:51.355020 ngm_salam-0.0.8/ngm_salam.egg-info/
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      501 2023-06-08 04:24:51.000000 ngm_salam-0.0.8/ngm_salam.egg-info/PKG-INFO
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      312 2023-06-08 04:24:51.000000 ngm_salam-0.0.8/ngm_salam.egg-info/SOURCES.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)        1 2023-06-08 04:24:51.000000 ngm_salam-0.0.8/ngm_salam.egg-info/dependency_links.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       50 2023-06-08 04:24:51.000000 ngm_salam-0.0.8/ngm_salam.egg-info/entry_points.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       16 2023-06-08 04:24:51.000000 ngm_salam-0.0.8/ngm_salam.egg-info/requires.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       10 2023-06-08 04:24:51.000000 ngm_salam-0.0.8/ngm_salam.egg-info/top_level.txt
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)      574 2023-06-08 04:23:54.000000 ngm_salam-0.0.8/pyproject.toml
+-rw-r--r--   0 ngmaibulat   (502) staff       (20)       38 2023-06-08 04:24:51.356074 ngm_salam-0.0.8/setup.cfg
```

### Comparing `ngm_salam-0.0.7/ngm_salam/sysparams.py` & `ngm_salam-0.0.8/ngm_salam/sysparams.py`

 * *Files identical despite different names*

