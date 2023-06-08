# Comparing `tmp/evodflow-0.1.6.291.tar.gz` & `tmp/evodflow-0.1.6.292.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodflow-0.1.6.291.tar", last modified: Thu Jun  8 09:30:46 2023, max compression
+gzip compressed data, was "evodflow-0.1.6.292.tar", last modified: Thu Jun  8 09:38:05 2023, max compression
```

## Comparing `evodflow-0.1.6.291.tar` & `evodflow-0.1.6.292.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.031355 evodflow-0.1.6.291/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-08 09:30:46.031355 evodflow-0.1.6.291/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.023354 evodflow-0.1.6.291/evodflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-08 09:30:45.000000 evodflow-0.1.6.291/evodflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-08 09:30:45.000000 evodflow-0.1.6.291/evodflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:30:45.000000 evodflow-0.1.6.291/evodflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 09:30:45.000000 evodflow-0.1.6.291/evodflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 09:30:45.000000 evodflow-0.1.6.291/evodflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 09:30:45.000000 evodflow-0.1.6.291/evodflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.023354 evodflow-0.1.6.291/evoflow/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/__info__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.023354 evodflow-0.1.6.291/evoflow/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/common_step_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.023354 evodflow-0.1.6.291/evoflow/controller/data_manipulate/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/data_manipulate/PdfFileOperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/data_manipulate/PptxFileOperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/data_manipulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/data_manipulate/data_manipulate.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/data_manipulate/excel_file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/data_manipulate/file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/data_manipulate/image_file_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/log_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/controller/visualize_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/entities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/entities/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/entities/common/step/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/common/step/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/entities/common/step/browser/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/common/step/browser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/common/step/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/entities/common/step/file_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/common/step/file_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/common/step/open_excel_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/entities/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/core/base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/core/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/core/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/core/step_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/entities/data_manipulate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/data_manipulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/data_manipulate/abstract_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/dataframe_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/image_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/pdf_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/pptx_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/entities/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/exceptions/base_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/exceptions/evo_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/entities/global_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/operators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/operators/base_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/operators/empty_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/operators/python_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.027354 evodflow-0.1.6.291/evoflow/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/services/abstract_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.031355 evodflow-0.1.6.291/evoflow/services/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/services/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/services/ocr/easy_ocr_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/services/ocr/ocr_service.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/services/ocr/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/services/ocr/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/services/service_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.031355 evodflow-0.1.6.291/evoflow/services/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/services/templates/item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.031355 evodflow-0.1.6.291/evoflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/utils/create_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/utils/ultilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/evoflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:30:46.031355 evodflow-0.1.6.291/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:46.031355 evodflow-0.1.6.291/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 09:30:36.000000 evodflow-0.1.6.291/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.771239 evodflow-0.1.6.292/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.763239 evodflow-0.1.6.292/evodflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-08 09:38:05.000000 evodflow-0.1.6.292/evodflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-08 09:38:05.000000 evodflow-0.1.6.292/evodflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:38:05.000000 evodflow-0.1.6.292/evodflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 09:38:05.000000 evodflow-0.1.6.292/evodflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 09:38:05.000000 evodflow-0.1.6.292/evodflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 09:38:05.000000 evodflow-0.1.6.292/evodflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.763239 evodflow-0.1.6.292/evoflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.763239 evodflow-0.1.6.292/evoflow/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/common_step_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.763239 evodflow-0.1.6.292/evoflow/controller/data_manipulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/data_manipulate/PdfFileOperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/data_manipulate/PptxFileOperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/data_manipulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/data_manipulate/data_manipulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/data_manipulate/excel_file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/data_manipulate/file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/data_manipulate/image_file_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/log_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/controller/visualize_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.763239 evodflow-0.1.6.292/evoflow/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.763239 evodflow-0.1.6.292/evoflow/entities/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/entities/common/step/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/common/step/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/entities/common/step/browser/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/common/step/browser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/common/step/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/entities/common/step/file_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/common/step/file_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/common/step/open_excel_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/entities/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/core/base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/core/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/core/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/core/step_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/entities/data_manipulate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/data_manipulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/data_manipulate/abstract_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/dataframe_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/image_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/pdf_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/pptx_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/entities/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/exceptions/base_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/exceptions/evo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/entities/global_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/operators/base_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/operators/empty_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/operators/python_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/services/abstract_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/services/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/services/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/services/ocr/easy_ocr_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/services/ocr/ocr_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/services/ocr/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/services/ocr/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/services/service_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/services/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/services/templates/item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/evoflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/utils/create_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/utils/ultilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/evoflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:38:05.771239 evodflow-0.1.6.292/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:38:05.767239 evodflow-0.1.6.292/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 09:37:54.000000 evodflow-0.1.6.292/tests/test_base.py
```

### Comparing `evodflow-0.1.6.291/LICENSE` & `evodflow-0.1.6.292/LICENSE`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/PKG-INFO` & `evodflow-0.1.6.292/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodflow
-Version: 0.1.6.291
+Version: 0.1.6.292
 Summary: Awesome evoflow created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-flow/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `evodflow-0.1.6.291/README.md` & `evodflow-0.1.6.292/README.md`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evodflow.egg-info/PKG-INFO` & `evodflow-0.1.6.292/evodflow.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evodflow
-Version: 0.1.6.291
+Version: 0.1.6.292
 Summary: Awesome evoflow created by maycuatroi
 Home-page: https://github.com/maycuatroi/evo-flow/
 Author: maycuatroi
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `evodflow-0.1.6.291/evodflow.egg-info/SOURCES.txt` & `evodflow-0.1.6.292/evodflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/__init__.py` & `evodflow-0.1.6.292/evoflow/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/cli.py` & `evodflow-0.1.6.292/evoflow/cli.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/controller/data_manipulate/PdfFileOperator.py` & `evodflow-0.1.6.292/evoflow/controller/data_manipulate/PdfFileOperator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/controller/data_manipulate/PptxFileOperator.py` & `evodflow-0.1.6.292/evoflow/controller/data_manipulate/PptxFileOperator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/controller/data_manipulate/excel_file_operator.py` & `evodflow-0.1.6.292/evoflow/controller/data_manipulate/excel_file_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/controller/data_manipulate/file_operator.py` & `evodflow-0.1.6.292/evoflow/controller/data_manipulate/file_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/controller/data_manipulate/image_file_operator.py` & `evodflow-0.1.6.292/evoflow/controller/data_manipulate/image_file_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/controller/log_controller.py` & `evodflow-0.1.6.292/evoflow/controller/log_controller.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/common/step/__init__.py` & `evodflow-0.1.6.292/evoflow/entities/common/step/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/common/step/browser/__init__.py` & `evodflow-0.1.6.292/evoflow/entities/common/step/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/common/step/downloader.py` & `evodflow-0.1.6.292/evoflow/entities/common/step/downloader.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/common/step/open_excel_file.py` & `evodflow-0.1.6.292/evoflow/entities/common/step/open_excel_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/core/base_object.py` & `evodflow-0.1.6.292/evoflow/entities/core/base_object.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/core/condition.py` & `evodflow-0.1.6.292/evoflow/entities/core/condition.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/core/job.py` & `evodflow-0.1.6.292/evoflow/entities/core/job.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/core/step.py` & `evodflow-0.1.6.292/evoflow/entities/core/step.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/core/step_list.py` & `evodflow-0.1.6.292/evoflow/entities/core/step_list.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/core/transaction.py` & `evodflow-0.1.6.292/evoflow/entities/core/transaction.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/core/workflow.py` & `evodflow-0.1.6.292/evoflow/entities/core/workflow.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/data_manipulate/abstract_data.py` & `evodflow-0.1.6.292/evoflow/entities/data_manipulate/abstract_data.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/dataframe_file.py` & `evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/dataframe_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/file.py` & `evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/image_file.py` & `evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/image_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/pdf_file.py` & `evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/pdf_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/data_manipulate/file_operator/pptx_file.py` & `evodflow-0.1.6.292/evoflow/entities/data_manipulate/file_operator/pptx_file.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/entities/global_vars.py` & `evodflow-0.1.6.292/evoflow/entities/global_vars.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/operators/empty_operator.py` & `evodflow-0.1.6.292/evoflow/operators/empty_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/operators/python_operator.py` & `evodflow-0.1.6.292/evoflow/operators/python_operator.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/services/ocr/easy_ocr_engine.py` & `evodflow-0.1.6.292/evoflow/services/ocr/easy_ocr_engine.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/services/ocr/ocr_service.py` & `evodflow-0.1.6.292/evoflow/services/ocr/ocr_service.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/services/ocr/result.py` & `evodflow-0.1.6.292/evoflow/services/ocr/result.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/services/service_controller.py` & `evodflow-0.1.6.292/evoflow/services/service_controller.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/evoflow/utils/ultilities.py` & `evodflow-0.1.6.292/evoflow/utils/ultilities.py`

 * *Files identical despite different names*

### Comparing `evodflow-0.1.6.291/setup.py` & `evodflow-0.1.6.292/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,12 +33,13 @@
     name="evodflow",
     version=read("evoflow", "VERSION"),
     description="Awesome evoflow created by maycuatroi",
     url="https://github.com/maycuatroi/evo-flow/",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="maycuatroi",
+    package_data={"evoflow": ["VERSION"]},
     packages=find_packages(exclude=["tests", ".github"]),
     install_requires=read_requirements("requirements.txt"),
     entry_points={"console_scripts": ["evoflow = evoflow.__main__:main"]},
     extras_require={"test": read_requirements("requirements-test.txt")},
 )
```

