# Comparing `tmp/beginai-2.0.2.tar.gz` & `tmp/beginai-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beginai-2.0.2.tar", last modified: Wed Jun  7 18:32:24 2023, max compression
+gzip compressed data, was "beginai-2.0.3.tar", last modified: Thu Jun  8 12:59:01 2023, max compression
```

## Comparing `beginai-2.0.2.tar` & `beginai-2.0.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-07 18:32:24.445422 beginai-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-07 18:32:14.000000 beginai-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.441422 beginai-2.0.2/beginai/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.441422 beginai-2.0.2/beginai/conn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/conn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/conn/mqtt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.441422 beginai-2.0.2/beginai/exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.441422 beginai-2.0.2/beginai/exec/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/exec/embeddings/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/date.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/exec/embeddings/instructions/deep_text/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/deep_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/deep_text/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/instructions/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/master.py
--rw-r--r--   0 runner    (1001) docker     (123)    17517 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/embeddings/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/execute_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/exec/remote_compute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/orchapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/orchapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/orchapi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/storage/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/storage/sqllite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/tests/exec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/tests/exec/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/boolean_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/category_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/interaction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/location_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/number_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/instructions/text_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/mock_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_interaction_attributes_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/tests/exec/embeddings/worker_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.445422 beginai-2.0.2/beginai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-07 18:32:14.000000 beginai-2.0.2/beginai/utils/syft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:32:24.441422 beginai-2.0.2/beginai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-07 18:32:24.000000 beginai-2.0.2/beginai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-07 18:32:24.000000 beginai-2.0.2/beginai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:32:24.000000 beginai-2.0.2/beginai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-07 18:32:24.000000 beginai-2.0.2/beginai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:32:24.000000 beginai-2.0.2/beginai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 18:32:24.445422 beginai-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-07 18:32:23.000000 beginai-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.839487 beginai-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-08 12:59:01.839487 beginai-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-08 12:58:44.000000 beginai-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.831487 beginai-2.0.3/beginai/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.831487 beginai-2.0.3/beginai/conn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/conn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/conn/mqtt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.835487 beginai-2.0.3/beginai/exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.835487 beginai-2.0.3/beginai/exec/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.835487 beginai-2.0.3/beginai/exec/embeddings/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/date.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.835487 beginai-2.0.3/beginai/exec/embeddings/instructions/deep_text/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/deep_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/deep_text/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/instructions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17513 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/embeddings/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/execute_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/exec/remote_compute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.839487 beginai-2.0.3/beginai/orchapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/orchapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/orchapi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.839487 beginai-2.0.3/beginai/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/storage/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/storage/sqllite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.839487 beginai-2.0.3/beginai/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.839487 beginai-2.0.3/beginai/tests/exec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.839487 beginai-2.0.3/beginai/tests/exec/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.839487 beginai-2.0.3/beginai/tests/exec/embeddings/instructions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/instructions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/instructions/boolean_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/instructions/category_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/instructions/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/instructions/interaction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/instructions/location_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/instructions/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16426 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/instructions/parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/instructions/text_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/mock_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/worker_methods_validation_interaction_attributes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22951 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/tests/exec/embeddings/worker_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.839487 beginai-2.0.3/beginai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-08 12:58:44.000000 beginai-2.0.3/beginai/utils/syft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:59:01.831487 beginai-2.0.3/beginai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-08 12:59:01.000000 beginai-2.0.3/beginai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-06-08 12:59:01.000000 beginai-2.0.3/beginai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:59:01.000000 beginai-2.0.3/beginai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-08 12:59:01.000000 beginai-2.0.3/beginai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 12:59:01.000000 beginai-2.0.3/beginai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 12:59:01.839487 beginai-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-06-08 12:58:59.000000 beginai-2.0.3/setup.py
```

### Comparing `beginai-2.0.2/PKG-INFO` & `beginai-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beginai
-Version: 2.0.2
+Version: 2.0.3
 Summary: A library to interact with Begin AI platform in order to build personalisation algorithms.
 Home-page: https://docs.begin.ai
 Author: Begin AI Research & Engineering
 Author-email: engineering@begin.ai
 License: Proprietary
 Description: 
                 This is Begin AI python SDK for both batch processing and application integration.
```

### Comparing `beginai-2.0.2/beginai/conn/mqtt.py` & `beginai-2.0.3/beginai/conn/mqtt.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/apply.py` & `beginai-2.0.3/beginai/exec/embeddings/apply.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/instructions/__init__.py` & `beginai-2.0.3/beginai/exec/embeddings/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/instructions/date.py` & `beginai-2.0.3/beginai/exec/embeddings/instructions/date.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/instructions/deep_text/bpe.py` & `beginai-2.0.3/beginai/exec/embeddings/instructions/deep_text/bpe.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/instructions/interaction.py` & `beginai-2.0.3/beginai/exec/embeddings/instructions/interaction.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/instructions/location.py` & `beginai-2.0.3/beginai/exec/embeddings/instructions/location.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/instructions/number.py` & `beginai-2.0.3/beginai/exec/embeddings/instructions/number.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/instructions/parser.py` & `beginai-2.0.3/beginai/exec/embeddings/instructions/parser.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/instructions/text.py` & `beginai-2.0.3/beginai/exec/embeddings/instructions/text.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/instructions/utils.py` & `beginai-2.0.3/beginai/exec/embeddings/instructions/utils.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/embeddings/worker.py` & `beginai-2.0.3/beginai/exec/embeddings/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
         if self._is_valid_type(value, str) == False:
             raise ValueError("Value must be a String")
 
         self._set_value(object_id, field, value, object_name)
 
     def update_object_category_field(self, object_name, object_id, field, value: str):
-        self.update_object_category_field(object_name, object_id, field, value)
+        self.update_object_text_field(object_name, object_id, field, value)
 
     def update_object_boolean_field(self, object_name, object_id, field, value: bool):
         self._validate_properties_for_other_object(
             object_name, object_id, field, value)
 
         if self._is_valid_type(value, bool) == False:
             raise ValueError("Value must be Boolean")
```

### Comparing `beginai-2.0.2/beginai/exec/execute_compute.py` & `beginai-2.0.3/beginai/exec/execute_compute.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/exec/remote_compute.py` & `beginai-2.0.3/beginai/exec/remote_compute.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/orchapi/api.py` & `beginai-2.0.3/beginai/orchapi/api.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/boolean_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/instructions/boolean_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/category_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/instructions/category_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/date_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/instructions/date_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/interaction_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/instructions/interaction_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/location_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/instructions/location_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/number_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/instructions/number_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/parser_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/instructions/parser_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/instructions/text_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/instructions/text_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/mock_service.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/mock_service.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_interaction_attributes_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/worker_methods_validation_interaction_attributes_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/worker_methods_validation_interaction_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/worker_methods_validation_labels_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/worker_methods_validation_object_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/worker_methods_validation_user_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/tests/exec/embeddings/worker_test.py` & `beginai-2.0.3/beginai/tests/exec/embeddings/worker_test.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai/utils/syft.py` & `beginai-2.0.3/beginai/utils/syft.py`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/beginai.egg-info/PKG-INFO` & `beginai-2.0.3/beginai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beginai
-Version: 2.0.2
+Version: 2.0.3
 Summary: A library to interact with Begin AI platform in order to build personalisation algorithms.
 Home-page: https://docs.begin.ai
 Author: Begin AI Research & Engineering
 Author-email: engineering@begin.ai
 License: Proprietary
 Description: 
                 This is Begin AI python SDK for both batch processing and application integration.
```

### Comparing `beginai-2.0.2/beginai.egg-info/SOURCES.txt` & `beginai-2.0.3/beginai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beginai-2.0.2/setup.py` & `beginai-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 REQ_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), "pip-dep")
 core_reqs, core_dependency_links = get_requirements(os.path.join(REQ_DIR, "requirements.txt"))
 
 
 if __name__ == "__main__":
     setup(
         name="beginai",
-        version="2.0.2",
+        version="2.0.3",
         author="Begin AI Research & Engineering",
         author_email="engineering@begin.ai",
         description="A library to interact with Begin AI platform in order to build personalisation algorithms.",
         long_description="""
         This is Begin AI python SDK for both batch processing and application integration. 
         It can be used to integrate applications with Begin.ai orchestration platform to deliver applications with
         personalisation algorithms to do:
```

