# Comparing `tmp/pydatafabric-0.4.7.tar.gz` & `tmp/pydatafabric-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydatafabric-0.4.7.tar", last modified: Mon Jul 25 11:38:48 2022, max compression
+gzip compressed data, was "pydatafabric-0.4.8.tar", last modified: Mon Jul 25 20:40:48 2022, max compression
```

## Comparing `pydatafabric-0.4.7.tar` & `pydatafabric-0.4.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:48.561237 pydatafabric-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (116)     1090 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     4311 2022-07-25 11:38:48.561237 pydatafabric-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2873 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:48.561237 pydatafabric-0.4.7/google/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:48.561237 pydatafabric-0.4.7/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/google/cloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:48.561237 pydatafabric-0.4.7/google/cloud/spark/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/google/cloud/spark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:48.561237 pydatafabric-0.4.7/google/cloud/spark/bigquery/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/google/cloud/spark/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1062 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/google/cloud/spark/bigquery/big_numeric_support.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:48.561237 pydatafabric-0.4.7/pydatafabric/
--rw-r--r--   0 runner    (1001) docker     (116)      105 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/pydatafabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    27384 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/pydatafabric/gcp.py
--rw-r--r--   0 runner    (1001) docker     (116)     3370 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/pydatafabric/github_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1733 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/pydatafabric/nes.py
--rw-r--r--   0 runner    (1001) docker     (116)    11088 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/pydatafabric/oracle.py
--rw-r--r--   0 runner    (1001) docker     (116)      728 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/pydatafabric/spark_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      279 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/pydatafabric/vault_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    14587 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/pydatafabric/ye.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 11:38:48.561237 pydatafabric-0.4.7/pydatafabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4311 2022-07-25 11:38:48.000000 pydatafabric-0.4.7/pydatafabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      602 2022-07-25 11:38:48.000000 pydatafabric-0.4.7/pydatafabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-25 11:38:48.000000 pydatafabric-0.4.7/pydatafabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       49 2022-07-25 11:38:48.000000 pydatafabric-0.4.7/pydatafabric.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      964 2022-07-25 11:38:48.000000 pydatafabric-0.4.7/pydatafabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       20 2022-07-25 11:38:48.000000 pydatafabric-0.4.7/pydatafabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-07-25 11:38:48.561237 pydatafabric-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3069 2022-07-25 11:38:46.000000 pydatafabric-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:48.290696 pydatafabric-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (116)     1090 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     4311 2022-07-25 20:40:48.290696 pydatafabric-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2873 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:48.286696 pydatafabric-0.4.8/google/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:48.286696 pydatafabric-0.4.8/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/google/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:48.286696 pydatafabric-0.4.8/google/cloud/spark/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/google/cloud/spark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:48.286696 pydatafabric-0.4.8/google/cloud/spark/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/google/cloud/spark/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1062 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/google/cloud/spark/bigquery/big_numeric_support.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:48.290696 pydatafabric-0.4.8/pydatafabric/
+-rw-r--r--   0 runner    (1001) docker     (116)      105 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/pydatafabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27384 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/pydatafabric/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3370 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/pydatafabric/github_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1733 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/pydatafabric/nes.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11088 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/pydatafabric/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (116)      728 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/pydatafabric/spark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      279 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/pydatafabric/vault_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14587 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/pydatafabric/ye.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-07-25 20:40:48.290696 pydatafabric-0.4.8/pydatafabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4311 2022-07-25 20:40:48.000000 pydatafabric-0.4.8/pydatafabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      602 2022-07-25 20:40:48.000000 pydatafabric-0.4.8/pydatafabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-07-25 20:40:48.000000 pydatafabric-0.4.8/pydatafabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2022-07-25 20:40:48.000000 pydatafabric-0.4.8/pydatafabric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      986 2022-07-25 20:40:48.000000 pydatafabric-0.4.8/pydatafabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       20 2022-07-25 20:40:48.000000 pydatafabric-0.4.8/pydatafabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2022-07-25 20:40:48.290696 pydatafabric-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     3098 2022-07-25 20:40:43.000000 pydatafabric-0.4.8/setup.py
```

### Comparing `pydatafabric-0.4.7/LICENSE` & `pydatafabric-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pydatafabric-0.4.7/PKG-INFO` & `pydatafabric-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatafabric
-Version: 0.4.7
+Version: 0.4.8
 Summary: SHINSEGAE DataFabric Python Package
 Home-page: https://github.com/emartddt/dataplaltform-python-dist
 Author: SHINSEGAE DataFabric
 Author-email: admin@shinsegae.ai
 License: MIT License
 Description: # SHINSEGAE DataFabric Python Package
```

### Comparing `pydatafabric-0.4.7/README.md` & `pydatafabric-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pydatafabric-0.4.7/google/cloud/spark/bigquery/big_numeric_support.py` & `pydatafabric-0.4.8/google/cloud/spark/bigquery/big_numeric_support.py`

 * *Files identical despite different names*

### Comparing `pydatafabric-0.4.7/pydatafabric/gcp.py` & `pydatafabric-0.4.8/pydatafabric/gcp.py`

 * *Files identical despite different names*

### Comparing `pydatafabric-0.4.7/pydatafabric/github_utils.py` & `pydatafabric-0.4.8/pydatafabric/github_utils.py`

 * *Files identical despite different names*

### Comparing `pydatafabric-0.4.7/pydatafabric/nes.py` & `pydatafabric-0.4.8/pydatafabric/nes.py`

 * *Files identical despite different names*

### Comparing `pydatafabric-0.4.7/pydatafabric/oracle.py` & `pydatafabric-0.4.8/pydatafabric/oracle.py`

 * *Files identical despite different names*

### Comparing `pydatafabric-0.4.7/pydatafabric/spark_utils.py` & `pydatafabric-0.4.8/pydatafabric/spark_utils.py`

 * *Files identical despite different names*

### Comparing `pydatafabric-0.4.7/pydatafabric/ye.py` & `pydatafabric-0.4.8/pydatafabric/ye.py`

 * *Files identical despite different names*

### Comparing `pydatafabric-0.4.7/pydatafabric.egg-info/PKG-INFO` & `pydatafabric-0.4.8/pydatafabric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydatafabric
-Version: 0.4.7
+Version: 0.4.8
 Summary: SHINSEGAE DataFabric Python Package
 Home-page: https://github.com/emartddt/dataplaltform-python-dist
 Author: SHINSEGAE DataFabric
 Author-email: admin@shinsegae.ai
 License: MIT License
 Description: # SHINSEGAE DataFabric Python Package
```

### Comparing `pydatafabric-0.4.7/pydatafabric.egg-info/SOURCES.txt` & `pydatafabric-0.4.8/pydatafabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydatafabric-0.4.7/pydatafabric.egg-info/requires.txt` & `pydatafabric-0.4.8/pydatafabric.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -41,7 +41,8 @@
 seaborn==0.11.2
 matplotlib==3.5.1
 openpyxl==3.0.9
 xgboost==1.5.2
 scikit-learn==1.0.2
 bayesian-optimization==1.2.0
 scipy<1.8.0,>=1.7.3
+numpy<1.22.2,>=1.15.0
```

### Comparing `pydatafabric-0.4.7/setup.py` & `pydatafabric-0.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     # "implicit==0.5.2",
     "matplotlib==3.5.1",
     "openpyxl==3.0.9",
     "xgboost==1.5.2",
     "scikit-learn==1.0.2",
     "bayesian-optimization==1.2.0",
     "scipy<1.8.0,>=1.7.3",
+    "numpy<1.22.2,>=1.15.0",
 ]
 
 install_requires = [
     "thrift-sasl==0.4.3",
     "hvac==0.11.2",
     "pyhive[hive]==0.6.5",
     "pyarrow==6.0.1",
```

