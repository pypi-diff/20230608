# Comparing `tmp/milvus-ingestion-0.4.0.tar.gz` & `tmp/milvus-ingestion-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus-ingestion-0.4.0.tar", last modified: Tue Jun  6 13:25:11 2023, max compression
+gzip compressed data, was "milvus-ingestion-0.5.0.tar", last modified: Thu Jun  8 07:08:20 2023, max compression
```

## Comparing `milvus-ingestion-0.4.0.tar` & `milvus-ingestion-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-06-06 13:25:11.877547 milvus-ingestion-0.4.0/
--rw-r--r--   0 michaelmo   (501) staff       (20)    11357 2023-06-04 15:51:31.000000 milvus-ingestion-0.4.0/LICENSE
--rw-r--r--   0 michaelmo   (501) staff       (20)     4235 2023-06-06 13:25:11.877101 milvus-ingestion-0.4.0/PKG-INFO
--rw-r--r--   0 michaelmo   (501) staff       (20)     3663 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/README.md
-drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-06-06 13:25:11.874669 milvus-ingestion-0.4.0/milvus_ingestion/
--rw-r--r--   0 michaelmo   (501) staff       (20)      969 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/__init__.py
--rw-r--r--   0 michaelmo   (501) staff       (20)    17876 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/buffer.py
--rw-r--r--   0 michaelmo   (501) staff       (20)      973 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/constants.py
--rw-r--r--   0 michaelmo   (501) staff       (20)    14361 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/data_buffer.py
--rw-r--r--   0 michaelmo   (501) staff       (20)     2665 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/data_info.py
--rw-r--r--   0 michaelmo   (501) staff       (20)     7631 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/milvus_connector.py
--rw-r--r--   0 michaelmo   (501) staff       (20)     5355 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/uploader.py
--rw-r--r--   0 michaelmo   (501) staff       (20)     1424 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/milvus_ingestion/util.py
-drwxr-xr-x   0 michaelmo   (501) staff       (20)        0 2023-06-06 13:25:11.876588 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/
--rw-r--r--   0 michaelmo   (501) staff       (20)     4235 2023-06-06 13:25:11.000000 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/PKG-INFO
--rw-r--r--   0 michaelmo   (501) staff       (20)      464 2023-06-06 13:25:11.000000 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/SOURCES.txt
--rw-r--r--   0 michaelmo   (501) staff       (20)        1 2023-06-06 13:25:11.000000 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/dependency_links.txt
--rw-r--r--   0 michaelmo   (501) staff       (20)       63 2023-06-06 13:25:11.000000 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/requires.txt
--rw-r--r--   0 michaelmo   (501) staff       (20)       17 2023-06-06 13:25:11.000000 milvus-ingestion-0.4.0/milvus_ingestion.egg-info/top_level.txt
--rw-r--r--   0 michaelmo   (501) staff       (20)       38 2023-06-06 13:25:11.877677 milvus-ingestion-0.4.0/setup.cfg
--rw-r--r--   0 michaelmo   (501) staff       (20)      976 2023-06-06 13:21:56.000000 milvus-ingestion-0.4.0/setup.py
+drwxrwxr-x   0 yhmo      (1000) yhmo      (1000)        0 2023-06-08 07:08:20.902845 milvus-ingestion-0.5.0/
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)    11357 2023-05-26 08:00:33.000000 milvus-ingestion-0.5.0/LICENSE
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)    19757 2023-06-08 07:08:20.902845 milvus-ingestion-0.5.0/PKG-INFO
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)    19186 2023-06-07 11:20:52.000000 milvus-ingestion-0.5.0/README.md
+drwxrwxr-x   0 yhmo      (1000) yhmo      (1000)        0 2023-06-08 07:08:20.898846 milvus-ingestion-0.5.0/milvus_ingestion/
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)      874 2023-06-07 04:09:26.000000 milvus-ingestion-0.5.0/milvus_ingestion/__init__.py
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)    20550 2023-06-08 06:06:58.000000 milvus-ingestion-0.5.0/milvus_ingestion/buffer.py
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     1116 2023-06-07 08:42:45.000000 milvus-ingestion-0.5.0/milvus_ingestion/constants.py
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)    16113 2023-06-08 07:01:06.000000 milvus-ingestion-0.5.0/milvus_ingestion/data_buffer.py
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     3340 2023-06-08 06:05:13.000000 milvus-ingestion-0.5.0/milvus_ingestion/data_info.py
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     1117 2023-06-08 06:05:13.000000 milvus-ingestion-0.5.0/milvus_ingestion/exceptions.py
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     7648 2023-06-08 06:05:13.000000 milvus-ingestion-0.5.0/milvus_ingestion/milvus_connector.py
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     5899 2023-06-08 06:05:13.000000 milvus-ingestion-0.5.0/milvus_ingestion/uploader.py
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)     1369 2023-06-08 06:05:13.000000 milvus-ingestion-0.5.0/milvus_ingestion/util.py
+drwxrwxr-x   0 yhmo      (1000) yhmo      (1000)        0 2023-06-08 07:08:20.902845 milvus-ingestion-0.5.0/milvus_ingestion.egg-info/
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)    19757 2023-06-08 07:08:20.000000 milvus-ingestion-0.5.0/milvus_ingestion.egg-info/PKG-INFO
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)      495 2023-06-08 07:08:20.000000 milvus-ingestion-0.5.0/milvus_ingestion.egg-info/SOURCES.txt
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)        1 2023-06-08 07:08:20.000000 milvus-ingestion-0.5.0/milvus_ingestion.egg-info/dependency_links.txt
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)       63 2023-06-08 07:08:20.000000 milvus-ingestion-0.5.0/milvus_ingestion.egg-info/requires.txt
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)       17 2023-06-08 07:08:20.000000 milvus-ingestion-0.5.0/milvus_ingestion.egg-info/top_level.txt
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)       38 2023-06-08 07:08:20.902845 milvus-ingestion-0.5.0/setup.cfg
+-rw-rw-r--   0 yhmo      (1000) yhmo      (1000)      976 2023-06-08 07:08:02.000000 milvus-ingestion-0.5.0/setup.py
```

### Comparing `milvus-ingestion-0.4.0/LICENSE` & `milvus-ingestion-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `milvus-ingestion-0.4.0/milvus_ingestion/buffer.py` & `milvus-ingestion-0.5.0/milvus_ingestion/buffer.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # the License.
 
 import os
 import json
 from typing import List
 
 import numpy
-import datetime
 
 from logging import Logger
 from threading import Lock
 
 from pymilvus import (
     DataType,
 )
@@ -26,25 +25,31 @@
     Base,
     default_logger,
     _current_datetime,
 )
 
 from .constants import (
     IngestionType,
+    TaskState,
     DEFAULT_PARTITION_NAME,
     DYNAMIC_FIELD_NAME,
     COLLECTION_NAME_KEY,
     MB,
     GB,
 )
 
 from .data_info import (
     DataInfo,
 )
 
+from .exceptions import (
+    IngestionException,
+    ErrorCode,
+)
+
 default_values = {
     DataType.BOOL.name: False,
     DataType.INT8.name: 0,
     DataType.INT16.name: 0,
     DataType.INT32.name: 0,
     DataType.INT64.name: 0,
     DataType.FLOAT.name: 0.0,
@@ -86,15 +91,15 @@
         ):
         super().__init__(logger=logger)
         self._collection_schema = collection_schema
         self._partition_name = partition_name
         self._target_fields = {}
         self._buffer_size = 0
         self._buffer_row_count = 0
-        self._buffer_lock = Lock()
+        self._sealed = False
 
         for field in self._collection_schema['fields']:
             self._target_fields[field['name']] = field
 
     @property
     def collection_schema(self) -> dict:
         return self._collection_schema
@@ -120,14 +125,21 @@
     def buffer_size(self)->int:
         return self._buffer_size
 
     @property
     def buffer_row_count(self)->int:
         return self._buffer_row_count
 
+    @property
+    def sealed(self)->bool:
+        return self._sealed
+
+    def set_sealed(self):
+        self._sealed = True
+
     def append_row(self, row: dict, partition_name: str = None):
         msg = "The append_row() interface is not implemented"
         self._print_err(msg)
         raise Exception(msg)
 
     def persist(self, local_path: str):
         msg = "The persist() interface is not implemented"
@@ -177,15 +189,17 @@
             dtype = DataType(field['type'])
             validator = type_validator[dtype.name]
             if dtype == DataType.BINARY_VECTOR or dtype == DataType.FLOAT_VECTOR:
                 dim = field['params']['dim']
                 if not validator(row[k], dim):
                     self._print_err("Illegal vector data for vector field '{}'".format(dtype.name))
                     return False
-                row_size = row_size + len(row[k])
+
+                vec_size = len(row[k])*4 if dtype == DataType.FLOAT_VECTOR else len(row[k])/8
+                row_size = row_size + vec_size
             elif dtype == DataType.VARCHAR:
                 max_len = field['params']['max_length']
                 if not validator(row[k], max_len):
                     self._print_err("Illegal varchar value for field '{}'".format(dtype.name))
                     return False
                 row_size = row_size + len(row[k])
             else:
@@ -200,15 +214,15 @@
 
 
 class RowBuffer(Buffer):
     def __init__(
             self,
             collection_schema: dict,
             partition_name: str = None,
-            logger: Logger = default_logger(),
+            logger: Logger = default_logger,
         ):
         super().__init__(collection_schema=collection_schema, partition_name=partition_name, logger=logger)
         self._buffer = []
 
     @property
     def ingestion_type(self)->IngestionType:
         return IngestionType.ROW_BASED
@@ -222,67 +236,69 @@
         # {"id":1, "vec":[], "$meta": {"x": 5}, "y": 1} --> {"id":1, "vec":[], "x": 5, "y": 1}
         if DYNAMIC_FIELD_NAME in row:
             if isinstance(row[DYNAMIC_FIELD_NAME], dict):
                 dynamic_values = row[DYNAMIC_FIELD_NAME]
                 del row[DYNAMIC_FIELD_NAME]
                 row.update(dynamic_values)
 
-        self._buffer_lock.acquire()
+        if self.sealed:
+            raise IngestionException(code=ErrorCode.BUFFER_SEALED)
         self._buffer.append(row)
-        self._buffer_lock.release()
         return True
 
     def persist(self, local_path: str)->DataInfo:
         full_file_name = os.path.join(local_path, "rows.json")
 
-        self._buffer_lock.acquire()
+        row_count = len(self._buffer)
+        if row_count != self._buffer_row_count:
+            self._print_err("Actual row count {} doesn't equal to calculated row count {}"
+                            .format(row_count, self._buffer_row_count))
+
         content = {
             "rows": self._buffer,
         }
         try:
             with open(full_file_name, 'w', encoding='utf-8') as f:
                 json.dump(obj=content, fp=f, ensure_ascii=False)
             self._print_info("Successfully persist row-based file {}".format(full_file_name))
         except Exception as e:
             self._print_err("Failed to persist row-based file {}, error: {}".format(full_file_name, e))
 
-        self._buffer_lock.release()
-
         info = DataInfo()
         info.collection_name = self.collection_name
         info.partition_name = self.partition_name
         info.local_folder = local_path
         info.ingestion_type = self.ingestion_type
         info.data_size = self.buffer_size
         info.row_count = self.buffer_row_count
         info.local_files = [full_file_name]
+        info.bulkinsert_state = TaskState.Persisted.name
         info.save()
         return info
 
     def pop(self, row_count: int)->list:
         if row_count <= 0:
             self._print_err("Illegal row_count value: {}".format(row_count))
             return []
 
         if len(self._buffer) == 0:
             return []
 
-        self._buffer_lock.acquire()
         rows = self._buffer[:row_count]
         self._buffer = self._buffer[row_count:]
         self._buffer_row_count = len(self._buffer)
-        self._buffer_lock.release()
         return rows
 
+
 class ColumnBuffer(Buffer):
     def __init__(
             self,
             collection_schema: dict,
             partition_name: str = None,
-            logger: Logger = default_logger(),
+            logger: Logger = default_logger,
         ):
         super().__init__(collection_schema=collection_schema, partition_name=partition_name, logger=logger)
         self._buffer = {}
         for field_name in self._target_fields:
             self._buffer[field_name] = []
 
         # dynamic field, internal name is '$meta'
@@ -300,44 +316,54 @@
 
         dynamic_values = {}
         if DYNAMIC_FIELD_NAME in row:
             if not isinstance(row[DYNAMIC_FIELD_NAME], dict):
                 self._print_err("Dynamic field '{}' value should be JSON format".format(DYNAMIC_FIELD_NAME))
                 return False
 
-        self._buffer_lock.acquire()
+        if self.sealed:
+            raise IngestionException(code=ErrorCode.BUFFER_SEALED)
+
         for k in row:
             if k == DYNAMIC_FIELD_NAME:
                 dynamic_values.update(row[k])
                 continue
 
             if k not in self._buffer:
                 dynamic_values[k] = row[k]
             else:
                 self._buffer[k].append(row[k])
 
         self._buffer[DYNAMIC_FIELD_NAME].append(json.dumps(dynamic_values))
-        self._buffer_lock.release()
         return True
 
     def persist(self, local_path: str)-> DataInfo:
         file_list = []
-        self._buffer_lock.acquire()
+        row_count = -1
         for k in self._buffer:
+            if row_count < 0:
+                row_count = len(self._buffer[k])
+            elif row_count != len(self._buffer[k]):
+                self._print_err("Column `{}` row count {} doesn't equal to the first column row count {}"
+                                .format(k, len(self._buffer[k]), row_count))
+
             full_file_name = os.path.join(local_path, k + ".npy")
             file_list.append(full_file_name)
             try:
                 numpy.save(full_file_name, self._buffer[k])
             except Exception as e:
                 self._print_err("Failed to persist column-based file {}, error: {}".format(full_file_name, e))
                 break
 
             self._print_info("Successfully persist column-based file {}".format(full_file_name))
 
-        self._buffer_lock.release()
+        if row_count != self._buffer_row_count:
+            self._print_err("Actual row count {} doesn't equal to calculated row count {}"
+                            .format(row_count, self._buffer_row_count))
+
         if len(file_list) != len(self._buffer):
             self._print_err("Some of fields were not persisted successfully, abort the files")
             for f in file_list:
                 os.unlink(f)
             os.rmdir(local_path)
             file_list.clear()
 
@@ -345,14 +371,15 @@
         info.collection_name = self.collection_name
         info.partition_name =self.partition_name
         info.local_folder = local_path
         info.ingestion_type = self.ingestion_type
         info.data_size = self.buffer_size
         info.row_count = self.buffer_row_count
         info.local_files = file_list
+        info.bulkinsert_state = TaskState.Persisted.name
         info.save()
         return info
 
     def pop(self, row_count: int)->list:
         if row_count <= 0:
             self._print_err("Illegal row_count value: {}".format(row_count))
             return []
@@ -363,15 +390,14 @@
         # avoid an unexpected case that row count of fields are unequal
         total_row_count = len(self._buffer[0])
         for k in self._buffer:
             if len(self._buffer[k]) < total_row_count:
                 total_row_count = len(self._buffer[k])
 
         rows = []
-        self._buffer_lock.acquire()
         for i in range(row_count):
             if i >= total_row_count:
                 break
             row = {}
             for k in self._buffer:
                 if k == DYNAMIC_FIELD_NAME:
                     row.update(self._buffer[k])
@@ -380,107 +406,153 @@
             rows.append(row)
 
         # cut the buffer
         for k in self._buffer:
             self._buffer[k] = self._buffer[k][len(rows):]
 
         self._buffer_row_count = len(self._buffer[0])
-        self._buffer_lock.release()
         return rows
 
 
 class MultiBuffer(Buffer):
     def __init__(
             self,
             collection_schema: dict,
             ingestion_type: IngestionType,
             buffer_max_size: int = 512*MB,
-            logger: Logger = default_logger(),
+            logger: Logger = default_logger,
         ):
         super().__init__(collection_schema=collection_schema,
                          partition_name=None,
                          logger=logger)
         self._ingestion_type = ingestion_type
         self._buffers = {}
         self._buffer_max_size = buffer_max_size
+        self._buffer_lock = Lock()
 
     def set_buffer_max_size(self, max_size: int):
         if max_size <= 0:
             max_size = 512*MB
         self._buffer_max_size = max_size
 
     @property
     def ingestion_type(self)->IngestionType:
         return self._ingestion_type
 
     @property
     def buffer_row_count(self) -> int:
         total_count = 0
-        for k in self._buffers:
-            total_count = total_count + self._buffers[k].buffer_row_count
+        with self._buffer_lock:
+            for k in self._buffers:
+                total_count = total_count + self._buffers[k].buffer_row_count
         return total_count
 
     @property
     def buffer_size(self) -> int:
         total_size = 0
-        for k in self._buffers:
-            total_size = total_size + self._buffers[k].buffer_size
+        with self._buffer_lock:
+            for k in self._buffers:
+                total_size = total_size + self._buffers[k].buffer_size
         return total_size
 
+    def _new_buffer(self, partition_name: str):
+        # here we always create RowBuffer because the append() method of RowBuffer is thread-safe,
+        # we convert RowBuffer to ColumnBuffer when persist() is called.
+        return RowBuffer(collection_schema=self._collection_schema,
+                         partition_name=partition_name,
+                         logger=self._logger)
+
     def append_row(self, row: dict, partition_name: str = None) -> bool:
         if self._collection_schema is None:
             self._print_err("Failed to append row, collection not specified")
             return False
 
         if partition_name is None:
             partition_name = DEFAULT_PARTITION_NAME
 
-        if partition_name not in self._buffers:
-            if self._ingestion_type == IngestionType.ROW_BASED:
-                self._buffers[partition_name] = RowBuffer(collection_schema=self._collection_schema,
-                                                          partition_name=partition_name,
-                                                          logger=self._logger)
-            elif self._ingestion_type == IngestionType.COLUMN_BASED:
-                self._buffers[partition_name] = ColumnBuffer(collection_schema=self._collection_schema,
-                                                             partition_name=partition_name,
-                                                             logger=self._logger)
+        with self._buffer_lock:
+            if partition_name not in self._buffers:
+                self._buffers[partition_name] = self._new_buffer(partition_name=partition_name)
 
-        return self._buffers[partition_name].append_row(row=row)
+        try:
+            ok = self._buffers[partition_name].append_row(row=row)
+            return ok
+        except IngestionException as e:
+            # sealed buffer not allow append, might be in persist process, retry again
+            if e.code == ErrorCode.BUFFER_SEALED:
+                return self._buffers[partition_name].append_row(row=row)
 
     def has_large_buffer(self)->bool:
-        for k in self._buffers:
-            if self._buffers[k].buffer_size >= self._buffer_max_size:
-                return True
+        with self._buffer_lock:
+            for k in self._buffers:
+                if self._buffers[k].buffer_size >= self._buffer_max_size:
+                    return True
         return False
 
+    def _convert_buffer(self, row_buffer: RowBuffer)->ColumnBuffer:
+        if row_buffer.buffer_row_count <= 0:
+            return None
+
+        size_per_row = row_buffer.buffer_size/row_buffer.buffer_row_count
+        if size_per_row < 1:
+            size_per_row = 1
+        batch_row_count = int(8*MB/size_per_row)
+        if batch_row_count < 1:
+            batch_row_count = 1
+
+        new_buffer = ColumnBuffer(collection_schema=row_buffer.collection_schema,
+                                  partition_name=row_buffer.partition_name,
+                                  logger=self._logger)
+        while True:
+            rows = row_buffer.pop(batch_row_count)
+            if len(rows) == 0:
+                break
+            for row in rows:
+                new_buffer.append_row(row)
+
+        return new_buffer
+
     def persist(self, local_path: str, force: bool=False)->List[DataInfo]:
         os.makedirs(name=local_path, exist_ok=True)
-        info_list = []
-        for k in self._buffers:
-            if (not force) and (self._buffers[k].buffer_size < self._buffer_max_size):
-                continue
 
-            if force:
-                self._print_info("Force to persist buffer to local data path"
-                                 .format(self._buffers[k].buffer_size, self._buffer_max_size))
-            else:
-                self._print_info("Buffer size({} bytes) exceeds max size({} bytes), persist to local data path"
-                                 .format(self._buffers[k].buffer_size, self._buffer_max_size))
+        to_persist_buffers = []
+        with self._buffer_lock:
+            for k in self._buffers:
+                if (not force) and (self._buffers[k].buffer_size < self._buffer_max_size):
+                    continue
+
+                if force:
+                    self._print_info("Force to persist buffer to local data path"
+                                     .format(self._buffers[k].buffer_size, self._buffer_max_size))
+                else:
+                    self._print_info("Buffer size({} bytes) exceeds max size({} bytes), persist to local data path"
+                                     .format(self._buffers[k].buffer_size, self._buffer_max_size))
+                to_persist_buffers.append(self._buffers[k])
+                self._buffers[k].set_sealed()
+                self._buffers[k] = self._new_buffer(partition_name=k)
+
+        info_list = []
+        for buffer in to_persist_buffers:
+            if self.ingestion_type == IngestionType.COLUMN_BASED and isinstance(buffer, RowBuffer):
+                new_buffer = self._convert_buffer(buffer)
+                if new_buffer is None:
+                    continue
+                buffer = new_buffer
 
             # create path [local_data_path]/[collection_name]/[partition_name]/[datetime]/
             collection_folder = os.path.join(local_path, self._collection_schema[COLLECTION_NAME_KEY])
             os.makedirs(name=collection_folder, exist_ok=True)
-            partition_folder = os.path.join(collection_folder, k)
+            partition_folder = os.path.join(collection_folder, buffer.partition_name)
             os.makedirs(name=partition_folder, exist_ok=True)
             dt_folder = os.path.join(partition_folder, _current_datetime())
             os.makedirs(name=dt_folder, exist_ok=True)
-            info = self._buffers[k].persist(dt_folder)
+            info = buffer.persist(dt_folder)
             info_list.append(info)
 
-            self._print_info("Successfully persist files: {}".format(info.local_files))
+            self._print_info("Successfully persist files: {} with row count {}".format(info.local_files, info.row_count))
 
         return info_list
 
     def pop(self, row_count: int)->(str, list):
         empty_buffers = []
         partition_name = ""
         pop_rows = []
```

### Comparing `milvus-ingestion-0.4.0/milvus_ingestion/constants.py` & `milvus-ingestion-0.5.0/milvus_ingestion/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,7 +24,16 @@
     COLUMN_BASED = 2
 
 
 class CleanDataOptions(IntEnum):
     CLEAN_SUCCEED_IMPORT_DATA = 1
     CLEAN_FAILED_IMPORT_DATA = 2
     CLEAN_ALL_DATA = CLEAN_SUCCEED_IMPORT_DATA | CLEAN_FAILED_IMPORT_DATA
+
+
+class TaskState(IntEnum):
+    NoState = 0
+    Persisted = 1
+    Uploaded = 2
+    ImportStarted = 3
+    ImportFailed = 4
+    ImportSucceed = 5
```

### Comparing `milvus-ingestion-0.4.0/milvus_ingestion/data_buffer.py` & `milvus-ingestion-0.5.0/milvus_ingestion/data_buffer.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import os
 import shutil
+import threading
 from typing import List
 
 from logging import Logger
-from threading import Lock
+from threading import Lock, Thread
 
 from pymilvus import BulkInsertState
 
 from .util import (
     Base,
     default_logger,
 )
 
 from .constants import (
     IngestionType,
+    TaskState,
     CleanDataOptions,
     OUTPUT_FOLDER,
     DEFAULT_PARTITION_NAME,
     MB,
-    GB,
 )
 
 from .milvus_connector import (
     MilvusConnector,
     default_milvus,
 )
 
@@ -55,29 +56,30 @@
     def __init__(
             self,
             target_collection: str,
             local_data_path: str = OUTPUT_FOLDER,
             milvus_connector: MilvusConnector = default_milvus,
             uploader: Uploader = default_uploader,
             ingestion_type: IngestionType = IngestionType.COLUMN_BASED,
-            logger: Logger = default_logger(),
+            logger: Logger = default_logger,
         ):
         self._args_check(target_collection, local_data_path, milvus_connector, uploader, ingestion_type)
         super().__init__(logger=logger)
         self._local_data_path = local_data_path
         self._milvus_connector = milvus_connector
         self._uploader = uploader
         self._ingestion_type = ingestion_type
         self._buffer_max_size = 512*MB
         self._buffer:MultiBuffer = None # RowBuffer or ColumnBuffer
 
         self._collection_schema = None
         self._set_target_collection(target_collection)
 
-        self._upload_lock = Lock()
+        self._bulkinsert_lock = Lock()
+        self._working_thread = {}
 
     def _args_check(self,
                     target_collection: str,
                     local_data_path: str,
                     milvus_connector: MilvusConnector,
                     uploader: Uploader,
                     ingestion_type: IngestionType,
@@ -97,14 +99,15 @@
         if not isinstance(ingestion_type, IngestionType):
             _raise_err("illegal ingestion type: {}".format(ingestion_type))
 
     def set_buffer_max_size(self, max_size: int):
         if max_size <= 0:
             max_size = 512*MB
         self._buffer_max_size = max_size
+
         if self._buffer is not None:
             self._buffer.set_buffer_max_size(self._buffer_max_size)
 
     def _set_target_collection(self, collection_name: str):
         if self._milvus_connector is None:
             msg = "Milvus connector is None"
             self._print_err(msg)
@@ -124,42 +127,44 @@
 
     def append_row(self, row: dict, partition_name: str = None)->bool:
         if self._buffer is None:
             msg = "Failed to append row, collection not specified"
             self._print_err(msg)
             raise Exception(msg)
 
-        if not self._buffer.append_row(row=row, partition_name=partition_name):
+        ok = self._buffer.append_row(row=row, partition_name=partition_name)
+        if not ok:
             return False
 
         if self._buffer.has_large_buffer():
-            info_list = self._persist(force=False)
-            for info in info_list:
-                self._upload_import(info)
+            self._persist(force=False, _async=True)
 
         return True
 
-    def current_row_count(self):
-        return self._buffer.buffer_row_count
+    def current_row_count(self)->int:
+        count = self._buffer.buffer_row_count
+        return count
 
-    def _persist(self, force: bool)->List[DataInfo]:
+    def _persist(self, force: bool, _async: bool=False)->List[DataInfo]:
         os.makedirs(name=self._local_data_path, exist_ok=True)
 
-        to_persist_buffer = self._buffer
-        self._buffer = MultiBuffer(collection_schema=self._collection_schema,
-                                   ingestion_type=self._ingestion_type,
-                                   logger=self._logger)
-
-        info_list = to_persist_buffer.persist(local_path=self._local_data_path, force=force)
-        if len(info_list) == 0:
-            self._print_info("Nothing to persist")
+        def _call_persist():
+            self._working_thread[threading.current_thread().name] = threading.current_thread()
+            infos = self._buffer.persist(local_path=self._local_data_path, force=force)
+            self._print_info("Successfully persist {}, {} data blocks are persisted"
+                             .format(self._local_data_path, len(infos)))
+            del self._working_thread[threading.current_thread().name]
+            return infos
+
+        if _async:
+            x = Thread(target=_call_persist, args=())
+            x.start()
             return []
-
-        self._print_info("Successfully persist, buffer is reset")
-        return info_list
+        else:
+            return _call_persist()
 
     def persist(self) -> List[str]:
         info_list = self._persist(force=True)
         return [info.local_folder for info in info_list]
 
     def _update_info(self, info: DataInfo):
         ok, msg = info.save()
@@ -174,50 +179,52 @@
         if self._uploader is None:
             self._print_err("Uploader is None")
             return 0
 
         if self._milvus_connector is not None:
             ok, msg = self._milvus_connector.verify_input(info.collection_name, info.partition_name)
             if not ok:
-                msg = "Unable to import files {}, error: {}".format(info.local_files, msg)
-                self._print_err(msg)
-                info.bulkinsert_done = False
-                info.bulkinsert_err = msg
+                self._print_err("Unable to import files {}, error: {}".format(info.local_files, msg))
+                info.bulkinsert_state = TaskState.ImportFailed.name
+                info.bulkinsert_err = "Unable to import files, error: {}".format(msg)
                 self._update_info(info)
                 return 0
 
         # upload files
-        ok, remote_files = self._uploader.upload(files=info.local_files, relative_path=self._local_data_path)
+        ok, remote_files, err = self._uploader.upload(files=info.local_files, relative_path=self._local_data_path)
         if not ok:
-            msg = "Failed to upload files {}".format(info.local_files)
-            self._print_err(msg)
-            info.bulkinsert_done = False
-            info.bulkinsert_err = msg
+            self._print_err("Failed to upload files {}, error: {}".format(info.local_files, err))
+            info.bulkinsert_state = TaskState.ImportFailed.name
+            info.bulkinsert_err = "Failed to upload files, error: {}".format(err)
             self._update_info(info)
             return 0
 
+        info.bulkinsert_state = TaskState.Uploaded.name
+        self._update_info(info)
+
         if self._milvus_connector is None:
             self._print_err("Milvus connector is None")
             return 0
 
         # call bulkinsert
         partition_name = None if info.partition_name == DEFAULT_PARTITION_NAME else info.partition_name
         task_id, msg = self._milvus_connector.bulk_insert(files=remote_files,
                                                           collection_name=info.collection_name,
                                                           partition_name=partition_name)
         if task_id == 0:
             self._print_err("Failed to import to collection '{}', partition '{}', error: {}"
                             .format(info.collection_name, partition_name, msg))
-            info.bulkinsert_done = False
+            info.bulkinsert_state = TaskState.ImportFailed.name
             info.bulkinsert_err = msg
             return 0
         self._print_info("Start a bulkinsert task to import files {}, task id: {}".format(remote_files, task_id))
 
         # write infomation into a json file
         info.bulkinsert_id = task_id
+        info.bulkinsert_state = TaskState.ImportStarted.name
         info.remote_files = remote_files
         ok, msg = info.save()
         if not ok:
             self._print_err(msg)
 
         return task_id
 
@@ -225,63 +232,76 @@
         if self._uploader is None:
             self._print_err("Uploader is None")
             return []
 
         if data_folder is None:
             data_folder = self._local_data_path
 
+        # wait all persist task finished
+        for x in self._working_thread:
+            if x is not None:
+                x.join()
+
         task_list = []
-        info_list = self._list_bulkinsert_tasks(data_folder)
-        for info in info_list:
-            if info.bulkinsert_done:
-                continue
+        # the lock is to avoid duplicated bulkinsert task, only allow one thread run into this section
+        with self._bulkinsert_lock:
+            info_list = self._list_bulkinsert_tasks(data_folder)
+            for info in info_list:
+                if (info.bulkinsert_state == TaskState.ImportStarted.name)\
+                        or (info.bulkinsert_state == TaskState.ImportSucceed.name):
+                    continue
 
-            task_id = self._upload_import(info)
-            if task_id > 0:
-                task_list.append(task_id)
+                task_id = self._upload_import(info)
+                if task_id > 0:
+                    task_list.append(task_id)
 
         return task_list
 
     def wait_upload_finish(self, task_list: List[int]=None)->bool:
         if self._milvus_connector is None:
             self._print_err("Milvus connector is None")
             return False
 
         wait_info_list = []
         # find out the unfinished tasks
         all_info_list = self._list_bulkinsert_tasks()
         for info in all_info_list:
-            if info.bulkinsert_id is None or info.bulkinsert_done:
+            if (info.bulkinsert_id is None) or (info.bulkinsert_state != TaskState.ImportStarted.name):
                 continue
             if task_list is not None:
                 if info.bulkinsert_id in task_list:
                     wait_info_list.append(info)
             else:
                 wait_info_list.append(info)
 
+        if len(wait_info_list) == 0:
+            return True
+
         # wait the unfinished tasks
         collection_list = []
         for info in wait_info_list:
             if info.collection_name not in collection_list:
                 collection_list.append(info.collection_name)
             state = self._milvus_connector.wait_bulkinsert_task(info.bulkinsert_id)
-            if state.state == BulkInsertState.ImportCompleted:
+            if state is None:
+                self._print_err("Unable to get state of bulklinsert task {}")
+                info.bulkinsert_state = TaskState.ImportFailed.name
+                info.bulkinsert_err = "Unable to get state of bulklinsert task"
+            elif state.state == BulkInsertState.ImportCompleted:
                 self._print_info("Bulklinsert task {} completed".format(info.bulkinsert_id))
-                info.bulkinsert_done = True
+                info.bulkinsert_state = TaskState.ImportSucceed.name
                 info.bulkinsert_pk_ranges = list(state.id_ranges)
             elif state.state == BulkInsertState.ImportFailed or state.state == BulkInsertState.ImportFailedAndCleaned:
                 self._print_err("Bulklinsert task {} failed with reason: {}"
-                                .format(info.bulkinsert_id, info.bulkinsert_err))
-                info.bulkinsert_done = False
+                                .format(info.bulkinsert_id, state.failed_reason))
+                info.bulkinsert_state = TaskState.ImportFailed.name
                 info.bulkinsert_err = state.failed_reason
 
             # update the info
-            ok, msg = info.save()
-            if not ok:
-                self._print_err(msg)
+            self._update_info(info)
 
         # refresh load the collections
         self._milvus_connector.refresh_load(collection_list)
         return True
 
     def _list_bulkinsert_tasks(self, data_folder: str=None)->List[DataInfo]:
         if data_folder is None:
@@ -299,68 +319,78 @@
         return info_list
 
     def list_bulkinsert_tasks(self) -> List[dict]:
         info_list = self._list_bulkinsert_tasks(self._local_data_path)
         return [info.to_dict() for info in info_list]
 
     def clear_data_folder(self, options: CleanDataOptions=CleanDataOptions.CLEAN_SUCCEED_IMPORT_DATA):
-        self._print_warn("Clear the data folder '{}', all the local data will be deleted".format(self._local_data_path))
+        self._print_warn("Clear the data folder '{}' with option {}".format(self._local_data_path, options))
 
-        def _remove_files(info: DataInfo):
-            if len(info.local_files) > 0:
-                for file in info.local_files:
-                    os.remove(file)
-            if len(info.remote_files) > 0:
-                if self._uploader != None:
-                    self._uploader.remove(info.remote_files)
-            shutil.rmtree(info.local_folder)
-
-        sub_paths = os.listdir(self._local_data_path)
-        for p in sub_paths:
-            full_path = os.path.join(self._local_data_path, p)
-            if os.path.isdir(full_path):
-                if options == CleanDataOptions.CLEAN_ALL_DATA:
-                    shutil.rmtree(full_path)
-                    continue
+        def _is_dir_empty(dir_path: str):
+            return len(os.listdir(dir_path)) == 0
 
-                info_list = self._list_bulkinsert_tasks(full_path)
-                for info in info_list:
-                    if info.bulkinsert_done and (options & CleanDataOptions.CLEAN_SUCCEED_IMPORT_DATA):
-                        _remove_files(info)
-                    if (not info.bulkinsert_done) and (options & CleanDataOptions.CLEAN_FAILED_IMPORT_DATA):
-                        _remove_files(info)
+        def _remove_files(info: DataInfo):
+            try:
+                if len(info.local_files) > 0:
+                    for file in info.local_files:
+                        os.remove(file)
+                if len(info.remote_files) > 0:
+                    if self._uploader != None:
+                        self._uploader.remove(info.remote_files)
+                shutil.rmtree(info.local_folder)
+                parent_dir = os.path.dirname(info.local_folder.rstrip('/'))
+                if _is_dir_empty(parent_dir):
+                    os.rmdir(parent_dir)
+            except Exception as e:
+                self._print_err("Failed to delete files of data folder {}, error: {}".format(info.local_folder, e))
+
+        try:
+            sub_paths = os.listdir(self._local_data_path)
+            for p in sub_paths:
+                full_path = os.path.join(self._local_data_path, p)
+                if os.path.isdir(full_path):
+                    if options == CleanDataOptions.CLEAN_ALL_DATA:
+                        shutil.rmtree(full_path)
+                        continue
+
+                    info_list = self._list_bulkinsert_tasks(full_path)
+                    for info in info_list:
+                        if (info.bulkinsert_state == TaskState.ImportSucceed.name)\
+                                and (options & CleanDataOptions.CLEAN_SUCCEED_IMPORT_DATA):
+                            _remove_files(info)
+                        if (info.bulkinsert_state == TaskState.ImportFailed.name)\
+                                and (options & CleanDataOptions.CLEAN_FAILED_IMPORT_DATA):
+                            _remove_files(info)
+                    if _is_dir_empty(full_path):
+                        os.rmdir(full_path)
+        except Exception as e:
+            self._print_err("Failed to clear data folder, error: {}".format(e))
 
-    def direct_insert(self)->list:
+    def direct_insert(self)->List[int]:
         if self._milvus_connector is None:
             self._print_err("Milvus connector is None")
             return []
 
         row_count = self._buffer.buffer_row_count
         if self._buffer is None or row_count == 0:
             self._print_err("Buffer is empty")
             return []
 
-        # reset the buffer
-        to_persist_buffer = self._buffer
-        self._buffer = MultiBuffer(collection_schema=self._collection_schema,
-                                   ingestion_type=self._ingestion_type,
-                                   logger=self._logger)
-
-        size_per_row = to_persist_buffer.buffer_size/row_count
+        size_per_row = self._buffer.buffer_size/row_count
         batch = int(8*MB/size_per_row)
         if batch > row_count:
             batch = row_count
 
         self._print_info("{} rows in buffer, prepare to insert batch by batch, {} rows per batch"
                          .format(row_count, batch))
 
-        collection_name = to_persist_buffer.collection_name
+        collection_name = self._buffer.collection_name
         primary_ids = []
         while True:
-            partition_name, rows = to_persist_buffer.pop(batch)
+            partition_name, rows = self._buffer.pop(batch)
             if len(rows) == 0:
                 break
 
             if (partition_name == DEFAULT_PARTITION_NAME) or (len(partition_name) == 0):
                 partition_name = None
             ids = self._milvus_connector.insert(data=rows,
                                                 collection_name=collection_name,
```

### Comparing `milvus-ingestion-0.4.0/milvus_ingestion/milvus_connector.py` & `milvus-ingestion-0.5.0/milvus_ingestion/milvus_connector.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             host: str = None,
             port: str = None,
             secure: bool = False,
             client_key_path: str = None,
             ca_pem_path: str = None,
             server_pem_path: str = None,
             server_name: str = None,
-            logger: Logger = default_logger(),
+            logger: Logger = default_logger,
         ):
         super().__init__(logger=logger)
         self._address = address
         self._alias = alias
         self._user = user
         self._password = password
         self._db_name = db_name
@@ -145,22 +145,23 @@
                 state = utility.get_bulk_insert_state(task_id=task_id)
                 if state.state == BulkInsertState.ImportFailed \
                         or state.state == BulkInsertState.ImportFailedAndCleaned:
                     self._print_err("The bulkinsert task {} failed, reason: {}"
                                     .format(state.task_id, state.failed_reason))
                     return state
                 elif state.state == BulkInsertState.ImportCompleted:
-                    self._print_info("The bulkinsert task {} is done, {} rows were persisted into collection '{}' partition '{}'"
+                    self._print_info("The bulkinsert task {} is done, {} rows were imported into collection '{}' partition '{}'"
                                      .format(task_id, state.row_count, state.collection_name, state.partition_name))
                     return state
             except Exception as e:
                 self._print_err("Failed to get state of bulkinsert task {}, error: {}".format(task_id, e))
                 break
 
             time.sleep(1)
+        return None
 
     def refresh_load(self, collection_list: List[str]):
         for collection_name in collection_list:
             state = utility.load_state(collection_name=collection_name)
             if state == LoadState.Loaded:
                 self._print_info("Waiting for the new data be fully indexed in collection '{}' ..."
                                  .format(collection_name))
```

### Comparing `milvus-ingestion-0.4.0/milvus_ingestion/uploader.py` & `milvus-ingestion-0.5.0/milvus_ingestion/uploader.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import os
+import time
 
 from minio import Minio
 from minio.error import S3Error
+from minio.error import MinioException
 from logging import Logger
 from typing import List
 
 from .util import (
     Base,
     default_logger,
 )
 
 DEFAULT_BUCKET_NAME = "a-bucket"
 DEFAULT_REMOTE_PATH = "milvus-ingestion"
 
 class Uploader(Base):
-    def __init__(self, logger: Logger = default_logger()):
+    def __init__(self, logger: Logger = default_logger):
         self._logger = logger
 
     def upload(self,
                files: List[str],
                relative_path: str):
         msg = "The upload() interface of Uploader is not implemented"
         self._print_err(msg)
@@ -37,26 +39,28 @@
     def remove(self, files: List[str]):
         msg = "The remove() interface of Uploader is not implemented"
         self._print_err(msg)
         raise Exception(msg)
 
 
 class MinioUploader(Base):
-    def __init__(self,
-                 bucket_name: str=DEFAULT_BUCKET_NAME,
-                 remote_path: str=DEFAULT_REMOTE_PATH,
-                 endpoint: str=None,
-                 access_key: str=None,
-                 secret_key: str=None,
-                 secure: bool=True,
-                 session_token: str=None,
-                 region: str=None,
-                 http_client=None,
-                 credentials=None,
-                 logger: Logger = default_logger()):
+    def __init__(
+            self,
+            bucket_name: str=DEFAULT_BUCKET_NAME,
+            remote_path: str=DEFAULT_REMOTE_PATH,
+            endpoint: str=None,
+            access_key: str=None,
+            secret_key: str=None,
+            secure: bool=True,
+            session_token: str=None,
+            region: str=None,
+            http_client=None,
+            credentials=None,
+            logger: Logger = default_logger
+         ):
         super().__init__(logger=logger)
         self._client = None
         self._bucket_name = bucket_name
         self._remote_path = remote_path
         self._endpoint = endpoint
         self._access_key = access_key
         self._secret_key = secret_key
@@ -76,43 +80,57 @@
                                  secure=arg_parse(self._secure),
                                  session_token=arg_parse(self._session_token),
                                  region=arg_parse(self._region),
                                  http_client=arg_parse(self._http_client),
                                  credentials=arg_parse(self._credentials))
         return self._client
 
+    def _exists(self, file: str)->bool:
+        try:
+            minio_client = self._get_client()
+            minio_client.stat_object(bucket_name=self._bucket_name, object_name=file)
+            return True
+        except MinioException as err:
+            return False
+
     def upload(self, files: List[str],
-               relative_path: str)->(bool, List[str]):
+               relative_path: str)->(bool, List[str], str):
         remote_files = []
         try:
             self._print_info("Prepare upload files")
             minio_client = self._get_client()
             found = minio_client.bucket_exists(self._bucket_name)
             if not found:
-                self._print_err("MinIO bucket '{}' doesn't exist".format(self._bucket_name))
-                return False, []
+                msg = "MinIO bucket '{}' doesn't exist".format(self._bucket_name)
+                self._print_err(msg)
+                return False, [], msg
 
             for file_path in files:
                 ext = os.path.splitext(file_path)
                 if len(ext) != 2 or (ext[1] != ".json" and ext[1] != ".npy"):
                     continue
 
                 relative_file_path = file_path.strip(relative_path).lstrip('/')
                 minio_file_path = os.path.join(self._remote_path, relative_file_path)
-                minio_client.fput_object(bucket_name=self._bucket_name,
-                                         object_name=minio_file_path,
-                                         file_path=file_path)
-                self._print_info("Upload file '{}' to '{}'".format(file_path, minio_file_path))
+
+                if not self._exists(minio_file_path):
+                    minio_client.fput_object(bucket_name=self._bucket_name,
+                                             object_name=minio_file_path,
+                                             file_path=file_path)
+                    self._print_info("Upload file '{}' to '{}'".format(file_path, minio_file_path))
+                else:
+                    self._print_info("Remote file '{}' already exists".format(minio_file_path))
                 remote_files.append(minio_file_path)
         except Exception as e:
-            self._print_err("Failed to call MinIO/S3 api, error: {}".format(e))
-            return False, []
+            msg = "Failed to call MinIO/S3 api, error: {}".format(e)
+            self._print_err(msg)
+            return False, [], msg
 
         self._print_info("Successfully upload files: {}".format(files))
-        return True, remote_files
+        return True, remote_files, ""
 
     def remove(self, files: List[str])->bool:
         try:
             self._print_info("Prepare delete remote files")
             minio_client = self._get_client()
             found = minio_client.bucket_exists(self._bucket_name)
             if not found:
```

### Comparing `milvus-ingestion-0.4.0/milvus_ingestion/util.py` & `milvus-ingestion-0.5.0/milvus_ingestion/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,40 +8,36 @@
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 
 import datetime
 import logging
 from logging import Logger
 
-defaultLogger = logging.getLogger()
+default_logger = logging.getLogger()
 fmt = '%(asctime)s|%(funcName)s|%(lineno)s|%(levelname)s|%(message)s'
 formatter = logging.Formatter(fmt)
 handler = logging.StreamHandler()
 handler.setFormatter(formatter)
-defaultLogger.addHandler(handler)
-defaultLogger.setLevel('DEBUG')
-
-
-def default_logger()->Logger:
-    return defaultLogger
+default_logger.addHandler(handler)
+default_logger.setLevel('DEBUG')
 
 
 def _current_datetime() -> str:
     dt = datetime.datetime.now()
     return dt.strftime('%Y-%m-%d_%H:%M:%S.%f')
 
 
 class Base:
-    def __init__(self, logger: Logger = default_logger()):
+    def __init__(self, logger: Logger = default_logger):
         self._logger = logger
 
     def _print_info(self, msg):
         if self._logger:
             self._logger.info(msg)
 
     def _print_warn(self, msg):
         if self._logger:
             self._logger.warning(msg)
 
     def _print_err(self, msg):
         if self._logger:
-            self._logger.error(msg)
+            self._logger.error(msg)
```

### Comparing `milvus-ingestion-0.4.0/setup.py` & `milvus-ingestion-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / 'README.md').read_text()
 
 setuptools.setup(
     name="milvus-ingestion",
-    version="0.4.0",
+    version="0.5.0",
     author='yihua.mo',
     author_email='yihua.mo@zilliz.com',
     description="A tool to help data ingestion for Milvus",
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/yhmo/milvus-ingestion',
     license="Apache-2.0",
```

