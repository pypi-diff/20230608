# Comparing `tmp/dagster_gcp_pyspark-0.19.7.tar.gz` & `tmp/dagster_gcp_pyspark-0.19.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_gcp_pyspark-0.19.7.tar", last modified: Thu Jun  1 18:26:54 2023, max compression
+gzip compressed data, was "dagster_gcp_pyspark-0.19.8.tar", last modified: Thu Jun  8 16:33:34 2023, max compression
```

## Comparing `dagster_gcp_pyspark-0.19.7.tar` & `dagster_gcp_pyspark-0.19.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:26:54.061576 dagster_gcp_pyspark-0.19.7/
--rw-r--r--   0 root         (0) root         (0)    11343 2023-06-01 18:14:54.000000 dagster_gcp_pyspark-0.19.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-01 18:14:54.000000 dagster_gcp_pyspark-0.19.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      649 2023-06-01 18:26:54.061576 dagster_gcp_pyspark-0.19.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-01 18:14:54.000000 dagster_gcp_pyspark-0.19.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:26:54.057576 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark/
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-01 18:14:54.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:26:54.061576 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9900 2023-06-01 18:14:54.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 18:14:54.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-01 18:14:54.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:26:54.061576 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-06-01 18:26:53.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-01 18:26:54.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:26:53.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:26:53.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-01 18:26:53.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-01 18:26:53.000000 dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-06-01 18:26:54.061576 dagster_gcp_pyspark-0.19.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1366 2023-06-01 18:14:54.000000 dagster_gcp_pyspark-0.19.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:33:34.341936 dagster_gcp_pyspark-0.19.8/
+-rw-r--r--   0 root         (0) root         (0)    11343 2023-06-08 16:23:49.000000 dagster_gcp_pyspark-0.19.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-08 16:23:49.000000 dagster_gcp_pyspark-0.19.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      649 2023-06-08 16:33:34.341936 dagster_gcp_pyspark-0.19.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      143 2023-06-08 16:23:49.000000 dagster_gcp_pyspark-0.19.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:33:34.337936 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark/
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-08 16:23:49.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:33:34.337936 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9900 2023-06-08 16:23:49.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-08 16:23:49.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-08 16:23:49.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:33:34.337936 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-06-08 16:33:34.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-08 16:33:34.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:33:34.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:33:34.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-08 16:33:34.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 16:33:34.000000 dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      166 2023-06-08 16:33:34.341936 dagster_gcp_pyspark-0.19.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-06-08 16:23:49.000000 dagster_gcp_pyspark-0.19.8/setup.py
```

### Comparing `dagster_gcp_pyspark-0.19.7/LICENSE` & `dagster_gcp_pyspark-0.19.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.19.7/PKG-INFO` & `dagster_gcp_pyspark-0.19.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_gcp_pyspark
-Version: 0.19.7
+Version: 0.19.8
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py` & `dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark/bigquery/bigquery_pyspark_type_handler.py`

 * *Files identical despite different names*

### Comparing `dagster_gcp_pyspark-0.19.7/dagster_gcp_pyspark.egg-info/PKG-INFO` & `dagster_gcp_pyspark-0.19.8/dagster_gcp_pyspark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-gcp-pyspark
-Version: 0.19.7
+Version: 0.19.8
 Summary: Package for storing PySpark DataFrames in GCP
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-gcp-pyspark
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster_gcp_pyspark-0.19.7/setup.py` & `dagster_gcp_pyspark-0.19.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,14 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_gcp_pyspark_tests*"]),
     install_requires=[
-        "dagster==1.3.7",
-        "dagster-gcp==0.19.7",
+        "dagster==1.3.8",
+        "dagster-gcp==0.19.8",
         "pyspark",
     ],
     extras_require={"test": ["pandas-gbq"]},
     zip_safe=False,
 )
```

