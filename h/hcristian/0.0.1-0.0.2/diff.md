# Comparing `tmp/hcristian-0.0.1.tar.gz` & `tmp/hcristian-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcristian-0.0.1.tar", last modified: Thu Jun  8 06:16:05 2023, max compression
+gzip compressed data, was "hcristian-0.0.2.tar", last modified: Thu Jun  8 07:06:26 2023, max compression
```

## Comparing `hcristian-0.0.1.tar` & `hcristian-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-06-08 06:16:05.146764 hcristian-0.0.1/
--rw-rw-r--   0 cristian  (1000) cristian  (1000)      168 2023-06-08 06:16:05.146764 hcristian-0.0.1/PKG-INFO
--rw-rw-r--   0 cristian  (1000) cristian  (1000)       45 2023-06-07 05:42:18.000000 hcristian-0.0.1/README.md
--rw-rw-r--   0 cristian  (1000) cristian  (1000)       90 2023-06-03 13:34:11.000000 hcristian-0.0.1/pyproject.toml
--rw-rw-r--   0 cristian  (1000) cristian  (1000)      928 2023-06-08 06:16:05.146764 hcristian-0.0.1/setup.cfg
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-06-08 06:16:05.146764 hcristian-0.0.1/src/
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-06-08 06:16:05.146764 hcristian-0.0.1/src/hcristian/
--rw-rw-r--   0 cristian  (1000) cristian  (1000)        0 2023-06-03 13:55:59.000000 hcristian-0.0.1/src/hcristian/__init__.py
--rw-rw-r--   0 cristian  (1000) cristian  (1000)      638 2023-06-08 06:15:19.000000 hcristian-0.0.1/src/hcristian/main.py
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-06-08 06:16:05.146764 hcristian-0.0.1/src/hcristian.egg-info/
--rw-rw-r--   0 cristian  (1000) cristian  (1000)      168 2023-06-08 06:16:05.000000 hcristian-0.0.1/src/hcristian.egg-info/PKG-INFO
--rw-rw-r--   0 cristian  (1000) cristian  (1000)      322 2023-06-08 06:16:05.000000 hcristian-0.0.1/src/hcristian.egg-info/SOURCES.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)        1 2023-06-08 06:16:05.000000 hcristian-0.0.1/src/hcristian.egg-info/dependency_links.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)       52 2023-06-08 06:16:05.000000 hcristian-0.0.1/src/hcristian.egg-info/entry_points.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)       11 2023-06-08 06:16:05.000000 hcristian-0.0.1/src/hcristian.egg-info/requires.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)       10 2023-06-08 06:16:05.000000 hcristian-0.0.1/src/hcristian.egg-info/top_level.txt
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-06-08 06:16:05.146764 hcristian-0.0.1/test/
--rw-rw-r--   0 cristian  (1000) cristian  (1000)     1325 2023-06-08 06:14:59.000000 hcristian-0.0.1/test/test_hc.py
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-06-08 07:06:26.506984 hcristian-0.0.2/
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)      201 2023-06-08 07:06:26.506984 hcristian-0.0.2/PKG-INFO
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)       78 2023-06-08 07:05:50.000000 hcristian-0.0.2/README.md
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)       90 2023-06-03 13:34:11.000000 hcristian-0.0.2/pyproject.toml
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)      928 2023-06-08 07:06:26.506984 hcristian-0.0.2/setup.cfg
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-06-08 07:06:26.502984 hcristian-0.0.2/src/
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-06-08 07:06:26.502984 hcristian-0.0.2/src/hcristian/
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)        0 2023-06-03 13:55:59.000000 hcristian-0.0.2/src/hcristian/__init__.py
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)      638 2023-06-08 06:15:19.000000 hcristian-0.0.2/src/hcristian/main.py
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-06-08 07:06:26.506984 hcristian-0.0.2/src/hcristian.egg-info/
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)      201 2023-06-08 07:06:26.000000 hcristian-0.0.2/src/hcristian.egg-info/PKG-INFO
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)      322 2023-06-08 07:06:26.000000 hcristian-0.0.2/src/hcristian.egg-info/SOURCES.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)        1 2023-06-08 07:06:26.000000 hcristian-0.0.2/src/hcristian.egg-info/dependency_links.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)       52 2023-06-08 07:06:26.000000 hcristian-0.0.2/src/hcristian.egg-info/entry_points.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)       11 2023-06-08 07:06:26.000000 hcristian-0.0.2/src/hcristian.egg-info/requires.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)       10 2023-06-08 07:06:26.000000 hcristian-0.0.2/src/hcristian.egg-info/top_level.txt
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-06-08 07:06:26.506984 hcristian-0.0.2/test/
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)     1325 2023-06-08 06:14:59.000000 hcristian-0.0.2/test/test_hc.py
```

### Comparing `hcristian-0.0.1/setup.cfg` & `hcristian-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hcristian
-version = 0.0.1
+version = 0.0.2
 description = Juniper checks
 long_description = file: README.md
 author = CB
 author_email = "CB" <cb@gmail.com>
 
 [options]
 package_dir =
```

### Comparing `hcristian-0.0.1/src/hcristian/main.py` & `hcristian-0.0.2/src/hcristian/main.py`

 * *Files identical despite different names*

### Comparing `hcristian-0.0.1/test/test_hc.py` & `hcristian-0.0.2/test/test_hc.py`

 * *Files identical despite different names*

