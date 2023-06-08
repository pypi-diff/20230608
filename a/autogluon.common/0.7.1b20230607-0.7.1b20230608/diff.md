# Comparing `tmp/autogluon.common-0.7.1b20230607.tar.gz` & `tmp/autogluon.common-0.7.1b20230608.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.common-0.7.1b20230607.tar", last modified: Wed Jun  7 09:03:47 2023, max compression
+gzip compressed data, was "autogluon.common-0.7.1b20230608.tar", last modified: Thu Jun  8 09:04:00 2023, max compression
```

## Comparing `autogluon.common-0.7.1b20230607.tar` & `autogluon.common-0.7.1b20230608.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:47.618664 autogluon.common-0.7.1b20230607/
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-07 09:03:47.618664 autogluon.common-0.7.1b20230607/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:03:47.618664 autogluon.common-0.7.1b20230607/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:47.610664 autogluon.common-0.7.1b20230607/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:47.610664 autogluon.common-0.7.1b20230607/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:47.614663 autogluon.common-0.7.1b20230607/src/autogluon/common/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:47.614663 autogluon.common-0.7.1b20230607/src/autogluon/common/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/features/feature_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/features/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/features/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:47.614663 autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_str.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:47.618664 autogluon.common-0.7.1b20230607/src/autogluon/common/model_filter/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/model_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/model_filter/_model_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:47.618664 autogluon.common-0.7.1b20230607/src/autogluon/common/savers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/savers/save_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/savers/save_pd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/savers/save_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/savers/save_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/savers/save_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:47.618664 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/compression_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/deprecated_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/distribute_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/multiprocessing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/nvutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/pandas_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/path_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/resource_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/try_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-07 09:03:36.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 09:03:46.000000 autogluon.common-0.7.1b20230607/src/autogluon/common/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:03:47.614663 autogluon.common-0.7.1b20230607/src/autogluon.common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-07 09:03:47.000000 autogluon.common-0.7.1b20230607/src/autogluon.common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-07 09:03:47.000000 autogluon.common-0.7.1b20230607/src/autogluon.common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:03:47.000000 autogluon.common-0.7.1b20230607/src/autogluon.common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 09:03:47.000000 autogluon.common-0.7.1b20230607/src/autogluon.common.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 09:03:47.000000 autogluon.common-0.7.1b20230607/src/autogluon.common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 09:03:47.000000 autogluon.common-0.7.1b20230607/src/autogluon.common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:03:47.000000 autogluon.common-0.7.1b20230607/src/autogluon.common.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:00.890077 autogluon.common-0.7.1b20230608/
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-08 09:04:00.890077 autogluon.common-0.7.1b20230608/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:04:00.890077 autogluon.common-0.7.1b20230608/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:00.882077 autogluon.common-0.7.1b20230608/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:00.882077 autogluon.common-0.7.1b20230608/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:00.882077 autogluon.common-0.7.1b20230608/src/autogluon/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:00.886077 autogluon.common-0.7.1b20230608/src/autogluon/common/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/features/feature_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/features/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/features/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:00.886077 autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10152 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:00.886077 autogluon.common-0.7.1b20230608/src/autogluon/common/model_filter/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/model_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/model_filter/_model_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:00.886077 autogluon.common-0.7.1b20230608/src/autogluon/common/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/savers/save_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/savers/save_pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/savers/save_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/savers/save_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/savers/save_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:00.890077 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/compression_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/deprecated_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/distribute_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/multiprocessing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/nvutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/pandas_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/path_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/resource_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16670 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/try_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-08 09:03:43.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 09:04:00.000000 autogluon.common-0.7.1b20230608/src/autogluon/common/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:00.882077 autogluon.common-0.7.1b20230608/src/autogluon.common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-06-08 09:04:00.000000 autogluon.common-0.7.1b20230608/src/autogluon.common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-08 09:04:00.000000 autogluon.common-0.7.1b20230608/src/autogluon.common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:04:00.000000 autogluon.common-0.7.1b20230608/src/autogluon.common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 09:04:00.000000 autogluon.common-0.7.1b20230608/src/autogluon.common.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-08 09:04:00.000000 autogluon.common-0.7.1b20230608/src/autogluon.common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 09:04:00.000000 autogluon.common-0.7.1b20230608/src/autogluon.common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:04:00.000000 autogluon.common-0.7.1b20230608/src/autogluon.common.egg-info/zip-safe
```

### Comparing `autogluon.common-0.7.1b20230607/LICENSE` & `autogluon.common-0.7.1b20230608/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/PKG-INFO` & `autogluon.common-0.7.1b20230608/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230607
+Version: 0.7.1b20230608
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230607/setup.py` & `autogluon.common-0.7.1b20230608/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/features/feature_metadata.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/features/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/features/infer_types.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/features/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/features/types.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/features/types.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/_utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_pd.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_pkl.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_pointer.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_pointer.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_s3.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_s3.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_str.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/loaders/load_zip.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/loaders/load_zip.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/model_filter/_model_filter.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/model_filter/_model_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Class to filter models given user requirements"""
 
     @staticmethod
     def include_models(
         models: Union[Dict[str, Any], List[str]], included_model_types: List[str]
     ) -> Union[Dict[str, Any], List[str]]:
         """
-        Only include models specifeid in `included_model_types`, other models will be removed
+        Only include models specified in `included_model_types`, other models will be removed
         If model specified in `included_model_types` doesn't present in `models`, will warn users and ignore
 
         Parameters
         ----------
         models: Union[Dict[str, Any], List[str]]
             A dictionary containing models and their hyperparameters
         included_model_types: List[str]
@@ -29,17 +29,19 @@
         """
         if isinstance(models, dict):
             included_models = {model: val for model, val in models.items() if model in included_model_types}
             missing_models = set(included_model_types) - set(included_models.keys())
         elif isinstance(models, list):
             included_models = [model for model in models if model in included_model_types]
             missing_models = set(included_model_types) - set(included_models)
+        if included_model_types is not None:
+            logger.log(20, f"Included models: {list(included_model_types)} (Specified by `included_model_types`, all other model types will be skipped)")
         if len(missing_models) > 0:
             logger.warning(
-                f"The models types {missing_models} are not present in the model list specified by the user and will be ignored:"
+                f"\tThe models types {list(missing_models)} are not present in the model list specified by the user and will be ignored:"
             )
         return included_models
 
     @staticmethod
     def exclude_models(
         models: Union[Dict[str, Any], List[str]], excluded_model_types: List[str]
     ) -> Union[Dict[str, Any], List[str]]:
@@ -63,15 +65,15 @@
         if isinstance(models, dict):
             models_after_exclusion = {model: val for model, val in models.items() if model not in excluded_model_types}
             excluded_models = set(models.keys()) - set(models_after_exclusion.keys())
         elif isinstance(models, list):
             models_after_exclusion = [model for model in models if model not in excluded_model_types]
             excluded_models = set(models) - set(models_after_exclusion)
         if excluded_models is not None:
-            logger.log(20, f"Excluded models: {excluded_models}")
+            logger.log(20, f"Excluded models: {list(excluded_models)} (Specified by `excluded_model_types`)")
         return models_after_exclusion
 
     @staticmethod
     def filter_models(
         models: Union[Dict[str, Any], List[str]],
         included_model_types: Optional[List[str]] = None,
         excluded_model_types: Optional[List[str]] = None,
```

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/savers/save_json.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/savers/save_json.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/savers/save_pd.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/savers/save_pd.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/savers/save_pkl.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/savers/save_pkl.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/savers/save_str.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/savers/save_str.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/space.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/compression_utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/compression_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/deprecated_utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/deprecated_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/distribute_utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/distribute_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/file_utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/log_utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/multiprocessing_utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/multiprocessing_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/nvutil.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/nvutil.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/pandas_utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/path_converter.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/path_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/resource_utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/resource_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/s3_utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/try_import.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/try_import.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon/common/utils/utils.py` & `autogluon.common-0.7.1b20230608/src/autogluon/common/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon.common.egg-info/PKG-INFO` & `autogluon.common-0.7.1b20230608/src/autogluon.common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.common
-Version: 0.7.1b20230607
+Version: 0.7.1b20230608
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.common-0.7.1b20230607/src/autogluon.common.egg-info/SOURCES.txt` & `autogluon.common-0.7.1b20230608/src/autogluon.common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

