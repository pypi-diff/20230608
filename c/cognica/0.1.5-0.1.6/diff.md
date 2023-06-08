# Comparing `tmp/cognica-0.1.5.tar.gz` & `tmp/cognica-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognica-0.1.5.tar", last modified: Wed Jun  7 10:52:30 2023, max compression
+gzip compressed data, was "cognica-0.1.6.tar", last modified: Thu Jun  8 05:49:19 2023, max compression
```

## Comparing `cognica-0.1.5.tar` & `cognica-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 10:52:30.312876 cognica-0.1.5/
--rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-29 03:56:50.000000 cognica-0.1.5/LICENSE
--rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-07 10:52:30.312696 cognica-0.1.5/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 05:58:03.000000 cognica-0.1.5/README.md
--rw-r--r--   0 jaepil     (501) staff       (20)     1282 2023-06-07 10:52:14.000000 cognica-0.1.5/pyproject.toml
--rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-07 10:52:30.312929 cognica-0.1.5/setup.cfg
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 10:52:30.309246 cognica-0.1.5/src/
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 10:52:30.310431 cognica-0.1.5/src/cognica/
--rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-15 08:05:25.000000 cognica-0.1.5/src/cognica/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-15 08:05:26.000000 cognica-0.1.5/src/cognica/channel.py
--rw-r--r--   0 jaepil     (501) staff       (20)    17063 2023-06-07 10:50:53.000000 cognica-0.1.5/src/cognica/document_db.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 03:46:32.000000 cognica-0.1.5/src/cognica/fts_analysis_pipeline.py
--rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 03:46:59.000000 cognica-0.1.5/src/cognica/key_value_db.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 10:52:30.312494 cognica-0.1.5/src/cognica/protobuf/
--rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-15 08:05:26.000000 cognica-0.1.5/src/cognica/protobuf/__init__.py
--rw-r--r--   0 jaepil     (501) staff       (20)    13536 2023-06-07 03:42:37.000000 cognica-0.1.5/src/cognica/protobuf/document_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-03 01:34:57.000000 cognica-0.1.5/src/cognica/protobuf/document_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-06-03 01:33:38.000000 cognica-0.1.5/src/cognica/protobuf/document_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-03 01:33:38.000000 cognica-0.1.5/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-06-03 01:35:26.000000 cognica-0.1.5/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-03 01:33:38.000000 cognica-0.1.5/src/cognica/protobuf/key_value_db_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-06-03 01:35:45.000000 cognica-0.1.5/src/cognica/protobuf/key_value_db_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-03 01:33:38.000000 cognica-0.1.5/src/cognica/protobuf/sentence_transformer_pb2.py
--rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-06-03 01:36:10.000000 cognica-0.1.5/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
--rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 03:47:19.000000 cognica-0.1.5/src/cognica/sentence_transformer.py
-drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-07 10:52:30.311070 cognica-0.1.5/src/cognica.egg-info/
--rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-07 10:52:30.000000 cognica-0.1.5/src/cognica.egg-info/PKG-INFO
--rw-r--r--   0 jaepil     (501) staff       (20)      831 2023-06-07 10:52:30.000000 cognica-0.1.5/src/cognica.egg-info/SOURCES.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-07 10:52:30.000000 cognica-0.1.5/src/cognica.egg-info/dependency_links.txt
--rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-07 10:52:30.000000 cognica-0.1.5/src/cognica.egg-info/requires.txt
--rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-07 10:52:30.000000 cognica-0.1.5/src/cognica.egg-info/top_level.txt
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 05:49:19.567047 cognica-0.1.6/
+-rw-r--r--   0 jaepil     (501) staff       (20)    11357 2023-03-31 12:58:01.000000 cognica-0.1.6/LICENSE
+-rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-08 05:49:19.566854 cognica-0.1.6/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)     1534 2023-05-30 12:36:07.000000 cognica-0.1.6/README.md
+-rw-r--r--   0 jaepil     (501) staff       (20)     1282 2023-06-08 05:47:20.000000 cognica-0.1.6/pyproject.toml
+-rw-r--r--   0 jaepil     (501) staff       (20)       38 2023-06-08 05:49:19.567088 cognica-0.1.6/setup.cfg
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 05:49:19.557807 cognica-0.1.6/src/
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 05:49:19.559634 cognica-0.1.6/src/cognica/
+-rw-r--r--   0 jaepil     (501) staff       (20)      702 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     1847 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/channel.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    17063 2023-06-07 12:02:01.000000 cognica-0.1.6/src/cognica/document_db.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2840 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/fts_analysis_pipeline.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    11164 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/key_value_db.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 05:49:19.564493 cognica-0.1.6/src/cognica/protobuf/
+-rw-r--r--   0 jaepil     (501) staff       (20)       51 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/protobuf/__init__.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    15294 2023-06-08 05:46:47.000000 cognica-0.1.6/src/cognica/protobuf/document_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    24931 2023-06-08 05:46:39.000000 cognica-0.1.6/src/cognica/protobuf/document_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2293 2023-03-31 12:58:01.000000 cognica-0.1.6/src/cognica/protobuf/document_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     2669 2023-06-06 15:38:54.000000 cognica-0.1.6/src/cognica/protobuf/fts_analysis_pipeline_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     4508 2023-03-31 12:58:01.000000 cognica-0.1.6/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     7337 2023-06-06 15:38:54.000000 cognica-0.1.6/src/cognica/protobuf/key_value_db_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    19310 2023-03-31 12:58:01.000000 cognica-0.1.6/src/cognica/protobuf/key_value_db_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     6085 2023-06-06 15:38:54.000000 cognica-0.1.6/src/cognica/protobuf/sentence_transformer_pb2.py
+-rw-r--r--   0 jaepil     (501) staff       (20)    10071 2023-03-31 12:58:01.000000 cognica-0.1.6/src/cognica/protobuf/sentence_transformer_pb2_grpc.py
+-rw-r--r--   0 jaepil     (501) staff       (20)     9259 2023-05-16 12:19:52.000000 cognica-0.1.6/src/cognica/sentence_transformer.py
+drwxr-xr-x   0 jaepil     (501) staff       (20)        0 2023-06-08 05:49:19.560386 cognica-0.1.6/src/cognica.egg-info/
+-rw-r--r--   0 jaepil     (501) staff       (20)    15524 2023-06-08 05:49:19.000000 cognica-0.1.6/src/cognica.egg-info/PKG-INFO
+-rw-r--r--   0 jaepil     (501) staff       (20)      831 2023-06-08 05:49:19.000000 cognica-0.1.6/src/cognica.egg-info/SOURCES.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        1 2023-06-08 05:49:19.000000 cognica-0.1.6/src/cognica.egg-info/dependency_links.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)      105 2023-06-08 05:49:19.000000 cognica-0.1.6/src/cognica.egg-info/requires.txt
+-rw-r--r--   0 jaepil     (501) staff       (20)        8 2023-06-08 05:49:19.000000 cognica-0.1.6/src/cognica.egg-info/top_level.txt
```

### Comparing `cognica-0.1.5/LICENSE` & `cognica-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/PKG-INFO` & `cognica-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python client for Cognica database
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cognica-0.1.5/README.md` & `cognica-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/pyproject.toml` & `cognica-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cognica"
-version = "0.1.5"
+version = "0.1.6"
 authors = [{ name = "Cognica, Inc.", email = "jaepil@cognica.io" }]
 description = "Python client for Cognica database"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
   "pandas>=1.5.3",
```

### Comparing `cognica-0.1.5/src/cognica/__init__.py` & `cognica-0.1.6/src/cognica/__init__.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/channel.py` & `cognica-0.1.6/src/cognica/channel.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/document_db.py` & `cognica-0.1.6/src/cognica/document_db.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/fts_analysis_pipeline.py` & `cognica-0.1.6/src/cognica/fts_analysis_pipeline.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/key_value_db.py` & `cognica-0.1.6/src/cognica/key_value_db.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/protobuf/document_db_pb2.py` & `cognica-0.1.6/src/cognica/protobuf/document_db_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,110 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: document_db.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 import cognica.protobuf.document_pb2 as document__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64ocument_db.proto\x12\x17\x63ognica.rpc.db.document\x1a\x0e\x64ocument.proto\"\xf9\x01\n\x0fIndexDescriptor\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x03(\t\x12\x0e\n\x06unique\x18\x04 \x01(\x08\x12\x36\n\nindex_type\x18\x05 \x01(\x0e\x32\".cognica.rpc.db.document.IndexType\x12\x34\n\x06status\x18\x06 \x01(\x0e\x32$.cognica.rpc.db.document.IndexStatus\x12\x32\n\x07options\x18\x07 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\x94\x02\n\nIndexStats\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x19\n\x11\x61pproximated_size\x18\x03 \x01(\x04\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12\x10\n\x08\x61\x63\x63\x65ssed\x18\x05 \x01(\x04\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x06 \x01(\x04\x12\x0f\n\x07updated\x18\x07 \x01(\x04\x12\x0f\n\x07\x64\x65leted\x18\x08 \x01(\x04\x12\x0e\n\x06merged\x18\t \x01(\x04\x12\x13\n\x0b\x61\x63\x63\x65ssed_at\x18\n \x01(\x03\x12\x10\n\x08\x61\x64\x64\x65\x64_at\x18\x0b \x01(\x03\x12\x12\n\nupdated_at\x18\x0c \x01(\x03\x12\x12\n\ndeleted_at\x18\r \x01(\x03\x12\x11\n\tmerged_at\x18\x0e \x01(\x03\"\xa8\x01\n\x0e\x43ollectionInfo\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x43\n\x11index_descriptors\x18\x02 \x03(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\x12\x38\n\x0bindex_stats\x18\x03 \x03(\x0b\x32#.cognica.rpc.db.document.IndexStats\"\x7f\n\x0bProfileInfo\x12\x0f\n\x07matched\x18\x01 \x01(\x04\x12\x0f\n\x07scanned\x18\x02 \x01(\x04\x12\x10\n\x08\x66iltered\x18\x03 \x01(\x04\x12\x19\n\x11query_duration_us\x18\x04 \x01(\x04\x12!\n\x19serialization_duration_us\x18\x05 \x01(\x04\"V\n\x17\x43reateCollectionRequest\x12;\n\ncollection\x18\x01 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\"r\n\x18\x43reateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"0\n\x15\x44ropCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"p\n\x16\x44ropCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"/\n\x14GetCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\xac\x01\n\x15GetCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12;\n\ncollection\x18\x03 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"k\n\x12\x43reateIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12<\n\nindex_desc\x18\x02 \x01(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\"m\n\x13\x43reateIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"?\n\x10\x44ropIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"k\n\x11\x44ropIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\">\n\x0fGetIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\xfb\x01\n\x10GetIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12<\n\nindex_desc\x18\x04 \x01(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\x12\x38\n\x0bindex_stats\x18\x05 \x01(\x0b\x32#.cognica.rpc.db.document.IndexStats\x12\x35\n\x07profile\x18\x06 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"R\n\x05Query\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x05query\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\xe4\x01\n\x0b\x46indRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\x15\n\rindex_columns\x18\x03 \x03(\t\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12@\n\x06\x64types\x18\x05 \x03(\x0b\x32\x30.cognica.rpc.db.document.FindRequest.DtypesEntry\x1a-\n\x0b\x44typesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"|\n\x0c\x46indResponse\x12\x13\n\x0bnum_columns\x18\x01 \x01(\x05\x12\x10\n\x08num_rows\x18\x02 \x01(\x05\x12\x0e\n\x06\x62uffer\x18\x03 \x01(\x0c\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"J\n\x10\x46indBatchRequest\x12\x36\n\x08requests\x18\x01 \x03(\x0b\x32$.cognica.rpc.db.document.FindRequest\"M\n\x11\x46indBatchResponse\x12\x38\n\tresponses\x18\x01 \x03(\x0b\x32%.cognica.rpc.db.document.FindResponse\"=\n\x0c\x43ountRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"v\n\rCountResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x03\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"@\n\x0f\x43ontainsRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"y\n\x10\x43ontainsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x66ound\x18\x03 \x01(\x08\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rInsertRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eInsertResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x8f\x01\n\rUpdateRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x06\x66ilter\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\x12\x32\n\x07updates\x18\x03 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"h\n\x0eUpdateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rRemoveRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eRemoveResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"4\n\x19TruncateCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"t\n\x1aTruncateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x18\n\x16ListCollectionsRequest\"\x8b\x01\n\x17ListCollectionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo*e\n\tIndexType\x12\x0f\n\x0bkPrimaryKey\x10\x00\x12\x11\n\rkSecondaryKey\x10\x01\x12\x1a\n\x16kClusteredSecondaryKey\x10\x02\x12\x18\n\x14kFullTextSearchIndex\x10\x03*\x8d\x01\n\x0bIndexStatus\x12\x0c\n\x08kEnabled\x10\x00\x12\r\n\tkDisabled\x10\x01\x12\x0f\n\x0bkReadyToUse\x10\x02\x12\x14\n\x10kBuildInProgress\x10\x03\x12\x12\n\x0ekBuildFinished\x10\x04\x12\x13\n\x0fkDropInProgress\x10\x05\x12\x11\n\rkDropFinished\x10\x06\x32\xbe\x0c\n\x11\x44ocumentDBService\x12U\n\x04\x66ind\x12$.cognica.rpc.db.document.FindRequest\x1a%.cognica.rpc.db.document.FindResponse\"\x00\x12\x65\n\nfind_batch\x12).cognica.rpc.db.document.FindBatchRequest\x1a*.cognica.rpc.db.document.FindBatchResponse\"\x00\x12X\n\x05\x63ount\x12%.cognica.rpc.db.document.CountRequest\x1a&.cognica.rpc.db.document.CountResponse\"\x00\x12\x61\n\x08\x63ontains\x12(.cognica.rpc.db.document.ContainsRequest\x1a).cognica.rpc.db.document.ContainsResponse\"\x00\x12[\n\x06insert\x12&.cognica.rpc.db.document.InsertRequest\x1a\'.cognica.rpc.db.document.InsertResponse\"\x00\x12[\n\x06update\x12&.cognica.rpc.db.document.UpdateRequest\x1a\'.cognica.rpc.db.document.UpdateResponse\"\x00\x12[\n\x06remove\x12&.cognica.rpc.db.document.RemoveRequest\x1a\'.cognica.rpc.db.document.RemoveResponse\"\x00\x12z\n\x11\x63reate_collection\x12\x30.cognica.rpc.db.document.CreateCollectionRequest\x1a\x31.cognica.rpc.db.document.CreateCollectionResponse\"\x00\x12t\n\x0f\x64rop_collection\x12..cognica.rpc.db.document.DropCollectionRequest\x1a/.cognica.rpc.db.document.DropCollectionResponse\"\x00\x12q\n\x0eget_collection\x12-.cognica.rpc.db.document.GetCollectionRequest\x1a..cognica.rpc.db.document.GetCollectionResponse\"\x00\x12w\n\x10list_collections\x12/.cognica.rpc.db.document.ListCollectionsRequest\x1a\x30.cognica.rpc.db.document.ListCollectionsResponse\"\x00\x12\x80\x01\n\x13truncate_collection\x12\x32.cognica.rpc.db.document.TruncateCollectionRequest\x1a\x33.cognica.rpc.db.document.TruncateCollectionResponse\"\x00\x12k\n\x0c\x63reate_index\x12+.cognica.rpc.db.document.CreateIndexRequest\x1a,.cognica.rpc.db.document.CreateIndexResponse\"\x00\x12\x65\n\ndrop_index\x12).cognica.rpc.db.document.DropIndexRequest\x1a*.cognica.rpc.db.document.DropIndexResponse\"\x00\x12\x62\n\tget_index\x12(.cognica.rpc.db.document.GetIndexRequest\x1a).cognica.rpc.db.document.GetIndexResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x64ocument_db.proto\x12\x17\x63ognica.rpc.db.document\x1a\x0e\x64ocument.proto\"\xf9\x01\n\x0fIndexDescriptor\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x0e\n\x06\x66ields\x18\x03 \x03(\t\x12\x0e\n\x06unique\x18\x04 \x01(\x08\x12\x36\n\nindex_type\x18\x05 \x01(\x0e\x32\".cognica.rpc.db.document.IndexType\x12\x34\n\x06status\x18\x06 \x01(\x0e\x32$.cognica.rpc.db.document.IndexStatus\x12\x32\n\x07options\x18\x07 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\xa6\x01\n\rFTSFieldStats\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x17\n\x0ftotal_doc_count\x18\x02 \x01(\x03\x12\x16\n\x0etotal_doc_size\x18\x03 \x01(\x03\x12\x11\n\tdoc_count\x18\x04 \x01(\x03\x12\x10\n\x08\x64oc_size\x18\x05 \x01(\x03\x12\x15\n\rsum_term_freq\x18\x06 \x01(\x03\x12\x14\n\x0csum_doc_freq\x18\x07 \x01(\x03\"q\n\rFTSIndexStats\x12\x11\n\tdoc_count\x18\x01 \x01(\x03\x12\x10\n\x08\x64oc_size\x18\x02 \x01(\x03\x12;\n\x0b\x66ield_stats\x18\x03 \x03(\x0b\x32&.cognica.rpc.db.document.FTSFieldStats\"\xcf\x02\n\nIndexStats\x12\x10\n\x08index_id\x18\x01 \x01(\r\x12\x12\n\nindex_name\x18\x02 \x01(\t\x12\x19\n\x11\x61pproximated_size\x18\x03 \x01(\x04\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12\x10\n\x08\x61\x63\x63\x65ssed\x18\x05 \x01(\x04\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x06 \x01(\x04\x12\x0f\n\x07updated\x18\x07 \x01(\x04\x12\x0f\n\x07\x64\x65leted\x18\x08 \x01(\x04\x12\x0e\n\x06merged\x18\t \x01(\x04\x12\x13\n\x0b\x61\x63\x63\x65ssed_at\x18\n \x01(\x03\x12\x10\n\x08\x61\x64\x64\x65\x64_at\x18\x0b \x01(\x03\x12\x12\n\nupdated_at\x18\x0c \x01(\x03\x12\x12\n\ndeleted_at\x18\r \x01(\x03\x12\x11\n\tmerged_at\x18\x0e \x01(\x03\x12\x39\n\tfts_stats\x18\x0f \x01(\x0b\x32&.cognica.rpc.db.document.FTSIndexStats\"\xa8\x01\n\x0e\x43ollectionInfo\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x43\n\x11index_descriptors\x18\x02 \x03(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\x12\x38\n\x0bindex_stats\x18\x03 \x03(\x0b\x32#.cognica.rpc.db.document.IndexStats\"\x7f\n\x0bProfileInfo\x12\x0f\n\x07matched\x18\x01 \x01(\x04\x12\x0f\n\x07scanned\x18\x02 \x01(\x04\x12\x10\n\x08\x66iltered\x18\x03 \x01(\x04\x12\x19\n\x11query_duration_us\x18\x04 \x01(\x04\x12!\n\x19serialization_duration_us\x18\x05 \x01(\x04\"V\n\x17\x43reateCollectionRequest\x12;\n\ncollection\x18\x01 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\"r\n\x18\x43reateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"0\n\x15\x44ropCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"p\n\x16\x44ropCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"/\n\x14GetCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"\xac\x01\n\x15GetCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12;\n\ncollection\x18\x03 \x01(\x0b\x32\'.cognica.rpc.db.document.CollectionInfo\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"k\n\x12\x43reateIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12<\n\nindex_desc\x18\x02 \x01(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\"m\n\x13\x43reateIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"?\n\x10\x44ropIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"k\n\x11\x44ropIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\">\n\x0fGetIndexRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"\xfb\x01\n\x10GetIndexResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x17\n\x0f\x63ollection_name\x18\x03 \x01(\t\x12<\n\nindex_desc\x18\x04 \x01(\x0b\x32(.cognica.rpc.db.document.IndexDescriptor\x12\x38\n\x0bindex_stats\x18\x05 \x01(\x0b\x32#.cognica.rpc.db.document.IndexStats\x12\x35\n\x07profile\x18\x06 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"R\n\x05Query\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x30\n\x05query\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"\xe4\x01\n\x0b\x46indRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\x12\r\n\x05limit\x18\x02 \x01(\x05\x12\x15\n\rindex_columns\x18\x03 \x03(\t\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12@\n\x06\x64types\x18\x05 \x03(\x0b\x32\x30.cognica.rpc.db.document.FindRequest.DtypesEntry\x1a-\n\x0b\x44typesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"|\n\x0c\x46indResponse\x12\x13\n\x0bnum_columns\x18\x01 \x01(\x05\x12\x10\n\x08num_rows\x18\x02 \x01(\x05\x12\x0e\n\x06\x62uffer\x18\x03 \x01(\x0c\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"J\n\x10\x46indBatchRequest\x12\x36\n\x08requests\x18\x01 \x03(\x0b\x32$.cognica.rpc.db.document.FindRequest\"M\n\x11\x46indBatchResponse\x12\x38\n\tresponses\x18\x01 \x03(\x0b\x32%.cognica.rpc.db.document.FindResponse\"=\n\x0c\x43ountRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"v\n\rCountResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x03\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"@\n\x0f\x43ontainsRequest\x12-\n\x05query\x18\x01 \x01(\x0b\x32\x1e.cognica.rpc.db.document.Query\"y\n\x10\x43ontainsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\r\n\x05\x66ound\x18\x03 \x01(\x08\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rInsertRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eInsertResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x8f\x01\n\rUpdateRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\x12\x31\n\x06\x66ilter\x18\x02 \x01(\x0b\x32!.cognica.rpc.db.document.Document\x12\x32\n\x07updates\x18\x03 \x01(\x0b\x32!.cognica.rpc.db.document.Document\"h\n\x0eUpdateResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"A\n\rRemoveRequest\x12\x30\n\x08requests\x18\x01 \x03(\x0b\x32\x1e.cognica.rpc.db.document.Query\"h\n\x0eRemoveResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"4\n\x19TruncateCollectionRequest\x12\x17\n\x0f\x63ollection_name\x18\x01 \x01(\t\"t\n\x1aTruncateCollectionResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x35\n\x07profile\x18\x03 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo\"\x18\n\x16ListCollectionsRequest\"\x8b\x01\n\x17ListCollectionsResponse\x12\x0e\n\x06status\x18\x01 \x01(\x05\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x18\n\x10\x63ollection_names\x18\x03 \x03(\t\x12\x35\n\x07profile\x18\x04 \x01(\x0b\x32$.cognica.rpc.db.document.ProfileInfo*e\n\tIndexType\x12\x0f\n\x0bkPrimaryKey\x10\x00\x12\x11\n\rkSecondaryKey\x10\x01\x12\x1a\n\x16kClusteredSecondaryKey\x10\x02\x12\x18\n\x14kFullTextSearchIndex\x10\x03*\x8d\x01\n\x0bIndexStatus\x12\x0c\n\x08kEnabled\x10\x00\x12\r\n\tkDisabled\x10\x01\x12\x0f\n\x0bkReadyToUse\x10\x02\x12\x14\n\x10kBuildInProgress\x10\x03\x12\x12\n\x0ekBuildFinished\x10\x04\x12\x13\n\x0fkDropInProgress\x10\x05\x12\x11\n\rkDropFinished\x10\x06\x32\xbe\x0c\n\x11\x44ocumentDBService\x12U\n\x04\x66ind\x12$.cognica.rpc.db.document.FindRequest\x1a%.cognica.rpc.db.document.FindResponse\"\x00\x12\x65\n\nfind_batch\x12).cognica.rpc.db.document.FindBatchRequest\x1a*.cognica.rpc.db.document.FindBatchResponse\"\x00\x12X\n\x05\x63ount\x12%.cognica.rpc.db.document.CountRequest\x1a&.cognica.rpc.db.document.CountResponse\"\x00\x12\x61\n\x08\x63ontains\x12(.cognica.rpc.db.document.ContainsRequest\x1a).cognica.rpc.db.document.ContainsResponse\"\x00\x12[\n\x06insert\x12&.cognica.rpc.db.document.InsertRequest\x1a\'.cognica.rpc.db.document.InsertResponse\"\x00\x12[\n\x06update\x12&.cognica.rpc.db.document.UpdateRequest\x1a\'.cognica.rpc.db.document.UpdateResponse\"\x00\x12[\n\x06remove\x12&.cognica.rpc.db.document.RemoveRequest\x1a\'.cognica.rpc.db.document.RemoveResponse\"\x00\x12z\n\x11\x63reate_collection\x12\x30.cognica.rpc.db.document.CreateCollectionRequest\x1a\x31.cognica.rpc.db.document.CreateCollectionResponse\"\x00\x12t\n\x0f\x64rop_collection\x12..cognica.rpc.db.document.DropCollectionRequest\x1a/.cognica.rpc.db.document.DropCollectionResponse\"\x00\x12q\n\x0eget_collection\x12-.cognica.rpc.db.document.GetCollectionRequest\x1a..cognica.rpc.db.document.GetCollectionResponse\"\x00\x12w\n\x10list_collections\x12/.cognica.rpc.db.document.ListCollectionsRequest\x1a\x30.cognica.rpc.db.document.ListCollectionsResponse\"\x00\x12\x80\x01\n\x13truncate_collection\x12\x32.cognica.rpc.db.document.TruncateCollectionRequest\x1a\x33.cognica.rpc.db.document.TruncateCollectionResponse\"\x00\x12k\n\x0c\x63reate_index\x12+.cognica.rpc.db.document.CreateIndexRequest\x1a,.cognica.rpc.db.document.CreateIndexResponse\"\x00\x12\x65\n\ndrop_index\x12).cognica.rpc.db.document.DropIndexRequest\x1a*.cognica.rpc.db.document.DropIndexResponse\"\x00\x12\x62\n\tget_index\x12(.cognica.rpc.db.document.GetIndexRequest\x1a).cognica.rpc.db.document.GetIndexResponse\"\x00\x42\x03\xf8\x01\x01\x62\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'document_db_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'document_db_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\370\001\001'
   _FINDREQUEST_DTYPESENTRY._options = None
   _FINDREQUEST_DTYPESENTRY._serialized_options = b'8\001'
-  _INDEXTYPE._serialized_start=4103
-  _INDEXTYPE._serialized_end=4204
-  _INDEXSTATUS._serialized_start=4207
-  _INDEXSTATUS._serialized_end=4348
-  _INDEXDESCRIPTOR._serialized_start=63
-  _INDEXDESCRIPTOR._serialized_end=312
-  _INDEXSTATS._serialized_start=315
-  _INDEXSTATS._serialized_end=591
-  _COLLECTIONINFO._serialized_start=594
-  _COLLECTIONINFO._serialized_end=762
-  _PROFILEINFO._serialized_start=764
-  _PROFILEINFO._serialized_end=891
-  _CREATECOLLECTIONREQUEST._serialized_start=893
-  _CREATECOLLECTIONREQUEST._serialized_end=979
-  _CREATECOLLECTIONRESPONSE._serialized_start=981
-  _CREATECOLLECTIONRESPONSE._serialized_end=1095
-  _DROPCOLLECTIONREQUEST._serialized_start=1097
-  _DROPCOLLECTIONREQUEST._serialized_end=1145
-  _DROPCOLLECTIONRESPONSE._serialized_start=1147
-  _DROPCOLLECTIONRESPONSE._serialized_end=1259
-  _GETCOLLECTIONREQUEST._serialized_start=1261
-  _GETCOLLECTIONREQUEST._serialized_end=1308
-  _GETCOLLECTIONRESPONSE._serialized_start=1311
-  _GETCOLLECTIONRESPONSE._serialized_end=1483
-  _CREATEINDEXREQUEST._serialized_start=1485
-  _CREATEINDEXREQUEST._serialized_end=1592
-  _CREATEINDEXRESPONSE._serialized_start=1594
-  _CREATEINDEXRESPONSE._serialized_end=1703
-  _DROPINDEXREQUEST._serialized_start=1705
-  _DROPINDEXREQUEST._serialized_end=1768
-  _DROPINDEXRESPONSE._serialized_start=1770
-  _DROPINDEXRESPONSE._serialized_end=1877
-  _GETINDEXREQUEST._serialized_start=1879
-  _GETINDEXREQUEST._serialized_end=1941
-  _GETINDEXRESPONSE._serialized_start=1944
-  _GETINDEXRESPONSE._serialized_end=2195
-  _QUERY._serialized_start=2197
-  _QUERY._serialized_end=2279
-  _FINDREQUEST._serialized_start=2282
-  _FINDREQUEST._serialized_end=2510
-  _FINDREQUEST_DTYPESENTRY._serialized_start=2465
-  _FINDREQUEST_DTYPESENTRY._serialized_end=2510
-  _FINDRESPONSE._serialized_start=2512
-  _FINDRESPONSE._serialized_end=2636
-  _FINDBATCHREQUEST._serialized_start=2638
-  _FINDBATCHREQUEST._serialized_end=2712
-  _FINDBATCHRESPONSE._serialized_start=2714
-  _FINDBATCHRESPONSE._serialized_end=2791
-  _COUNTREQUEST._serialized_start=2793
-  _COUNTREQUEST._serialized_end=2854
-  _COUNTRESPONSE._serialized_start=2856
-  _COUNTRESPONSE._serialized_end=2974
-  _CONTAINSREQUEST._serialized_start=2976
-  _CONTAINSREQUEST._serialized_end=3040
-  _CONTAINSRESPONSE._serialized_start=3042
-  _CONTAINSRESPONSE._serialized_end=3163
-  _INSERTREQUEST._serialized_start=3165
-  _INSERTREQUEST._serialized_end=3230
-  _INSERTRESPONSE._serialized_start=3232
-  _INSERTRESPONSE._serialized_end=3336
-  _UPDATEREQUEST._serialized_start=3339
-  _UPDATEREQUEST._serialized_end=3482
-  _UPDATERESPONSE._serialized_start=3484
-  _UPDATERESPONSE._serialized_end=3588
-  _REMOVEREQUEST._serialized_start=3590
-  _REMOVEREQUEST._serialized_end=3655
-  _REMOVERESPONSE._serialized_start=3657
-  _REMOVERESPONSE._serialized_end=3761
-  _TRUNCATECOLLECTIONREQUEST._serialized_start=3763
-  _TRUNCATECOLLECTIONREQUEST._serialized_end=3815
-  _TRUNCATECOLLECTIONRESPONSE._serialized_start=3817
-  _TRUNCATECOLLECTIONRESPONSE._serialized_end=3933
-  _LISTCOLLECTIONSREQUEST._serialized_start=3935
-  _LISTCOLLECTIONSREQUEST._serialized_end=3959
-  _LISTCOLLECTIONSRESPONSE._serialized_start=3962
-  _LISTCOLLECTIONSRESPONSE._serialized_end=4101
-  _DOCUMENTDBSERVICE._serialized_start=4351
-  _DOCUMENTDBSERVICE._serialized_end=5949
+  _globals['_INDEXTYPE']._serialized_start=4446
+  _globals['_INDEXTYPE']._serialized_end=4547
+  _globals['_INDEXSTATUS']._serialized_start=4550
+  _globals['_INDEXSTATUS']._serialized_end=4691
+  _globals['_INDEXDESCRIPTOR']._serialized_start=63
+  _globals['_INDEXDESCRIPTOR']._serialized_end=312
+  _globals['_FTSFIELDSTATS']._serialized_start=315
+  _globals['_FTSFIELDSTATS']._serialized_end=481
+  _globals['_FTSINDEXSTATS']._serialized_start=483
+  _globals['_FTSINDEXSTATS']._serialized_end=596
+  _globals['_INDEXSTATS']._serialized_start=599
+  _globals['_INDEXSTATS']._serialized_end=934
+  _globals['_COLLECTIONINFO']._serialized_start=937
+  _globals['_COLLECTIONINFO']._serialized_end=1105
+  _globals['_PROFILEINFO']._serialized_start=1107
+  _globals['_PROFILEINFO']._serialized_end=1234
+  _globals['_CREATECOLLECTIONREQUEST']._serialized_start=1236
+  _globals['_CREATECOLLECTIONREQUEST']._serialized_end=1322
+  _globals['_CREATECOLLECTIONRESPONSE']._serialized_start=1324
+  _globals['_CREATECOLLECTIONRESPONSE']._serialized_end=1438
+  _globals['_DROPCOLLECTIONREQUEST']._serialized_start=1440
+  _globals['_DROPCOLLECTIONREQUEST']._serialized_end=1488
+  _globals['_DROPCOLLECTIONRESPONSE']._serialized_start=1490
+  _globals['_DROPCOLLECTIONRESPONSE']._serialized_end=1602
+  _globals['_GETCOLLECTIONREQUEST']._serialized_start=1604
+  _globals['_GETCOLLECTIONREQUEST']._serialized_end=1651
+  _globals['_GETCOLLECTIONRESPONSE']._serialized_start=1654
+  _globals['_GETCOLLECTIONRESPONSE']._serialized_end=1826
+  _globals['_CREATEINDEXREQUEST']._serialized_start=1828
+  _globals['_CREATEINDEXREQUEST']._serialized_end=1935
+  _globals['_CREATEINDEXRESPONSE']._serialized_start=1937
+  _globals['_CREATEINDEXRESPONSE']._serialized_end=2046
+  _globals['_DROPINDEXREQUEST']._serialized_start=2048
+  _globals['_DROPINDEXREQUEST']._serialized_end=2111
+  _globals['_DROPINDEXRESPONSE']._serialized_start=2113
+  _globals['_DROPINDEXRESPONSE']._serialized_end=2220
+  _globals['_GETINDEXREQUEST']._serialized_start=2222
+  _globals['_GETINDEXREQUEST']._serialized_end=2284
+  _globals['_GETINDEXRESPONSE']._serialized_start=2287
+  _globals['_GETINDEXRESPONSE']._serialized_end=2538
+  _globals['_QUERY']._serialized_start=2540
+  _globals['_QUERY']._serialized_end=2622
+  _globals['_FINDREQUEST']._serialized_start=2625
+  _globals['_FINDREQUEST']._serialized_end=2853
+  _globals['_FINDREQUEST_DTYPESENTRY']._serialized_start=2808
+  _globals['_FINDREQUEST_DTYPESENTRY']._serialized_end=2853
+  _globals['_FINDRESPONSE']._serialized_start=2855
+  _globals['_FINDRESPONSE']._serialized_end=2979
+  _globals['_FINDBATCHREQUEST']._serialized_start=2981
+  _globals['_FINDBATCHREQUEST']._serialized_end=3055
+  _globals['_FINDBATCHRESPONSE']._serialized_start=3057
+  _globals['_FINDBATCHRESPONSE']._serialized_end=3134
+  _globals['_COUNTREQUEST']._serialized_start=3136
+  _globals['_COUNTREQUEST']._serialized_end=3197
+  _globals['_COUNTRESPONSE']._serialized_start=3199
+  _globals['_COUNTRESPONSE']._serialized_end=3317
+  _globals['_CONTAINSREQUEST']._serialized_start=3319
+  _globals['_CONTAINSREQUEST']._serialized_end=3383
+  _globals['_CONTAINSRESPONSE']._serialized_start=3385
+  _globals['_CONTAINSRESPONSE']._serialized_end=3506
+  _globals['_INSERTREQUEST']._serialized_start=3508
+  _globals['_INSERTREQUEST']._serialized_end=3573
+  _globals['_INSERTRESPONSE']._serialized_start=3575
+  _globals['_INSERTRESPONSE']._serialized_end=3679
+  _globals['_UPDATEREQUEST']._serialized_start=3682
+  _globals['_UPDATEREQUEST']._serialized_end=3825
+  _globals['_UPDATERESPONSE']._serialized_start=3827
+  _globals['_UPDATERESPONSE']._serialized_end=3931
+  _globals['_REMOVEREQUEST']._serialized_start=3933
+  _globals['_REMOVEREQUEST']._serialized_end=3998
+  _globals['_REMOVERESPONSE']._serialized_start=4000
+  _globals['_REMOVERESPONSE']._serialized_end=4104
+  _globals['_TRUNCATECOLLECTIONREQUEST']._serialized_start=4106
+  _globals['_TRUNCATECOLLECTIONREQUEST']._serialized_end=4158
+  _globals['_TRUNCATECOLLECTIONRESPONSE']._serialized_start=4160
+  _globals['_TRUNCATECOLLECTIONRESPONSE']._serialized_end=4276
+  _globals['_LISTCOLLECTIONSREQUEST']._serialized_start=4278
+  _globals['_LISTCOLLECTIONSREQUEST']._serialized_end=4302
+  _globals['_LISTCOLLECTIONSRESPONSE']._serialized_start=4305
+  _globals['_LISTCOLLECTIONSRESPONSE']._serialized_end=4444
+  _globals['_DOCUMENTDBSERVICE']._serialized_start=4694
+  _globals['_DOCUMENTDBSERVICE']._serialized_end=6292
 # @@protoc_insertion_point(module_scope)
```

### Comparing `cognica-0.1.5/src/cognica/protobuf/document_db_pb2_grpc.py` & `cognica-0.1.6/src/cognica/protobuf/document_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/protobuf/document_pb2.py` & `cognica-0.1.6/src/cognica/protobuf/document_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/protobuf/fts_analysis_pipeline_pb2.py` & `cognica-0.1.6/src/cognica/protobuf/fts_analysis_pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py` & `cognica-0.1.6/src/cognica/protobuf/fts_analysis_pipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/protobuf/key_value_db_pb2.py` & `cognica-0.1.6/src/cognica/protobuf/key_value_db_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/protobuf/key_value_db_pb2_grpc.py` & `cognica-0.1.6/src/cognica/protobuf/key_value_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/protobuf/sentence_transformer_pb2.py` & `cognica-0.1.6/src/cognica/protobuf/sentence_transformer_pb2.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/protobuf/sentence_transformer_pb2_grpc.py` & `cognica-0.1.6/src/cognica/protobuf/sentence_transformer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica/sentence_transformer.py` & `cognica-0.1.6/src/cognica/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `cognica-0.1.5/src/cognica.egg-info/PKG-INFO` & `cognica-0.1.6/src/cognica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognica
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python client for Cognica database
 Author-email: "Cognica, Inc." <jaepil@cognica.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cognica-0.1.5/src/cognica.egg-info/SOURCES.txt` & `cognica-0.1.6/src/cognica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

