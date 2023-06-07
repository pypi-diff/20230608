# Comparing `tmp/LiamHsieh toolbox-0.3.4.4.tar.gz` & `tmp/LiamHsieh toolbox-0.3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LiamHsieh toolbox-0.3.4.4.tar", last modified: Wed Jun  7 23:45:00 2023, max compression
+gzip compressed data, was "LiamHsieh toolbox-0.3.4.5.tar", last modified: Wed Jun  7 23:48:25 2023, max compression
```

## Comparing `LiamHsieh toolbox-0.3.4.4.tar` & `LiamHsieh toolbox-0.3.4.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.834376 LiamHsieh toolbox-0.3.4.4/
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/LiamHsieh_toolbox.egg-info/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1264 2023-06-07 23:45:00.000000 LiamHsieh toolbox-0.3.4.4/LiamHsieh_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1481 2023-06-07 23:45:00.000000 LiamHsieh toolbox-0.3.4.4/LiamHsieh_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        1 2023-06-07 23:45:00.000000 LiamHsieh toolbox-0.3.4.4/LiamHsieh_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      308 2023-06-07 23:45:00.000000 LiamHsieh toolbox-0.3.4.4/LiamHsieh_toolbox.egg-info/requires.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        8 2023-06-07 23:45:00.000000 LiamHsieh toolbox-0.3.4.4/LiamHsieh_toolbox.egg-info/top_level.txt
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1264 2023-06-07 23:45:00.834376 LiamHsieh toolbox-0.3.4.4/PKG-INFO
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      836 2023-06-06 22:25:15.000000 LiamHsieh toolbox-0.3.4.4/README.md
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       38 2023-06-07 23:45:00.834376 LiamHsieh toolbox-0.3.4.4/setup.cfg
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1412 2023-06-07 23:44:56.000000 LiamHsieh toolbox-0.3.4.4/setup.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/toolbox/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       16 2023-06-07 00:20:41.000000 LiamHsieh toolbox-0.3.4.4/toolbox/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/toolbox/container/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       54 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/container/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      431 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/container/namedtuple_from_dict.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/toolbox/dao/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       24 2022-10-14 15:49:23.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/toolbox/dao/connector/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      110 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/connector/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    11674 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/connector/blob_connector.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     7806 2023-06-07 23:43:40.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/connector/db_connector.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-20 00:12:45.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/connector/excel_connector.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        2 2022-08-22 23:23:30.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/connector/sqlite_connector.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1063 2022-10-14 03:38:34.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/dtypes.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    11400 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/feed.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/toolbox/dao/files/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      237 2022-09-08 21:52:27.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/files/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      219 2022-09-01 18:22:27.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/files/dtype_detect.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1846 2022-09-02 15:12:44.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/files/ftype_detect.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    10649 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/files/loader.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1339 2022-09-08 01:05:55.000000 LiamHsieh toolbox-0.3.4.4/toolbox/dao/files/utility.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/toolbox/metaheuristic/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.4/toolbox/metaheuristic/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/toolbox/optimization/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.4/toolbox/optimization/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/toolbox/optimization/docplex/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       91 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.4/toolbox/optimization/docplex/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       49 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.4/toolbox/optimization/docplex/model.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       53 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.4/toolbox/optimization/docplex/model_feed.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       53 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.4/toolbox/optimization/docplex/procedure.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/toolbox/stats/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       86 2022-09-29 00:15:54.000000 LiamHsieh toolbox-0.3.4.4/toolbox/stats/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.824376 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/__init__.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.834376 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/component/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      164 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/component/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     6663 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/component/blob_container_explorer.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1316 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/component/supplement.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     3059 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/component/whiteboard.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.834376 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/toybox/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      109 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/toybox/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1270 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/toybox/toybox.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      696 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/toybox/toybox_functions.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.834376 LiamHsieh toolbox-0.3.4.4/toolbox/string/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      141 2023-06-07 00:35:26.000000 LiamHsieh toolbox-0.3.4.4/toolbox/string/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      522 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/string/convert_functions.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     2513 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.4/toolbox/utility.py
-drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:45:00.834376 LiamHsieh toolbox-0.3.4.4/toolbox/watcher/
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       65 2022-10-14 20:44:54.000000 LiamHsieh toolbox-0.3.4.4/toolbox/watcher/__init__.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      693 2022-10-14 21:17:50.000000 LiamHsieh toolbox-0.3.4.4/toolbox/watcher/get_obj_size.py
--rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      809 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.4/toolbox/watcher/timeit.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.374376 LiamHsieh toolbox-0.3.4.5/
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.354376 LiamHsieh toolbox-0.3.4.5/LiamHsieh_toolbox.egg-info/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1264 2023-06-07 23:48:25.000000 LiamHsieh toolbox-0.3.4.5/LiamHsieh_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1481 2023-06-07 23:48:25.000000 LiamHsieh toolbox-0.3.4.5/LiamHsieh_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        1 2023-06-07 23:48:25.000000 LiamHsieh toolbox-0.3.4.5/LiamHsieh_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      308 2023-06-07 23:48:25.000000 LiamHsieh toolbox-0.3.4.5/LiamHsieh_toolbox.egg-info/requires.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        8 2023-06-07 23:48:25.000000 LiamHsieh toolbox-0.3.4.5/LiamHsieh_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1264 2023-06-07 23:48:25.374376 LiamHsieh toolbox-0.3.4.5/PKG-INFO
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      836 2023-06-06 22:25:15.000000 LiamHsieh toolbox-0.3.4.5/README.md
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       38 2023-06-07 23:48:25.374376 LiamHsieh toolbox-0.3.4.5/setup.cfg
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1412 2023-06-07 23:48:16.000000 LiamHsieh toolbox-0.3.4.5/setup.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.354376 LiamHsieh toolbox-0.3.4.5/toolbox/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       16 2023-06-07 00:20:41.000000 LiamHsieh toolbox-0.3.4.5/toolbox/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.354376 LiamHsieh toolbox-0.3.4.5/toolbox/container/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       54 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/container/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      431 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/container/namedtuple_from_dict.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.364376 LiamHsieh toolbox-0.3.4.5/toolbox/dao/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       24 2022-10-14 15:49:23.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.364376 LiamHsieh toolbox-0.3.4.5/toolbox/dao/connector/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      110 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/connector/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    11674 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/connector/blob_connector.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     7806 2023-06-07 23:43:40.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/connector/db_connector.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-20 00:12:45.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/connector/excel_connector.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        2 2022-08-22 23:23:30.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/connector/sqlite_connector.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1063 2022-10-14 03:38:34.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/dtypes.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    11400 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/feed.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.364376 LiamHsieh toolbox-0.3.4.5/toolbox/dao/files/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      237 2022-09-08 21:52:27.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/files/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      219 2022-09-01 18:22:27.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/files/dtype_detect.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1846 2022-09-02 15:12:44.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/files/ftype_detect.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)    10649 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/files/loader.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1339 2022-09-08 01:05:55.000000 LiamHsieh toolbox-0.3.4.5/toolbox/dao/files/utility.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.364376 LiamHsieh toolbox-0.3.4.5/toolbox/metaheuristic/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.5/toolbox/metaheuristic/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.364376 LiamHsieh toolbox-0.3.4.5/toolbox/optimization/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.5/toolbox/optimization/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.364376 LiamHsieh toolbox-0.3.4.5/toolbox/optimization/docplex/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       91 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.5/toolbox/optimization/docplex/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       49 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.5/toolbox/optimization/docplex/model.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       53 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.5/toolbox/optimization/docplex/model_feed.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       53 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.5/toolbox/optimization/docplex/procedure.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.364376 LiamHsieh toolbox-0.3.4.5/toolbox/stats/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       86 2022-09-29 00:15:54.000000 LiamHsieh toolbox-0.3.4.5/toolbox/stats/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.364376 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)        0 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/__init__.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.374376 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/component/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      164 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/component/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     6663 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/component/blob_container_explorer.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1316 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/component/supplement.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     3059 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/component/whiteboard.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.374376 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/toybox/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      109 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/toybox/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     1270 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/toybox/toybox.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      696 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/toybox/toybox_functions.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.374376 LiamHsieh toolbox-0.3.4.5/toolbox/string/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      141 2023-06-07 00:35:26.000000 LiamHsieh toolbox-0.3.4.5/toolbox/string/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      522 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/string/convert_functions.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)     2513 2023-03-23 00:54:07.000000 LiamHsieh toolbox-0.3.4.5/toolbox/utility.py
+drwxr-xr-x   0 lhsieh    (1000) lhsieh    (1000)        0 2023-06-07 23:48:25.374376 LiamHsieh toolbox-0.3.4.5/toolbox/watcher/
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)       65 2022-10-14 20:44:54.000000 LiamHsieh toolbox-0.3.4.5/toolbox/watcher/__init__.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      693 2022-10-14 21:17:50.000000 LiamHsieh toolbox-0.3.4.5/toolbox/watcher/get_obj_size.py
+-rw-r--r--   0 lhsieh    (1000) lhsieh    (1000)      809 2022-08-19 18:39:08.000000 LiamHsieh toolbox-0.3.4.5/toolbox/watcher/timeit.py
```

### Comparing `LiamHsieh toolbox-0.3.4.4/LiamHsieh_toolbox.egg-info/PKG-INFO` & `LiamHsieh toolbox-0.3.4.5/LiamHsieh_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LiamHsieh-toolbox
-Version: 0.3.4.4
+Version: 0.3.4.5
 Summary: Collections of Python utility, suppose to be built with Jonathan Carson but he left
 Author: Liam Y. Hsieh, PhD
 Author-email: liamhsieh@ieee.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
```

### Comparing `LiamHsieh toolbox-0.3.4.4/LiamHsieh_toolbox.egg-info/SOURCES.txt` & `LiamHsieh toolbox-0.3.4.5/LiamHsieh_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/PKG-INFO` & `LiamHsieh toolbox-0.3.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LiamHsieh toolbox
-Version: 0.3.4.4
+Version: 0.3.4.5
 Summary: Collections of Python utility, suppose to be built with Jonathan Carson but he left
 Author: Liam Y. Hsieh, PhD
 Author-email: liamhsieh@ieee.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.10
```

### Comparing `LiamHsieh toolbox-0.3.4.4/README.md` & `LiamHsieh toolbox-0.3.4.5/README.md`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/setup.py` & `LiamHsieh toolbox-0.3.4.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="LiamHsieh toolbox",
-    version = '0.3.4.4',
+    version = '0.3.4.5',
     description = "Collections of Python utility, suppose to be built with Jonathan Carson but he left",
     author = 'Liam Y. Hsieh, PhD',
     author_email = 'liamhsieh@ieee.org',
     long_description = long_description,
     long_description_content_type = "text/markdown",
     packages = setuptools.find_packages(),
     classifiers = [
```

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/dao/connector/blob_connector.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/dao/connector/blob_connector.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/dao/connector/db_connector.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/dao/connector/db_connector.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/dao/dtypes.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/dao/dtypes.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/dao/feed.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/dao/feed.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/dao/files/ftype_detect.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/dao/files/ftype_detect.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/dao/files/loader.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/dao/files/loader.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/dao/files/utility.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/dao/files/utility.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/component/blob_container_explorer.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/component/blob_container_explorer.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/component/supplement.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/component/supplement.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/component/whiteboard.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/component/whiteboard.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/toybox/toybox.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/toybox/toybox.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/streamlit/toybox/toybox_functions.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/streamlit/toybox/toybox_functions.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/string/convert_functions.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/string/convert_functions.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/utility.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/utility.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/watcher/get_obj_size.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/watcher/get_obj_size.py`

 * *Files identical despite different names*

### Comparing `LiamHsieh toolbox-0.3.4.4/toolbox/watcher/timeit.py` & `LiamHsieh toolbox-0.3.4.5/toolbox/watcher/timeit.py`

 * *Files identical despite different names*

