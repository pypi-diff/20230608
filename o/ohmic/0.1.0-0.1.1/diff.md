# Comparing `tmp/ohmic-0.1.0.tar.gz` & `tmp/ohmic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmic-0.1.0.tar", last modified: Wed Jun  7 13:04:47 2023, max compression
+gzip compressed data, was "ohmic-0.1.1.tar", last modified: Thu Jun  8 06:41:27 2023, max compression
```

## Comparing `ohmic-0.1.0.tar` & `ohmic-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:04:47.580751 ohmic-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 13:04:05.000000 ohmic-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-07 13:04:47.580751 ohmic-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-07 13:04:05.000000 ohmic-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:04:47.580751 ohmic-0.1.0/ohmic/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-07 13:04:45.000000 ohmic-0.1.0/ohmic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:04:47.580751 ohmic-0.1.0/ohmic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-07 13:04:47.000000 ohmic-0.1.0/ohmic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-07 13:04:47.000000 ohmic-0.1.0/ohmic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:04:47.000000 ohmic-0.1.0/ohmic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:04:47.000000 ohmic-0.1.0/ohmic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 13:04:47.000000 ohmic-0.1.0/ohmic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 13:04:47.000000 ohmic-0.1.0/ohmic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 13:04:47.580751 ohmic-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-07 13:04:05.000000 ohmic-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:27.189990 ohmic-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 06:40:34.000000 ohmic-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 06:41:27.193990 ohmic-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 06:40:34.000000 ohmic-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:27.189990 ohmic-0.1.1/ohmic/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-08 06:40:34.000000 ohmic-0.1.1/ohmic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-08 06:41:26.000000 ohmic-0.1.1/ohmic/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:41:27.189990 ohmic-0.1.1/ohmic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 06:41:27.000000 ohmic-0.1.1/ohmic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 06:41:27.000000 ohmic-0.1.1/ohmic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:41:27.000000 ohmic-0.1.1/ohmic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:41:27.000000 ohmic-0.1.1/ohmic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 06:41:27.000000 ohmic-0.1.1/ohmic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 06:41:27.000000 ohmic-0.1.1/ohmic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-08 06:41:27.193990 ohmic-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 06:40:34.000000 ohmic-0.1.1/setup.py
```

### Comparing `ohmic-0.1.0/LICENSE` & `ohmic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmic-0.1.0/ohmic/__init__.py` & `ohmic-0.1.1/ohmic/__init__.py`

 * *Files identical despite different names*

