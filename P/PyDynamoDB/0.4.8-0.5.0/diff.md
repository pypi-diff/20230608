# Comparing `tmp/PyDynamoDB-0.4.8.tar.gz` & `tmp/PyDynamoDB-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDynamoDB-0.4.8.tar", last modified: Tue Jun  6 06:34:13 2023, max compression
+gzip compressed data, was "PyDynamoDB-0.5.0.tar", last modified: Thu Jun  8 03:29:56 2023, max compression
```

## Comparing `PyDynamoDB-0.4.8.tar` & `PyDynamoDB-0.5.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.150694 PyDynamoDB-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-06 06:34:13.150694 PyDynamoDB-0.4.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.142694 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 06:34:13.000000 PyDynamoDB-0.4.8/PyDynamoDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.142694 PyDynamoDB-0.4.8/pydynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    20306 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/result_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.146695 PyDynamoDB-0.4.8/pydynamodb/sql/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16127 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/ddl_alter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/ddl_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/ddl_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/ddl_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/dml_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/dml_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sql/util_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.146695 PyDynamoDB-0.4.8/pydynamodb/sqlalchemy_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sqlalchemy_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:34:13.150694 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/dml_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/pydnamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/querydb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/querydb_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/pydynamodb/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-06 06:34:13.150694 PyDynamoDB-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-06 06:34:00.000000 PyDynamoDB-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:29:56.696932 PyDynamoDB-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-08 03:29:56.696932 PyDynamoDB-0.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:29:56.688932 PyDynamoDB-0.5.0/PyDynamoDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-08 03:29:56.000000 PyDynamoDB-0.5.0/PyDynamoDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-08 03:29:56.000000 PyDynamoDB-0.5.0/PyDynamoDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:29:56.000000 PyDynamoDB-0.5.0/PyDynamoDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 03:29:56.000000 PyDynamoDB-0.5.0/PyDynamoDB.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:29:56.000000 PyDynamoDB-0.5.0/PyDynamoDB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 03:29:56.000000 PyDynamoDB-0.5.0/PyDynamoDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 03:29:56.000000 PyDynamoDB-0.5.0/PyDynamoDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:29:56.692932 PyDynamoDB-0.5.0/pydynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21412 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/result_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:29:56.692932 PyDynamoDB-0.5.0/pydynamodb/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16127 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12786 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/ddl_alter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/ddl_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/ddl_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/ddl_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/dml_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/dml_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sql/util_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:29:56.692932 PyDynamoDB-0.5.0/pydynamodb/sqlalchemy_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sqlalchemy_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:29:56.696932 PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/dml_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/pydnamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/querydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/querydb_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/pydynamodb/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 03:29:56.696932 PyDynamoDB-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-08 03:29:46.000000 PyDynamoDB-0.5.0/setup.py
```

### Comparing `PyDynamoDB-0.4.8/LICENSE` & `PyDynamoDB-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/PKG-INFO` & `PyDynamoDB-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDynamoDB
-Version: 0.4.8
+Version: 0.5.0
 Summary: Python DB API 2.0 (PEP 249) client for Amazon DynamoDB
 Home-page: https://github.com/passren/PyDynamoDB
 Author: Peng Ren
 Author-email: passren9099@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/passren/PyDynamoDB/wiki
 Project-URL: Source, https://github.com/passren/PyDynamoDB
@@ -125,30 +125,30 @@
 ~~~~~~~~~~~
 
 .. code:: python
 
     from pydynamodb import connect
 
     cursor = connect(aws_access_key_id="aws_access_key_id",
-                    aws_secret_access_key="aws_secret_access_key"
-                     region_name="region_name").cursor()
+                    aws_secret_access_key="aws_secret_access_key",
+                    region_name="region_name").cursor()
     cursor.execute('SELECT * FROM "ddb_table_name"')
     print(cursor.fetchall())
 
 
 Cursor iteration
 ~~~~~~~~~~~~~~~~
 
 .. code:: python
 
     from pydynamodb import connect
 
     cursor = connect(aws_access_key_id="aws_access_key_id",
-                    aws_secret_access_key="aws_secret_access_key"
-                     region_name="region_name").cursor()
+                    aws_secret_access_key="aws_secret_access_key",
+                    region_name="region_name").cursor()
     cursor.execute('SELECT * FROM "ddb_table_name"')
     rows = cursor.fetchall()
     for row in rows:
         print(row)
 
 
 Query with parameters
@@ -158,16 +158,16 @@
 and deserialize the response to Python built-in types.
 
 .. code:: python
 
     from pydynamodb import connect
     from datetime import date, datetime
     cursor = connect(aws_access_key_id="aws_access_key_id",
-                    aws_secret_access_key="aws_secret_access_key"
-                     region_name="region_name").cursor()
+                    aws_secret_access_key="aws_secret_access_key",
+                    region_name="region_name").cursor()
     cursor.execute("""INSERT INTO "ddb_table_name" VALUE {
                         'partition_key' = ?, 'sort_key' = ?, 'col_str' = ?,
                         'col_num' = ?, 'col_byte' = ?, 'col_ss' = ?,
                         'col_ns' = ?, 'col_bs' = ?, 'col_list' = ?,
                         'col_map' = ?, 'col_nested' = ?,
                         'col_date' = ?, 'col_datetime' = ?
                     }""", ["pkey_value", "skey_value", "str", 100, b"ABC", # String, Number, Bytes
```

### Comparing `PyDynamoDB-0.4.8/PyDynamoDB.egg-info/PKG-INFO` & `PyDynamoDB-0.5.0/PyDynamoDB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDynamoDB
-Version: 0.4.8
+Version: 0.5.0
 Summary: Python DB API 2.0 (PEP 249) client for Amazon DynamoDB
 Home-page: https://github.com/passren/PyDynamoDB
 Author: Peng Ren
 Author-email: passren9099@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/passren/PyDynamoDB/wiki
 Project-URL: Source, https://github.com/passren/PyDynamoDB
@@ -125,30 +125,30 @@
 ~~~~~~~~~~~
 
 .. code:: python
 
     from pydynamodb import connect
 
     cursor = connect(aws_access_key_id="aws_access_key_id",
-                    aws_secret_access_key="aws_secret_access_key"
-                     region_name="region_name").cursor()
+                    aws_secret_access_key="aws_secret_access_key",
+                    region_name="region_name").cursor()
     cursor.execute('SELECT * FROM "ddb_table_name"')
     print(cursor.fetchall())
 
 
 Cursor iteration
 ~~~~~~~~~~~~~~~~
 
 .. code:: python
 
     from pydynamodb import connect
 
     cursor = connect(aws_access_key_id="aws_access_key_id",
-                    aws_secret_access_key="aws_secret_access_key"
-                     region_name="region_name").cursor()
+                    aws_secret_access_key="aws_secret_access_key",
+                    region_name="region_name").cursor()
     cursor.execute('SELECT * FROM "ddb_table_name"')
     rows = cursor.fetchall()
     for row in rows:
         print(row)
 
 
 Query with parameters
@@ -158,16 +158,16 @@
 and deserialize the response to Python built-in types.
 
 .. code:: python
 
     from pydynamodb import connect
     from datetime import date, datetime
     cursor = connect(aws_access_key_id="aws_access_key_id",
-                    aws_secret_access_key="aws_secret_access_key"
-                     region_name="region_name").cursor()
+                    aws_secret_access_key="aws_secret_access_key",
+                    region_name="region_name").cursor()
     cursor.execute("""INSERT INTO "ddb_table_name" VALUE {
                         'partition_key' = ?, 'sort_key' = ?, 'col_str' = ?,
                         'col_num' = ?, 'col_byte' = ?, 'col_ss' = ?,
                         'col_ns' = ?, 'col_bs' = ?, 'col_list' = ?,
                         'col_map' = ?, 'col_nested' = ?,
                         'col_date' = ?, 'col_datetime' = ?
                     }""", ["pkey_value", "skey_value", "str", 100, b"ABC", # String, Number, Bytes
```

### Comparing `PyDynamoDB-0.4.8/PyDynamoDB.egg-info/SOURCES.txt` & `PyDynamoDB-0.5.0/PyDynamoDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/README.rst` & `PyDynamoDB-0.5.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -97,30 +97,30 @@
 ~~~~~~~~~~~
 
 .. code:: python
 
     from pydynamodb import connect
 
     cursor = connect(aws_access_key_id="aws_access_key_id",
-                    aws_secret_access_key="aws_secret_access_key"
-                     region_name="region_name").cursor()
+                    aws_secret_access_key="aws_secret_access_key",
+                    region_name="region_name").cursor()
     cursor.execute('SELECT * FROM "ddb_table_name"')
     print(cursor.fetchall())
 
 
 Cursor iteration
 ~~~~~~~~~~~~~~~~
 
 .. code:: python
 
     from pydynamodb import connect
 
     cursor = connect(aws_access_key_id="aws_access_key_id",
-                    aws_secret_access_key="aws_secret_access_key"
-                     region_name="region_name").cursor()
+                    aws_secret_access_key="aws_secret_access_key",
+                    region_name="region_name").cursor()
     cursor.execute('SELECT * FROM "ddb_table_name"')
     rows = cursor.fetchall()
     for row in rows:
         print(row)
 
 
 Query with parameters
@@ -130,16 +130,16 @@
 and deserialize the response to Python built-in types.
 
 .. code:: python
 
     from pydynamodb import connect
     from datetime import date, datetime
     cursor = connect(aws_access_key_id="aws_access_key_id",
-                    aws_secret_access_key="aws_secret_access_key"
-                     region_name="region_name").cursor()
+                    aws_secret_access_key="aws_secret_access_key",
+                    region_name="region_name").cursor()
     cursor.execute("""INSERT INTO "ddb_table_name" VALUE {
                         'partition_key' = ?, 'sort_key' = ?, 'col_str' = ?,
                         'col_num' = ?, 'col_byte' = ?, 'col_ss' = ?,
                         'col_ns' = ?, 'col_bs' = ?, 'col_list' = ?,
                         'col_map' = ?, 'col_nested' = ?,
                         'col_date' = ?, 'col_datetime' = ?
                     }""", ["pkey_value", "skey_value", "str", 100, b"ABC", # String, Number, Bytes
```

### Comparing `PyDynamoDB-0.4.8/pydynamodb/__init__.py` & `PyDynamoDB-0.5.0/pydynamodb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TYPE_CHECKING, FrozenSet
 
 from .error import *  # noqa
 
 if TYPE_CHECKING:
     from .connection import Connection
 
-__version__: str = "0.4.8"
+__version__: str = "0.5.0"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 3
 paramstyle: str = "qmark"
```

### Comparing `PyDynamoDB-0.4.8/pydynamodb/common.py` & `PyDynamoDB-0.5.0/pydynamodb/common.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/connection.py` & `PyDynamoDB-0.5.0/pydynamodb/connection.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/converter.py` & `PyDynamoDB-0.5.0/pydynamodb/converter.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/cursor.py` & `PyDynamoDB-0.5.0/pydynamodb/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,12 +196,22 @@
     def _reset_state(self) -> None:
         if self.result_set and not self.result_set.is_closed:
             self.result_set.close()
         self.result_set = None  # type: ignore
 
 
 class DictCursor(Cursor):
-    def __init__(self, **kwargs) -> None:
-        super().__init__(**kwargs)
+    def __init__(
+        self,
+        connection: "Connection",
+        converter: Converter,
+        retry_config: RetryConfig,
+        **kwargs
+    ) -> None:
+        super().__init__(
+            connection=connection,
+            converter=converter,
+            retry_config=retry_config,
+            **kwargs,
+        )
+        self._result_set: Optional[DynamoDBDictResultSet] = None
         self._result_set_class = DynamoDBDictResultSet
-        if "dict_type" in kwargs:
-            DynamoDBDictResultSet.dict_type = kwargs["dict_type"]
```

### Comparing `PyDynamoDB-0.4.8/pydynamodb/error.py` & `PyDynamoDB-0.5.0/pydynamodb/error.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/executor.py` & `PyDynamoDB-0.5.0/pydynamodb/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,14 +271,53 @@
                         )
                     )
                 self._is_predef_metadata = True
         else:
             self._is_predef_metadata = False
 
 
+class DmlStatementDictExecutor(DmlStatementExecutor):
+    def __init__(
+        self,
+        connection: "Connection",
+        converter: Converter,
+        statements: Statements,
+        retry_config: RetryConfig,
+        **kwargs,
+    ) -> None:
+        super().__init__(
+            connection=connection,
+            converter=converter,
+            statements=statements,
+            retry_config=retry_config,
+            **kwargs,
+        )
+
+    def process_rows(self, response: Dict[str, Any]) -> None:
+        rows = response.get("Items", None)
+        if rows is None:
+            raise DataError("KeyError `Items`")
+
+        processed_rows = list()
+        for row in rows:
+            row_ = self._process_row_item(row)
+            processed_rows.append(row_)
+
+        self._rows.extend(processed_rows)
+        self._next_token = response.get("NextToken", None)
+
+    def _process_row_item(self, row) -> Optional[Dict[str, Any]]:
+        row_ = dict()
+        for col, val in row.items():
+            val_ = self._converter.deserialize(val)
+            row_[col] = val_
+
+        return row_
+
+
 class DmlBatchExecutor(DmlStatementExecutor):
     def __init__(
         self,
         connection: "Connection",
         converter: Converter,
         statements: Statements,
         retry_config: RetryConfig,
```

### Comparing `PyDynamoDB-0.4.8/pydynamodb/model.py` & `PyDynamoDB-0.5.0/pydynamodb/model.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/result_set.py` & `PyDynamoDB-0.5.0/pydynamodb/result_set.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 import logging
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type, cast
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, cast
 
 from .converter import Converter
 from .common import CursorIterator
 from .model import Statements, Metadata
 from .executor import BaseExecutor, dispatch_executor
+from .executor import DmlStatementDictExecutor
 from .error import ProgrammingError
 from .util import RetryConfig
 
 if TYPE_CHECKING:
     from .connection import Connection
 
 _logger = logging.getLogger(__name__)  # type: ignore
@@ -135,9 +136,31 @@
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
 
 
 class DynamoDBDictResultSet(DynamoDBResultSet):
-    # You can override this to use OrderedDict or other dict-like types.
-    dict_type: Type[Any] = dict
+    def __init__(
+        self,
+        connection: "Connection",
+        converter: Converter,
+        statements: Statements,
+        arraysize: int,
+        retry_config: RetryConfig,
+        is_transaction: bool = False,
+        executor_class: BaseExecutor = None,
+        **kwargs
+    ) -> None:
+        assert (
+            statements.query_type[0] == "DML" and len(statements) == 1
+        ), "DictExecutor can only support single DML statement"
+        super().__init__(
+            connection=connection,
+            converter=converter,
+            statements=statements,
+            arraysize=arraysize,
+            retry_config=retry_config,
+            is_transaction=is_transaction,
+            executor_class=DmlStatementDictExecutor,
+            **kwargs
+        )
```

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/base.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/base.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/common.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/common.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/ddl_alter.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/ddl_alter.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/ddl_create.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/ddl_create.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/ddl_drop.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/ddl_drop.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/ddl_sql.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/ddl_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/dml_select.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/dml_select.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/dml_sql.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/dml_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/parser.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/parser.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/util.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/util.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sql/util_sql.py` & `PyDynamoDB-0.5.0/pydynamodb/sql/util_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py` & `PyDynamoDB-0.5.0/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/dml_select.py` & `PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/dml_select.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/helper.py` & `PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/helper.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/pydnamodb.py` & `PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/pydnamodb.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/querydb.py` & `PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/querydb.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/superset_dynamodb/querydb_sqlite.py` & `PyDynamoDB-0.5.0/pydynamodb/superset_dynamodb/querydb_sqlite.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/pydynamodb/util.py` & `PyDynamoDB-0.5.0/pydynamodb/util.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.4.8/setup.py` & `PyDynamoDB-0.5.0/setup.py`

 * *Files identical despite different names*

