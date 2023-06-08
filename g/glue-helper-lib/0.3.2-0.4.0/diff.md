# Comparing `tmp/glue_helper_lib-0.3.2.tar.gz` & `tmp/glue_helper_lib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_helper_lib-0.3.2.tar", max compression
+gzip compressed data, was "glue_helper_lib-0.4.0.tar", max compression
```

## Comparing `glue_helper_lib-0.3.2.tar` & `glue_helper_lib-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-03-25 11:21:46.068544 glue_helper_lib-0.3.2/LICENSE
--rw-r--r--   0        0        0       61 2023-04-09 13:42:48.332388 glue_helper_lib-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-03-25 11:33:42.478539 glue_helper_lib-0.3.2/glue_helper_lib/__init__.py
--rw-r--r--   0        0        0     1714 2023-04-09 13:08:52.592360 glue_helper_lib-0.3.2/glue_helper_lib/arguments.py
--rw-r--r--   0        0        0        0 2023-04-29 15:40:12.399875 glue_helper_lib-0.3.2/glue_helper_lib/hudi/__init__.py
--rw-r--r--   0        0        0     8811 2023-04-30 14:55:32.831653 glue_helper_lib-0.3.2/glue_helper_lib/hudi/config.py
--rw-r--r--   0        0        0     1148 2023-05-02 12:40:59.679248 glue_helper_lib-0.3.2/glue_helper_lib/hudi/session.py
--rw-r--r--   0        0        0     1899 2023-04-30 14:55:09.631653 glue_helper_lib-0.3.2/glue_helper_lib/hudi/table.py
--rw-r--r--   0        0        0     1163 2023-04-09 13:56:20.652399 glue_helper_lib-0.3.2/glue_helper_lib/logging.py
--rw-r--r--   0        0        0      700 2023-05-02 12:38:54.926123 glue_helper_lib-0.3.2/glue_helper_lib/session.py
--rw-r--r--   0        0        0     1562 2023-05-02 15:07:44.250302 glue_helper_lib-0.3.2/glue_helper_lib/table.py
--rw-r--r--   0        0        0      711 2023-05-02 15:44:35.083278 glue_helper_lib-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 glue_helper_lib-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-25 11:21:46.068544 glue_helper_lib-0.4.0/LICENSE
+-rw-r--r--   0        0        0       61 2023-04-09 13:42:48.332388 glue_helper_lib-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-25 11:33:42.478539 glue_helper_lib-0.4.0/glue_helper_lib/__init__.py
+-rw-r--r--   0        0        0     1714 2023-04-09 13:08:52.592360 glue_helper_lib-0.4.0/glue_helper_lib/arguments.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:40:12.399875 glue_helper_lib-0.4.0/glue_helper_lib/hudi/__init__.py
+-rw-r--r--   0        0        0     8811 2023-04-30 14:55:32.831653 glue_helper_lib-0.4.0/glue_helper_lib/hudi/config.py
+-rw-r--r--   0        0        0     1148 2023-05-02 12:40:59.679248 glue_helper_lib-0.4.0/glue_helper_lib/hudi/session.py
+-rw-r--r--   0        0        0     2005 2023-06-08 15:16:47.875481 glue_helper_lib-0.4.0/glue_helper_lib/hudi/table.py
+-rw-r--r--   0        0        0     1163 2023-05-03 09:40:20.828320 glue_helper_lib-0.4.0/glue_helper_lib/logging.py
+-rw-r--r--   0        0        0      700 2023-05-02 12:38:54.926123 glue_helper_lib-0.4.0/glue_helper_lib/session.py
+-rw-r--r--   0        0        0     1562 2023-05-02 15:07:44.250302 glue_helper_lib-0.4.0/glue_helper_lib/table.py
+-rw-r--r--   0        0        0      711 2023-06-08 15:51:53.095481 glue_helper_lib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 glue_helper_lib-0.4.0/PKG-INFO
```

### Comparing `glue_helper_lib-0.3.2/LICENSE` & `glue_helper_lib-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.3.2/glue_helper_lib/arguments.py` & `glue_helper_lib-0.4.0/glue_helper_lib/arguments.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.3.2/glue_helper_lib/hudi/config.py` & `glue_helper_lib-0.4.0/glue_helper_lib/hudi/config.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.3.2/glue_helper_lib/hudi/session.py` & `glue_helper_lib-0.4.0/glue_helper_lib/hudi/session.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.3.2/glue_helper_lib/hudi/table.py` & `glue_helper_lib-0.4.0/glue_helper_lib/hudi/table.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,54 +8,58 @@
 
 @dataclasses.dataclass
 class Partitioning:
     partition_column: typing.Optional[str]
     is_datetime: bool
 
 
+class WriteMode(enum.Enum):
+    OVERWRITE = "overwrite"
+    UPSERT = "upsert"
+
+
 @dataclasses.dataclass
-class HudiTableArguments:
-    storage_location: table.StorageLocation
+class WriteHudiTableArguments:
     catalog: table.GlueCatalogArguments
     index_type: config.IndexType
     table_type: config.TableType
     record_key_colums: typing.List[str]
     precombine_column: str
     partitioning: Partitioning
-
-
-class WriteMode(enum.Enum):
-    OVERWRITE = "overwrite"
-    UPSERT = "upsert"
+    write_mode: WriteMode
 
 
 class HudiGlueTable:
     _write_mode_to_mode_string = {
         WriteMode.OVERWRITE: "overwrite",
         WriteMode.UPSERT: "append",
     }
 
-    def __init__(self, table_arguments: HudiTableArguments) -> None:
-        self._args = table_arguments
-        self._hudi_config = config.get_hudi_options(
-            database_name=self._args.catalog.database,
-            table_name=self._args.catalog.table,
-            hudi_table_path=str(self._args.storage_location),
-            table_type=self._args.table_type,
-            index_type=self._args.index_type,
-            record_key_columns=self._args.record_key_colums,
-            precombine_column_name=self._args.precombine_column,
-            partition_key_column_name=self._args.partitioning.partition_column,
-            partitioned_on_datetime=self._args.partitioning.is_datetime,
+    def __init__(self, storage_location: table.StorageLocation) -> None:
+        self._storage_location = storage_location
+
+    def _get_hudi_config(self, write_args: WriteHudiTableArguments):
+        return config.get_hudi_options(
+            database_name=write_args.catalog.database,
+            table_name=write_args.catalog.table,
+            hudi_table_path=str(self._storage_location),
+            table_type=write_args.table_type,
+            index_type=write_args.index_type,
+            record_key_columns=write_args.record_key_colums,
+            precombine_column_name=write_args.precombine_column,
+            partition_key_column_name=write_args.partitioning.partition_column,
+            partitioned_on_datetime=write_args.partitioning.is_datetime,
         )
 
-    def write(self, df: pyspark.sql.DataFrame, write_mode: WriteMode):
-        df.write.format("hudi").options(**self._hudi_config).mode(
-            self._write_mode_to_mode_string[write_mode]
-        ).save()
+    def write(
+        self, df: pyspark.sql.DataFrame, write_args: WriteHudiTableArguments
+    ):
+        df.write.format("hudi").options(
+            **self._get_hudi_config(write_args)
+        ).mode(self._write_mode_to_mode_string[write_args.write_mode]).save()
 
     def read(
         self, spark_session: pyspark.sql.SparkSession
     ) -> pyspark.sql.DataFrame:
         return spark_session.read.format("hudi").load(
-            str(self._args.storage_location)
+            str(self._storage_location)
         )
```

### Comparing `glue_helper_lib-0.3.2/glue_helper_lib/logging.py` & `glue_helper_lib-0.4.0/glue_helper_lib/logging.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.3.2/glue_helper_lib/session.py` & `glue_helper_lib-0.4.0/glue_helper_lib/session.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.3.2/glue_helper_lib/table.py` & `glue_helper_lib-0.4.0/glue_helper_lib/table.py`

 * *Files identical despite different names*

### Comparing `glue_helper_lib-0.3.2/pyproject.toml` & `glue_helper_lib-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-helper-lib"
-version = "0.3.2"
+version = "0.4.0"
 description = "A library containing multiple helper and utility functionalities for AWS Glue"
 authors = ["Martijn Sturm <martijn.sturm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "glue_helper_lib" }]
 
 [tool.poetry.dependencies]
```

### Comparing `glue_helper_lib-0.3.2/PKG-INFO` & `glue_helper_lib-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-helper-lib
-Version: 0.3.2
+Version: 0.4.0
 Summary: A library containing multiple helper and utility functionalities for AWS Glue
 License: MIT
 Author: Martijn Sturm
 Author-email: martijn.sturm@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

