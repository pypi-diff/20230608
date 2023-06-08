# Comparing `tmp/dagster-mysql-0.19.9rc0.tar.gz` & `tmp/dagster-mysql-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-mysql-0.19.9rc0.tar", last modified: Thu Jun  8 18:28:57 2023, max compression
+gzip compressed data, was "dagster-mysql-1.0.5.tar", last modified: Fri Aug 26 13:46:41 2022, max compression
```

## Comparing `dagster-mysql-0.19.9rc0.tar` & `dagster-mysql-1.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      126 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      605 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      125 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.567206 dagster-mysql-0.19.9rc0/dagster_mysql/
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/alembic/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/event_log/
--rw-r--r--   0 root         (0) root         (0)       68 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8792 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/event_log/event_log.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7883 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6277 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     3730 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/storage.py
--rw-r--r--   0 root         (0) root         (0)     6404 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/utils.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/dagster_mysql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      605 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      704 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       41 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 18:28:57.000000 dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-08 18:28:57.571205 dagster-mysql-0.19.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1296 2023-06-08 18:20:46.000000 dagster-mysql-0.19.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:41.740862 dagster-mysql-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      126 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      629 2022-08-26 13:46:41.740862 dagster-mysql-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      125 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:41.732862 dagster-mysql-1.0.5/dagster_mysql/
+-rw-r--r--   0 root         (0) root         (0)      435 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:41.732862 dagster-mysql-1.0.5/dagster_mysql/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1039 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/alembic/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:41.736862 dagster-mysql-1.0.5/dagster_mysql/event_log/
+-rw-r--r--   0 root         (0) root         (0)       44 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6933 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/event_log/event_log.py
+-rw-r--r--   0 root         (0) root         (0)        8 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:41.736862 dagster-mysql-1.0.5/dagster_mysql/run_storage/
+-rw-r--r--   0 root         (0) root         (0)       41 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/run_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6870 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/run_storage/run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:41.736862 dagster-mysql-1.0.5/dagster_mysql/schedule_storage/
+-rw-r--r--   0 root         (0) root         (0)       51 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/schedule_storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5583 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/schedule_storage/schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3465 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/storage.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/dagster_mysql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-26 13:46:41.732862 dagster-mysql-1.0.5/dagster_mysql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      629 2022-08-26 13:46:41.000000 dagster-mysql-1.0.5/dagster_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      704 2022-08-26 13:46:41.000000 dagster-mysql-1.0.5/dagster_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:41.000000 dagster-mysql-1.0.5/dagster_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-08-26 13:46:41.000000 dagster-mysql-1.0.5/dagster_mysql.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       38 2022-08-26 13:46:41.000000 dagster-mysql-1.0.5/dagster_mysql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2022-08-26 13:46:41.000000 dagster-mysql-1.0.5/dagster_mysql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2022-08-26 13:46:41.740862 dagster-mysql-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1409 2022-08-26 13:33:01.000000 dagster-mysql-1.0.5/setup.py
```

### Comparing `dagster-mysql-0.19.9rc0/LICENSE` & `dagster-mysql-1.0.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2023 Elementl, Inc.
+   Copyright {yyyy} {name of copyright owner}
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `dagster-mysql-0.19.9rc0/PKG-INFO` & `dagster-mysql-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.19.9rc0
+Version: 1.0.5
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql/alembic/alembic.ini` & `dagster-mysql-1.0.5/dagster_mysql/alembic/alembic.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [alembic]
 # path to migration scripts
-script_location = dagster:_core/storage/alembic
+script_location = dagster:core/storage/alembic
 
 
 [post_write_hooks]
 # post_write_hooks defines scripts or Python functions that are run
 # on newly generated revision scripts.  See the documentation for further
 # detail and examples
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql/run_storage/run_storage.py` & `dagster-mysql-1.0.5/dagster_mysql/run_storage/run_storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,40 @@
-from typing import ContextManager, Mapping, Optional, cast
+from typing import Dict
 
-import dagster._check as check
 import sqlalchemy as db
-import sqlalchemy.dialects as db_dialects
-import sqlalchemy.pool as db_pool
-from dagster._config.config_schema import UserConfigSchema
-from dagster._core.storage.config import MySqlStorageConfig, mysql_config
+from packaging.version import parse
+
+import dagster._check as check
+from dagster._core.storage.config import mysql_config
 from dagster._core.storage.runs import (
     DaemonHeartbeatsTable,
     InstanceInfo,
     RunStorageSqlMetadata,
     SqlRunStorage,
 )
 from dagster._core.storage.runs.schema import KeyValueStoreTable
 from dagster._core.storage.sql import (
-    AlembicVersion,
     check_alembic_revision,
     create_engine,
     run_alembic_upgrade,
     stamp_alembic_rev,
 )
-from dagster._daemon.types import DaemonHeartbeat
-from dagster._serdes import ConfigurableClass, ConfigurableClassData, serialize_value
+from dagster._serdes import ConfigurableClass, ConfigurableClassData, serialize_dagster_namedtuple
 from dagster._utils import utc_datetime_from_timestamp
-from sqlalchemy.engine import Connection
 
 from ..utils import (
+    MYSQL_POOL_RECYCLE,
     create_mysql_connection,
     mysql_alembic_config,
-    mysql_isolation_level,
     mysql_url_from_config,
-    parse_mysql_version,
     retry_mysql_connection_fn,
     retry_mysql_creation_fn,
 )
 
 MINIMUM_MYSQL_BUCKET_VERSION = "8.0.0"
-MINIMUM_MYSQL_INTERSECT_VERSION = "8.0.31"
 
 
 class MySQLRunStorage(SqlRunStorage, ConfigurableClass):
     """MySQL-backed run storage.
 
     Users should not directly instantiate this class; it is instantiated by internal machinery when
     ``dagit`` and ``dagster-graphql`` load, based on the values in the ``dagster.yaml`` file in
@@ -53,23 +47,23 @@
        :end-before: end_marker_runs
        :language: YAML
 
     Note that the fields in this config are :py:class:`~dagster.StringSource` and
     :py:class:`~dagster.IntSource` and can be configured from environment variables.
     """
 
-    def __init__(self, mysql_url: str, inst_data: Optional[ConfigurableClassData] = None):
+    def __init__(self, mysql_url, inst_data=None):
         self._inst_data = check.opt_inst_param(inst_data, "inst_data", ConfigurableClassData)
         self.mysql_url = mysql_url
 
         # Default to not holding any connections open to prevent accumulating connections per DagsterInstance
         self._engine = create_engine(
             self.mysql_url,
-            isolation_level=mysql_isolation_level(),
-            poolclass=db_pool.NullPool,
+            isolation_level="AUTOCOMMIT",
+            poolclass=db.pool.NullPool,
         )
 
         self._index_migration_cache = {}
         table_names = retry_mysql_connection_fn(db.inspect(self._engine).get_table_names)
 
         # Stamp and create tables if the main table does not exist (we can't check alembic
         # revision because alembic config may be shared with other storage classes)
@@ -81,131 +75,118 @@
         elif "instance_info" not in table_names:
             InstanceInfo.create(self._engine)
 
         self._mysql_version = self.get_server_version()
 
         super().__init__()
 
-    def _init_db(self) -> None:
+    def _init_db(self):
         with self.connect() as conn:
-            RunStorageSqlMetadata.create_all(conn)
-            stamp_alembic_rev(mysql_alembic_config(__file__), conn)
+            with conn.begin():
+                RunStorageSqlMetadata.create_all(conn)
+                stamp_alembic_rev(mysql_alembic_config(__file__), conn)
 
-    def optimize_for_dagit(self, statement_timeout: int, pool_recycle: int) -> None:
+    def optimize_for_dagit(self, statement_timeout):
         # When running in dagit, hold 1 open connection
         # https://github.com/dagster-io/dagster/issues/3719
         self._engine = create_engine(
             self.mysql_url,
-            isolation_level=mysql_isolation_level(),
+            isolation_level="AUTOCOMMIT",
             pool_size=1,
-            pool_recycle=pool_recycle,
+            pool_recycle=MYSQL_POOL_RECYCLE,
         )
 
     @property
-    def inst_data(self) -> Optional[ConfigurableClassData]:
+    def inst_data(self):
         return self._inst_data
 
     @classmethod
-    def config_type(cls) -> UserConfigSchema:
+    def config_type(cls):
         return mysql_config()
 
-    def get_server_version(self) -> Optional[str]:
-        with self.connect() as conn:
-            row = conn.execute(db.text("select version()")).fetchone()
-
+    def get_server_version(self):
+        row = self.fetchone("select version()")
         if not row:
             return None
 
-        return cast(str, row[0])
+        return row[0]
 
-    @classmethod
-    def from_config_value(
-        cls, inst_data: Optional[ConfigurableClassData], config_value: MySqlStorageConfig
-    ) -> "MySQLRunStorage":
+    @staticmethod
+    def from_config_value(inst_data, config_value):
         return MySQLRunStorage(inst_data=inst_data, mysql_url=mysql_url_from_config(config_value))
 
     @staticmethod
-    def wipe_storage(mysql_url: str) -> None:
-        engine = create_engine(
-            mysql_url, isolation_level=mysql_isolation_level(), poolclass=db_pool.NullPool
-        )
+    def wipe_storage(mysql_url):
+        engine = create_engine(mysql_url, isolation_level="AUTOCOMMIT", poolclass=db.pool.NullPool)
         try:
             RunStorageSqlMetadata.drop_all(engine)
         finally:
             engine.dispose()
 
     @staticmethod
-    def create_clean_storage(mysql_url: str) -> "MySQLRunStorage":
+    def create_clean_storage(mysql_url):
         MySQLRunStorage.wipe_storage(mysql_url)
         return MySQLRunStorage(mysql_url)
 
-    def connect(self, run_id: Optional[str] = None) -> ContextManager[Connection]:
+    def connect(self, run_id=None):  # pylint: disable=arguments-differ, unused-argument
         return create_mysql_connection(self._engine, __file__, "run")
 
-    def upgrade(self) -> None:
+    def upgrade(self):
         alembic_config = mysql_alembic_config(__file__)
         with self.connect() as conn:
             run_alembic_upgrade(alembic_config, conn)
 
-    def has_built_index(self, migration_name: str) -> None:
+    def has_built_index(self, migration_name):
         if migration_name not in self._index_migration_cache:
             self._index_migration_cache[migration_name] = super(
                 MySQLRunStorage, self
             ).has_built_index(migration_name)
         return self._index_migration_cache[migration_name]
 
-    def mark_index_built(self, migration_name: str) -> None:
+    def mark_index_built(self, migration_name):
         super(MySQLRunStorage, self).mark_index_built(migration_name)
         if migration_name in self._index_migration_cache:
             del self._index_migration_cache[migration_name]
 
     @property
-    def supports_bucket_queries(self) -> bool:
+    def supports_bucket_queries(self):
         if not super().supports_bucket_queries:
             return False
 
         if not self._mysql_version:
             return False
 
-        return parse_mysql_version(self._mysql_version) >= parse_mysql_version(
-            MINIMUM_MYSQL_BUCKET_VERSION
-        )
-
-    @property
-    def supports_intersect(self) -> bool:
-        return parse_mysql_version(self._mysql_version) >= parse_mysql_version(  # type: ignore
-            MINIMUM_MYSQL_INTERSECT_VERSION
-        )
+        return parse(self._mysql_version) >= parse(MINIMUM_MYSQL_BUCKET_VERSION)
 
-    def add_daemon_heartbeat(self, daemon_heartbeat: DaemonHeartbeat) -> None:
+    def add_daemon_heartbeat(self, daemon_heartbeat):
         with self.connect() as conn:
             conn.execute(
-                db_dialects.mysql.insert(DaemonHeartbeatsTable)
+                db.dialects.mysql.insert(DaemonHeartbeatsTable)
                 .values(
                     timestamp=utc_datetime_from_timestamp(daemon_heartbeat.timestamp),
                     daemon_type=daemon_heartbeat.daemon_type,
                     daemon_id=daemon_heartbeat.daemon_id,
-                    body=serialize_value(daemon_heartbeat),
+                    body=serialize_dagster_namedtuple(daemon_heartbeat),
                 )
                 .on_duplicate_key_update(
                     timestamp=utc_datetime_from_timestamp(daemon_heartbeat.timestamp),
                     daemon_id=daemon_heartbeat.daemon_id,
-                    body=serialize_value(daemon_heartbeat),
+                    body=serialize_dagster_namedtuple(daemon_heartbeat),
                 )
             )
 
-    def set_cursor_values(self, pairs: Mapping[str, str]) -> None:
-        check.mapping_param(pairs, "pairs", key_type=str, value_type=str)
+    def kvs_set(self, pairs: Dict[str, str]) -> None:
+        check.dict_param(pairs, "pairs", key_type=str, value_type=str)
         db_values = [{"key": k, "value": v} for k, v in pairs.items()]
 
         with self.connect() as conn:
-            insert_stmt = db_dialects.mysql.insert(KeyValueStoreTable).values(db_values)
+            insert_stmt = db.dialects.mysql.insert(KeyValueStoreTable).values(db_values)
             conn.execute(
                 insert_stmt.on_duplicate_key_update(
                     value=insert_stmt.inserted.value,
                 )
             )
 
-    def alembic_version(self) -> AlembicVersion:
+    def alembic_version(self):
         alembic_config = mysql_alembic_config(__file__)
         with self.connect() as conn:
             return check_alembic_revision(alembic_config, conn)
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql/schedule_storage/schedule_storage.py` & `dagster-mysql-1.0.5/dagster_mysql/event_log/event_log.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,171 +1,195 @@
-from typing import ContextManager, Optional, cast
+import sqlalchemy as db
 
 import dagster._check as check
-import pendulum
-import sqlalchemy as db
-import sqlalchemy.dialects as db_dialects
-import sqlalchemy.pool as db_pool
-from dagster._config.config_schema import UserConfigSchema
-from dagster._core.storage.config import MySqlStorageConfig, mysql_config
-from dagster._core.storage.schedules import ScheduleStorageSqlMetadata, SqlScheduleStorage
-from dagster._core.storage.schedules.schema import InstigatorsTable
+from dagster._core.storage.config import mysql_config
+from dagster._core.storage.event_log import (
+    AssetKeyTable,
+    SqlEventLogStorage,
+    SqlEventLogStorageMetadata,
+    SqlPollingEventWatcher,
+)
+from dagster._core.storage.event_log.base import EventLogCursor
+from dagster._core.storage.event_log.migration import ASSET_KEY_INDEX_COLS
 from dagster._core.storage.sql import (
-    AlembicVersion,
     check_alembic_revision,
     create_engine,
     run_alembic_upgrade,
     stamp_alembic_rev,
 )
-from dagster._serdes import ConfigurableClass, ConfigurableClassData, serialize_value
-from sqlalchemy.engine import Connection
+from dagster._serdes import ConfigurableClass, ConfigurableClassData
 
 from ..utils import (
+    MYSQL_POOL_RECYCLE,
     create_mysql_connection,
     mysql_alembic_config,
-    mysql_isolation_level,
     mysql_url_from_config,
-    parse_mysql_version,
     retry_mysql_connection_fn,
     retry_mysql_creation_fn,
 )
 
-MINIMUM_MYSQL_BATCH_VERSION = "8.0.0"
 
-
-class MySQLScheduleStorage(SqlScheduleStorage, ConfigurableClass):
-    """MySQL-backed run storage.
+class MySQLEventLogStorage(SqlEventLogStorage, ConfigurableClass):
+    """MySQL-backed event log storage.
 
     Users should not directly instantiate this class; it is instantiated by internal machinery when
     ``dagit`` and ``dagster-graphql`` load, based on the values in the ``dagster.yaml`` file in
     ``$DAGSTER_HOME``. Configuration of this class should be done by setting values in that file.
 
     .. literalinclude:: ../../../../../../examples/docs_snippets/docs_snippets/deploying/dagster-mysql-legacy.yaml
        :caption: dagster.yaml
-       :start-after: start_marker_schedules
-       :end-before: end_marker_schedules
+       :start-after: start_marker_event_log
+       :end-before: end_marker_event_log
        :language: YAML
 
     Note that the fields in this config are :py:class:`~dagster.StringSource` and
     :py:class:`~dagster.IntSource` and can be configured from environment variables.
+
     """
 
-    def __init__(self, mysql_url: str, inst_data: Optional[ConfigurableClassData] = None):
+    def __init__(self, mysql_url, inst_data=None):
         self._inst_data = check.opt_inst_param(inst_data, "inst_data", ConfigurableClassData)
-        self.mysql_url = mysql_url
+        self.mysql_url = check.str_param(mysql_url, "mysql_url")
+        self._disposed = False
+
+        self._event_watcher = SqlPollingEventWatcher(self)
 
         # Default to not holding any connections open to prevent accumulating connections per DagsterInstance
         self._engine = create_engine(
             self.mysql_url,
-            isolation_level=mysql_isolation_level(),
-            poolclass=db_pool.NullPool,
+            isolation_level="AUTOCOMMIT",
+            poolclass=db.pool.NullPool,
         )
+        self._secondary_index_cache = {}
+
+        table_names = retry_mysql_connection_fn(db.inspect(self._engine).get_table_names)
 
         # Stamp and create tables if the main table does not exist (we can't check alembic
         # revision because alembic config may be shared with other storage classes)
-        table_names = retry_mysql_connection_fn(db.inspect(self._engine).get_table_names)
-        if "jobs" not in table_names:
+        if "event_logs" not in table_names:
             retry_mysql_creation_fn(self._init_db)
-
-        self._mysql_version = self.get_server_version()
+            # mark all secondary indexes to be used
+            self.reindex_events()
+            self.reindex_assets()
 
         super().__init__()
 
-    def _init_db(self) -> None:
-        with self.connect() as conn:
-            ScheduleStorageSqlMetadata.create_all(conn)
-            stamp_alembic_rev(mysql_alembic_config(__file__), conn)
-
-        # mark all the data migrations as applied
-        self.migrate()
-        self.optimize()
+    def _init_db(self):
+        with self._connect() as conn:
+            with conn.begin():
+                SqlEventLogStorageMetadata.create_all(conn)
+                stamp_alembic_rev(mysql_alembic_config(__file__), conn)
 
-    def optimize_for_dagit(self, statement_timeout: int, pool_recycle: int) -> None:
+    def optimize_for_dagit(self, statement_timeout):
         # When running in dagit, hold an open connection
         # https://github.com/dagster-io/dagster/issues/3719
         self._engine = create_engine(
             self.mysql_url,
-            isolation_level=mysql_isolation_level(),
+            isolation_level="AUTOCOMMIT",
             pool_size=1,
-            pool_recycle=pool_recycle,
+            pool_recycle=MYSQL_POOL_RECYCLE,
         )
 
+    def upgrade(self):
+        alembic_config = mysql_alembic_config(__file__)
+        with self._connect() as conn:
+            run_alembic_upgrade(alembic_config, conn)
+
     @property
-    def inst_data(self) -> Optional[ConfigurableClassData]:
+    def inst_data(self):
         return self._inst_data
 
     @classmethod
-    def config_type(cls) -> UserConfigSchema:
+    def config_type(cls):
         return mysql_config()
 
-    @classmethod
-    def from_config_value(
-        cls, inst_data: Optional[ConfigurableClassData], config_value: MySqlStorageConfig
-    ) -> "MySQLScheduleStorage":
-        return MySQLScheduleStorage(
+    @staticmethod
+    def from_config_value(inst_data, config_value):
+        return MySQLEventLogStorage(
             inst_data=inst_data, mysql_url=mysql_url_from_config(config_value)
         )
 
     @staticmethod
-    def wipe_storage(mysql_url: str) -> None:
-        engine = create_engine(
-            mysql_url, isolation_level=mysql_isolation_level(), poolclass=db_pool.NullPool
-        )
+    def wipe_storage(mysql_url):
+        engine = create_engine(mysql_url, isolation_level="AUTOCOMMIT", poolclass=db.pool.NullPool)
         try:
-            ScheduleStorageSqlMetadata.drop_all(engine)
+            SqlEventLogStorageMetadata.drop_all(engine)
         finally:
             engine.dispose()
 
     @staticmethod
-    def create_clean_storage(mysql_url: str) -> "MySQLScheduleStorage":
-        MySQLScheduleStorage.wipe_storage(mysql_url)
-        return MySQLScheduleStorage(mysql_url)
+    def create_clean_storage(conn_string):
+        MySQLEventLogStorage.wipe_storage(conn_string)
+        return MySQLEventLogStorage(conn_string)
+
+    def store_asset_event(self, event):
+        # last_materialization_timestamp is updated upon observation, materialization, materialization_planned
+        # See SqlEventLogStorage.store_asset_event method for more details
+
+        values = self._get_asset_entry_values(event, self.has_secondary_index(ASSET_KEY_INDEX_COLS))
+        with self.index_connection() as conn:
+            if values:
+                conn.execute(
+                    db.dialects.mysql.insert(AssetKeyTable)
+                    .values(
+                        asset_key=event.dagster_event.asset_key.to_string(),
+                        **values,
+                    )
+                    .on_duplicate_key_update(
+                        **values,
+                    )
+                )
+            else:
+                try:
+                    conn.execute(
+                        db.dialects.mysql.insert(AssetKeyTable).values(
+                            asset_key=event.dagster_event.asset_key.to_string(),
+                        )
+                    )
+                except db.exc.IntegrityError:
+                    pass
+
+    def _connect(self):
+        return create_mysql_connection(self._engine, __file__, "event log")
+
+    def run_connection(self, run_id=None):
+        return self._connect()
+
+    def index_connection(self):
+        return self._connect()
+
+    def has_secondary_index(self, name):
+        if name not in self._secondary_index_cache:
+            self._secondary_index_cache[name] = super(
+                MySQLEventLogStorage, self
+            ).has_secondary_index(name)
+        return self._secondary_index_cache[name]
+
+    def enable_secondary_index(self, name):
+        super(MySQLEventLogStorage, self).enable_secondary_index(name)
+        if name in self._secondary_index_cache:
+            del self._secondary_index_cache[name]
+
+    def watch(self, run_id, cursor, callback):
+        if cursor and EventLogCursor.parse(cursor).is_offset_cursor():
+            check.failed("Cannot call `watch` with an offset cursor")
+        self._event_watcher.watch_run(run_id, cursor, callback)
 
-    def connect(self) -> ContextManager[Connection]:
-        return create_mysql_connection(self._engine, __file__, "schedule")
+    def end_watch(self, run_id, handler):
+        self._event_watcher.unwatch_run(run_id, handler)
 
     @property
-    def supports_batch_queries(self) -> bool:
-        if not self._mysql_version:
-            return False
+    def event_watcher(self):
+        return self._event_watcher
 
-        return parse_mysql_version(self._mysql_version) >= parse_mysql_version(
-            MINIMUM_MYSQL_BATCH_VERSION
-        )
+    def __del__(self):
+        self.dispose()
 
-    def get_server_version(self) -> Optional[str]:
-        with self.connect() as conn:
-            row = conn.execute(db.text("select version()")).fetchone()
-
-        if not row:
-            return None
-
-        return cast(str, row[0])
-
-    def upgrade(self) -> None:
-        with self.connect() as conn:
-            alembic_config = mysql_alembic_config(__file__)
-            run_alembic_upgrade(alembic_config, conn)
-
-    def _add_or_update_instigators_table(self, conn: Connection, state) -> None:
-        selector_id = state.selector_id
-        conn.execute(
-            db_dialects.mysql.insert(InstigatorsTable)
-            .values(
-                selector_id=selector_id,
-                repository_selector_id=state.repository_selector_id,
-                status=state.status.value,
-                instigator_type=state.instigator_type.value,
-                instigator_body=serialize_value(state),
-            )
-            .on_duplicate_key_update(
-                status=state.status.value,
-                instigator_type=state.instigator_type.value,
-                instigator_body=serialize_value(state),
-                update_timestamp=pendulum.now("UTC"),
-            )
-        )
+    def dispose(self):
+        if not self._disposed:
+            self._disposed = True
+            self._event_watcher.close()
 
-    def alembic_version(self) -> AlembicVersion:
+    def alembic_version(self):
         alembic_config = mysql_alembic_config(__file__)
-        with self.connect() as conn:
+        with self._connect() as conn:
             return check_alembic_revision(alembic_config, conn)
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql/storage.py` & `dagster-mysql-1.0.5/dagster_mysql/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Optional
 
 from dagster import _check as check
-from dagster._config.config_schema import UserConfigSchema
 from dagster._core.storage.base_storage import DagsterStorage
-from dagster._core.storage.config import MySqlStorageConfig, mysql_config
+from dagster._core.storage.config import mysql_config
 from dagster._core.storage.event_log import EventLogStorage
 from dagster._core.storage.runs import RunStorage
 from dagster._core.storage.schedules import ScheduleStorage
 from dagster._serdes import ConfigurableClass, ConfigurableClassData
 
 from .event_log import MySQLEventLogStorage
 from .run_storage import MySQLRunStorage
@@ -29,34 +28,32 @@
        :caption: dagster.yaml
        :language: YAML
 
     Note that the fields in this config are :py:class:`~dagster.StringSource` and
     :py:class:`~dagster.IntSource` and can be configured from environment variables.
     """
 
-    def __init__(self, mysql_url, inst_data: Optional[ConfigurableClassData] = None):
+    def __init__(self, mysql_url, inst_data=None):
         self.mysql_url = mysql_url
         self._inst_data = check.opt_inst_param(inst_data, "inst_data", ConfigurableClassData)
         self._run_storage = MySQLRunStorage(mysql_url)
         self._event_log_storage = MySQLEventLogStorage(mysql_url)
         self._schedule_storage = MySQLScheduleStorage(mysql_url)
         super().__init__()
 
     @property
-    def inst_data(self) -> Optional[ConfigurableClassData]:
+    def inst_data(self):
         return self._inst_data
 
     @classmethod
-    def config_type(cls) -> UserConfigSchema:
+    def config_type(cls):
         return mysql_config()
 
-    @classmethod
-    def from_config_value(
-        cls, inst_data: Optional[ConfigurableClassData], config_value: MySqlStorageConfig
-    ) -> "DagsterMySQLStorage":
+    @staticmethod
+    def from_config_value(inst_data, config_value):
         return DagsterMySQLStorage(
             inst_data=inst_data,
             mysql_url=mysql_url_from_config(config_value),
         )
 
     @property
     def event_log_storage(self) -> EventLogStorage:
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/PKG-INFO` & `dagster-mysql-1.0.5/dagster_mysql.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: dagster-mysql
-Version: 0.19.9rc0
+Version: 1.0.5
 Summary: A Dagster integration for MySQL
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `dagster-mysql-0.19.9rc0/dagster_mysql.egg-info/SOURCES.txt` & `dagster-mysql-1.0.5/dagster_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-mysql-0.19.9rc0/setup.py` & `dagster-mysql-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,41 @@
-from pathlib import Path
-
 from setuptools import find_packages, setup
 
 
 def get_version():
     version = {}
-    with open(Path(__file__).parent / "dagster_mysql/version.py", encoding="utf8") as fp:
-        exec(fp.read(), version)
+    with open("dagster_mysql/version.py", encoding="utf8") as fp:
+        exec(fp.read(), version)  # pylint: disable=W0122
 
     return version["__version__"]
 
 
-ver = get_version()
-# dont pin dev installs to avoid pip dep resolver issues
-pin = "" if ver == "1!0+dev" else f"=={ver}"
-setup(
-    name="dagster-mysql",
-    version=ver,
-    author="Elementl",
-    author_email="hello@elementl.com",
-    license="Apache-2.0",
-    description="A Dagster integration for MySQL",
-    url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql",
-    classifiers=[
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "License :: OSI Approved :: Apache Software License",
-        "Operating System :: OS Independent",
-    ],
-    packages=find_packages(exclude=["dagster_mysql_tests*"]),
-    package_data={
-        "dagster-mysql": [
-            "dagster_mysql/alembic/*",
-        ]
-    },
-    include_package_data=True,
-    install_requires=["dagster==1.3.9rc0", "mysql-connector-python"],
-    zip_safe=False,
-)
+if __name__ == "__main__":
+    ver = get_version()
+    # dont pin dev installs to avoid pip dep resolver issues
+    pin = "" if ver == "0+dev" else f"=={ver}"
+    setup(
+        name="dagster-mysql",
+        version=ver,
+        author="Elementl",
+        author_email="hello@elementl.com",
+        license="Apache-2.0",
+        description="A Dagster integration for MySQL",
+        url="https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-mysql",
+        classifiers=[
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
+            "Programming Language :: Python :: 3.9",
+            "Programming Language :: Python :: 3.10",
+            "License :: OSI Approved :: Apache Software License",
+            "Operating System :: OS Independent",
+        ],
+        packages=find_packages(exclude=["dagster_mysql_tests*"]),
+        package_data={
+            "dagster-mysql": [
+                "dagster_mysql/alembic/*",
+            ]
+        },
+        include_package_data=True,
+        install_requires=["dagster==1.0.5", "mysql-connector-python"],
+        zip_safe=False,
+    )
```

