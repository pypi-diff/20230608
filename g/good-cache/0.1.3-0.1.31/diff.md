# Comparing `tmp/good_cache-0.1.3.tar.gz` & `tmp/good_cache-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "good_cache-0.1.3.tar", last modified: Thu Jun  8 02:09:31 2023, max compression
+gzip compressed data, was "good_cache-0.1.31.tar", last modified: Thu Jun  8 02:25:55 2023, max compression
```

## Comparing `good_cache-0.1.3.tar` & `good_cache-0.1.31.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:09:31.835906 good_cache-0.1.3/
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)    11357 2023-05-04 02:17:26.000000 good_cache-0.1.3/LICENSE
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      337 2023-06-08 02:09:31.835906 good_cache-0.1.3/PKG-INFO
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1204 2023-06-08 02:08:37.000000 good_cache-0.1.3/README.md
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       38 2023-06-08 02:09:31.835906 good_cache-0.1.3/setup.cfg
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      585 2023-06-08 02:09:25.000000 good_cache-0.1.3/setup.py
-drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:09:31.835906 good_cache-0.1.3/src/
-drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:09:31.835906 good_cache-0.1.3/src/good_cache.egg-info/
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      337 2023-06-08 02:09:31.000000 good_cache-0.1.3/src/good_cache.egg-info/PKG-INFO
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      215 2023-06-08 02:09:31.000000 good_cache-0.1.3/src/good_cache.egg-info/SOURCES.txt
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)        1 2023-06-08 02:09:31.000000 good_cache-0.1.3/src/good_cache.egg-info/dependency_links.txt
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       11 2023-06-08 02:09:31.000000 good_cache-0.1.3/src/good_cache.egg-info/requires.txt
--rw-rw-r--   0 asundaram  (1000) asundaram  (1000)        1 2023-06-08 02:09:31.000000 good_cache-0.1.3/src/good_cache.egg-info/top_level.txt
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:25:55.551959 good_cache-0.1.31/
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)    11357 2023-05-04 02:17:26.000000 good_cache-0.1.31/LICENSE
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1575 2023-06-08 02:25:55.551959 good_cache-0.1.31/PKG-INFO
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1204 2023-06-08 02:11:57.000000 good_cache-0.1.31/README.md
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       38 2023-06-08 02:25:55.551959 good_cache-0.1.31/setup.cfg
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      759 2023-06-08 02:20:59.000000 good_cache-0.1.31/setup.py
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:25:55.547959 good_cache-0.1.31/src/
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:25:55.551959 good_cache-0.1.31/src/good_cache/
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       48 2023-06-08 02:11:57.000000 good_cache-0.1.31/src/good_cache/__init__.py
+-rwxrwxr-x   0 asundaram  (1000) asundaram  (1000)     7901 2023-06-08 02:11:57.000000 good_cache-0.1.31/src/good_cache/cache.py
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1239 2023-05-04 02:17:26.000000 good_cache-0.1.31/src/good_cache/utils.py
+drwxrwxr-x   0 asundaram  (1000) asundaram  (1000)        0 2023-06-08 02:25:55.551959 good_cache-0.1.31/src/good_cache.egg-info/
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)     1575 2023-06-08 02:25:55.000000 good_cache-0.1.31/src/good_cache.egg-info/PKG-INFO
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)      290 2023-06-08 02:25:55.000000 good_cache-0.1.31/src/good_cache.egg-info/SOURCES.txt
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)        1 2023-06-08 02:25:55.000000 good_cache-0.1.31/src/good_cache.egg-info/dependency_links.txt
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       11 2023-06-08 02:25:55.000000 good_cache-0.1.31/src/good_cache.egg-info/requires.txt
+-rw-rw-r--   0 asundaram  (1000) asundaram  (1000)       11 2023-06-08 02:25:55.000000 good_cache-0.1.31/src/good_cache.egg-info/top_level.txt
```

### Comparing `good_cache-0.1.3/LICENSE` & `good_cache-0.1.31/LICENSE`

 * *Files identical despite different names*

### Comparing `good_cache-0.1.3/README.md` & `good_cache-0.1.31/README.md`

 * *Files identical despite different names*

