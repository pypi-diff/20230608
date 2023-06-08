# Comparing `tmp/kg-utils-0.0.1.tar.gz` & `tmp/kg_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kg-utils-0.0.1.tar", last modified: Wed May 17 13:37:50 2023, max compression
+gzip compressed data, was "kg_utils-0.0.2.tar", last modified: Thu Jun  8 19:14:18 2023, max compression
```

## Comparing `kg-utils-0.0.1.tar` & `kg_utils-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:37:50.360962 kg-utils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-17 13:37:41.000000 kg-utils-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-17 13:37:50.360962 kg-utils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-17 13:37:41.000000 kg-utils-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:37:50.356962 kg-utils-0.0.1/kg_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-17 13:37:41.000000 kg-utils-0.0.1/kg_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-05-17 13:37:41.000000 kg-utils-0.0.1/kg_utils/merging.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-17 13:37:41.000000 kg-utils-0.0.1/kg_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 13:37:50.360962 kg-utils-0.0.1/kg_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-17 13:37:50.000000 kg-utils-0.0.1/kg_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-17 13:37:50.000000 kg-utils-0.0.1/kg_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:37:50.000000 kg-utils-0.0.1/kg_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 13:37:50.000000 kg-utils-0.0.1/kg_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-17 13:37:50.000000 kg-utils-0.0.1/kg_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-17 13:37:50.000000 kg-utils-0.0.1/kg_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 13:37:50.360962 kg-utils-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-17 13:37:41.000000 kg-utils-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:14:18.440332 kg_utils-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 19:14:13.000000 kg_utils-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-08 19:14:18.440332 kg_utils-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 19:14:13.000000 kg_utils-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:14:18.440332 kg_utils-0.0.2/kg_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 19:14:13.000000 kg_utils-0.0.2/kg_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-06-08 19:14:13.000000 kg_utils-0.0.2/kg_utils/merging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-08 19:14:13.000000 kg_utils-0.0.2/kg_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:14:18.440332 kg_utils-0.0.2/kg_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-08 19:14:18.000000 kg_utils-0.0.2/kg_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 19:14:18.000000 kg_utils-0.0.2/kg_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:14:18.000000 kg_utils-0.0.2/kg_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:14:18.000000 kg_utils-0.0.2/kg_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-08 19:14:18.000000 kg_utils-0.0.2/kg_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 19:14:18.000000 kg_utils-0.0.2/kg_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:14:18.440332 kg_utils-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-08 19:14:13.000000 kg_utils-0.0.2/setup.py
```

### Comparing `kg-utils-0.0.1/LICENSE` & `kg_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kg-utils-0.0.1/kg_utils/merging.py` & `kg_utils-0.0.2/kg_utils/merging.py`

 * *Files identical despite different names*

### Comparing `kg-utils-0.0.1/kg_utils/utils.py` & `kg_utils-0.0.2/kg_utils/utils.py`

 * *Files identical despite different names*

