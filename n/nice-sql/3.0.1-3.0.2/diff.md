# Comparing `tmp/nice-sql-3.0.1.tar.gz` & `tmp/nice-sql-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice-sql-3.0.1.tar", last modified: Wed Jun  7 09:01:02 2023, max compression
+gzip compressed data, was "nice-sql-3.0.2.tar", last modified: Thu Jun  8 09:16:58 2023, max compression
```

## Comparing `nice-sql-3.0.1.tar` & `nice-sql-3.0.2.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.406733 nice-sql-3.0.1/
--rw-r--r--   0 lichengming   (502) staff       (20)     2618 2023-06-07 09:01:02.406087 nice-sql-3.0.1/PKG-INFO
--rw-r--r--   0 lichengming   (502) staff       (20)     2303 2023-06-07 08:10:43.000000 nice-sql-3.0.1/README.md
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.386022 nice-sql-3.0.1/nice_sql.egg-info/
--rw-r--r--   0 lichengming   (502) staff       (20)     2618 2023-06-07 09:01:02.000000 nice-sql-3.0.1/nice_sql.egg-info/PKG-INFO
--rw-r--r--   0 lichengming   (502) staff       (20)      629 2023-06-07 09:01:02.000000 nice-sql-3.0.1/nice_sql.egg-info/SOURCES.txt
--rw-r--r--   0 lichengming   (502) staff       (20)        1 2023-06-07 09:01:02.000000 nice-sql-3.0.1/nice_sql.egg-info/dependency_links.txt
--rw-r--r--   0 lichengming   (502) staff       (20)       53 2023-06-07 09:01:02.000000 nice-sql-3.0.1/nice_sql.egg-info/requires.txt
--rw-r--r--   0 lichengming   (502) staff       (20)        8 2023-06-07 09:01:02.000000 nice-sql-3.0.1/nice_sql.egg-info/top_level.txt
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.386326 nice-sql-3.0.1/nicesql/
--rw-r--r--   0 lichengming   (502) staff       (20)        0 2023-05-31 15:43:52.000000 nice-sql-3.0.1/nicesql/__init__.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.393185 nice-sql-3.0.1/nicesql/db/
--rw-r--r--   0 lichengming   (502) staff       (20)      167 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/db/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1175 2023-06-03 08:26:25.000000 nice-sql-3.0.1/nicesql/db/_driver.py
--rw-r--r--   0 lichengming   (502) staff       (20)     2091 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/db/_driver_mysql.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1868 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/db/_execute.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1527 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/db/_register.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1128 2023-05-30 07:03:46.000000 nice-sql-3.0.1/nicesql/db/_result.py
--rw-r--r--   0 lichengming   (502) staff       (20)     1355 2023-05-29 11:43:20.000000 nice-sql-3.0.1/nicesql/db/_sqlconv.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.400848 nice-sql-3.0.1/nicesql/shortcut/
--rw-r--r--   0 lichengming   (502) staff       (20)      215 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)      841 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/_base.py
--rw-r--r--   0 lichengming   (502) staff       (20)      344 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/_delete.py
--rw-r--r--   0 lichengming   (502) staff       (20)      368 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/_insert.py
--rw-r--r--   0 lichengming   (502) staff       (20)      875 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/_select.py
--rw-r--r--   0 lichengming   (502) staff       (20)      344 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/shortcut/_update.py
--rw-r--r--   0 lichengming   (502) staff       (20)      628 2023-06-07 06:55:37.000000 nice-sql-3.0.1/nicesql/shortcut/_utils.py
-drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-07 09:01:02.404791 nice-sql-3.0.1/nicesql/utils/
--rw-r--r--   0 lichengming   (502) staff       (20)       74 2023-06-07 08:03:25.000000 nice-sql-3.0.1/nicesql/utils/__init__.py
--rw-r--r--   0 lichengming   (502) staff       (20)       55 2023-06-02 08:01:20.000000 nice-sql-3.0.1/nicesql/utils/_logger.py
--rw-r--r--   0 lichengming   (502) staff       (20)      347 2023-06-05 14:24:21.000000 nice-sql-3.0.1/nicesql/utils/_tls.py
--rw-r--r--   0 lichengming   (502) staff       (20)       38 2023-06-07 09:01:02.406910 nice-sql-3.0.1/setup.cfg
--rw-r--r--   0 lichengming   (502) staff       (20)      783 2023-06-07 08:05:45.000000 nice-sql-3.0.1/setup.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-08 09:16:58.752806 nice-sql-3.0.2/
+-rw-r--r--   0 lichengming   (502) staff       (20)     2611 2023-06-08 09:16:58.752369 nice-sql-3.0.2/PKG-INFO
+-rw-r--r--   0 lichengming   (502) staff       (20)     2296 2023-06-08 09:12:38.000000 nice-sql-3.0.2/README.md
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-08 09:16:58.737815 nice-sql-3.0.2/nice_sql.egg-info/
+-rw-r--r--   0 lichengming   (502) staff       (20)     2611 2023-06-08 09:16:58.000000 nice-sql-3.0.2/nice_sql.egg-info/PKG-INFO
+-rw-r--r--   0 lichengming   (502) staff       (20)      658 2023-06-08 09:16:58.000000 nice-sql-3.0.2/nice_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)        1 2023-06-08 09:16:58.000000 nice-sql-3.0.2/nice_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)       53 2023-06-08 09:16:58.000000 nice-sql-3.0.2/nice_sql.egg-info/requires.txt
+-rw-r--r--   0 lichengming   (502) staff       (20)        8 2023-06-08 09:16:58.000000 nice-sql-3.0.2/nice_sql.egg-info/top_level.txt
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-08 09:16:58.738557 nice-sql-3.0.2/nicesql/
+-rw-r--r--   0 lichengming   (502) staff       (20)        0 2023-05-31 15:43:52.000000 nice-sql-3.0.2/nicesql/__init__.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-08 09:16:58.746669 nice-sql-3.0.2/nicesql/db/
+-rw-r--r--   0 lichengming   (502) staff       (20)      167 2023-06-07 08:03:25.000000 nice-sql-3.0.2/nicesql/db/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1175 2023-06-03 08:26:25.000000 nice-sql-3.0.2/nicesql/db/_driver.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     2159 2023-06-07 09:58:36.000000 nice-sql-3.0.2/nicesql/db/_driver_mysql.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     2595 2023-06-08 08:26:19.000000 nice-sql-3.0.2/nicesql/db/_driver_sqlite.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1910 2023-06-08 08:54:12.000000 nice-sql-3.0.2/nicesql/db/_execute.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1639 2023-06-08 07:05:40.000000 nice-sql-3.0.2/nicesql/db/_register.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1128 2023-05-30 07:03:46.000000 nice-sql-3.0.2/nicesql/db/_result.py
+-rw-r--r--   0 lichengming   (502) staff       (20)     1355 2023-05-29 11:43:20.000000 nice-sql-3.0.2/nicesql/db/_sqlconv.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-08 09:16:58.750293 nice-sql-3.0.2/nicesql/shortcut/
+-rw-r--r--   0 lichengming   (502) staff       (20)      215 2023-06-07 08:03:25.000000 nice-sql-3.0.2/nicesql/shortcut/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      841 2023-06-07 08:03:25.000000 nice-sql-3.0.2/nicesql/shortcut/_base.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      344 2023-06-07 08:03:25.000000 nice-sql-3.0.2/nicesql/shortcut/_delete.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      368 2023-06-07 08:03:25.000000 nice-sql-3.0.2/nicesql/shortcut/_insert.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      875 2023-06-07 08:03:25.000000 nice-sql-3.0.2/nicesql/shortcut/_select.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      344 2023-06-07 08:03:25.000000 nice-sql-3.0.2/nicesql/shortcut/_update.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      628 2023-06-07 06:55:37.000000 nice-sql-3.0.2/nicesql/shortcut/_utils.py
+drwxr-xr-x   0 lichengming   (502) staff       (20)        0 2023-06-08 09:16:58.751932 nice-sql-3.0.2/nicesql/utils/
+-rw-r--r--   0 lichengming   (502) staff       (20)       74 2023-06-07 08:03:25.000000 nice-sql-3.0.2/nicesql/utils/__init__.py
+-rw-r--r--   0 lichengming   (502) staff       (20)       55 2023-06-02 08:01:20.000000 nice-sql-3.0.2/nicesql/utils/_logger.py
+-rw-r--r--   0 lichengming   (502) staff       (20)      347 2023-06-05 14:24:21.000000 nice-sql-3.0.2/nicesql/utils/_tls.py
+-rw-r--r--   0 lichengming   (502) staff       (20)       38 2023-06-08 09:16:58.752895 nice-sql-3.0.2/setup.cfg
+-rw-r--r--   0 lichengming   (502) staff       (20)      783 2023-06-08 09:13:51.000000 nice-sql-3.0.2/setup.py
```

### Comparing `nice-sql-3.0.1/PKG-INFO` & `nice-sql-3.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice-sql
-Version: 3.0.1
+Version: 3.0.2
 Summary: easy/lite/simple db query for python db api 2.0
 Home-page: https://github.com/minusli/nicesql
 Author: minusli
 Author-email: minusli@foxmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3
@@ -12,15 +12,15 @@
 
 # 使用手册
 
 ------
 
 # 如何安装？
 
-`pip install nice-sql==2.0.0`
+`pip install nice-sql`
 
 # 如何使用？
 
 ### Step 1: 添加 db 配置
 
 ```python
 from nicesql.db import add_db
```

### Comparing `nice-sql-3.0.1/README.md` & `nice-sql-3.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 使用手册
 
 ------
 
 # 如何安装？
 
-`pip install nice-sql==2.0.0`
+`pip install nice-sql`
 
 # 如何使用？
 
 ### Step 1: 添加 db 配置
 
 ```python
 from nicesql.db import add_db
```

### Comparing `nice-sql-3.0.1/nice_sql.egg-info/PKG-INFO` & `nice-sql-3.0.2/nice_sql.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice-sql
-Version: 3.0.1
+Version: 3.0.2
 Summary: easy/lite/simple db query for python db api 2.0
 Home-page: https://github.com/minusli/nicesql
 Author: minusli
 Author-email: minusli@foxmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Requires-Python: >=3
@@ -12,15 +12,15 @@
 
 # 使用手册
 
 ------
 
 # 如何安装？
 
-`pip install nice-sql==2.0.0`
+`pip install nice-sql`
 
 # 如何使用？
 
 ### Step 1: 添加 db 配置
 
 ```python
 from nicesql.db import add_db
```

### Comparing `nice-sql-3.0.1/nice_sql.egg-info/SOURCES.txt` & `nice-sql-3.0.2/nice_sql.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 nice_sql.egg-info/dependency_links.txt
 nice_sql.egg-info/requires.txt
 nice_sql.egg-info/top_level.txt
 nicesql/__init__.py
 nicesql/db/__init__.py
 nicesql/db/_driver.py
 nicesql/db/_driver_mysql.py
+nicesql/db/_driver_sqlite.py
 nicesql/db/_execute.py
 nicesql/db/_register.py
 nicesql/db/_result.py
 nicesql/db/_sqlconv.py
 nicesql/shortcut/__init__.py
 nicesql/shortcut/_base.py
 nicesql/shortcut/_delete.py
```

### Comparing `nice-sql-3.0.1/nicesql/db/_driver.py` & `nice-sql-3.0.2/nicesql/db/_driver.py`

 * *Files identical despite different names*

### Comparing `nice-sql-3.0.1/nicesql/db/_driver_mysql.py` & `nice-sql-3.0.2/nicesql/db/_driver_mysql.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import List, Dict, Any
 
-import pymysql.cursors
+import pymysql
 from dbutils.pooled_db import PooledDB, PooledSharedDBConnection, PooledDedicatedDBConnection
+from pymysql.cursors import Cursor, DictCursor
 
 from nicesql.db._driver import LiteDriver, LiteConnection, LiteCursor
 
 
 class Mysql(LiteDriver):
     def __init__(self, hostname: str, port: int, username: str, password: str, database: str, **kwargs):
         super().__init__(hostname, port, username, password, database, **kwargs)
 
         autocommit = self.get_autocommit()
         charset = self.get_charset()
 
         self.pool = PooledDB(creator=pymysql, host=self.hostname, port=self.port, database=self.database, user=self.username, password=self.password,
-                             blocking=True, cursorclass=pymysql.cursors.DictCursor, charset=charset, autocommit=autocommit)
+                             blocking=True, cursorclass=DictCursor, charset=charset, autocommit=autocommit)
 
     def connection(self) -> "LiteConnection":
         return MysqlConnection(self.pool.connection())
 
     def get_autocommit(self) -> bool:
         return str(self.kwargs.get("autocommit", "")).lower() in ("true", "1")
 
@@ -43,25 +44,26 @@
         return MysqlCursor(self.connection.cursor())
 
     def close(self):
         self.connection.close()
 
 
 class MysqlCursor(LiteCursor):
-    def __init__(self, cursor):
+    def __init__(self, cursor: Cursor):
         self.cursor = cursor
 
     def execute(self, sql: str, params: List[Any]):
         sql = sql.replace("?", "%s")
         self.cursor.execute(sql, params)
 
     def lastrowid(self) -> int | str:
         return self.cursor.lastrowid
 
     def rowcount(self) -> int:
         return self.cursor.rowcount
 
     def fetchall(self) -> List[Dict[str, Any]]:
+        # noinspection PyTypeChecker
         return self.cursor.fetchall()
 
     def close(self):
         self.cursor.close()
```

### Comparing `nice-sql-3.0.1/nicesql/db/_execute.py` & `nice-sql-3.0.2/nicesql/db/_execute.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     logger.debug("SQL: {} => {}".format(sql, sql))
 
     conn: LiteConnection = tls.get(_TLS_KEY_OF_CONNECTION.format(db))
     if conn:
         return _execute(conn, sql, params)
 
     conn = get_db(db).connection()
+    conn.begin()
     try:
         result = _execute(conn, sql, params)
         conn.commit()
         return result
     except Exception:
         conn.rollback()
         raise
@@ -47,14 +48,15 @@
     def decorator(fn):
         def wrapper(*args, **kwargs):
             conn = tls.get(_TLS_KEY_OF_CONNECTION.format(db))
             if conn:
                 return fn(*args, **kwargs)
 
             conn = get_db(db).connection()
+            conn.begin()
             try:
                 tls.put(_TLS_KEY_OF_CONNECTION.format(db), conn)
                 r = fn(*args, **kwargs)
                 conn.commit()
                 return r
             except Exception:
                 conn.rollback()
```

### Comparing `nice-sql-3.0.1/nicesql/db/_register.py` & `nice-sql-3.0.2/nicesql/db/_register.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Dict, Type, Any
 
 import dsnparse
 
 from nicesql.db._driver import LiteDriver
 from nicesql.db._driver_mysql import Mysql
+from nicesql.db._driver_sqlite import Sqlite
 
 __dbs: Dict[str, LiteDriver] = {}
 __dbtypes: Dict[str, Type[LiteDriver]] = {
-    "mysql": Mysql
+    "mysql": Mysql,
+    "sqlite": Sqlite
 }
 
 
 def register_driver(schema: str, engine: Type[LiteDriver]):
     __dbtypes[schema] = engine
 
 
@@ -41,14 +43,14 @@
     dsn = dsnparse.parse(dsn)
     return _DSN(
         driver=dsn.scheme,
         username=dsn.username,
         password=dsn.password,
         hostname=dsn.hostname,
         port=dsn.port,
-        database=dsn.database,
+        database=dsn.database.strip("/") if dsn.database else dsn.database,
         params=dsn.query_params
     )
 
 
 if __name__ == '__main__':
     _parse_dsn("a+prom.interface.postgres.Interface://testuser:testpw@localhost:1234/testdb/xx/?a=1&b=01&c=abc&d=true&e=false&f=1.1&f=1.2")
```

### Comparing `nice-sql-3.0.1/nicesql/db/_result.py` & `nice-sql-3.0.2/nicesql/db/_result.py`

 * *Files identical despite different names*

### Comparing `nice-sql-3.0.1/nicesql/db/_sqlconv.py` & `nice-sql-3.0.2/nicesql/db/_sqlconv.py`

 * *Files identical despite different names*

### Comparing `nice-sql-3.0.1/nicesql/shortcut/_base.py` & `nice-sql-3.0.2/nicesql/shortcut/_base.py`

 * *Files identical despite different names*

### Comparing `nice-sql-3.0.1/nicesql/shortcut/_select.py` & `nice-sql-3.0.2/nicesql/shortcut/_select.py`

 * *Files identical despite different names*

### Comparing `nice-sql-3.0.1/nicesql/shortcut/_utils.py` & `nice-sql-3.0.2/nicesql/shortcut/_utils.py`

 * *Files identical despite different names*

### Comparing `nice-sql-3.0.1/setup.py` & `nice-sql-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # upload pypi
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
 
 setup(
     name='nice-sql',
-    version='3.0.1',
+    version='3.0.2',
     author='minusli',
     author_email='minusli@foxmail.com',
     url='https://github.com/minusli/nicesql',
     description='easy/lite/simple db query for python db api 2.0',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["tests"]),
```

