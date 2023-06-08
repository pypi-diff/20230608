# Comparing `tmp/batch_processing_discovery-0.4.1.tar.gz` & `tmp/batch_processing_discovery-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch_processing_discovery-0.4.1.tar", max compression
+gzip compressed data, was "batch_processing_discovery-0.4.2.tar", max compression
```

## Comparing `batch_processing_discovery-0.4.1.tar` & `batch_processing_discovery-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11349 2023-06-08 14:47:13.622473 batch_processing_discovery-0.4.1/LICENSE
--rw-r--r--   0        0        0     4075 2023-06-08 14:49:47.933374 batch_processing_discovery-0.4.1/README.md
--rw-r--r--   0        0        0      648 2023-06-08 14:53:16.332857 batch_processing_discovery-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       59 2023-06-08 14:47:13.622912 batch_processing_discovery-0.4.1/src/batch_processing_discovery/__init__.py
--rw-r--r--   0        0        0     8792 2023-06-08 14:47:13.623045 batch_processing_discovery-0.4.1/src/batch_processing_discovery/batch_characteristics.py
--rw-r--r--   0        0        0     2264 2023-06-08 14:47:13.623199 batch_processing_discovery-0.4.1/src/batch_processing_discovery/config.py
--rw-r--r--   0        0        0     5618 2023-06-08 14:47:13.623282 batch_processing_discovery-0.4.1/src/batch_processing_discovery/discovery.py
--rw-r--r--   0        0        0     6681 2023-06-08 14:47:13.623393 batch_processing_discovery-0.4.1/src/batch_processing_discovery/features_table.py
--rw-r--r--   0        0        0     4876 2023-06-08 14:47:13.623476 batch_processing_discovery-0.4.1/src/batch_processing_discovery/rules.py
--rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 batch_processing_discovery-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/LICENSE
+-rw-r--r--   0        0        0     4075 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/README.md
+-rw-r--r--   0        0        0      648 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/__init__.py
+-rw-r--r--   0        0        0     8792 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/batch_characteristics.py
+-rw-r--r--   0        0        0     2264 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/config.py
+-rw-r--r--   0        0        0     5618 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/discovery.py
+-rw-r--r--   0        0        0     6681 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/features_table.py
+-rw-r--r--   0        0        0     4876 2023-06-08 14:56:03.158977 batch_processing_discovery-0.4.2/src/batch_processing_discovery/rules.py
+-rw-r--r--   0        0        0     4689 1970-01-01 00:00:00.000000 batch_processing_discovery-0.4.2/PKG-INFO
```

### Comparing `batch_processing_discovery-0.4.1/LICENSE` & `batch_processing_discovery-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.1/README.md` & `batch_processing_discovery-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.1/pyproject.toml` & `batch_processing_discovery-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "batch-processing-discovery"
-version = "0.4.1"
+version = "0.4.2"
 description = "Python algorithm to discover, from an event log, activity instances that are executed in a batch."
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "batch_processing_discovery", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `batch_processing_discovery-0.4.1/src/batch_processing_discovery/batch_characteristics.py` & `batch_processing_discovery-0.4.2/src/batch_processing_discovery/batch_characteristics.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.1/src/batch_processing_discovery/config.py` & `batch_processing_discovery-0.4.2/src/batch_processing_discovery/config.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.1/src/batch_processing_discovery/discovery.py` & `batch_processing_discovery-0.4.2/src/batch_processing_discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.1/src/batch_processing_discovery/features_table.py` & `batch_processing_discovery-0.4.2/src/batch_processing_discovery/features_table.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.1/src/batch_processing_discovery/rules.py` & `batch_processing_discovery-0.4.2/src/batch_processing_discovery/rules.py`

 * *Files identical despite different names*

### Comparing `batch_processing_discovery-0.4.1/PKG-INFO` & `batch_processing_discovery-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batch-processing-discovery
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python algorithm to discover, from an event log, activity instances that are executed in a batch.
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

