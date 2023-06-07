# Comparing `tmp/LiamHsieh toolbox-0.3.4.1.tar.gz` & `tmp/LiamHsieh toolbox-0.3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LiamHsieh toolbox-0.3.4.1.tar", last modified: Wed Jun  7 00:26:36 2023, max compression
+gzip compressed data, was "LiamHsieh toolbox-0.3.4.2.tar", last modified: Wed Jun  7 00:37:00 2023, max compression
```

## Comparing `LiamHsieh toolbox-0.3.4.1.tar` & `LiamHsieh toolbox-0.3.4.2.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.401184 LiamHsieh toolbox-0.3.4.1/LiamHsieh_toolbox.egg-info/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1263 2023-06-07 00:26:36.000000 LiamHsieh toolbox-0.3.4.1/LiamHsieh_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1418 2023-06-07 00:26:36.000000 LiamHsieh toolbox-0.3.4.1/LiamHsieh_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        1 2023-06-07 00:26:36.000000 LiamHsieh toolbox-0.3.4.1/LiamHsieh_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      308 2023-06-07 00:26:36.000000 LiamHsieh toolbox-0.3.4.1/LiamHsieh_toolbox.egg-info/requires.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        8 2023-06-07 00:26:36.000000 LiamHsieh toolbox-0.3.4.1/LiamHsieh_toolbox.egg-info/top_level.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1263 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/PKG-INFO
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      836 2023-06-06 22:25:15.000000 LiamHsieh toolbox-0.3.4.1/README.md
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       38 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/setup.cfg
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1411 2023-06-07 00:26:17.000000 LiamHsieh toolbox-0.3.4.1/setup.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.401184 LiamHsieh toolbox-0.3.4.1/toolbox/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       16 2023-06-07 00:20:41.000000 LiamHsieh toolbox-0.3.4.1/toolbox/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.401184 LiamHsieh toolbox-0.3.4.1/toolbox/container/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       54 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/container/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      431 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/container/namedtuple_from_dict.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/dao/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       24 2022-10-14 15:49:23.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/dao/connector/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      110 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/connector/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    11674 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/connector/blob_connector.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     7757 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/connector/db_connector.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-20 00:12:45.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/connector/excel_connector.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        2 2022-08-22 23:23:30.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/connector/sqlite_connector.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1063 2022-10-14 03:38:34.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/dtypes.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    11400 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/feed.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/dao/files/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      237 2022-09-08 21:52:27.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/files/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      219 2022-09-01 18:22:27.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/files/dtype_detect.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1846 2022-09-02 15:12:44.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/files/ftype_detect.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    10649 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/files/loader.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1339 2022-09-08 01:05:55.000000 LiamHsieh toolbox-0.3.4.1/toolbox/dao/files/utility.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/metaheuristic/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.1/toolbox/metaheuristic/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/optimization/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.1/toolbox/optimization/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/optimization/docplex/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       91 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.1/toolbox/optimization/docplex/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       49 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.1/toolbox/optimization/docplex/model.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       53 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.1/toolbox/optimization/docplex/model_feed.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       53 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.1/toolbox/optimization/docplex/procedure.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/stats/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       86 2022-09-29 00:15:54.000000 LiamHsieh toolbox-0.3.4.1/toolbox/stats/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/component/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      164 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/component/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     6663 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/component/blob_container_explorer.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1316 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/component/supplement.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     3059 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/component/whiteboard.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/toybox/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      109 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/toybox/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1270 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/toybox/toybox.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      696 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/toybox/toybox_functions.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     2513 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.1/toolbox/utility.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:26:36.411184 LiamHsieh toolbox-0.3.4.1/toolbox/watcher/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       65 2022-10-14 20:44:54.000000 LiamHsieh toolbox-0.3.4.1/toolbox/watcher/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      693 2022-10-14 21:17:50.000000 LiamHsieh toolbox-0.3.4.1/toolbox/watcher/get_obj_size.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      809 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.1/toolbox/watcher/timeit.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.371184 LiamHsieh toolbox-0.3.4.2/
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/LiamHsieh_toolbox.egg-info/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1263 2023-06-07 00:37:00.000000 LiamHsieh toolbox-0.3.4.2/LiamHsieh_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1481 2023-06-07 00:37:00.000000 LiamHsieh toolbox-0.3.4.2/LiamHsieh_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        1 2023-06-07 00:37:00.000000 LiamHsieh toolbox-0.3.4.2/LiamHsieh_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      308 2023-06-07 00:37:00.000000 LiamHsieh toolbox-0.3.4.2/LiamHsieh_toolbox.egg-info/requires.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        8 2023-06-07 00:37:00.000000 LiamHsieh toolbox-0.3.4.2/LiamHsieh_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1263 2023-06-07 00:37:00.371184 LiamHsieh toolbox-0.3.4.2/PKG-INFO
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      836 2023-06-06 22:25:15.000000 LiamHsieh toolbox-0.3.4.2/README.md
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       38 2023-06-07 00:37:00.371184 LiamHsieh toolbox-0.3.4.2/setup.cfg
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1411 2023-06-07 00:36:02.000000 LiamHsieh toolbox-0.3.4.2/setup.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       16 2023-06-07 00:20:41.000000 LiamHsieh toolbox-0.3.4.2/toolbox/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/container/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       54 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/container/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      431 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/container/namedtuple_from_dict.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/dao/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       24 2022-10-14 15:49:23.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/dao/connector/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      110 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/connector/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    11674 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/connector/blob_connector.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     7757 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/connector/db_connector.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-20 00:12:45.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/connector/excel_connector.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        2 2022-08-22 23:23:30.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/connector/sqlite_connector.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1063 2022-10-14 03:38:34.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/dtypes.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    11400 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/feed.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/dao/files/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      237 2022-09-08 21:52:27.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/files/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      219 2022-09-01 18:22:27.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/files/dtype_detect.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1846 2022-09-02 15:12:44.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/files/ftype_detect.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    10649 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/files/loader.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1339 2022-09-08 01:05:55.000000 LiamHsieh toolbox-0.3.4.2/toolbox/dao/files/utility.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/metaheuristic/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.2/toolbox/metaheuristic/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/optimization/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.2/toolbox/optimization/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/optimization/docplex/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       91 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.2/toolbox/optimization/docplex/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       49 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.2/toolbox/optimization/docplex/model.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       53 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.2/toolbox/optimization/docplex/model_feed.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       53 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.2/toolbox/optimization/docplex/procedure.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/stats/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       86 2022-09-29 00:15:54.000000 LiamHsieh toolbox-0.3.4.2/toolbox/stats/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/component/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      164 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/component/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     6663 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/component/blob_container_explorer.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1316 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/component/supplement.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     3059 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/component/whiteboard.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.361184 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/toybox/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      109 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/toybox/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1270 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/toybox/toybox.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      696 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/toybox/toybox_functions.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.371184 LiamHsieh toolbox-0.3.4.2/toolbox/string/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      141 2023-06-07 00:35:26.000000 LiamHsieh toolbox-0.3.4.2/toolbox/string/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      522 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/string/convert_functions.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     2513 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.2/toolbox/utility.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 00:37:00.371184 LiamHsieh toolbox-0.3.4.2/toolbox/watcher/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       65 2022-10-14 20:44:54.000000 LiamHsieh toolbox-0.3.4.2/toolbox/watcher/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      693 2022-10-14 21:17:50.000000 LiamHsieh toolbox-0.3.4.2/toolbox/watcher/get_obj_size.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      809 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.2/toolbox/watcher/timeit.py
```

### Comparing `LiamHsieh toolbox-0.3.4.1/LiamHsieh_toolbox.egg-info/PKG-INFO` & `LiamHsieh toolbox-0.3.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: LiamHsieh-toolbox
-Version: 0.3.4.1
+Name: LiamHsieh toolbox
+Version: 0.3.4.2
 Summary: Collections of Python utility, suppose to be built with Jonathan Carson but he left
 Author: Liam Y. Hsieh, PhD
 Author-email: liamhsieh@ieee.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.9
```

### Comparing `LiamHsieh toolbox-0.3.4.1/LiamHsieh_toolbox.egg-info/SOURCES.txt` & `LiamHsieh toolbox-0.3.4.2/LiamHsieh_toolbox.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -33,10 +33,12 @@
 toolbox/streamlit/component/__init__.py
 toolbox/streamlit/component/blob_container_explorer.py
 toolbox/streamlit/component/supplement.py
 toolbox/streamlit/component/whiteboard.py
 toolbox/streamlit/toybox/__init__.py
 toolbox/streamlit/toybox/toybox.py
 toolbox/streamlit/toybox/toybox_functions.py
+toolbox/string/__init__.py
+toolbox/string/convert_functions.py
 toolbox/watcher/__init__.py
 toolbox/watcher/get_obj_size.py
 toolbox/watcher/timeit.py
```

### Comparing `LiamHsieh toolbox-0.3.4.1/PKG-INFO` & `LiamHsieh toolbox-0.3.4.2/LiamHsieh_toolbox.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: LiamHsieh toolbox
-Version: 0.3.4.1
+Name: LiamHsieh-toolbox
+Version: 0.3.4.2
 Summary: Collections of Python utility, suppose to be built with Jonathan Carson but he left
 Author: Liam Y. Hsieh, PhD
 Author-email: liamhsieh@ieee.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.9
```

### Comparing `LiamHsieh toolbox-0.3.4.1/README.md` & `LiamHsieh toolbox-0.3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/setup.py` & `LiamHsieh toolbox-0.3.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="LiamHsieh toolbox",
-    version = '0.3.4.1',
+    version = '0.3.4.2',
     description = "Collections of Python utility, suppose to be built with Jonathan Carson but he left",
     author = 'Liam Y. Hsieh, PhD',
     author_email = 'liamhsieh@ieee.org',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     classifiers = [
```

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/dao/connector/blob_connector.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/dao/connector/blob_connector.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/dao/connector/db_connector.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/dao/connector/db_connector.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/dao/dtypes.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/dao/dtypes.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/dao/feed.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/dao/feed.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/dao/files/ftype_detect.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/dao/files/ftype_detect.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/dao/files/loader.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/dao/files/loader.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/dao/files/utility.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/dao/files/utility.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/component/blob_container_explorer.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/component/blob_container_explorer.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/component/supplement.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/component/supplement.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/component/whiteboard.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/component/whiteboard.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/toybox/toybox.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/toybox/toybox.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/streamlit/toybox/toybox_functions.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/streamlit/toybox/toybox_functions.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/utility.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/utility.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/watcher/get_obj_size.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/watcher/get_obj_size.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.1/toolbox/watcher/timeit.py` & `LiamHsieh toolbox-0.3.4.2/toolbox/watcher/timeit.py`

 * *Files identical despite different names*

