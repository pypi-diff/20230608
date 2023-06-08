# Comparing `tmp/cognica-0.1.7.tar.gz` & `tmp/cognica-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognica-0.1.7.tar", last modified: Thu Jun  8 09:22:48 2023, max compression
+gzip compressed data, was "cognica-0.1.8.tar", last modified: Thu Jun  8 09:27:06 2023, max compression
```

## Comparing `cognica-0.1.7.tar` & `cognica-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:22:48.232744 cognica-0.1.7/
--rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-29 03:56:50.000000 cognica-0.1.7/LICENSE
--rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-08 09:22:48.232582 cognica-0.1.7/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 05:58:03.000000 cognica-0.1.7/README.md
--rw-r--r--   0 jaepil     (501) staff       (20)     1282 2023-06-08 09:22:42.000000 cognica-0.1.7/pyproject.toml
--rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-08 09:22:48.232785 cognica-0.1.7/setup.cfg
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:22:48.228815 cognica-0.1.7/src/
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:22:48.230013 cognica-0.1.7/src/cognica/
--rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-15 08:05:25.000000 cognica-0.1.7/src/cognica/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-15 08:05:26.000000 cognica-0.1.7/src/cognica/channel.py
--rw-r--r--   0 jaepil     (501) staff       (20)    18849 2023-06-08 09:21:57.000000 cognica-0.1.7/src/cognica/document_db.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 03:46:32.000000 cognica-0.1.7/src/cognica/fts_analysis_pipeline.py
--rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 03:46:59.000000 cognica-0.1.7/src/cognica/key_value_db.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:22:48.232375 cognica-0.1.7/src/cognica/protobuf/
--rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-15 08:05:26.000000 cognica-0.1.7/src/cognica/protobuf/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)    15294 2023-06-08 06:20:57.000000 cognica-0.1.7/src/cognica/protobuf/document_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-03 01:34:57.000000 cognica-0.1.7/src/cognica/protobuf/document_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-06-03 01:33:38.000000 cognica-0.1.7/src/cognica/protobuf/document_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-03 01:33:38.000000 cognica-0.1.7/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-06-03 01:35:26.000000 cognica-0.1.7/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-03 01:33:38.000000 cognica-0.1.7/src/cognica/protobuf/key_value_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-06-03 01:35:45.000000 cognica-0.1.7/src/cognica/protobuf/key_value_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-03 01:33:38.000000 cognica-0.1.7/src/cognica/protobuf/sentence_transformer_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-06-03 01:36:10.000000 cognica-0.1.7/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 03:47:19.000000 cognica-0.1.7/src/cognica/sentence_transformer.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:22:48.230691 cognica-0.1.7/src/cognica.egg-info/
--rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-08 09:22:48.000000 cognica-0.1.7/src/cognica.egg-info/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)      831 2023-06-08 09:22:48.000000 cognica-0.1.7/src/cognica.egg-info/SOURCES.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-08 09:22:48.000000 cognica-0.1.7/src/cognica.egg-info/dependency_links.txt
--rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-08 09:22:48.000000 cognica-0.1.7/src/cognica.egg-info/requires.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-08 09:22:48.000000 cognica-0.1.7/src/cognica.egg-info/top_level.txt
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:27:06.015794 cognica-0.1.8/
+-rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-29 03:56:50.000000 cognica-0.1.8/LICENSE
+-rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-08 09:27:06.015606 cognica-0.1.8/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 05:58:03.000000 cognica-0.1.8/README.md
+-rw-r--r--   0 jaepil     (501) staff       (20)     1282 2023-06-08 09:26:58.000000 cognica-0.1.8/pyproject.toml
+-rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-08 09:27:06.015837 cognica-0.1.8/setup.cfg
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:27:06.011570 cognica-0.1.8/src/
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:27:06.012849 cognica-0.1.8/src/cognica/
+-rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-15 08:05:25.000000 cognica-0.1.8/src/cognica/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-15 08:05:26.000000 cognica-0.1.8/src/cognica/channel.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    18851 2023-06-08 09:26:29.000000 cognica-0.1.8/src/cognica/document_db.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 03:46:32.000000 cognica-0.1.8/src/cognica/fts_analysis_pipeline.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 03:46:59.000000 cognica-0.1.8/src/cognica/key_value_db.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:27:06.015375 cognica-0.1.8/src/cognica/protobuf/
+-rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-15 08:05:26.000000 cognica-0.1.8/src/cognica/protobuf/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    15294 2023-06-08 06:20:57.000000 cognica-0.1.8/src/cognica/protobuf/document_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-03 01:34:57.000000 cognica-0.1.8/src/cognica/protobuf/document_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-06-03 01:33:38.000000 cognica-0.1.8/src/cognica/protobuf/document_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-03 01:33:38.000000 cognica-0.1.8/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-06-03 01:35:26.000000 cognica-0.1.8/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-03 01:33:38.000000 cognica-0.1.8/src/cognica/protobuf/key_value_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-06-03 01:35:45.000000 cognica-0.1.8/src/cognica/protobuf/key_value_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-03 01:33:38.000000 cognica-0.1.8/src/cognica/protobuf/sentence_transformer_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-06-03 01:36:10.000000 cognica-0.1.8/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 03:47:19.000000 cognica-0.1.8/src/cognica/sentence_transformer.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:27:06.013595 cognica-0.1.8/src/cognica.egg-info/
+-rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-08 09:27:06.000000 cognica-0.1.8/src/cognica.egg-info/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)      831 2023-06-08 09:27:06.000000 cognica-0.1.8/src/cognica.egg-info/SOURCES.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-08 09:27:06.000000 cognica-0.1.8/src/cognica.egg-info/dependency_links.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-08 09:27:06.000000 cognica-0.1.8/src/cognica.egg-info/requires.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-08 09:27:06.000000 cognica-0.1.8/src/cognica.egg-info/top_level.txt
```

### Comparing `cognica-0.1.7/LICENSE` & `cognica-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/PKG-INFO` & `cognica-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python client for Cognica database
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cognica-0.1.7/README.md` & `cognica-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/pyproject.toml` & `cognica-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cognica"
-version = "0.1.7"
+version = "0.1.8"
 authors = [{ name = "Cognica, Inc.", email = "jaepil@cognica.io" }]
 description = "Python client for Cognica database"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
   "pandas>=1.5.3",
```

### Comparing `cognica-0.1.7/src/cognica/__init__.py` & `cognica-0.1.8/src/cognica/__init__.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/channel.py` & `cognica-0.1.8/src/cognica/channel.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/document_db.py` & `cognica-0.1.8/src/cognica/document_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
                 "added_at": resp_index_stats.added_at,
                 "updated_at": resp_index_stats.updated_at,
                 "deleted_at": resp_index_stats.deleted_at,
                 "merged_at": resp_index_stats.merged_at,
             }
 
             if resp_index_desc.index_type == IndexType.kFullTextSearchIndex:
-                resp_fts_stats = resp.collection.fts_stats
+                resp_fts_stats = resp_index_stats.fts_stats
                 fts_stats = {
                     "doc_count": resp_fts_stats.doc_count,
                     "doc_size": resp_fts_stats.doc_size,
                     "field_stats": [
                         {
                             "field_name": field_stats.field_name,
                             "total_doc_count": field_stats.total_doc_count,
@@ -430,15 +430,15 @@
             "accessed_at": resp.index_stats.accessed_at,
             "added_at": resp.index_stats.added_at,
             "updated_at": resp.index_stats.updated_at,
             "deleted_at": resp.index_stats.deleted_at,
             "merged_at": resp.index_stats.merged_at,
         }
         if resp.index_desc.index_type == IndexType.kFullTextSearchIndex:
-            resp_fts_stats = resp.collection.fts_stats
+            resp_fts_stats = resp.index_stats.fts_stats
             fts_stats = {
                 "doc_count": resp_fts_stats.doc_count,
                 "doc_size": resp_fts_stats.doc_size,
                 "field_stats": [
                     {
                         "field_name": field_stats.field_name,
                         "total_doc_count": field_stats.total_doc_count,
```

### Comparing `cognica-0.1.7/src/cognica/fts_analysis_pipeline.py` & `cognica-0.1.8/src/cognica/fts_analysis_pipeline.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/key_value_db.py` & `cognica-0.1.8/src/cognica/key_value_db.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/protobuf/document_db_pb2.py` & `cognica-0.1.8/src/cognica/protobuf/document_db_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/protobuf/document_db_pb2_grpc.py` & `cognica-0.1.8/src/cognica/protobuf/document_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/protobuf/document_pb2.py` & `cognica-0.1.8/src/cognica/protobuf/document_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/protobuf/fts_analysis_pipeline_pb2.py` & `cognica-0.1.8/src/cognica/protobuf/fts_analysis_pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py` & `cognica-0.1.8/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/protobuf/key_value_db_pb2.py` & `cognica-0.1.8/src/cognica/protobuf/key_value_db_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/protobuf/key_value_db_pb2_grpc.py` & `cognica-0.1.8/src/cognica/protobuf/key_value_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/protobuf/sentence_transformer_pb2.py` & `cognica-0.1.8/src/cognica/protobuf/sentence_transformer_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/protobuf/sentence_transformer_pb2_grpc.py` & `cognica-0.1.8/src/cognica/protobuf/sentence_transformer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica/sentence_transformer.py` & `cognica-0.1.8/src/cognica/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.7/src/cognica.egg-info/PKG-INFO` & `cognica-0.1.8/src/cognica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python client for Cognica database
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cognica-0.1.7/src/cognica.egg-info/SOURCES.txt` & `cognica-0.1.8/src/cognica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

