# Comparing `tmp/watchmen_storage_mysql-16.5.7.tar.gz` & `tmp/watchmen_storage_mysql-16.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_mysql-16.5.7.tar", max compression
+gzip compressed data, was "watchmen_storage_mysql-16.5.8.tar", max compression
```

## Comparing `watchmen_storage_mysql-16.5.7.tar` & `watchmen_storage_mysql-16.5.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-06-07 11:34:15.651987 watchmen_storage_mysql-16.5.7/LICENSE
--rw-r--r--   0        0        0      485 2023-06-07 11:34:15.651987 watchmen_storage_mysql-16.5.7/pyproject.toml
--rw-r--r--   0        0        0      258 2023-06-07 11:34:15.651987 watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/__init__.py
--rw-r--r--   0        0        0     2836 2023-06-07 11:34:15.651987 watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/data_source_mysql.py
--rw-r--r--   0        0        0     2197 2023-06-07 11:34:15.651987 watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/script_builder_mysql.py
--rw-r--r--   0        0        0     5301 2023-06-07 11:34:15.651987 watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/storage_mysql.py
--rw-r--r--   0        0        0     1965 2023-06-07 11:34:15.651987 watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/storage_mysql_configuration.py
--rw-r--r--   0        0        0     8699 2023-06-07 11:34:15.651987 watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/table_creator.py
--rw-r--r--   0        0        0    11939 2023-06-07 11:34:15.655987 watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/where_build.py
--rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 watchmen_storage_mysql-16.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.223631 watchmen_storage_mysql-16.5.8/LICENSE
+-rw-r--r--   0        0        0      485 2023-06-08 03:33:39.227631 watchmen_storage_mysql-16.5.8/pyproject.toml
+-rw-r--r--   0        0        0      258 2023-06-08 03:33:39.227631 watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/__init__.py
+-rw-r--r--   0        0        0     2859 2023-06-08 03:33:39.227631 watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/data_source_mysql.py
+-rw-r--r--   0        0        0     2197 2023-06-08 03:33:39.227631 watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/script_builder_mysql.py
+-rw-r--r--   0        0        0     5301 2023-06-08 03:33:39.227631 watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/storage_mysql.py
+-rw-r--r--   0        0        0     1965 2023-06-08 03:33:39.227631 watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/storage_mysql_configuration.py
+-rw-r--r--   0        0        0     8699 2023-06-08 03:33:39.227631 watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/table_creator.py
+-rw-r--r--   0        0        0    11939 2023-06-08 03:33:39.227631 watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/where_build.py
+-rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 watchmen_storage_mysql-16.5.8/PKG-INFO
```

### Comparing `watchmen_storage_mysql-16.5.7/LICENSE` & `watchmen_storage_mysql-16.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/data_source_mysql.py` & `watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/data_source_mysql.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 	def acquire_engine_by_url(url: str, params: MySQLDataSourceParams) -> Engine:
 		return create_engine(
 			redress_url_by_pymysql(url),
 			echo=params.echo,
 			future=True,
 			pool_recycle=params.poolRecycle,
 			json_serializer=serialize_to_json,
-			encoding='utf-8'
+			encoding='utf-8',
+			pool_pre_ping=True
 		)
 
 	# noinspection DuplicatedCode
 	@staticmethod
 	def find_param(params: Optional[List[DataSourceParam]], key: str) -> Optional[str]:
 		if params is None:
 			return None
```

### Comparing `watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/script_builder_mysql.py` & `watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/script_builder_mysql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/storage_mysql.py` & `watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/storage_mysql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/storage_mysql_configuration.py` & `watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/storage_mysql_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/table_creator.py` & `watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/table_creator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.7/src/watchmen_storage_mysql/where_build.py` & `watchmen_storage_mysql-16.5.8/src/watchmen_storage_mysql/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_mysql-16.5.7/PKG-INFO` & `watchmen_storage_mysql-16.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-mysql
-Version: 16.5.7
+Version: 16.5.8
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyMySQL (>=1.0.2,<2.0.0)
 Requires-Dist: cryptography (>=36.0.2,<37.0.0)
-Requires-Dist: watchmen-storage-rds (==16.5.7)
+Requires-Dist: watchmen-storage-rds (==16.5.8)
```

