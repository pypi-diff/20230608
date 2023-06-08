# Comparing `tmp/kwenta-1.0.3.tar.gz` & `tmp/kwenta-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kwenta-1.0.3.tar", last modified: Thu May 18 20:26:03 2023, max compression
+gzip compressed data, was "kwenta-1.0.4.tar", last modified: Thu Jun  8 13:40:02 2023, max compression
```

## Comparing `kwenta-1.0.3.tar` & `kwenta-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:26:03.035464 kwenta-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-18 20:26:03.035464 kwenta-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:26:03.031464 kwenta-1.0.3/kwenta/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 20:25:29.000000 kwenta-1.0.3/kwenta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-18 20:25:29.000000 kwenta-1.0.3/kwenta/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    43018 2023-05-18 20:25:29.000000 kwenta-1.0.3/kwenta/kwenta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 20:26:03.035464 kwenta-1.0.3/kwenta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-18 20:26:03.000000 kwenta-1.0.3/kwenta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 20:26:03.035464 kwenta-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-18 20:25:29.000000 kwenta-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:40:02.173539 kwenta-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 13:40:02.173539 kwenta-1.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:40:02.169539 kwenta-1.0.4/kwenta/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:40:02.169539 kwenta-1.0.4/kwenta/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/alerts/alerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:40:02.169539 kwenta-1.0.4/kwenta/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/cli/kwenta_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:40:02.169539 kwenta-1.0.4/kwenta/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/contracts/contracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:40:02.169539 kwenta-1.0.4/kwenta/contracts/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/contracts/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43018 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/kwenta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:40:02.173539 kwenta-1.0.4/kwenta/pyth/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/pyth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/pyth/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/pyth/pyth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:40:02.173539 kwenta-1.0.4/kwenta/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/queries/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/queries/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-08 13:39:23.000000 kwenta-1.0.4/kwenta/queries/queries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:40:02.169539 kwenta-1.0.4/kwenta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-08 13:40:02.000000 kwenta-1.0.4/kwenta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-08 13:40:02.000000 kwenta-1.0.4/kwenta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:40:02.000000 kwenta-1.0.4/kwenta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 13:40:02.000000 kwenta-1.0.4/kwenta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:40:02.000000 kwenta-1.0.4/kwenta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 13:40:02.000000 kwenta-1.0.4/kwenta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:40:02.173539 kwenta-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-08 13:39:23.000000 kwenta-1.0.4/setup.py
```

### Comparing `kwenta-1.0.3/PKG-INFO` & `kwenta-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `kwenta-1.0.3/kwenta/constants.py` & `kwenta-1.0.4/kwenta/constants.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.3/kwenta/kwenta.py` & `kwenta-1.0.4/kwenta/kwenta.py`

 * *Files identical despite different names*

### Comparing `kwenta-1.0.3/kwenta.egg-info/PKG-INFO` & `kwenta-1.0.4/kwenta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kwenta
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python SDK for Kwenta
 Author: Kwenta DAO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

