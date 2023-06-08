# Comparing `tmp/aie-sdk-2.2.5.tar.gz` & `tmp/aie-sdk-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aie-sdk-2.2.5.tar", last modified: Thu May 25 12:36:32 2023, max compression
+gzip compressed data, was "aie-sdk-3.0.1.tar", last modified: Thu Jun  8 06:03:53 2023, max compression
```

## Comparing `aie-sdk-2.2.5.tar` & `aie-sdk-3.0.1.tar`

### file list

```diff
@@ -1,64 +1,13 @@
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.959792 aie-sdk-2.2.5/
--rw-r--r--   0 songci     (502) staff       (20)     1068 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/LICENSE
--rw-r--r--   0 songci     (502) staff       (20)       21 2023-04-13 02:48:48.000000 aie-sdk-2.2.5/MANIFEST.in
--rw-r--r--   0 songci     (502) staff       (20)      429 2023-05-25 12:36:32.959282 aie-sdk-2.2.5/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/README.md
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.926748 aie-sdk-2.2.5/aie/
--rw-r--r--   0 songci     (502) staff       (20)     1128 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     2302 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/aie_env.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.936093 aie-sdk-2.2.5/aie/aie_object/
--rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/aie_object/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)    16718 2023-05-25 12:36:30.000000 aie-sdk-2.2.5/aie/aie_object/classifier.py
--rw-r--r--   0 songci     (502) staff       (20)     5220 2023-05-25 12:36:23.000000 aie-sdk-2.2.5/aie/aie_object/collection.py
--rw-r--r--   0 songci     (502) staff       (20)     2989 2023-05-25 12:36:31.000000 aie-sdk-2.2.5/aie/aie_object/confusion_matrix.py
--rw-r--r--   0 songci     (502) staff       (20)    25029 2023-05-25 12:36:26.000000 aie-sdk-2.2.5/aie/aie_object/feature.py
--rw-r--r--   0 songci     (502) staff       (20)    27844 2023-05-25 12:36:27.000000 aie-sdk-2.2.5/aie/aie_object/feature_collection.py
--rw-r--r--   0 songci     (502) staff       (20)    22776 2023-05-25 12:36:28.000000 aie-sdk-2.2.5/aie/aie_object/filter.py
--rw-r--r--   0 songci     (502) staff       (20)    24100 2023-05-25 12:36:25.000000 aie-sdk-2.2.5/aie/aie_object/geometry.py
--rw-r--r--   0 songci     (502) staff       (20)    81635 2023-05-25 12:36:23.000000 aie-sdk-2.2.5/aie/aie_object/image.py
--rw-r--r--   0 songci     (502) staff       (20)    24036 2023-05-25 12:36:24.000000 aie-sdk-2.2.5/aie/aie_object/image_collection.py
--rw-r--r--   0 songci     (502) staff       (20)    29090 2023-05-25 12:36:30.000000 aie-sdk-2.2.5/aie/aie_object/kernel.py
--rw-r--r--   0 songci     (502) staff       (20)     1462 2023-05-25 12:36:31.000000 aie-sdk-2.2.5/aie/aie_object/model.py
--rw-r--r--   0 songci     (502) staff       (20)    13971 2023-05-25 12:36:28.000000 aie-sdk-2.2.5/aie/aie_object/reducer.py
--rw-r--r--   0 songci     (502) staff       (20)     2958 2023-05-25 12:36:29.000000 aie-sdk-2.2.5/aie/aie_object/terrain.py
--rw-r--r--   0 songci     (502) staff       (20)     2570 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/auth.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.945643 aie-sdk-2.2.5/aie/client/
--rw-r--r--   0 songci     (502) staff       (20)      275 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     6639 2023-05-15 03:43:12.000000 aie-sdk-2.2.5/aie/client/client.py
--rw-r--r--   0 songci     (502) staff       (20)      775 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/constants.py
--rw-r--r--   0 songci     (502) staff       (20)     3278 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/dataset.py
--rw-r--r--   0 songci     (502) staff       (20)     1370 2022-11-21 11:41:47.000000 aie-sdk-2.2.5/aie/client/endpoints.py
--rw-r--r--   0 songci     (502) staff       (20)     8211 2023-05-15 03:43:12.000000 aie-sdk-2.2.5/aie/client/interactive_session.py
--rw-r--r--   0 songci     (502) staff       (20)     1647 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/maps.py
--rw-r--r--   0 songci     (502) staff       (20)    15854 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/mlproxy.py
--rw-r--r--   0 songci     (502) staff       (20)    18381 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/client/mlproxy_back.py
--rw-r--r--   0 songci     (502) staff       (20)     2543 2023-05-08 04:13:45.000000 aie-sdk-2.2.5/aie/client/task.py
--rw-r--r--   0 songci     (502) staff       (20)      232 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/customfunction_node.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.947429 aie-sdk-2.2.5/aie/error/
--rw-r--r--   0 songci     (502) staff       (20)      115 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/error/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)      849 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/error/aie_error.py
--rw-r--r--   0 songci     (502) staff       (20)     4264 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/export.py
--rw-r--r--   0 songci     (502) staff       (20)     1706 2023-04-10 02:23:35.000000 aie-sdk-2.2.5/aie/function_helper.py
--rw-r--r--   0 songci     (502) staff       (20)      500 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/function_node.py
--rw-r--r--   0 songci     (502) staff       (20)      907 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/g_var.py
--rw-r--r--   0 songci     (502) staff       (20)    11531 2022-12-09 06:48:05.000000 aie-sdk-2.2.5/aie/gen_python_functions.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.951750 aie-sdk-2.2.5/aie/map/
--rw-r--r--   0 songci     (502) staff       (20)       46 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/map/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     2544 2022-12-01 11:50:21.000000 aie-sdk-2.2.5/aie/map/aie_color.py
--rw-r--r--   0 songci     (502) staff       (20)     8578 2022-12-01 11:50:21.000000 aie-sdk-2.2.5/aie/map/aie_layer.py
--rw-r--r--   0 songci     (502) staff       (20)     4947 2022-12-01 11:50:21.000000 aie-sdk-2.2.5/aie/map/aie_map.py
--rw-r--r--   0 songci     (502) staff       (20)     5860 2022-12-01 11:50:21.000000 aie-sdk-2.2.5/aie/map/color.csv
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.955480 aie-sdk-2.2.5/aie/serialize/
--rw-r--r--   0 songci     (502) staff       (20)      113 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/serialize/__init__.py
--rw-r--r--   0 songci     (502) staff       (20)     4678 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/serialize/gen_visitor.py
--rw-r--r--   0 songci     (502) staff       (20)     3380 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/serialize/optimizer.py
--rw-r--r--   0 songci     (502) staff       (20)      724 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/serialize/serializer_impl.py
--rw-r--r--   0 songci     (502) staff       (20)      269 2022-11-21 06:06:45.000000 aie-sdk-2.2.5/aie/variable_node.py
-drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-05-25 12:36:32.958589 aie-sdk-2.2.5/aie_sdk.egg-info/
--rw-r--r--   0 songci     (502) staff       (20)      429 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie_sdk.egg-info/PKG-INFO
--rw-r--r--   0 songci     (502) staff       (20)     1271 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 songci     (502) staff       (20)        1 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 songci     (502) staff       (20)       79 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie_sdk.egg-info/requires.txt
--rw-r--r--   0 songci     (502) staff       (20)        4 2023-05-25 12:36:32.000000 aie-sdk-2.2.5/aie_sdk.egg-info/top_level.txt
--rw-r--r--   0 songci     (502) staff       (20)       38 2023-05-25 12:36:32.959934 aie-sdk-2.2.5/setup.cfg
--rw-r--r--   0 songci     (502) staff       (20)      891 2023-04-13 02:48:49.000000 aie-sdk-2.2.5/setup.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:03:53.916916 aie-sdk-3.0.1/
+-rw-r--r--   0 songci     (502) staff       (20)      454 2023-06-08 06:03:53.916441 aie-sdk-3.0.1/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      209 2022-11-21 06:06:45.000000 aie-sdk-3.0.1/README.md
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:03:53.912358 aie-sdk-3.0.1/aie/
+-rw-r--r--   0 songci     (502) staff       (20)      214 2023-06-06 06:51:25.000000 aie-sdk-3.0.1/aie/__init__.py
+drwxr-xr-x   0 songci     (502) staff       (20)        0 2023-06-08 06:03:53.915461 aie-sdk-3.0.1/aie_sdk.egg-info/
+-rw-r--r--   0 songci     (502) staff       (20)      454 2023-06-08 06:03:53.000000 aie-sdk-3.0.1/aie_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 songci     (502) staff       (20)      188 2023-06-08 06:03:53.000000 aie-sdk-3.0.1/aie_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 songci     (502) staff       (20)        1 2023-06-08 06:03:53.000000 aie-sdk-3.0.1/aie_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 songci     (502) staff       (20)      248 2023-06-08 06:03:53.000000 aie-sdk-3.0.1/aie_sdk.egg-info/requires.txt
+-rw-r--r--   0 songci     (502) staff       (20)        4 2023-06-08 06:03:53.000000 aie-sdk-3.0.1/aie_sdk.egg-info/top_level.txt
+-rw-r--r--   0 songci     (502) staff       (20)       38 2023-06-08 06:03:53.917051 aie-sdk-3.0.1/setup.cfg
+-rw-r--r--   0 songci     (502) staff       (20)     1103 2023-06-08 06:03:40.000000 aie-sdk-3.0.1/setup.py
```

