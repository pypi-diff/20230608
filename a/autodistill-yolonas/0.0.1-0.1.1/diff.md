# Comparing `tmp/autodistill-yolonas-0.0.1.tar.gz` & `tmp/autodistill-yolonas-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-yolonas-0.0.1.tar", last modified: Wed Jun  7 11:06:54 2023, max compression
+gzip compressed data, was "autodistill-yolonas-0.1.1.tar", last modified: Thu Jun  8 14:05:23 2023, max compression
```

## Comparing `autodistill-yolonas-0.0.1.tar` & `autodistill-yolonas-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:54.676424 autodistill-yolonas-0.0.1/
--rw-r--r--   0 james      (501) staff       (20)      365 2023-06-07 11:06:54.676298 autodistill-yolonas-0.0.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)       20 2023-06-07 11:06:52.000000 autodistill-yolonas-0.0.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:54.675296 autodistill-yolonas-0.0.1/autodistill_yolonas/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-07 11:06:52.000000 autodistill-yolonas-0.0.1/autodistill_yolonas/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 11:06:54.676101 autodistill-yolonas-0.0.1/autodistill_yolonas.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      365 2023-06-07 11:06:54.000000 autodistill-yolonas-0.0.1/autodistill_yolonas.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      264 2023-06-07 11:06:54.000000 autodistill-yolonas-0.0.1/autodistill_yolonas.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 11:06:54.000000 autodistill-yolonas-0.0.1/autodistill_yolonas.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       53 2023-06-07 11:06:54.000000 autodistill-yolonas-0.0.1/autodistill_yolonas.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       20 2023-06-07 11:06:54.000000 autodistill-yolonas-0.0.1/autodistill_yolonas.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 11:06:54.676465 autodistill-yolonas-0.0.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)      983 2023-06-07 11:06:52.000000 autodistill-yolonas-0.0.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 14:05:23.730632 autodistill-yolonas-0.1.1/
+-rw-r--r--   0 james      (501) staff       (20)     2217 2023-06-08 09:29:55.000000 autodistill-yolonas-0.1.1/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2298 2023-06-08 14:05:23.730490 autodistill-yolonas-0.1.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1818 2023-06-08 09:30:19.000000 autodistill-yolonas-0.1.1/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 14:05:23.729577 autodistill-yolonas-0.1.1/autodistill_yolonas/
+-rw-r--r--   0 james      (501) staff       (20)       77 2023-06-08 14:05:13.000000 autodistill-yolonas-0.1.1/autodistill_yolonas/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     5126 2023-06-08 09:28:45.000000 autodistill-yolonas-0.1.1/autodistill_yolonas/yolonas_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 14:05:23.730312 autodistill-yolonas-0.1.1/autodistill_yolonas.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2298 2023-06-08 14:05:23.000000 autodistill-yolonas-0.1.1/autodistill_yolonas.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      309 2023-06-08 14:05:23.000000 autodistill-yolonas-0.1.1/autodistill_yolonas.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-08 14:05:23.000000 autodistill-yolonas-0.1.1/autodistill_yolonas.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      105 2023-06-08 14:05:23.000000 autodistill-yolonas-0.1.1/autodistill_yolonas.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       20 2023-06-08 14:05:23.000000 autodistill-yolonas-0.1.1/autodistill_yolonas.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-08 14:05:23.730677 autodistill-yolonas-0.1.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1142 2023-06-08 14:05:07.000000 autodistill-yolonas-0.1.1/setup.py
```

