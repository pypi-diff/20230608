# Comparing `tmp/py-data-mock-0.0.6.tar.gz` & `tmp/py-data-mock-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-data-mock-0.0.6.tar", last modified: Tue Jun  6 23:19:32 2023, max compression
+gzip compressed data, was "py-data-mock-0.0.7.tar", last modified: Thu Jun  8 05:48:22 2023, max compression
```

## Comparing `py-data-mock-0.0.6.tar` & `py-data-mock-0.0.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.688691 py-data-mock-0.0.6/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.680691 py-data-mock-0.0.6/data_mock/
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/__init__.py
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.680691 py-data-mock-0.0.6/data_mock/google/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.680691 py-data-mock-0.0.6/data_mock/google/cloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/
--rw-r--r--   0 root         (0) root         (0)      827 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6323 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/client.py
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/dataset.py
--rw-r--r--   0 root         (0) root         (0)     1427 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/enums.py
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/job/
--rw-r--r--   0 root         (0) root         (0)      329 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/job/load.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/job/query.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/retry.py
--rw-r--r--   0 root         (0) root         (0)      865 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/schema.py
--rw-r--r--   0 root         (0) root         (0)     3013 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/bigquery/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/data_mock/google/cloud/storage/
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/storage/blob.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/storage/bucket.py
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/google/cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/data_mock/mock_helpers/
--rw-r--r--   0 root         (0) root         (0)     8025 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/mock_helpers/generate_data.py
--rw-r--r--   0 root         (0) root         (0)     2238 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/mock_helpers/provider.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/mock_helpers/writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/data_mock/psycopg2/
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/psycopg2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4979 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/psycopg2/connect.py
--rw-r--r--   0 root         (0) root         (0)     5282 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/psycopg2/cursor.py
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/psycopg2/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/data_mock/psycopg2/extras.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 23:19:32.684691 py-data-mock-0.0.6/py_data_mock.egg-info/
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 23:19:32.000000 py-data-mock-0.0.6/py_data_mock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1117 2023-06-06 23:19:32.000000 py-data-mock-0.0.6/py_data_mock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 23:19:32.000000 py-data-mock-0.0.6/py_data_mock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-06 23:19:32.000000 py-data-mock-0.0.6/py_data_mock.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 23:19:32.688691 py-data-mock-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      635 2023-06-06 23:19:08.000000 py-data-mock-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.678570 py-data-mock-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-08 05:48:22.678570 py-data-mock-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.670570 py-data-mock-0.0.7/data_mock/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.670570 py-data-mock-0.0.7/data_mock/google/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.670570 py-data-mock-0.0.7/data_mock/google/cloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.674570 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/
+-rw-r--r--   0 root         (0) root         (0)      827 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6323 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/client.py
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1427 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/enums.py
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.674570 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/job/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/job/load.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/job/query.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/retry.py
+-rw-r--r--   0 root         (0) root         (0)      865 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/schema.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/bigquery/table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.674570 py-data-mock-0.0.7/data_mock/google/cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/storage/blob.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/storage/bucket.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/google/cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.674570 py-data-mock-0.0.7/data_mock/mock_helpers/
+-rw-r--r--   0 root         (0) root         (0)     8025 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/mock_helpers/generate_data.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/mock_helpers/provider.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/mock_helpers/writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.678570 py-data-mock-0.0.7/data_mock/psycopg2/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/psycopg2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4979 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/psycopg2/connect.py
+-rw-r--r--   0 root         (0) root         (0)     5282 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/psycopg2/cursor.py
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/psycopg2/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/data_mock/psycopg2/extras.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 05:48:22.678570 py-data-mock-0.0.7/py_data_mock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-08 05:48:22.000000 py-data-mock-0.0.7/py_data_mock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-06-08 05:48:22.000000 py-data-mock-0.0.7/py_data_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 05:48:22.000000 py-data-mock-0.0.7/py_data_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-08 05:48:22.000000 py-data-mock-0.0.7/py_data_mock.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 05:48:22.678570 py-data-mock-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      635 2023-06-08 05:47:59.000000 py-data-mock-0.0.7/setup.py
```

### Comparing `py-data-mock-0.0.6/LICENSE` & `py-data-mock-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/README.md` & `py-data-mock-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/data_mock/google/cloud/bigquery/__init__.py` & `py-data-mock-0.0.7/data_mock/google/cloud/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/data_mock/google/cloud/bigquery/client.py` & `py-data-mock-0.0.7/data_mock/google/cloud/bigquery/client.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/data_mock/google/cloud/bigquery/enums.py` & `py-data-mock-0.0.7/data_mock/google/cloud/bigquery/enums.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/data_mock/google/cloud/bigquery/schema.py` & `py-data-mock-0.0.7/data_mock/google/cloud/bigquery/schema.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/data_mock/google/cloud/bigquery/table.py` & `py-data-mock-0.0.7/data_mock/google/cloud/bigquery/table.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/data_mock/google/cloud/storage/blob.py` & `py-data-mock-0.0.7/data_mock/google/cloud/storage/blob.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/data_mock/google/cloud/storage/bucket.py` & `py-data-mock-0.0.7/data_mock/google/cloud/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/data_mock/mock_helpers/generate_data.py` & `py-data-mock-0.0.7/data_mock/mock_helpers/generate_data.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/data_mock/mock_helpers/provider.py` & `py-data-mock-0.0.7/data_mock/mock_helpers/provider.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 import types
 from typing import Union, List
 import data_mock.exceptions
 from data_mock.google.cloud import bigquery
 #from bigquery import SchemaField
 import types
 
+class EmptyGenerator:
+
+    def __init__(self):
+        self.metadata = {}
+
+    def gen_func(self):
+        for i in range(0):
+            yield i
+
+    def query_results(self):
+        return self.gen_func(), {'total_rows':0, 'schema' : None}
+
 class QueryResultsFromList:
 
     def __init__(self, data):
         self.data = data
         self.make_schema()
 
     def make_schema(self):
+        if len(self.data) == 0:
+            self.schema = None
+            return
         schema = []
         for i in self.data[0]:
             schema.append(bigquery.SchemaField(name = i[0], field_type = type(i[1])))
         self.schema = schema
 
     def gen_func(self):
         for i in self.data:
```

### Comparing `py-data-mock-0.0.6/data_mock/psycopg2/connect.py` & `py-data-mock-0.0.7/data_mock/psycopg2/connect.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/data_mock/psycopg2/cursor.py` & `py-data-mock-0.0.7/data_mock/psycopg2/cursor.py`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/py_data_mock.egg-info/SOURCES.txt` & `py-data-mock-0.0.7/py_data_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-data-mock-0.0.6/setup.py` & `py-data-mock-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='py-data-mock',
-    version='0.0.6',    
+    version='0.0.7',    
     description='Mock Data',
     url='https://github.com/paulhtremblay/py-data-mock',
     author='Henry Tremblay',
     author_email='paulhtremblay@gmail.com',
     license='GNU GENERAL PUBLIC LICENSE',
     packages=['data_mock/google/cloud/bigquery/job', 'data_mock/google/cloud/bigquery',
         'data_mock/google/cloud/storage','data_mock/mock_helpers', 'data_mock',
```

