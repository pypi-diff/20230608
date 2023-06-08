# Comparing `tmp/dbt-postgres-1.6.0b2.tar.gz` & `tmp/dbt-postgres-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-postgres-1.6.0b2.tar", last modified: Thu May 25 15:44:08 2023, max compression
+gzip compressed data, was "dbt-postgres-1.6.0b3.tar", last modified: Thu Jun  8 20:55:14 2023, max compression
```

## Comparing `dbt-postgres-1.6.0b2.tar` & `dbt-postgres-1.6.0b3.tar`

### file list

```diff
@@ -1,47 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.744696 dbt-postgres-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 15:44:08.744696 dbt-postgres-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/adapters/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/adapters/postgres/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.736696 dbt-postgres-1.6.0b2/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/include/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/incremental_strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.740696 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/materialized_view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/materialized_view/create.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/materialized_view/refresh.sql
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/relations.sql
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.744696 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/dbt/include/postgres/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:08.744696 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 15:44:08.000000 dbt-postgres-1.6.0b2/dbt_postgres.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:44:08.744696 dbt-postgres-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-25 15:43:54.000000 dbt-postgres-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.949818 dbt-postgres-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-08 20:55:14.949818 dbt-postgres-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.945818 dbt-postgres-1.6.0b3/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.945818 dbt-postgres-1.6.0b3/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.945818 dbt-postgres-1.6.0b3/dbt/adapters/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/postgres/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/postgres/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/postgres/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/postgres/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/postgres/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.949818 dbt-postgres-1.6.0b3/dbt/adapters/postgres/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/postgres/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/postgres/relation_configs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/postgres/relation_configs/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/adapters/postgres/relation_configs/materialized_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.945818 dbt-postgres-1.6.0b3/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.949818 dbt-postgres-1.6.0b3/dbt/include/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.949818 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.949818 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/materializations/materialized_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/relations.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.949818 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/dbt/include/postgres/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:14.949818 dbt-postgres-1.6.0b3/dbt_postgres.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-08 20:55:14.000000 dbt-postgres-1.6.0b3/dbt_postgres.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-08 20:55:14.000000 dbt-postgres-1.6.0b3/dbt_postgres.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:55:14.000000 dbt-postgres-1.6.0b3/dbt_postgres.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:55:14.000000 dbt-postgres-1.6.0b3/dbt_postgres.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 20:55:14.000000 dbt-postgres-1.6.0b3/dbt_postgres.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 20:55:14.000000 dbt-postgres-1.6.0b3/dbt_postgres.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:55:14.949818 dbt-postgres-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-08 20:55:01.000000 dbt-postgres-1.6.0b3/setup.py
```

### Comparing `dbt-postgres-1.6.0b2/PKG-INFO` & `dbt-postgres-1.6.0b3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-postgres
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: The postgres adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt-core/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-core/actions/workflows/main.yml">
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b2 Summary: The postgres
+Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b3 Summary: The postgres
 adapter plugin for dbt (data build tool) Home-page: https://github.com/dbt-
 labs/dbt-core Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8 Description-Content-Type: text/markdown
                                   [dbt logo]
                                   [CI_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-postgres The `dbt-postgres` package contains all of
```

### Comparing `dbt-postgres-1.6.0b2/README.md` & `dbt-postgres-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b2/dbt/adapters/postgres/__init__.py` & `dbt-postgres-1.6.0b3/dbt/adapters/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b2/dbt/adapters/postgres/connections.py` & `dbt-postgres-1.6.0b3/dbt/adapters/postgres/connections.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,24 @@
     def _connection_keys(self):
         return (
             "host",
             "port",
             "user",
             "database",
             "schema",
+            "connect_timeout",
+            "role",
             "search_path",
             "keepalives_idle",
             "sslmode",
+            "sslcert",
+            "sslkey",
+            "sslrootcert",
+            "application_name",
+            "retries",
         )
 
 
 class PostgresConnectionManager(SQLConnectionManager):
     TYPE = "postgres"
 
     @contextmanager
```

### Comparing `dbt-postgres-1.6.0b2/dbt/adapters/postgres/impl.py` & `dbt-postgres-1.6.0b3/dbt/adapters/postgres/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime
 from dataclasses import dataclass
 from typing import Optional, Set, List, Any
+
 from dbt.adapters.base.meta import available
 from dbt.adapters.base.impl import AdapterConfig, ConstraintSupport
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.postgres import PostgresConnectionManager
 from dbt.adapters.postgres.column import PostgresColumn
 from dbt.adapters.postgres import PostgresRelation
 from dbt.dataclass_schema import dbtClassMixin, ValidationError
@@ -136,7 +137,10 @@
         return f"{add_to} + interval '{number} {interval}'"
 
     def valid_incremental_strategies(self):
         """The set of standard builtin strategies which this adapter supports out-of-the-box.
         Not used to validate custom strategies defined by end users.
         """
         return ["append", "delete+insert"]
+
+    def debug_query(self):
+        self.execute("select 1 as id")
```

### Comparing `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/adapters.sql` & `dbt-postgres-1.6.0b3/dbt/include/postgres/macros/adapters.sql`

 * *Files 14% similar despite different names*

```diff
@@ -91,14 +91,22 @@
     select
       '{{ schema_relation.database }}' as database,
       viewname as name,
       schemaname as schema,
       'view' as type
     from pg_views
     where schemaname ilike '{{ schema_relation.schema }}'
+    union all
+    select
+      '{{ schema_relation.database }}' as database,
+      matviewname as name,
+      schemaname as schema,
+      'materialized_view' as type
+    from pg_matviews
+    where schemaname ilike '{{ schema_relation.schema }}'
   {% endcall %}
   {{ return(load_result('list_relations_without_caching').table) }}
 {% endmacro %}
 
 {% macro postgres__information_schema_name(database) -%}
   {% if database_name -%}
     {{ adapter.verify_database(database_name) }}
@@ -205,7 +213,38 @@
         and table_schema = '{{ relation.schema }}'
         and table_name = '{{ relation.identifier }}'
 {%- endmacro -%}
 
 {% macro postgres__copy_grants() %}
     {{ return(False) }}
 {% endmacro %}
+
+
+{% macro postgres__get_show_indexes_sql(relation) %}
+    select
+        i.relname                                   as name,
+        m.amname                                    as method,
+        ix.indisunique                              as "unique",
+        array_to_string(array_agg(a.attname), ',')  as column_names
+    from pg_index ix
+    join pg_class i
+        on i.oid = ix.indexrelid
+    join pg_am m
+        on m.oid=i.relam
+    join pg_class t
+        on t.oid = ix.indrelid
+    join pg_namespace n
+        on n.oid = t.relnamespace
+    join pg_attribute a
+        on a.attrelid = t.oid
+        and a.attnum = ANY(ix.indkey)
+    where t.relname = '{{ relation.identifier }}'
+      and n.nspname = '{{ relation.schema }}'
+      and t.relkind in ('r', 'm')
+    group by 1, 2, 3
+    order by 1, 2, 3
+{% endmacro %}
+
+
+{%- macro postgres__get_drop_index_sql(relation, index_name) -%}
+    drop index if exists "{{ index_name }}"
+{%- endmacro -%}
```

### Comparing `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/catalog.sql` & `dbt-postgres-1.6.0b3/dbt/include/postgres/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/materializations/snapshot_merge.sql` & `dbt-postgres-1.6.0b3/dbt/include/postgres/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/relations.sql` & `dbt-postgres-1.6.0b3/dbt/include/postgres/macros/relations.sql`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         select
             relation.id AS id,
             referenced_class.name ,
             referenced_class.schema ,
             referenced_class.kind
         from relation
         join class as referenced_class on relation.class=referenced_class.id
-        where referenced_class.kind in ('r', 'v')
+        where referenced_class.kind in ('r', 'v', 'm')
     ),
     relationships as (
         select
             referenced.name as referenced_name,
             referenced.schema as referenced_schema_id,
             dependent_class.name as dependent_name,
             dependent_class.schema as dependent_schema_id,
```

### Comparing `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/timestamps.sql` & `dbt-postgres-1.6.0b3/dbt/include/postgres/macros/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/datediff.sql` & `dbt-postgres-1.6.0b3/dbt/include/postgres/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b2/dbt/include/postgres/macros/utils/listagg.sql` & `dbt-postgres-1.6.0b3/dbt/include/postgres/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-postgres-1.6.0b2/dbt_postgres.egg-info/PKG-INFO` & `dbt-postgres-1.6.0b3/dbt_postgres.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-postgres
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: The postgres adapter plugin for dbt (data build tool)
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt-core/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-core/actions/workflows/main.yml">
```

#### html2text {}

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b2 Summary: The postgres
+Metadata-Version: 2.1 Name: dbt-postgres Version: 1.6.0b3 Summary: The postgres
 adapter plugin for dbt (data build tool) Home-page: https://github.com/dbt-
 labs/dbt-core Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
-:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Requires-Python: >=3.7 Description-
-Content-Type: text/markdown
+:: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.8 Description-Content-Type: text/markdown
                                   [dbt logo]
                                   [CI_Badge]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-postgres The `dbt-postgres` package contains all of
```

### Comparing `dbt-postgres-1.6.0b2/dbt_postgres.egg-info/SOURCES.txt` & `dbt-postgres-1.6.0b3/dbt_postgres.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 dbt/adapters/__init__.py
 dbt/adapters/postgres/__init__.py
 dbt/adapters/postgres/__version__.py
 dbt/adapters/postgres/column.py
 dbt/adapters/postgres/connections.py
 dbt/adapters/postgres/impl.py
 dbt/adapters/postgres/relation.py
+dbt/adapters/postgres/relation_configs/__init__.py
+dbt/adapters/postgres/relation_configs/constants.py
+dbt/adapters/postgres/relation_configs/index.py
+dbt/adapters/postgres/relation_configs/materialized_view.py
 dbt/include/postgres/__init__.py
 dbt/include/postgres/dbt_project.yml
 dbt/include/postgres/sample_profiles.yml
 dbt/include/postgres/macros/adapters.sql
 dbt/include/postgres/macros/catalog.sql
 dbt/include/postgres/macros/relations.sql
 dbt/include/postgres/macros/timestamps.sql
 dbt/include/postgres/macros/materializations/incremental_strategies.sql
+dbt/include/postgres/macros/materializations/materialized_view.sql
 dbt/include/postgres/macros/materializations/snapshot_merge.sql
-dbt/include/postgres/macros/materializations/materialized_view/create.sql
-dbt/include/postgres/macros/materializations/materialized_view/refresh.sql
 dbt/include/postgres/macros/utils/any_value.sql
 dbt/include/postgres/macros/utils/columns_spec_ddl.sql
 dbt/include/postgres/macros/utils/dateadd.sql
 dbt/include/postgres/macros/utils/datediff.sql
 dbt/include/postgres/macros/utils/last_day.sql
 dbt/include/postgres/macros/utils/listagg.sql
 dbt/include/postgres/macros/utils/split_part.sql
```

### Comparing `dbt-postgres-1.6.0b2/setup.py` & `dbt-postgres-1.6.0b3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import os
 import sys
 
-if sys.version_info < (3, 7):
+if sys.version_info < (3, 8):
     print("Error: dbt does not support this version of Python.")
-    print("Please upgrade to Python 3.7 or higher.")
+    print("Please upgrade to Python 3.8 or higher.")
     sys.exit(1)
 
 
 from setuptools import setup
 
 try:
     from setuptools import find_namespace_packages
@@ -37,15 +37,15 @@
 
     # default to psycopg2-binary for all OSes/versions
     print(PSYCOPG2_MESSAGE)
     return "psycopg2-binary"
 
 
 package_name = "dbt-postgres"
-package_version = "1.6.0b2"
+package_version = "1.6.0b3"
 description = """The postgres adapter plugin for dbt (data build tool)"""
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 DBT_PSYCOPG2_NAME = _dbt_psycopg2_name()
@@ -67,23 +67,24 @@
             "include/postgres/macros/*.sql",
             "include/postgres/macros/**/*.sql",
         ]
     },
     install_requires=[
         "dbt-core=={}".format(package_version),
         "{}~=2.8".format(DBT_PSYCOPG2_NAME),
+        # installed via dbt-core, but referenced directly, don't pin to avoid version conflicts with dbt-core
+        "agate",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

