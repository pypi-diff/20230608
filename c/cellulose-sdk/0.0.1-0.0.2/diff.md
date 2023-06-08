# Comparing `tmp/cellulose-sdk-0.0.1.tar.gz` & `tmp/cellulose-sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellulose-sdk-0.0.1.tar", last modified: Wed Jun  7 23:18:39 2023, max compression
+gzip compressed data, was "cellulose-sdk-0.0.2.tar", last modified: Thu Jun  8 00:06:06 2023, max compression
```

## Comparing `cellulose-sdk-0.0.1.tar` & `cellulose-sdk-0.0.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.411346 cellulose-sdk-0.0.1/
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1066 2023-06-07 06:11:27.000000 cellulose-sdk-0.0.1/LICENSE
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1517 2023-06-07 23:18:39.411231 cellulose-sdk-0.0.1/PKG-INFO
--rw-r--r--   0 tzhenghao   (501) staff       (20)      377 2023-06-07 06:13:41.000000 cellulose-sdk-0.0.1/README.md
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.404013 cellulose-sdk-0.0.1/cellulose/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/__init__.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.404336 cellulose-sdk-0.0.1/cellulose/api/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/api/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     3174 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/api/cellulose_context.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.404968 cellulose-sdk-0.0.1/cellulose/artifact/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/artifact/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      484 2023-06-07 04:03:32.000000 cellulose-sdk-0.0.1/cellulose/artifact/cellulose_artifact.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     6010 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/artifact/cellulose_artifact_manager.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.405788 cellulose-sdk-0.0.1/cellulose/base/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/base/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     2100 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/base/benchmark.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      102 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/base/checker.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      327 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/base/export.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      101 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/base/loader.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.406620 cellulose-sdk-0.0.1/cellulose/configs/
--rw-r--r--   0 tzhenghao   (501) staff       (20)      984 2023-06-07 05:08:49.000000 cellulose-sdk-0.0.1/cellulose/configs/.cellulose_config.toml
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/configs/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1996 2023-06-07 06:17:16.000000 cellulose-sdk-0.0.1/cellulose/configs/config.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     6885 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/configs/loader.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.406891 cellulose-sdk-0.0.1/cellulose/decorators/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/decorators/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     8400 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/decorators/cellulose.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.407033 cellulose-sdk-0.0.1/cellulose/infra/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/infra/__init__.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.407352 cellulose-sdk-0.0.1/cellulose/metrics/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/metrics/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      430 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/metrics/latency.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)       90 2023-06-07 04:03:32.000000 cellulose-sdk-0.0.1/cellulose/metrics/metrics.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.408321 cellulose-sdk-0.0.1/cellulose/onnx/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/onnx/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1608 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/onnx/benchmark.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      311 2023-06-07 06:23:27.000000 cellulose-sdk-0.0.1/cellulose/onnx/checker.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      499 2023-06-07 06:23:27.000000 cellulose-sdk-0.0.1/cellulose/onnx/loader.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      962 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/onnx/runtime.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.408579 cellulose-sdk-0.0.1/cellulose/output/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/output/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      403 2023-06-07 05:06:52.000000 cellulose-sdk-0.0.1/cellulose/output/output.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.409027 cellulose-sdk-0.0.1/cellulose/pytorch/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/pytorch/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1014 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/pytorch/benchmark.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)     4819 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/pytorch/export.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.409187 cellulose-sdk-0.0.1/cellulose/scripts/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/scripts/__init__.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.409283 cellulose-sdk-0.0.1/cellulose/tensorflow/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/tensorflow/__init__.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.410120 cellulose-sdk-0.0.1/cellulose/utils/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/utils/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      895 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.1/cellulose/utils/benchmark_results.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      967 2023-06-07 06:17:16.000000 cellulose-sdk-0.0.1/cellulose/utils/csv_utils.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      180 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/utils/devices.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      260 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/utils/engines.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      266 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/utils/numpy.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.410390 cellulose-sdk-0.0.1/cellulose/validation/
--rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/validation/__init__.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)      667 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/validation/validation.py
--rw-r--r--   0 tzhenghao   (501) staff       (20)       32 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.1/cellulose/version.py
-drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-07 23:18:39.411060 cellulose-sdk-0.0.1/cellulose_sdk.egg-info/
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1517 2023-06-07 23:18:39.000000 cellulose-sdk-0.0.1/cellulose_sdk.egg-info/PKG-INFO
--rw-r--r--   0 tzhenghao   (501) staff       (20)     1472 2023-06-07 23:18:39.000000 cellulose-sdk-0.0.1/cellulose_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 tzhenghao   (501) staff       (20)        1 2023-06-07 23:18:39.000000 cellulose-sdk-0.0.1/cellulose_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 tzhenghao   (501) staff       (20)      191 2023-06-07 23:18:39.000000 cellulose-sdk-0.0.1/cellulose_sdk.egg-info/requires.txt
--rw-r--r--   0 tzhenghao   (501) staff       (20)       10 2023-06-07 23:18:39.000000 cellulose-sdk-0.0.1/cellulose_sdk.egg-info/top_level.txt
--rw-r--r--   0 tzhenghao   (501) staff       (20)      505 2023-06-07 06:23:01.000000 cellulose-sdk-0.0.1/pyproject.toml
--rw-r--r--   0 tzhenghao   (501) staff       (20)       38 2023-06-07 23:18:39.411379 cellulose-sdk-0.0.1/setup.cfg
--rw-r--r--   0 tzhenghao   (501) staff       (20)     8574 2023-06-07 23:16:44.000000 cellulose-sdk-0.0.1/setup.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.444011 cellulose-sdk-0.0.2/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1066 2023-06-07 06:11:27.000000 cellulose-sdk-0.0.2/LICENSE
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1517 2023-06-08 00:06:06.443906 cellulose-sdk-0.0.2/PKG-INFO
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      377 2023-06-07 06:13:41.000000 cellulose-sdk-0.0.2/README.md
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.437448 cellulose-sdk-0.0.2/cellulose/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/__init__.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.437749 cellulose-sdk-0.0.2/cellulose/api/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/api/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     3174 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/api/cellulose_context.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.438215 cellulose-sdk-0.0.2/cellulose/artifact/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/artifact/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      423 2023-06-08 00:02:40.000000 cellulose-sdk-0.0.2/cellulose/artifact/cellulose_artifact.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     6179 2023-06-08 00:03:53.000000 cellulose-sdk-0.0.2/cellulose/artifact/cellulose_artifact_manager.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.438909 cellulose-sdk-0.0.2/cellulose/base/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/base/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     2100 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/base/benchmark.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      102 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/base/checker.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      327 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/base/export.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      101 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/base/loader.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.439712 cellulose-sdk-0.0.2/cellulose/configs/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      984 2023-06-07 05:08:49.000000 cellulose-sdk-0.0.2/cellulose/configs/.cellulose_config.toml
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/configs/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1996 2023-06-07 06:17:16.000000 cellulose-sdk-0.0.2/cellulose/configs/config.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     6885 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/configs/loader.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.439925 cellulose-sdk-0.0.2/cellulose/decorators/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/decorators/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     8400 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/decorators/cellulose.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.440058 cellulose-sdk-0.0.2/cellulose/infra/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/infra/__init__.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.440389 cellulose-sdk-0.0.2/cellulose/metrics/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/metrics/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      430 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/metrics/latency.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)       90 2023-06-07 04:03:32.000000 cellulose-sdk-0.0.2/cellulose/metrics/metrics.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.441308 cellulose-sdk-0.0.2/cellulose/onnx/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/onnx/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1608 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/onnx/benchmark.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      311 2023-06-07 06:23:27.000000 cellulose-sdk-0.0.2/cellulose/onnx/checker.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      499 2023-06-07 06:23:27.000000 cellulose-sdk-0.0.2/cellulose/onnx/loader.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      962 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/onnx/runtime.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.441557 cellulose-sdk-0.0.2/cellulose/output/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/output/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      403 2023-06-07 05:06:52.000000 cellulose-sdk-0.0.2/cellulose/output/output.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.441983 cellulose-sdk-0.0.2/cellulose/pytorch/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/pytorch/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1014 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/pytorch/benchmark.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     4819 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/pytorch/export.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.442113 cellulose-sdk-0.0.2/cellulose/scripts/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/scripts/__init__.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.442201 cellulose-sdk-0.0.2/cellulose/tensorflow/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/tensorflow/__init__.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.442955 cellulose-sdk-0.0.2/cellulose/utils/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/utils/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      895 2023-06-07 06:22:37.000000 cellulose-sdk-0.0.2/cellulose/utils/benchmark_results.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      967 2023-06-07 06:17:16.000000 cellulose-sdk-0.0.2/cellulose/utils/csv_utils.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      180 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/utils/devices.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      260 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/utils/engines.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      266 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/utils/numpy.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.443200 cellulose-sdk-0.0.2/cellulose/validation/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        0 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/validation/__init__.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      667 2023-05-30 00:03:23.000000 cellulose-sdk-0.0.2/cellulose/validation/validation.py
+-rw-r--r--   0 tzhenghao   (501) staff       (20)       32 2023-06-07 23:47:02.000000 cellulose-sdk-0.0.2/cellulose/version.py
+drwxr-xr-x   0 tzhenghao   (501) staff       (20)        0 2023-06-08 00:06:06.443769 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1517 2023-06-08 00:06:06.000000 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     1472 2023-06-08 00:06:06.000000 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 tzhenghao   (501) staff       (20)        1 2023-06-08 00:06:06.000000 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      191 2023-06-08 00:06:06.000000 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/requires.txt
+-rw-r--r--   0 tzhenghao   (501) staff       (20)       10 2023-06-08 00:06:06.000000 cellulose-sdk-0.0.2/cellulose_sdk.egg-info/top_level.txt
+-rw-r--r--   0 tzhenghao   (501) staff       (20)      505 2023-06-07 06:23:01.000000 cellulose-sdk-0.0.2/pyproject.toml
+-rw-r--r--   0 tzhenghao   (501) staff       (20)       38 2023-06-08 00:06:06.444040 cellulose-sdk-0.0.2/setup.cfg
+-rw-r--r--   0 tzhenghao   (501) staff       (20)     8573 2023-06-08 00:03:51.000000 cellulose-sdk-0.0.2/setup.py
```

### Comparing `cellulose-sdk-0.0.1/LICENSE` & `cellulose-sdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/PKG-INFO` & `cellulose-sdk-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellulose-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cellulose Python SDK
 Home-page: https://www.cellulose.ai
 Author: Cellulose engineering team
 Author-email: zheng@cellulose.ai
 Project-URL: Homepage, https://www.cellulose.ai
 Project-URL: Documentation, http://docs.cellulose.ai
 Keywords: artificial intelligence,benchmarking,debugging,development,onnx,profiler,profiling,pytorch,tensorflow
```

### Comparing `cellulose-sdk-0.0.1/cellulose/api/cellulose_context.py` & `cellulose-sdk-0.0.2/cellulose/api/cellulose_context.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/artifact/cellulose_artifact_manager.py` & `cellulose-sdk-0.0.2/cellulose/artifact/cellulose_artifact_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,31 @@
 
 # Third party imports
 import click
 import tomlkit
 from pydantic.dataclasses import dataclass
 
 # Cellulose imports
-from cellulose.artifact.cellulose_artifact import CelluloseArtifact
+from cellulose.artifact.cellulose_artifact import CelluloseArtifact, Metadata
 from cellulose.configs.config import AllConfig
 from cellulose.version import CELLULOSE_SDK_VERSION
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class CelluloseArtifactManager:
-    cellulose_artifact = CelluloseArtifact(file_paths=[])
+    cellulose_artifact = CelluloseArtifact(
+        file_paths=[],
+        metadata=Metadata(
+            title="",
+            created_at=datetime.utcnow(),
+            updated_at=datetime.utcnow(),
+        ),
+    )
     metadata_doc = tomlkit.document()
 
     def initialize_artifact_metadata(self):
         """
         This internal method initializes the title and created_at / updated_at
         parameters in the Cellulose artifact metadata file.
         """
```

### Comparing `cellulose-sdk-0.0.1/cellulose/base/benchmark.py` & `cellulose-sdk-0.0.2/cellulose/base/benchmark.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/configs/.cellulose_config.toml` & `cellulose-sdk-0.0.2/cellulose/configs/.cellulose_config.toml`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/configs/config.py` & `cellulose-sdk-0.0.2/cellulose/configs/config.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/configs/loader.py` & `cellulose-sdk-0.0.2/cellulose/configs/loader.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/decorators/cellulose.py` & `cellulose-sdk-0.0.2/cellulose/decorators/cellulose.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/onnx/benchmark.py` & `cellulose-sdk-0.0.2/cellulose/onnx/benchmark.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/onnx/runtime.py` & `cellulose-sdk-0.0.2/cellulose/onnx/runtime.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/pytorch/benchmark.py` & `cellulose-sdk-0.0.2/cellulose/pytorch/benchmark.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/pytorch/export.py` & `cellulose-sdk-0.0.2/cellulose/pytorch/export.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/utils/benchmark_results.py` & `cellulose-sdk-0.0.2/cellulose/utils/benchmark_results.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/utils/csv_utils.py` & `cellulose-sdk-0.0.2/cellulose/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose/validation/validation.py` & `cellulose-sdk-0.0.2/cellulose/validation/validation.py`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/cellulose_sdk.egg-info/PKG-INFO` & `cellulose-sdk-0.0.2/cellulose_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellulose-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Cellulose Python SDK
 Home-page: https://www.cellulose.ai
 Author: Cellulose engineering team
 Author-email: zheng@cellulose.ai
 Project-URL: Homepage, https://www.cellulose.ai
 Project-URL: Documentation, http://docs.cellulose.ai
 Keywords: artificial intelligence,benchmarking,debugging,development,onnx,profiler,profiling,pytorch,tensorflow
```

### Comparing `cellulose-sdk-0.0.1/cellulose_sdk.egg-info/SOURCES.txt` & `cellulose-sdk-0.0.2/cellulose_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellulose-sdk-0.0.1/setup.py` & `cellulose-sdk-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,7 @@
     # maintainers, and where to support the project financially. The key is
     # what's used to render the link text on PyPI.
     project_urls={  # Optional
         "Homepage": "https://www.cellulose.ai",
         "Documentation": "http://docs.cellulose.ai",
     },
 )
-
```

