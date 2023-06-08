# Comparing `tmp/cognica-0.1.6.tar.gz` & `tmp/cognica-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognica-0.1.6.tar", last modified: Thu Jun  8 05:49:19 2023, max compression
+gzip compressed data, was "cognica-0.1.7.tar", last modified: Thu Jun  8 09:22:48 2023, max compression
```

## Comparing `cognica-0.1.6.tar` & `cognica-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 05:49:19.567047 cognica-0.1.6/
--rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-31 12:58:01.000000 cognica-0.1.6/LICENSE
--rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-08 05:49:19.566854 cognica-0.1.6/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 12:36:07.000000 cognica-0.1.6/README.md
--rw-r--r--   0 jaepil     (501) staff       (20)     1282 2023-06-08 05:47:20.000000 cognica-0.1.6/pyproject.toml
--rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-08 05:49:19.567088 cognica-0.1.6/setup.cfg
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 05:49:19.557807 cognica-0.1.6/src/
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 05:49:19.559634 cognica-0.1.6/src/cognica/
--rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/channel.py
--rw-r--r--   0 jaepil     (501) staff       (20)    17063 2023-06-07 12:02:01.000000 cognica-0.1.6/src/cognica/document_db.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/fts_analysis_pipeline.py
--rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/key_value_db.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 05:49:19.564493 cognica-0.1.6/src/cognica/protobuf/
--rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/protobuf/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)    15294 2023-06-08 05:46:47.000000 cognica-0.1.6/src/cognica/protobuf/document_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-08 05:46:39.000000 cognica-0.1.6/src/cognica/protobuf/document_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-03-31 12:58:01.000000 cognica-0.1.6/src/cognica/protobuf/document_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-06 15:38:54.000000 cognica-0.1.6/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-03-31 12:58:01.000000 cognica-0.1.6/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-06 15:38:54.000000 cognica-0.1.6/src/cognica/protobuf/key_value_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-03-31 12:58:01.000000 cognica-0.1.6/src/cognica/protobuf/key_value_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-06 15:38:54.000000 cognica-0.1.6/src/cognica/protobuf/sentence_transformer_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-03-31 12:58:01.000000 cognica-0.1.6/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/sentence_transformer.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 05:49:19.560386 cognica-0.1.6/src/cognica.egg-info/
--rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-08 05:49:19.000000 cognica-0.1.6/src/cognica.egg-info/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)      831 2023-06-08 05:49:19.000000 cognica-0.1.6/src/cognica.egg-info/SOURCES.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-08 05:49:19.000000 cognica-0.1.6/src/cognica.egg-info/dependency_links.txt
--rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-08 05:49:19.000000 cognica-0.1.6/src/cognica.egg-info/requires.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-08 05:49:19.000000 cognica-0.1.6/src/cognica.egg-info/top_level.txt
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:22:48.232744 cognica-0.1.7/
+-rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-29 03:56:50.000000 cognica-0.1.7/LICENSE
+-rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-08 09:22:48.232582 cognica-0.1.7/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 05:58:03.000000 cognica-0.1.7/README.md
+-rw-r--r--   0 jaepil     (501) staff       (20)     1282 2023-06-08 09:22:42.000000 cognica-0.1.7/pyproject.toml
+-rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-08 09:22:48.232785 cognica-0.1.7/setup.cfg
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:22:48.228815 cognica-0.1.7/src/
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:22:48.230013 cognica-0.1.7/src/cognica/
+-rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-15 08:05:25.000000 cognica-0.1.7/src/cognica/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-15 08:05:26.000000 cognica-0.1.7/src/cognica/channel.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    18849 2023-06-08 09:21:57.000000 cognica-0.1.7/src/cognica/document_db.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 03:46:32.000000 cognica-0.1.7/src/cognica/fts_analysis_pipeline.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 03:46:59.000000 cognica-0.1.7/src/cognica/key_value_db.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:22:48.232375 cognica-0.1.7/src/cognica/protobuf/
+-rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-15 08:05:26.000000 cognica-0.1.7/src/cognica/protobuf/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    15294 2023-06-08 06:20:57.000000 cognica-0.1.7/src/cognica/protobuf/document_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-03 01:34:57.000000 cognica-0.1.7/src/cognica/protobuf/document_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-06-03 01:33:38.000000 cognica-0.1.7/src/cognica/protobuf/document_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-03 01:33:38.000000 cognica-0.1.7/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-06-03 01:35:26.000000 cognica-0.1.7/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-03 01:33:38.000000 cognica-0.1.7/src/cognica/protobuf/key_value_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-06-03 01:35:45.000000 cognica-0.1.7/src/cognica/protobuf/key_value_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-03 01:33:38.000000 cognica-0.1.7/src/cognica/protobuf/sentence_transformer_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-06-03 01:36:10.000000 cognica-0.1.7/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 03:47:19.000000 cognica-0.1.7/src/cognica/sentence_transformer.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 09:22:48.230691 cognica-0.1.7/src/cognica.egg-info/
+-rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-08 09:22:48.000000 cognica-0.1.7/src/cognica.egg-info/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)      831 2023-06-08 09:22:48.000000 cognica-0.1.7/src/cognica.egg-info/SOURCES.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-08 09:22:48.000000 cognica-0.1.7/src/cognica.egg-info/dependency_links.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-08 09:22:48.000000 cognica-0.1.7/src/cognica.egg-info/requires.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-08 09:22:48.000000 cognica-0.1.7/src/cognica.egg-info/top_level.txt
```

### Comparing `cognica-0.1.6/LICENSE` & `cognica-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/PKG-INFO` & `cognica-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python client for Cognica database
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cognica-0.1.6/README.md` & `cognica-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/pyproject.toml` & `cognica-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cognica"
-version = "0.1.6"
+version = "0.1.7"
 authors = [{ name = "Cognica, Inc.", email = "jaepil@cognica.io" }]
 description = "Python client for Cognica database"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
   "pandas>=1.5.3",
```

### Comparing `cognica-0.1.6/src/cognica/__init__.py` & `cognica-0.1.7/src/cognica/__init__.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/channel.py` & `cognica-0.1.7/src/cognica/channel.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/document_db.py` & `cognica-0.1.7/src/cognica/document_db.py`

 * *Files 14% similar despite different names*

```diff
@@ -288,53 +288,78 @@
 
     def get_collection(self, collection) -> t.Dict[str, t.Any]:
         req = GetCollectionRequest(collection_name=collection)
         resp: GetCollectionResponse = self._invoke(
             self._stub.get_collection, req, wait_for_ready=True
         )
 
+        index_desc_list = []
+        for resp_index_desc in resp.collection.index_descriptors:
+            index_desc = {
+                "index_id": resp_index_desc.index_id,
+                "index_name": resp_index_desc.index_name,
+                "fields": list(resp_index_desc.fields),
+                "unique": resp_index_desc.unique,
+                "index_type": IndexType.Name(resp_index_desc.index_type),
+                "status": IndexStatus.Name(resp_index_desc.status),
+                "options": json.loads(resp_index_desc.options.json or "{}"),
+            }
+            index_desc_list.append(index_desc)
+
+        index_stats_list = []
+        for index, resp_index_desc in enumerate(
+            resp.collection.index_descriptors
+        ):
+            resp_index_stats = resp.collection.index_stats[index]
+            index_stats = {
+                "index_id": resp_index_stats.index_id,
+                "index_name": resp_index_stats.index_name,
+                "approximated_size": resp_index_stats.approximated_size,
+                "num_docs": resp_index_stats.num_docs,
+                "accessed": resp_index_stats.accessed,
+                "added": resp_index_stats.added,
+                "updated": resp_index_stats.updated,
+                "deleted": resp_index_stats.deleted,
+                "merged": resp_index_stats.merged,
+                "accessed_at": resp_index_stats.accessed_at,
+                "added_at": resp_index_stats.added_at,
+                "updated_at": resp_index_stats.updated_at,
+                "deleted_at": resp_index_stats.deleted_at,
+                "merged_at": resp_index_stats.merged_at,
+            }
+
+            if resp_index_desc.index_type == IndexType.kFullTextSearchIndex:
+                resp_fts_stats = resp.collection.fts_stats
+                fts_stats = {
+                    "doc_count": resp_fts_stats.doc_count,
+                    "doc_size": resp_fts_stats.doc_size,
+                    "field_stats": [
+                        {
+                            "field_name": field_stats.field_name,
+                            "total_doc_count": field_stats.total_doc_count,
+                            "total_doc_size": field_stats.total_doc_size,
+                            "doc_count": field_stats.doc_count,
+                            "doc_size": field_stats.doc_size,
+                            "sum_term_freq": field_stats.sum_term_freq,
+                            "sum_doc_freq": field_stats.sum_doc_freq,
+                        }
+                        for field_stats in resp_fts_stats.field_stats
+                    ],
+                }
+                index_stats["fts_stats"] = fts_stats
+            index_stats_list.append(index_stats)
+
         return {
             "success": resp.status == 0,
             "message": resp.message,
             "data": [
                 {
                     "collection_name": resp.collection.collection_name,
-                    "index_descriptors": [
-                        {
-                            "index_id": index_desc.index_id,
-                            "index_name": index_desc.index_name,
-                            "fields": list(index_desc.fields),
-                            "unique": index_desc.unique,
-                            "index_type": IndexType.Name(index_desc.index_type),
-                            "status": IndexStatus.Name(index_desc.status),
-                            "options": json.loads(
-                                index_desc.options.json or "{}"
-                            ),
-                        }
-                        for index_desc in resp.collection.index_descriptors
-                    ],
-                    "index_stats": [
-                        {
-                            "index_id": index_stats.index_id,
-                            "index_name": index_stats.index_name,
-                            "approximated_size": index_stats.approximated_size,
-                            "num_docs": index_stats.num_docs,
-                            "accessed": index_stats.accessed,
-                            "added": index_stats.added,
-                            "updated": index_stats.updated,
-                            "deleted": index_stats.deleted,
-                            "merged": index_stats.merged,
-                            "accessed_at": index_stats.accessed_at,
-                            "added_at": index_stats.added_at,
-                            "updated_at": index_stats.updated_at,
-                            "deleted_at": index_stats.deleted_at,
-                            "merged_at": index_stats.merged_at,
-                        }
-                        for index_stats in resp.collection.index_stats
-                    ],
+                    "index_descriptors": index_desc_list,
+                    "index_stats": index_stats_list,
                 }
             ],
         }
 
     def list_collections(self) -> t.List[str]:
         req = ListCollectionsRequest()
 
@@ -378,48 +403,68 @@
         self._invoke(self._stub.drop_index, req, wait_for_ready=True)
 
     def get_index(self, collection, index_name) -> t.Dict[str, t.Any]:
         req = GetIndexRequest(collection_name=collection, index_name=index_name)
         resp: GetIndexResponse = self._invoke(
             self._stub.get_index, req, wait_for_ready=True
         )
-        index_desc = resp.index_desc
-        index_stats = resp.index_stats
+
+        index_desc = {
+            "index_id": resp.index_desc.index_id,
+            "index_name": resp.index_desc.index_name,
+            "fields": list(resp.index_desc.fields),
+            "unique": resp.index_desc.unique,
+            "index_type": IndexType.Name(resp.index_desc.index_type),
+            "status": IndexStatus.Name(resp.index_desc.status),
+            "options": json.loads(resp.index_desc.options.json or "{}"),
+        }
+        index_stats = {
+            "index_id": resp.index_stats.index_id,
+            "index_name": resp.index_stats.index_name,
+            "approximated_size": resp.index_stats.approximated_size,
+            "num_docs": resp.index_stats.num_docs,
+            "accessed": resp.index_stats.accessed,
+            "added": resp.index_stats.added,
+            "updated": resp.index_stats.updated,
+            "deleted": resp.index_stats.deleted,
+            "merged": resp.index_stats.merged,
+            "accessed_at": resp.index_stats.accessed_at,
+            "added_at": resp.index_stats.added_at,
+            "updated_at": resp.index_stats.updated_at,
+            "deleted_at": resp.index_stats.deleted_at,
+            "merged_at": resp.index_stats.merged_at,
+        }
+        if resp.index_desc.index_type == IndexType.kFullTextSearchIndex:
+            resp_fts_stats = resp.collection.fts_stats
+            fts_stats = {
+                "doc_count": resp_fts_stats.doc_count,
+                "doc_size": resp_fts_stats.doc_size,
+                "field_stats": [
+                    {
+                        "field_name": field_stats.field_name,
+                        "total_doc_count": field_stats.total_doc_count,
+                        "total_doc_size": field_stats.total_doc_size,
+                        "doc_count": field_stats.doc_count,
+                        "doc_size": field_stats.doc_size,
+                        "sum_term_freq": field_stats.sum_term_freq,
+                        "sum_doc_freq": field_stats.sum_doc_freq,
+                    }
+                    for field_stats in resp_fts_stats.field_stats
+                ],
+            }
+            index_stats["fts_stats"] = fts_stats
 
         return {
             "success": resp.status == 0,
             "message": resp.message,
             "data": [
                 {
                     "collection_name": resp.collection_name,
-                    "index_descriptor": {
-                        "index_id": index_desc.index_id,
-                        "index_name": index_desc.index_name,
-                        "fields": list(index_desc.fields),
-                        "unique": index_desc.unique,
-                        "index_type": IndexType.Name(index_desc.index_type),
-                        "status": IndexStatus.Name(index_desc.status),
-                        "options": json.loads(index_desc.options.json or "{}"),
-                    },
-                    "index_stats": {
-                        "index_id": index_stats.index_id,
-                        "index_name": index_stats.index_name,
-                        "approximated_size": index_stats.approximated_size,
-                        "num_docs": index_stats.num_docs,
-                        "accessed": index_stats.accessed,
-                        "added": index_stats.added,
-                        "updated": index_stats.updated,
-                        "deleted": index_stats.deleted,
-                        "merged": index_stats.merged,
-                        "accessed_at": index_stats.accessed_at,
-                        "added_at": index_stats.added_at,
-                        "updated_at": index_stats.updated_at,
-                        "deleted_at": index_stats.deleted_at,
-                        "merged_at": index_stats.merged_at,
-                    },
+                    "index_descriptor": index_desc,
+                    "index_stats": index_stats,
                 }
             ],
         }
 
     def empty(self, collection, query, dtypes=None) -> bool:
         df = self.find(collection, query, dtypes=dtypes, limit=1)
```

### Comparing `cognica-0.1.6/src/cognica/fts_analysis_pipeline.py` & `cognica-0.1.7/src/cognica/fts_analysis_pipeline.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/key_value_db.py` & `cognica-0.1.7/src/cognica/key_value_db.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/protobuf/document_db_pb2.py` & `cognica-0.1.7/src/cognica/protobuf/document_db_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/protobuf/document_db_pb2_grpc.py` & `cognica-0.1.7/src/cognica/protobuf/document_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/protobuf/document_pb2.py` & `cognica-0.1.7/src/cognica/protobuf/document_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/protobuf/fts_analysis_pipeline_pb2.py` & `cognica-0.1.7/src/cognica/protobuf/fts_analysis_pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py` & `cognica-0.1.7/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/protobuf/key_value_db_pb2.py` & `cognica-0.1.7/src/cognica/protobuf/key_value_db_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/protobuf/key_value_db_pb2_grpc.py` & `cognica-0.1.7/src/cognica/protobuf/key_value_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/protobuf/sentence_transformer_pb2.py` & `cognica-0.1.7/src/cognica/protobuf/sentence_transformer_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/protobuf/sentence_transformer_pb2_grpc.py` & `cognica-0.1.7/src/cognica/protobuf/sentence_transformer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica/sentence_transformer.py` & `cognica-0.1.7/src/cognica/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.6/src/cognica.egg-info/PKG-INFO` & `cognica-0.1.7/src/cognica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python client for Cognica database
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cognica-0.1.6/src/cognica.egg-info/SOURCES.txt` & `cognica-0.1.7/src/cognica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

