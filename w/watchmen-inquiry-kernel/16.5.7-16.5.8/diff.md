# Comparing `tmp/watchmen_inquiry_kernel-16.5.7.tar.gz` & `tmp/watchmen_inquiry_kernel-16.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_kernel-16.5.7.tar", max compression
+gzip compressed data, was "watchmen_inquiry_kernel-16.5.8.tar", max compression
```

## Comparing `watchmen_inquiry_kernel-16.5.7.tar` & `watchmen_inquiry_kernel-16.5.8.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1061 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/LICENSE
--rw-r--r--   0        0        0     1275 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/__init__.py
--rw-r--r--   0        0        0      112 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/common/__init__.py
--rw-r--r--   0        0        0       47 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/common/exception.py
--rw-r--r--   0        0        0      620 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/common/settings.py
--rw-r--r--   0        0        0       86 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/meta/enum_service.py
--rw-r--r--   0        0        0     1404 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/meta/report_service.py
--rw-r--r--   0        0        0     2358 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/meta/subject_service.py
--rw-r--r--   0        0        0       82 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/schema/__init__.py
--rw-r--r--   0        0        0     2178 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/schema/report_schema.py
--rw-r--r--   0        0        0    12544 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/schema/subject_schema.py
--rw-r--r--   0        0        0      104 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/storage/__init__.py
--rw-r--r--   0        0        0     1769 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/storage/report_data_service.py
--rw-r--r--   0        0        0     1496 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/storage/subject_data_service.py
--rw-r--r--   0        0        0    55779 2023-06-07 11:34:15.619986 watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/storage/subject_storage.py
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 watchmen_inquiry_kernel-16.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/LICENSE
+-rw-r--r--   0        0        0     1275 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/common/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/common/exception.py
+-rw-r--r--   0        0        0      620 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/common/settings.py
+-rw-r--r--   0        0        0      289 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/common/utils.py
+-rw-r--r--   0        0        0       86 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/enum_service.py
+-rw-r--r--   0        0        0     1404 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/report_service.py
+-rw-r--r--   0        0        0     2358 2023-06-08 03:33:39.195630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/subject_service.py
+-rw-r--r--   0        0        0       82 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/schema/__init__.py
+-rw-r--r--   0        0        0     2178 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/schema/report_schema.py
+-rw-r--r--   0        0        0    12544 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/schema/subject_schema.py
+-rw-r--r--   0        0        0      104 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     1769 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/report_data_service.py
+-rw-r--r--   0        0        0     1496 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/subject_data_service.py
+-rw-r--r--   0        0        0    55853 2023-06-08 03:33:39.199630 watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/subject_storage.py
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 watchmen_inquiry_kernel-16.5.8/PKG-INFO
```

### Comparing `watchmen_inquiry_kernel-16.5.7/LICENSE` & `watchmen_inquiry_kernel-16.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/common/settings.py` & `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/meta/enum_service.py` & `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/enum_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/meta/report_service.py` & `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/report_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/meta/subject_service.py` & `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/meta/subject_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/schema/report_schema.py` & `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/schema/report_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/schema/subject_schema.py` & `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/schema/subject_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/storage/report_data_service.py` & `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/report_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/storage/subject_data_service.py` & `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/subject_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.7/src/watchmen_inquiry_kernel/storage/subject_storage.py` & `watchmen_inquiry_kernel-16.5.8/src/watchmen_inquiry_kernel/storage/subject_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import abstractmethod
 from datetime import date
 from decimal import Decimal
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
+from watchmen_inquiry_kernel.common.utils import process_sql
 from watchmen_pipeline_kernel.pipeline.sql_performance_invoker import create_sql_performance_pipeline_invoker
 
 from watchmen_auth import PrincipalService
 from watchmen_data_kernel.common import ask_all_date_formats, ask_time_formats
 from watchmen_data_kernel.service import ask_topic_storage
 from watchmen_data_kernel.storage_bridge import ask_topic_data_entity_helper, parse_condition_for_storage, \
 	parse_parameter_for_storage, ParsedStorageCondition, PipelineVariables, PossibleParameterType
@@ -1198,15 +1199,15 @@
 
 	def aggregate_find_sql(self, report_schema: ReportSchema) -> str:
 		aggregator = self.ask_storage_aggregator(report_schema)
 		sql_monitor = SqlHandler()
 		aggregator.commandOnly = True
 		aggregator.queryPfmMonitor = sql_monitor.create_monitor()
 		self.find_data(lambda agent: agent.free_aggregate_find(aggregator))
-		return sql_monitor.sql
+		return process_sql(sql_monitor.sql)
 
 	def ask_storage_aggregate_pager(
 			self, report_schema: ReportSchema, pageable: Pageable) -> FreeAggregatePager:
 		aggregator = self.ask_storage_aggregator(report_schema)
 		return FreeAggregatePager(
 			columns=aggregator.columns,
 			joins=aggregator.joins,
```

### Comparing `watchmen_inquiry_kernel-16.5.7/PKG-INFO` & `watchmen_inquiry_kernel-16.5.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-kernel
-Version: 16.5.7
+Version: 16.5.8
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,16 +15,16 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-data-kernel (==16.5.7)
-Requires-Dist: watchmen-inquiry-trino (==16.5.7) ; extra == "trino"
-Requires-Dist: watchmen-storage-mongodb (==16.5.7) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.7) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.7) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.7) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.7) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.7) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.7) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.5.8)
+Requires-Dist: watchmen-inquiry-trino (==16.5.8) ; extra == "trino"
+Requires-Dist: watchmen-storage-mongodb (==16.5.8) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.8) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.8) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.8) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.8) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.8) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.8) ; extra == "s3"
```

