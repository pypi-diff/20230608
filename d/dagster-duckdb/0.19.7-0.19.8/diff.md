# Comparing `tmp/dagster-duckdb-0.19.7.tar.gz` & `tmp/dagster-duckdb-0.19.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-0.19.7.tar", last modified: Thu Jun  1 18:26:17 2023, max compression
+gzip compressed data, was "dagster-duckdb-0.19.8.tar", last modified: Thu Jun  8 16:32:47 2023, max compression
```

## Comparing `dagster-duckdb-0.19.7.tar` & `dagster-duckdb-0.19.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:26:17.641625 dagster-duckdb-0.19.7/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-01 18:14:54.000000 dagster-duckdb-0.19.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2023-06-01 18:14:54.000000 dagster-duckdb-0.19.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-01 18:26:17.641625 dagster-duckdb-0.19.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      128 2023-06-01 18:14:54.000000 dagster-duckdb-0.19.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:26:17.641625 dagster-duckdb-0.19.7/dagster_duckdb/
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-01 18:14:54.000000 dagster-duckdb-0.19.7/dagster_duckdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-06-01 18:14:54.000000 dagster-duckdb-0.19.7/dagster_duckdb/io_manager.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 18:14:54.000000 dagster-duckdb-0.19.7/dagster_duckdb/py.typed
--rw-r--r--   0 root         (0) root         (0)     1280 2023-06-01 18:14:54.000000 dagster-duckdb-0.19.7/dagster_duckdb/resource.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-01 18:14:54.000000 dagster-duckdb-0.19.7/dagster_duckdb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:26:17.641625 dagster-duckdb-0.19.7/dagster_duckdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-01 18:26:17.000000 dagster-duckdb-0.19.7/dagster_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-01 18:26:17.000000 dagster-duckdb-0.19.7/dagster_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:26:17.000000 dagster-duckdb-0.19.7/dagster_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:26:17.000000 dagster-duckdb-0.19.7/dagster_duckdb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      149 2023-06-01 18:26:17.000000 dagster-duckdb-0.19.7/dagster_duckdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-01 18:26:17.000000 dagster-duckdb-0.19.7/dagster_duckdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      125 2023-06-01 18:26:17.641625 dagster-duckdb-0.19.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1544 2023-06-01 18:14:54.000000 dagster-duckdb-0.19.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:32:47.669970 dagster-duckdb-0.19.8/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 16:23:49.000000 dagster-duckdb-0.19.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-08 16:23:49.000000 dagster-duckdb-0.19.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-08 16:32:47.669970 dagster-duckdb-0.19.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      128 2023-06-08 16:23:49.000000 dagster-duckdb-0.19.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:32:47.669970 dagster-duckdb-0.19.8/dagster_duckdb/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-08 16:23:49.000000 dagster-duckdb-0.19.8/dagster_duckdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-06-08 16:23:49.000000 dagster-duckdb-0.19.8/dagster_duckdb/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 16:23:49.000000 dagster-duckdb-0.19.8/dagster_duckdb/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-06-08 16:23:49.000000 dagster-duckdb-0.19.8/dagster_duckdb/resource.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 16:23:49.000000 dagster-duckdb-0.19.8/dagster_duckdb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:32:47.669970 dagster-duckdb-0.19.8/dagster_duckdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-08 16:32:47.000000 dagster-duckdb-0.19.8/dagster_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-08 16:32:47.000000 dagster-duckdb-0.19.8/dagster_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:32:47.000000 dagster-duckdb-0.19.8/dagster_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:32:47.000000 dagster-duckdb-0.19.8/dagster_duckdb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-08 16:32:47.000000 dagster-duckdb-0.19.8/dagster_duckdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 16:32:47.000000 dagster-duckdb-0.19.8/dagster_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      125 2023-06-08 16:32:47.673970 dagster-duckdb-0.19.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-08 16:23:49.000000 dagster-duckdb-0.19.8/setup.py
```

### Comparing `dagster-duckdb-0.19.7/LICENSE` & `dagster-duckdb-0.19.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.19.7/PKG-INFO` & `dagster-duckdb-0.19.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.19.7
+Version: 0.19.8
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-0.19.7/dagster_duckdb/io_manager.py` & `dagster-duckdb-0.19.8/dagster_duckdb/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.19.7/dagster_duckdb/resource.py` & `dagster-duckdb-0.19.8/dagster_duckdb/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-0.19.7/dagster_duckdb.egg-info/PKG-INFO` & `dagster-duckdb-0.19.8/dagster_duckdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb
-Version: 0.19.7
+Version: 0.19.8
 Summary: Package for DuckDB-specific Dagster framework op and resource components.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-duckdb-0.19.7/setup.py` & `dagster-duckdb-0.19.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_tests*"]),
     include_package_data=True,
     install_requires=[
         "duckdb",
-        "dagster==1.3.7",
+        "dagster==1.3.8",
     ],
     extras_require={
         "pandas": ["pandas"],
         # Pyspark 2.x is incompatible with Python 3.8+
         "pyspark": [
             'pyspark>=3.0.0; python_version >= "3.8"',
             'pyspark>=2.0.2; python_version < "3.8"',
```

