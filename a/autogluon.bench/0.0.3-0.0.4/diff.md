# Comparing `tmp/autogluon.bench-0.0.3.tar.gz` & `tmp/autogluon.bench-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.bench-0.0.3.tar", last modified: Thu Jun  1 18:35:31 2023, max compression
+gzip compressed data, was "autogluon.bench-0.0.4.tar", last modified: Wed Jun  7 23:47:01 2023, max compression
```

## Comparing `autogluon.bench-0.0.3.tar` & `autogluon.bench-0.0.4.tar`

### file list

```diff
@@ -1,71 +1,62 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10356 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8863 2023-06-01 16:49:32.000000 autogluon.bench-0.0.3/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      251 2023-04-20 19:12:31.000000 autogluon.bench-0.0.3/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      211 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4750 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.045658 autogluon.bench-0.0.3/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.045658 autogluon.bench-0.0.3/src/autogluon/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-05-30 17:48:22.000000 autogluon.bench-0.0.3/src/autogluon/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      308 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/Dockerfile
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       33 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/cloud/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/__init__.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1555 2023-04-17 16:24:01.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/app.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/constructs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2768 2023-05-30 06:51:07.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      847 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/lambdas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8029 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       26 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/lambdas/requirements.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11251 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/stack.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      379 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      330 2023-05-15 20:06:57.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/default_config.yaml
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)     1753 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/deploy.sh
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      997 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/destroy.sh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6305 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/stack_handler.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/datasets/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-05 22:42:24.000000 autogluon.bench-0.0.3/src/autogluon/bench/datasets/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      319 2023-05-05 22:42:24.000000 autogluon.bench-0.0.3/src/autogluon/bench/datasets/constants.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      413 2023-05-05 22:42:24.000000 autogluon.bench-0.0.3/src/autogluon/bench/datasets/dataset_registry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19773 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/datasets/multimodal_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2557 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/datasets/object_detection_dataset.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2861 2023-05-08 21:16:14.000000 autogluon.bench-0.0.3/src/autogluon/bench/datasets/registry.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/entrypoint.sh
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2439 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/benchmark.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/multimodal/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/multimodal/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6183 2023-06-01 18:07:07.000000 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/multimodal/exec.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3008 2023-06-01 17:52:33.000000 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      793 2023-06-01 17:53:11.000000 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/multimodal/setup.sh
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/tabular/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-03-30 17:06:59.000000 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/tabular/__init__.py
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      662 2023-04-20 19:12:31.000000 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/tabular/exec.sh
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      466 2023-04-20 19:12:31.000000 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/tabular/setup.sh
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2764 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      279 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/main.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12438 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/runbenchmark.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.049658 autogluon.bench-0.0.3/src/autogluon/bench/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      692 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/utils/dataset_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      551 2023-06-01 16:15:39.000000 autogluon.bench-0.0.3/src/autogluon/bench/utils/general_utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-06-01 18:35:30.000000 autogluon.bench-0.0.3/src/autogluon/bench/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 18:35:31.045658 autogluon.bench-0.0.3/src/autogluon.bench.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10356 2023-06-01 18:35:31.000000 autogluon.bench-0.0.3/src/autogluon.bench.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2395 2023-06-01 18:35:31.000000 autogluon.bench-0.0.3/src/autogluon.bench.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-01 18:35:31.000000 autogluon.bench-0.0.3/src/autogluon.bench.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       84 2023-06-01 18:35:31.000000 autogluon.bench-0.0.3/src/autogluon.bench.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-06-01 18:35:31.000000 autogluon.bench-0.0.3/src/autogluon.bench.egg-info/namespace_packages.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      374 2023-06-01 18:35:31.000000 autogluon.bench-0.0.3/src/autogluon.bench.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2023-06-01 18:35:31.000000 autogluon.bench-0.0.3/src/autogluon.bench.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-03 05:42:27.000000 autogluon.bench-0.0.3/src/autogluon.bench.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-07 23:47:01.386952 autogluon.bench-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-07 23:47:01.386952 autogluon.bench-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.378952 autogluon.bench-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.378952 autogluon.bench-0.0.4/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1555 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/lambdas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8091 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/stack_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/dataset_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19773 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/multimodal_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/object_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/datasets/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12444 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/runbenchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon/bench/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-07 23:46:50.000000 autogluon.bench-0.0.4/src/autogluon/bench/utils/general_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-07 23:47:00.000000 autogluon.bench-0.0.4/src/autogluon/bench/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:47:01.382952 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:47:01.000000 autogluon.bench-0.0.4/src/autogluon.bench.egg-info/zip-safe
```

### Comparing `autogluon.bench-0.0.3/LICENSE` & `autogluon.bench-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/PKG-INFO` & `autogluon.bench-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,189 @@
 Metadata-Version: 2.1
 Name: autogluon.bench
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/autogluon/autogluon-bench
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon-bench/issues
 Project-URL: Source, https://github.com/autogluon/autogluon-bench/
+Description: <div align="left">
+          <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
+        </div>
+        
+        # AutoGluon-Bench
+        
+        Welcome to AutoGluon-Bench, a suite for benchmarking your AutoML frameworks.
+        
+        ## Setup
+        
+        Follow the steps below to set up autogluon-bench:
+        
+        ```bash
+        # create virtual env
+        python3 -m venv .venv_agbench
+        source .venv_agbench/bin/activate
+        ```
+        
+        Install `autogloun-bench` from PyPI:
+        
+        ```bash
+        python3 -m pip install autogluon.bench
+        ```
+        
+        Or install `autogluon-bench` from source:
+        
+        ```bash
+        git clone https://github.com/autogluon/autogluon-bench.git
+        cd autogluon-bench
+        
+        # install from source in editable mode
+        pip install -e .
+        ```
+        
+        For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). To ensure that your local changes are reflected in the installed package, you may need to adjust the installation command as necessary. A recommended approach is to push your changes to a remote git branch and then pull from this branch, installing the package from source in the scripts.
+        
+        
+        ## Run benchmarks locally
+        
+        To run the benchmarks on your local machine, use the following command:
+        
+        ```
+        agbench run path/to/local_config_file
+        ```
+        
+        Check out our [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for local runs.
+        
+        The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
+        
+        
+        ### Tabular Benchmark
+        
+        To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
+        
+        The tabular module leverages the [AMLB](https://github.com/openml/automlbenchmark) benchmarking framework. Required and optional AMLB arguments are specified via the configuration file mentioned previously.
+        
+        To benchmark a custom branch of AutoGluon on `tabular` module, use `amlb_custom_branch: https://github.com/REPO/autogluon#BRANCH` in the configuration file.
+        
+        
+        ### Multimodal Benchmark
+        
+        For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
+        
+        You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
+        
+        ## Run benchmarks on AWS
+        
+        AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
+        
+        To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
+        
+        1. Install [Node Version Manager](https://github.com/nvm-sh/nvm#installing-and-updating).
+        2. Source profile or restart the terminal.
+        3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
+        ```bash
+        nvm install $VERSION  # install Node.js
+        npm install -g aws-cdk  # install aws-cdk
+        cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
+        ```
+        
+        To initiate benchmarking on the cloud, use the command below:
+        
+        ```
+        agbench run /path/to/cloud_config_file
+        ```
+        
+        This command automatically sets up an AWS Batch environment using instance specifications defined in the `cloud_config_file`. It also creates a lambda function named with your chosen `LAMBDA_FUNCTION_NAME`. This lambda function is automatically invoked with the cloud config file you provided, submitting multiple AWS Batch jobs to the job queue (named with the `PREFIX` you provided).
+        
+        In order for the Lambda function to submit multiple jobs simultaneously, you need to specify a list of values for each module-specific key. Each combination of configurations is saved and uploaded to your specified `METRICS_BUCKET` in S3, stored under `S3://{METRICS_BUCKET}/configs/{BENCHMARK_NAME}_{timestamp}/{BENCHMARK_NAME}_split_{UID}.yaml`. Here, `UID` is a unique ID assigned to the split.
+        
+        The AWS infrastructure configurations and submitted job IDs are saved locally at `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`. You can use this file to check the job status at any time:
+        
+        ```bash
+        agbench get-job-status --config-file /path/to/aws_configs.yaml
+        ```
+        
+        You can also check the job status using job IDs:
+        
+        ```bash
+        agbench get-job-status --job-ids JOB_ID_1 --job-ids JOB_ID_2 —cdk_deploy_region AWS_REGION
+        
+        ```
+        
+        Job logs can be viewed on the AWS console. Each job has an `UID` attached to the name, which you can use to identify the respective config split. After the jobs are completed and reach the `SUCCEEDED` status in the job queue, you'll find metrics saved under `S3://{METRICS_BUCKET}/{module}/{benchmark_name}_{timestamp}/{benchmark_name}_{timestamp}_{UID}`.
+        
+        By default, the infrastructure created is retained for future use. To automatically remove resources after the run, use the `--remove_resources` option:
+        
+        ```bash
+        agbench run path/to/cloud_config_file --remove_resources
+        ```
+        
+        This will check the job status every 2 minutes and remove resources after all jobs succeed. If any job fails, resources will be kept.
+        
+        If you want to manually remove resources later, use:
+        
+        ```bash
+        agbench destroy-stack STATIC_RESOURCE_STACK_NAME BATCH_STACK_NAME CDK_DEPLOY_ACCOUNT CDK_DEPLOY_REGION
+        ```
+        
+        where you can find all argument values in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`.
+        
+        
+        ### Configure the AWS infrastructure
+        
+        The default infrastructure configurations are located [here](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/cloud/aws/default_config.yaml).
+        
+        where:
+        - `CDK_DEPLOY_ACCOUNT` and `CDK_DEPLOY_REGION` should be overridden with your AWS account ID and desired region to create the stack.
+        - `PREFIX` is used as an identifier for the stack and resources created.
+        - `RESERVED_MEMORY_SIZE` is used together with the instance memory size to calculate the container shm_size.
+        - `BLOCK_DEVICE_VOLUME` is the size of storage device attached to instance.
+        - `LAMBDA_FUNCTION_NAME` lambda function to submit jobs to AWS Batch.
+        
+        To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/cloud_configs.yaml) for reference.
+        
+        ## Evaluating bechmark runs
+        
+        Innixma's `autogluon-benchmark` repository can be used to evaluate tabular benchmark runs whose results are in S3.
+        Using these utilities is ad-hoc at this time, but in a coming release we will integrate this capability into `autogluon-bench` and support evaulation of multimodal benchmarks.
+        
+        ### Evaluation Steps
+        
+        Clone the `autogluon-benchmark` repository:
+        ```
+        git clone https://github.com/gidler/autogluon-benchmark.git
+        ```
+        
+        Confirm that AWS credentials are setup for the AWS account that has the benchmark results in S3.
+        
+        Run the `aggregate_all.py` script
+        ```
+        python scripts/aggregate_all.py --s3_bucket {AWS_BUCKET} --s3_prefix {AWS_PREFIX} --version_name {BENCHMARK_VERSION_NAME}
+        
+        # example: python scripts/aggregate_all.py --s3_bucket autogluon-benchmark-metrics --s3_prefix tabular/ --version_name test_local_20230330T180916
+        ```
+        
+        This will create a new file in S3 with this signature:
+        ```
+        s3://{AWS_BUCKET}/aggregated/{AWS_PREFIX}/{BENCHMARK_VERSION_NAME}/results.csv
+        ```
+        
+        Run the `run_generate_clean_openml` python utility. You will need to manually set the `run_name_arg` and `path_prefix` variables in the script.
+        ```
+        python autogluon_benchmark/evaluation/runners/run_generate_clean_openml.py 
+        ```
+        This will create a local file of results in the `data/results/input/prepared/openml/` directory.
+        
+        Run the `benchmark_evaluation` python script. You will need to manually update the `frameworks_run` and `paths` variables in the script.
+        ```
+        python autogluon_benchmark/evaluation/runners/run_evaluation_openml.py
+        ```
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -27,198 +200,7 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.8, <3.10
 Description-Content-Type: text/markdown
 Provides-Extra: tests
-License-File: LICENSE
-
-<div align="left">
-  <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
-</div>
-
-# AutoGluon-Bench
-
-Welcome to AutoGluon-Bench, a suite for benchmarking your AutoML frameworks.
-
-## Setup
-
-Follow the steps below to set up autogluon-bench:
-
-```bash
-# create virtual env
-python3.9 -m venv .venv_agbench
-source .venv_agbench/bin/activate
-```
-
-Install `autogloun-bench` from PyPI:
-
-```bash
-python -m pip install autogluon.bench
-```
-
-
-Or install `autogluon-bench` from source:
-
-```bash
-git clone https://github.com/autogluon/autogluon-bench.git
-cd autogluon-bench
-
-# install from source in editable mode
-pip install -e .
-```
-Also, replace all `pip install autogluon.bench` with `pip install -e .` in the source code.
-
-
-## Run benchmarks locally
-
-To run the benchmarks on your local machine, use the following command:
-
-```
-agbench run path/to/local_config_file
-```
-
-Check out our [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for local runs.
-
-The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
-
-
-### Tabular Benchmark
-
-To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
-
-The tabular module leverages the [AMLB](https://github.com/openml/automlbenchmark) benchmarking framework. Required and optional AMLB arguments are specified via the configuration file mentioned previously.
-
-To benchmark a custom branch of AutoGluon on `tabular` module, use `amlb_custom_branch: https://github.com/REPO/autogluon#BRANCH` in the configuration file.
-
-
-### Multimodal Benchmark
-
-For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
-
-You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
-
-## Run benchmarks on AWS
-
-AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
-
-To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following commands:
-
-```bash
-curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash  # replace bash with other shell (e.g. zsh) if you are using a different one
-source ~/.bashrc
-nvm install 18.16.0  # install Node.js
-npm install -g aws-cdk  # install aws-cdk
-cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
-```
-
-To initiate benchmarking on the cloud, use the command below:
-
-```
-agbench run /path/to/cloud_config_file
-```
-
-This command automatically sets up an AWS Batch environment using instance specifications defined in the `cloud_config_file`. It also creates a lambda function named with your chosen `LAMBDA_FUNCTION_NAME`. This lambda function is automatically invoked with the cloud config file you provided, submitting multiple AWS Batch jobs to the job queue (named with the `PREFIX` you provided).
-
-In order for the Lambda function to submit multiple jobs simultaneously, you need to specify a list of values for each module-specific key. Each combination of configurations is saved and uploaded to your specified `METRICS_BUCKET` in S3, stored under `S3://{METRICS_BUCKET}/configs/{BENCHMARK_NAME}_{timestamp}/{BENCHMARK_NAME}_split_{UID}.yaml`. Here, `UID` is a unique ID assigned to the split.
-
-The AWS infrastructure configurations and submitted job IDs are saved locally at `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`. You can use this file to check the job status at any time:
-
-```bash
-agbench get-job-status --config-file /path/to/aws_configs.yaml
-```
-
-You can also check the job status using job IDs:
-
-```bash
-agbench get-job-status --job-ids JOB_ID_1 --job-ids JOB_ID_2 —cdk_deploy_region AWS_REGION
-
-```
-
-Job logs can be viewed on the AWS console. Each job has an `UID` attached to the name, which you can use to identify the respective config split. After the jobs are completed and reach the `SUCCEEDED` status in the job queue, you'll find metrics saved under `S3://{METRICS_BUCKET}/{module}/{benchmark_name}_{timestamp}/{benchmark_name}_{timestamp}_{UID}`.
-
-By default, the infrastructure created is retained for future use. To automatically remove resources after the run, use the `--remove_resources` option:
-
-```bash
-agbench run path/to/cloud_config_file --remove_resources
-```
-
-This will check the job status every 2 minutes and remove resources after all jobs succeed. If any job fails, resources will be kept.
-
-If you want to manually remove resources later, use:
-
-```bash
-agbench destroy-stack STATIC_RESOURCE_STACK_NAME BATCH_STACK_NAME CDK_DEPLOY_ACCOUNT CDK_DEPLOY_REGION
-```
-
-where you can find all argument values in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`.
-
-
-### Configure the AWS infrastructure
-
-The default infrastructure configurations are located [here](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/cloud/aws/default_config.yaml).
-
-```
-CDK_DEPLOY_ACCOUNT: dummy
-CDK_DEPLOY_REGION: dummy
-PREFIX: ag-bench-test
-RESERVED_MEMORY_SIZE: 15000
-MAX_MACHINE_NUM: 20
-BLOCK_DEVICE_VOLUME: 100
-INSTANCE: g4dn.2xlarge
-METRICS_BUCKET: autogluon-benchmark-metrics
-DATA_BUCKET: automl-mm-bench
-VPC_NAME: automm-batch-stack/automm-vpc
-LAMBDA_FUNCTION_NAME: ag-bench-test-job-function
-```
-where:
-- `CDK_DEPLOY_ACCOUNT` and `CDK_DEPLOY_REGION` should be overridden with your AWS account ID and desired region to create the stack.
-- `PREFIX` is used as an identifier for the stack and resources created.
-- `RESERVED_MEMORY_SIZE` is used together with the instance memory size to calculate the container shm_size.
-- `BLOCK_DEVICE_VOLUME` is the size of storage device attached to instance.
-- `METRICS_BUCKET` is the bucket to upload benchmarking metrics.
-- `DATA_BUCKET` is the bucket to download dataset from.
-- `VPC_NAME` is used to look up an existing VPC.
-- `LAMBDA_FUNCTION_NAME` lambda function to submit jobs to AWS Batch.
-
-To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/cloud_configs.yaml) for reference.
-
-## Evaluating bechmark runs
-
-Innixma's `autogluon-benchmark` repository can be used to evaluate tabular benchmark runs whose results are in S3.
-Using these utilities is ad-hoc at this time, but in a coming release we will integrate this capability into `autogluon-bench` and support evaulation of multimodal benchmarks.
-
-### Evaluation Steps
-
-Clone the `autogluon-benchmark` repository:
-```
-git clone https://github.com/gidler/autogluon-benchmark.git
-```
-
-Confirm that AWS credentials are setup for the AWS account that has the benchmark results in S3.
-
-Run the `aggregate_all.py` script
-```
-python scripts/aggregate_all.py --s3_bucket {AWS_BUCKET} --s3_prefix {AWS_PREFIX} --version_name {BENCHMARK_VERSION_NAME}
-
-# example: python scripts/aggregate_all.py --s3_bucket autogluon-benchmark-metrics --s3_prefix tabular/ --version_name test_local_20230330T180916
-```
-
-This will create a new file in S3 with this signature:
-```
-s3://{AWS_BUCKET}/aggregated/{AWS_PREFIX}/{BENCHMARK_VERSION_NAME}/results.csv
-```
-
-Run the `run_generate_clean_openml` python utility. You will need to manually set the `run_name_arg` and `path_prefix` variables in the script.
-```
-python autogluon_benchmark/evaluation/runners/run_generate_clean_openml.py 
-```
-This will create a local file of results in the `data/results/input/prepared/openml/` directory.
-
-Run the `benchmark_evaluation` python script. You will need to manually update the `frameworks_run` and `paths` variables in the script.
-```
-python autogluon_benchmark/evaluation/runners/run_evaluation_openml.py
-```
-
-
-
```

### Comparing `autogluon.bench-0.0.3/README.md` & `autogluon.bench-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,35 +8,35 @@
 
 ## Setup
 
 Follow the steps below to set up autogluon-bench:
 
 ```bash
 # create virtual env
-python3.9 -m venv .venv_agbench
+python3 -m venv .venv_agbench
 source .venv_agbench/bin/activate
 ```
 
 Install `autogloun-bench` from PyPI:
 
 ```bash
-python -m pip install autogluon.bench
+python3 -m pip install autogluon.bench
 ```
 
-
 Or install `autogluon-bench` from source:
 
 ```bash
 git clone https://github.com/autogluon/autogluon-bench.git
 cd autogluon-bench
 
 # install from source in editable mode
 pip install -e .
 ```
-Also, replace all `pip install autogluon.bench` with `pip install -e .` in the source code.
+
+For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). To ensure that your local changes are reflected in the installed package, you may need to adjust the installation command as necessary. A recommended approach is to push your changes to a remote git branch and then pull from this branch, installing the package from source in the scripts.
 
 
 ## Run benchmarks locally
 
 To run the benchmarks on your local machine, use the following command:
 
 ```
@@ -63,20 +63,21 @@
 
 You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
 
 ## Run benchmarks on AWS
 
 AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
 
-To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following commands:
+To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
 
+1. Install [Node Version Manager](https://github.com/nvm-sh/nvm#installing-and-updating).
+2. Source profile or restart the terminal.
+3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
 ```bash
-curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash  # replace bash with other shell (e.g. zsh) if you are using a different one
-source ~/.bashrc
-nvm install 18.16.0  # install Node.js
+nvm install $VERSION  # install Node.js
 npm install -g aws-cdk  # install aws-cdk
 cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
 ```
 
 To initiate benchmarking on the cloud, use the command below:
 
 ```
@@ -119,35 +120,19 @@
 where you can find all argument values in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`.
 
 
 ### Configure the AWS infrastructure
 
 The default infrastructure configurations are located [here](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/cloud/aws/default_config.yaml).
 
-```
-CDK_DEPLOY_ACCOUNT: dummy
-CDK_DEPLOY_REGION: dummy
-PREFIX: ag-bench-test
-RESERVED_MEMORY_SIZE: 15000
-MAX_MACHINE_NUM: 20
-BLOCK_DEVICE_VOLUME: 100
-INSTANCE: g4dn.2xlarge
-METRICS_BUCKET: autogluon-benchmark-metrics
-DATA_BUCKET: automl-mm-bench
-VPC_NAME: automm-batch-stack/automm-vpc
-LAMBDA_FUNCTION_NAME: ag-bench-test-job-function
-```
 where:
 - `CDK_DEPLOY_ACCOUNT` and `CDK_DEPLOY_REGION` should be overridden with your AWS account ID and desired region to create the stack.
 - `PREFIX` is used as an identifier for the stack and resources created.
 - `RESERVED_MEMORY_SIZE` is used together with the instance memory size to calculate the container shm_size.
 - `BLOCK_DEVICE_VOLUME` is the size of storage device attached to instance.
-- `METRICS_BUCKET` is the bucket to upload benchmarking metrics.
-- `DATA_BUCKET` is the bucket to download dataset from.
-- `VPC_NAME` is used to look up an existing VPC.
 - `LAMBDA_FUNCTION_NAME` lambda function to submit jobs to AWS Batch.
 
 To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/cloud_configs.yaml) for reference.
 
 ## Evaluating bechmark runs
 
 Innixma's `autogluon-benchmark` repository can be used to evaluate tabular benchmark runs whose results are in S3.
```

### Comparing `autogluon.bench-0.0.3/setup.py` & `autogluon.bench-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             [console_scripts]
             agbench=autogluon.bench.main:app
         """,
     )
     return setup_args
 
 
-version = "0.0.3"
+version = "0.0.4"
 version = update_version(version, use_file_if_exists=False, create_file=True)
 
 install_requires = [
     "autogluon.common>=0.7,<1.0",
     "awscliv2>=2.2.0,<2.3.0",
     "pandas>=1.2.5,<2.0",
     "boto3>=1.26.0,<1.26.99",
```

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/app.py` & `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/app.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py` & `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py` & `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py` & `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,24 +174,25 @@
     if "config_file" not in event or not event["config_file"].startswith("s3"):
         raise KeyError("S3 path of config file is required.")
 
     config_file_path = download_config(s3_path=event["config_file"])
     with open(config_file_path, "r") as f:
         configs = yaml.safe_load(f)
 
+    metrics_bucket = configs["cdk_context"]["METRICS_BUCKET"]
     del configs["cdk_context"]
 
     batch_job_queue = os.environ.get("BATCH_JOB_QUEUE")
     batch_job_definition = os.environ.get("BATCH_JOB_DEFINITION")
 
     module_configs = configs["module_configs"].pop(configs["module"])
     del configs["module_configs"]
     common_configs = configs
+    common_configs["METRICS_BUCKET"] = metrics_bucket
     common_configs["mode"] = "local"
-    metrics_bucket = common_configs["metrics_bucket"]
     common_configs = {key: [value] if not isinstance(value, list) else value for key, value in common_configs.items()}
 
     if common_configs["module"][0] == "tabular":
         amlb_benchmarks = module_configs.pop("amlb_benchmark", [])
         amlb_tasks = module_configs.pop("amlb_task", {})
 
     # Generate all combinations and submit jobs
```

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/batch_stack/stack.py` & `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/batch_stack/stack.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,66 +57,37 @@
                 self,
                 bucket_name,
                 bucket_name=bucket_name,
                 removal_policy=core.RemovalPolicy.RETAIN,
             )
         return bucket
 
-    def import_or_create_vpc(self, resource, vpc_name, prefix):
-        """
-        Imports an EC2 VPC if it already exists or creates a new one if it doesn't exist.
-
-        Args:
-            resource: A boto3 EC2 client object.
-            vpc_name: The name of the VPC.
-            prefix: The prefix to use for the VPC.
-
-        Returns:
-            An EC2 VPC object.
-        """
-        filters = [
-            {
-                "Name": "tag:Name",
-                "Values": [vpc_name],
-            }
-        ]
-        response = resource.describe_vpcs(Filters=filters)
-        if response["Vpcs"]:
-            vpc_id = response["Vpcs"][0]["VpcId"]
-            vpc = ec2.Vpc.from_lookup(self, f"{prefix}-vpc", vpc_id=vpc_id)
-        else:
-            vpc = ec2.Vpc(self, f"{prefix}-vpc", vpc_name=vpc_name, max_azs=1)
-        return vpc
-
     def create_s3_resources(self):
         """
         Creates S3 bucket resources.
         """
         region = os.environ["CDK_DEPLOY_REGION"]
         s3_resource = boto3.resource(service_name="s3", region_name=region)
         self.metrics_bucket = self.import_or_create_bucket(resource=s3_resource, bucket_name=self.metrics_bucket_name)
-        self.data_bucket = s3.Bucket.from_bucket_name(self, self.data_bucket_name, bucket_name=self.data_bucket_name)
-
-    def create_vpc_resources(self):
-        """
-        Creates VPC resources.
-        """
-        region = os.environ["CDK_DEPLOY_REGION"]
-        ec2_client = boto3.client("ec2", region_name=region)
-        self.vpc = self.import_or_create_vpc(resource=ec2_client, vpc_name=self.vpc_name, prefix=self.prefix)
+        if self.data_bucket_name:
+            self.data_bucket = s3.Bucket.from_bucket_name(
+                self, self.data_bucket_name, bucket_name=self.data_bucket_name
+            )
+        else:
+            self.data_bucket = None
 
     def __init__(self, scope: Construct, id: str, **kwargs) -> None:
         super().__init__(scope, id, **kwargs)
         self.metrics_bucket_name = self.node.try_get_context("METRICS_BUCKET")
         self.data_bucket_name = self.node.try_get_context("DATA_BUCKET")
         self.vpc_name = self.node.try_get_context("VPC_NAME")
         self.prefix = self.node.try_get_context("STACK_NAME_PREFIX")
 
         self.create_s3_resources()
-        self.create_vpc_resources()
+        self.vpc = ec2.Vpc.from_lookup(self, f"{self.prefix}-vpc", vpc_name=self.vpc_name) if self.vpc_name else None
 
 
 class BatchJobStack(core.Stack):
     def __init__(self, scope: Construct, id: str, static_stack: StaticResourceStack, **kwargs) -> None:
         """
         Defines a stack with the following:
         - A new Compute Environment with
@@ -148,14 +119,31 @@
 
         instances = []
         for instance in instance_types:
             instances.append(ec2.InstanceType(instance))
 
         vpc = static_stack.vpc
 
+        if vpc is None:
+            vpc = ec2.Vpc(
+                self,
+                f"{prefix}-vpc",
+                max_azs=2,  # You can increase this number for high availability
+                nat_gateways=1,
+                subnet_configuration=[
+                    ec2.SubnetConfiguration(
+                        name=f"{prefix}-PublicSubnet",
+                        subnet_type=ec2.SubnetType.PUBLIC,
+                    ),
+                    ec2.SubnetConfiguration(
+                        name=f"{prefix}-PrivateSubnet",
+                        subnet_type=ec2.SubnetType.PRIVATE_WITH_EGRESS,
+                    ),
+                ],
+            )
         sg = ec2.SecurityGroup(
             self,
             f"{prefix}-security-group",
             vpc=vpc,
         )
 
         # Currently CDK can only push to the default repo aws-cdk/assets
@@ -215,15 +203,16 @@
             managed_policies=[
                 iam.ManagedPolicy.from_aws_managed_policy_name("service-role/AmazonEC2ContainerServiceforEC2Role"),
             ],
         )
 
         metrics_bucket = static_stack.metrics_bucket
         data_bucket = static_stack.data_bucket
-        data_bucket.grant_read(batch_instance_role)
+        if data_bucket is not None:
+            data_bucket.grant_read(batch_instance_role)
         metrics_bucket.grant_read_write(batch_instance_role)
 
         batch_instance_profile = InstanceProfile(self, f"{prefix}-instance-profile", prefix=prefix)
         batch_instance_profile.attach_role(batch_instance_role)
 
         compute_environment = batch.ComputeEnvironment(
             self,
```

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/cloud/aws/stack_handler.py` & `autogluon.bench-0.0.4/src/autogluon/bench/cloud/aws/stack_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,40 +49,40 @@
         "CDK_DEPLOY_ACCOUNT": configs["CDK_DEPLOY_ACCOUNT"],
         "CDK_DEPLOY_REGION": configs["CDK_DEPLOY_REGION"],
         "STACK_NAME_PREFIX": prefix,  # aws resource tag key, also used as name prefix for resources created
         "STACK_NAME_TAG": "benchmark",  # aws resource tag value
         "STATIC_RESOURCE_STACK_NAME": f"{prefix}-static-resource-stack",
         "BATCH_STACK_NAME": f"{prefix}-batch-stack",
         "METRICS_BUCKET": configs["METRICS_BUCKET"],  # bucket to upload metrics
-        "DATA_BUCKET": configs["DATA_BUCKET"],  # bucket to download data
+        "DATA_BUCKET": configs.get("DATA_BUCKET", None),  # bucket to download data
         "INSTANCE_TYPES": [configs["INSTANCE"]],  # can be a list of instance families or instance types
         "COMPUTE_ENV_MAXV_CPUS": vcpu_map[configs["INSTANCE"]]
         * configs["MAX_MACHINE_NUM"],  # total max v_cpus in batch compute environment
         "CONTAINER_GPU": gpu_map[configs["INSTANCE"]],  # GPU reserved for container
         "CONTAINER_VCPU": vcpu_map[configs["INSTANCE"]],  # v_cpus reserved for container
         "CONTAINER_MEMORY": memory_map[configs["INSTANCE"]]
         - configs[
             "RESERVED_MEMORY_SIZE"
         ],  # memory in MB reserved for container, also used for shm_size, i.e. `shared_memory_size`
         "BLOCK_DEVICE_VOLUME": configs["BLOCK_DEVICE_VOLUME"],  # device attached to instance, in GB
         "LAMBDA_FUNCTION_NAME": f"{prefix}-batch-job-function",
-        "VPC_NAME": configs[
-            "VPC_NAME"
-        ],  # it's recommended to share a vpc for all benchmark infra, you can lookup an existing VPC name under aws console -> VPC, if you want to create a new one, assign a new name
+        "VPC_NAME": configs.get(
+            "VPC_NAME", None
+        ),  # it's recommended to share a vpc for all benchmark infra, you can lookup an existing VPC name under aws console -> VPC, if you want to create a new one, assign a new name
     }
     with open(CONTEXT_FILE, "w+") as f:
         try:
             cdk_config = json.load(f)
         except:
             cdk_config = {}
         cdk_config.update(context_to_parse)
         json.dump(cdk_config, f, indent=2)
         f.close()
     # set environment variables
-    os.environ["CDK_DEPLOY_ACCOUNT"] = configs["CDK_DEPLOY_ACCOUNT"]
+    os.environ["CDK_DEPLOY_ACCOUNT"] = str(configs["CDK_DEPLOY_ACCOUNT"])
     os.environ["CDK_DEPLOY_REGION"] = configs["CDK_DEPLOY_REGION"]
 
     return context_to_parse
 
 
 def deploy_stack(configs: Optional[dict] = None) -> dict:
     """
```

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/datasets/multimodal_dataset.py` & `autogluon.bench-0.0.4/src/autogluon/bench/datasets/multimodal_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/datasets/object_detection_dataset.py` & `autogluon.bench-0.0.4/src/autogluon/bench/datasets/object_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/datasets/registry.py` & `autogluon.bench-0.0.4/src/autogluon/bench/datasets/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/frameworks/benchmark.py` & `autogluon.bench-0.0.4/src/autogluon/bench/frameworks/benchmark.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/frameworks/multimodal/exec.py` & `autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/exec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import argparse
 import json
 import logging
 import os
+import time
 from datetime import datetime
 from typing import Optional
 
 from autogluon.bench.datasets.constants import (
     _IMAGE_SIMILARITY,
     _IMAGE_TEXT_SIMILARITY,
     _OBJECT_DETECTION,
     _TEXT_SIMILARITY,
 )
-from ...datasets.dataset_registry import multimodal_dataset_registry
-from ...utils.general_utils import NumpyEncoder
+from autogluon.bench.datasets.dataset_registry import multimodal_dataset_registry
+from autogluon.bench.utils.general_utils import NumpyEncoder
 from autogluon.multimodal import MultiModalPredictor
 
 logger = logging.getLogger(__name__)
 
 
 def get_args():
     parser = argparse.ArgumentParser()
@@ -138,32 +139,42 @@
     predictor = MultiModalPredictor(**predictor_args)
 
     fit_args = {
         "train_data": train_data.data,
         "hyperparameters": hyperparameters,
         "time_limit": time_limit,
     }
+
+    utc_time = datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S")
+    start_time = time.time()
     predictor.fit(**fit_args)
+    end_time = time.time()
+    training_duration = round(end_time - start_time, 1)
 
     evaluate_args = {
         "data": test_data.data,
         "label": label_column,
         "metrics": test_data.metric,
     }
     if test_data.problem_type == _IMAGE_TEXT_SIMILARITY:
         evaluate_args["query_data"] = test_data.data[test_data.text_columns[0]].unique().tolist()
         evaluate_args["response_data"] = test_data.data[test_data.image_columns[0]].unique().tolist()
         evaluate_args["cutoffs"] = [1, 5, 10]
+
+    start_time = time.time()
     scores = predictor.evaluate(**evaluate_args)
+    end_time = time.time()
+    predict_duration = round(end_time - start_time, 1)
 
-    timestamp = datetime.now()
     metrics = {
         "problem_type": predictor.problem_type,
+        "utc_time": utc_time,
+        "training_duration": training_duration,
+        "predict_duration": predict_duration,
         "scores": scores,
-        "timestamp": timestamp.strftime("%H:%M:%S"),
     }
     save_metrics(metrics_dir, metrics)
 
 
 if __name__ == "__main__":
     args = get_args()
     if args.hyperparameters is not None:
```

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py` & `autogluon.bench-0.0.4/src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import logging
 import os
 import subprocess
 import sys
 from typing import Optional
 
-from ....bench import __version__ as agbench_version
-from ..benchmark import Benchmark
+from autogluon.bench import __version__ as agbench_version
+from autogluon.bench.frameworks.benchmark import Benchmark
 
 logger = logging.getLogger(__name__)
 
 
 class MultiModalBenchmark(Benchmark):
     """
     A benchmark class for AutoGluon MultiModal.
```

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py` & `autogluon.bench-0.0.4/src/autogluon/bench/frameworks/tabular/tabular_benchmark.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/runbenchmark.py` & `autogluon.bench-0.0.4/src/autogluon/bench/runbenchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,17 +95,17 @@
 
     module_kwargs = get_kwargs(module=module_name, configs=configs)
     benchmark.setup(**module_kwargs.get("setup_kwargs", {}))
     benchmark.run(**module_kwargs.get("run_kwargs", {}))
     logger.info(f"Backing up benchmarking configs to {benchmark.metrics_dir}/configs.yaml")
     _dump_configs(benchmark_dir=benchmark.metrics_dir, configs=configs, file_name="configs.yaml")
 
-    if configs.get("metrics_bucket", None):
+    if configs.get("METRICS_BUCKET", None):
         s3_dir = f"{module_name}{benchmark_dir.split(module_name)[-1]}"
-        benchmark.upload_metrics(s3_bucket=configs["metrics_bucket"], s3_dir=s3_dir)
+        benchmark.upload_metrics(s3_bucket=configs["METRICS_BUCKET"], s3_dir=s3_dir)
 
 
 def upload_config(bucket: str, benchmark_name: str, file: str):
     """Uploads a configuration file to an S3 bucket.
 
     Args:
         bucket (str): The name of the S3 bucket to upload the file to.
@@ -289,15 +289,15 @@
         configs["benchmark_name"] = benchmark_name
         cloud_config_path = _dump_configs(
             benchmark_dir=benchmark_dir, configs=configs, file_name=os.path.basename(config_file)
         )
         os.environ["AG_BENCH_VERSION"] = agbench_version  # set the installed version for Dockerfile to align with
         infra_configs = deploy_stack(configs=configs.get("cdk_context", {}))
         config_s3_path = upload_config(
-            bucket=configs["metrics_bucket"], benchmark_name=benchmark_name, file=cloud_config_path
+            bucket=infra_configs["METRICS_BUCKET"], benchmark_name=benchmark_name, file=cloud_config_path
         )
         lambda_response = invoke_lambda(configs=infra_configs, config_file=config_s3_path)
         aws_configs = {**infra_configs, **lambda_response}
         logger.info(f"Saving infra configs and submitted job configs under {benchmark_dir}.")
         aws_config_path = _dump_configs(benchmark_dir=benchmark_dir, configs=aws_configs, file_name="aws_configs.yaml")
 
         if remove_resources:
```

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/utils/dataset_utils.py` & `autogluon.bench-0.0.4/src/autogluon/bench/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/src/autogluon/bench/utils/general_utils.py` & `autogluon.bench-0.0.4/src/autogluon/bench/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.bench-0.0.3/src/autogluon.bench.egg-info/PKG-INFO` & `autogluon.bench-0.0.4/src/autogluon.bench.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,189 @@
 Metadata-Version: 2.1
 Name: autogluon.bench
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/autogluon/autogluon-bench
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon-bench/issues
 Project-URL: Source, https://github.com/autogluon/autogluon-bench/
+Description: <div align="left">
+          <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
+        </div>
+        
+        # AutoGluon-Bench
+        
+        Welcome to AutoGluon-Bench, a suite for benchmarking your AutoML frameworks.
+        
+        ## Setup
+        
+        Follow the steps below to set up autogluon-bench:
+        
+        ```bash
+        # create virtual env
+        python3 -m venv .venv_agbench
+        source .venv_agbench/bin/activate
+        ```
+        
+        Install `autogloun-bench` from PyPI:
+        
+        ```bash
+        python3 -m pip install autogluon.bench
+        ```
+        
+        Or install `autogluon-bench` from source:
+        
+        ```bash
+        git clone https://github.com/autogluon/autogluon-bench.git
+        cd autogluon-bench
+        
+        # install from source in editable mode
+        pip install -e .
+        ```
+        
+        For development, please be aware that `autogluon.bench` is installed as a dependency in certain places, such as the [Dockerfile](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/Dockerfile) and [Multimodal Setup](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/frameworks/multimodal/setup.sh). To ensure that your local changes are reflected in the installed package, you may need to adjust the installation command as necessary. A recommended approach is to push your changes to a remote git branch and then pull from this branch, installing the package from source in the scripts.
+        
+        
+        ## Run benchmarks locally
+        
+        To run the benchmarks on your local machine, use the following command:
+        
+        ```
+        agbench run path/to/local_config_file
+        ```
+        
+        Check out our [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for local runs.
+        
+        The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
+        
+        
+        ### Tabular Benchmark
+        
+        To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
+        
+        The tabular module leverages the [AMLB](https://github.com/openml/automlbenchmark) benchmarking framework. Required and optional AMLB arguments are specified via the configuration file mentioned previously.
+        
+        To benchmark a custom branch of AutoGluon on `tabular` module, use `amlb_custom_branch: https://github.com/REPO/autogluon#BRANCH` in the configuration file.
+        
+        
+        ### Multimodal Benchmark
+        
+        For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
+        
+        You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
+        
+        ## Run benchmarks on AWS
+        
+        AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
+        
+        To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following instructions:
+        
+        1. Install [Node Version Manager](https://github.com/nvm-sh/nvm#installing-and-updating).
+        2. Source profile or restart the terminal.
+        3. Follow the `Prerequisites` section on the [AWS CDK Guide](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html) and install an appropriate version for your system:
+        ```bash
+        nvm install $VERSION  # install Node.js
+        npm install -g aws-cdk  # install aws-cdk
+        cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
+        ```
+        
+        To initiate benchmarking on the cloud, use the command below:
+        
+        ```
+        agbench run /path/to/cloud_config_file
+        ```
+        
+        This command automatically sets up an AWS Batch environment using instance specifications defined in the `cloud_config_file`. It also creates a lambda function named with your chosen `LAMBDA_FUNCTION_NAME`. This lambda function is automatically invoked with the cloud config file you provided, submitting multiple AWS Batch jobs to the job queue (named with the `PREFIX` you provided).
+        
+        In order for the Lambda function to submit multiple jobs simultaneously, you need to specify a list of values for each module-specific key. Each combination of configurations is saved and uploaded to your specified `METRICS_BUCKET` in S3, stored under `S3://{METRICS_BUCKET}/configs/{BENCHMARK_NAME}_{timestamp}/{BENCHMARK_NAME}_split_{UID}.yaml`. Here, `UID` is a unique ID assigned to the split.
+        
+        The AWS infrastructure configurations and submitted job IDs are saved locally at `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`. You can use this file to check the job status at any time:
+        
+        ```bash
+        agbench get-job-status --config-file /path/to/aws_configs.yaml
+        ```
+        
+        You can also check the job status using job IDs:
+        
+        ```bash
+        agbench get-job-status --job-ids JOB_ID_1 --job-ids JOB_ID_2 —cdk_deploy_region AWS_REGION
+        
+        ```
+        
+        Job logs can be viewed on the AWS console. Each job has an `UID` attached to the name, which you can use to identify the respective config split. After the jobs are completed and reach the `SUCCEEDED` status in the job queue, you'll find metrics saved under `S3://{METRICS_BUCKET}/{module}/{benchmark_name}_{timestamp}/{benchmark_name}_{timestamp}_{UID}`.
+        
+        By default, the infrastructure created is retained for future use. To automatically remove resources after the run, use the `--remove_resources` option:
+        
+        ```bash
+        agbench run path/to/cloud_config_file --remove_resources
+        ```
+        
+        This will check the job status every 2 minutes and remove resources after all jobs succeed. If any job fails, resources will be kept.
+        
+        If you want to manually remove resources later, use:
+        
+        ```bash
+        agbench destroy-stack STATIC_RESOURCE_STACK_NAME BATCH_STACK_NAME CDK_DEPLOY_ACCOUNT CDK_DEPLOY_REGION
+        ```
+        
+        where you can find all argument values in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`.
+        
+        
+        ### Configure the AWS infrastructure
+        
+        The default infrastructure configurations are located [here](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/cloud/aws/default_config.yaml).
+        
+        where:
+        - `CDK_DEPLOY_ACCOUNT` and `CDK_DEPLOY_REGION` should be overridden with your AWS account ID and desired region to create the stack.
+        - `PREFIX` is used as an identifier for the stack and resources created.
+        - `RESERVED_MEMORY_SIZE` is used together with the instance memory size to calculate the container shm_size.
+        - `BLOCK_DEVICE_VOLUME` is the size of storage device attached to instance.
+        - `LAMBDA_FUNCTION_NAME` lambda function to submit jobs to AWS Batch.
+        
+        To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/cloud_configs.yaml) for reference.
+        
+        ## Evaluating bechmark runs
+        
+        Innixma's `autogluon-benchmark` repository can be used to evaluate tabular benchmark runs whose results are in S3.
+        Using these utilities is ad-hoc at this time, but in a coming release we will integrate this capability into `autogluon-bench` and support evaulation of multimodal benchmarks.
+        
+        ### Evaluation Steps
+        
+        Clone the `autogluon-benchmark` repository:
+        ```
+        git clone https://github.com/gidler/autogluon-benchmark.git
+        ```
+        
+        Confirm that AWS credentials are setup for the AWS account that has the benchmark results in S3.
+        
+        Run the `aggregate_all.py` script
+        ```
+        python scripts/aggregate_all.py --s3_bucket {AWS_BUCKET} --s3_prefix {AWS_PREFIX} --version_name {BENCHMARK_VERSION_NAME}
+        
+        # example: python scripts/aggregate_all.py --s3_bucket autogluon-benchmark-metrics --s3_prefix tabular/ --version_name test_local_20230330T180916
+        ```
+        
+        This will create a new file in S3 with this signature:
+        ```
+        s3://{AWS_BUCKET}/aggregated/{AWS_PREFIX}/{BENCHMARK_VERSION_NAME}/results.csv
+        ```
+        
+        Run the `run_generate_clean_openml` python utility. You will need to manually set the `run_name_arg` and `path_prefix` variables in the script.
+        ```
+        python autogluon_benchmark/evaluation/runners/run_generate_clean_openml.py 
+        ```
+        This will create a local file of results in the `data/results/input/prepared/openml/` directory.
+        
+        Run the `benchmark_evaluation` python script. You will need to manually update the `frameworks_run` and `paths` variables in the script.
+        ```
+        python autogluon_benchmark/evaluation/runners/run_evaluation_openml.py
+        ```
+        
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Financial and Insurance Industry
@@ -27,198 +200,7 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Requires-Python: >=3.8, <3.10
 Description-Content-Type: text/markdown
 Provides-Extra: tests
-License-File: LICENSE
-
-<div align="left">
-  <img src="https://user-images.githubusercontent.com/16392542/77208906-224aa500-6aba-11ea-96bd-e81806074030.png" width="350">
-</div>
-
-# AutoGluon-Bench
-
-Welcome to AutoGluon-Bench, a suite for benchmarking your AutoML frameworks.
-
-## Setup
-
-Follow the steps below to set up autogluon-bench:
-
-```bash
-# create virtual env
-python3.9 -m venv .venv_agbench
-source .venv_agbench/bin/activate
-```
-
-Install `autogloun-bench` from PyPI:
-
-```bash
-python -m pip install autogluon.bench
-```
-
-
-Or install `autogluon-bench` from source:
-
-```bash
-git clone https://github.com/autogluon/autogluon-bench.git
-cd autogluon-bench
-
-# install from source in editable mode
-pip install -e .
-```
-Also, replace all `pip install autogluon.bench` with `pip install -e .` in the source code.
-
-
-## Run benchmarks locally
-
-To run the benchmarks on your local machine, use the following command:
-
-```
-agbench run path/to/local_config_file
-```
-
-Check out our [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for local runs.
-
-The results are stored in the following directory: `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}`.
-
-
-### Tabular Benchmark
-
-To perform tabular benchmarking, set the module to tabular. You must set both Benchmark Configurations and Tabular Specific configurations, and each should have a single value. Refer to the [sample configuration file](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/local_configs.yaml) for more details.
-
-The tabular module leverages the [AMLB](https://github.com/openml/automlbenchmark) benchmarking framework. Required and optional AMLB arguments are specified via the configuration file mentioned previously.
-
-To benchmark a custom branch of AutoGluon on `tabular` module, use `amlb_custom_branch: https://github.com/REPO/autogluon#BRANCH` in the configuration file.
-
-
-### Multimodal Benchmark
-
-For multimodal benchmarking, set the module to multimodal. We currently support benchmarking multimodal on a custom branch. Note that multimodal benchmarking directly calls the MultiModalPredictor, bypassing the extra layer of [AMLB](https://github.com/openml/automlbenchmark). Therefore, the required arguments are different from those for tabular.
-
-You can add more datasets to your benchmarking jobs. We provided sample [multimodal datasets](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/multimodal_dataset.py) and [object detection dataset](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/datasets/object_detection_dataset.py). Follow these samples to add custom datasets, then specify dataset_name in your local config file. Please follow the section `Install From Source` for more instructions on how to develop with source.
-
-## Run benchmarks on AWS
-
-AutoGluon-Bench uses the AWS CDK to build an AWS Batch compute environment for benchmarking.
-
-To get started, install [Node.js](https://nodejs.org/) and [AWS CDK](https://docs.aws.amazon.com/cdk/v2/guide/getting_started.html#getting_started_install) with the following commands:
-
-```bash
-curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | bash  # replace bash with other shell (e.g. zsh) if you are using a different one
-source ~/.bashrc
-nvm install 18.16.0  # install Node.js
-npm install -g aws-cdk  # install aws-cdk
-cdk --version  # verify the installation, you might need to update the Node.js version depending on the log.
-```
-
-To initiate benchmarking on the cloud, use the command below:
-
-```
-agbench run /path/to/cloud_config_file
-```
-
-This command automatically sets up an AWS Batch environment using instance specifications defined in the `cloud_config_file`. It also creates a lambda function named with your chosen `LAMBDA_FUNCTION_NAME`. This lambda function is automatically invoked with the cloud config file you provided, submitting multiple AWS Batch jobs to the job queue (named with the `PREFIX` you provided).
-
-In order for the Lambda function to submit multiple jobs simultaneously, you need to specify a list of values for each module-specific key. Each combination of configurations is saved and uploaded to your specified `METRICS_BUCKET` in S3, stored under `S3://{METRICS_BUCKET}/configs/{BENCHMARK_NAME}_{timestamp}/{BENCHMARK_NAME}_split_{UID}.yaml`. Here, `UID` is a unique ID assigned to the split.
-
-The AWS infrastructure configurations and submitted job IDs are saved locally at `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`. You can use this file to check the job status at any time:
-
-```bash
-agbench get-job-status --config-file /path/to/aws_configs.yaml
-```
-
-You can also check the job status using job IDs:
-
-```bash
-agbench get-job-status --job-ids JOB_ID_1 --job-ids JOB_ID_2 —cdk_deploy_region AWS_REGION
-
-```
-
-Job logs can be viewed on the AWS console. Each job has an `UID` attached to the name, which you can use to identify the respective config split. After the jobs are completed and reach the `SUCCEEDED` status in the job queue, you'll find metrics saved under `S3://{METRICS_BUCKET}/{module}/{benchmark_name}_{timestamp}/{benchmark_name}_{timestamp}_{UID}`.
-
-By default, the infrastructure created is retained for future use. To automatically remove resources after the run, use the `--remove_resources` option:
-
-```bash
-agbench run path/to/cloud_config_file --remove_resources
-```
-
-This will check the job status every 2 minutes and remove resources after all jobs succeed. If any job fails, resources will be kept.
-
-If you want to manually remove resources later, use:
-
-```bash
-agbench destroy-stack STATIC_RESOURCE_STACK_NAME BATCH_STACK_NAME CDK_DEPLOY_ACCOUNT CDK_DEPLOY_REGION
-```
-
-where you can find all argument values in `{WORKING_DIR}/{root_dir}/{module}/{benchmark_name}_{timestamp}/aws_configs.yaml`.
-
-
-### Configure the AWS infrastructure
-
-The default infrastructure configurations are located [here](https://github.com/autogluon/autogluon-bench/blob/master/src/autogluon/bench/cloud/aws/default_config.yaml).
-
-```
-CDK_DEPLOY_ACCOUNT: dummy
-CDK_DEPLOY_REGION: dummy
-PREFIX: ag-bench-test
-RESERVED_MEMORY_SIZE: 15000
-MAX_MACHINE_NUM: 20
-BLOCK_DEVICE_VOLUME: 100
-INSTANCE: g4dn.2xlarge
-METRICS_BUCKET: autogluon-benchmark-metrics
-DATA_BUCKET: automl-mm-bench
-VPC_NAME: automm-batch-stack/automm-vpc
-LAMBDA_FUNCTION_NAME: ag-bench-test-job-function
-```
-where:
-- `CDK_DEPLOY_ACCOUNT` and `CDK_DEPLOY_REGION` should be overridden with your AWS account ID and desired region to create the stack.
-- `PREFIX` is used as an identifier for the stack and resources created.
-- `RESERVED_MEMORY_SIZE` is used together with the instance memory size to calculate the container shm_size.
-- `BLOCK_DEVICE_VOLUME` is the size of storage device attached to instance.
-- `METRICS_BUCKET` is the bucket to upload benchmarking metrics.
-- `DATA_BUCKET` is the bucket to download dataset from.
-- `VPC_NAME` is used to look up an existing VPC.
-- `LAMBDA_FUNCTION_NAME` lambda function to submit jobs to AWS Batch.
-
-To override these configurations, use the `cdk_context` key in your custom config file. See our [sample cloud config](https://github.com/autogluon/autogluon-bench/blob/master/sample_configs/cloud_configs.yaml) for reference.
-
-## Evaluating bechmark runs
-
-Innixma's `autogluon-benchmark` repository can be used to evaluate tabular benchmark runs whose results are in S3.
-Using these utilities is ad-hoc at this time, but in a coming release we will integrate this capability into `autogluon-bench` and support evaulation of multimodal benchmarks.
-
-### Evaluation Steps
-
-Clone the `autogluon-benchmark` repository:
-```
-git clone https://github.com/gidler/autogluon-benchmark.git
-```
-
-Confirm that AWS credentials are setup for the AWS account that has the benchmark results in S3.
-
-Run the `aggregate_all.py` script
-```
-python scripts/aggregate_all.py --s3_bucket {AWS_BUCKET} --s3_prefix {AWS_PREFIX} --version_name {BENCHMARK_VERSION_NAME}
-
-# example: python scripts/aggregate_all.py --s3_bucket autogluon-benchmark-metrics --s3_prefix tabular/ --version_name test_local_20230330T180916
-```
-
-This will create a new file in S3 with this signature:
-```
-s3://{AWS_BUCKET}/aggregated/{AWS_PREFIX}/{BENCHMARK_VERSION_NAME}/results.csv
-```
-
-Run the `run_generate_clean_openml` python utility. You will need to manually set the `run_name_arg` and `path_prefix` variables in the script.
-```
-python autogluon_benchmark/evaluation/runners/run_generate_clean_openml.py 
-```
-This will create a local file of results in the `data/results/input/prepared/openml/` directory.
-
-Run the `benchmark_evaluation` python script. You will need to manually update the `frameworks_run` and `paths` variables in the script.
-```
-python autogluon_benchmark/evaluation/runners/run_evaluation_openml.py
-```
-
-
-
```

### Comparing `autogluon.bench-0.0.3/src/autogluon.bench.egg-info/SOURCES.txt` & `autogluon.bench-0.0.4/src/autogluon.bench.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,48 +8,39 @@
 src/autogluon.bench.egg-info/SOURCES.txt
 src/autogluon.bench.egg-info/dependency_links.txt
 src/autogluon.bench.egg-info/entry_points.txt
 src/autogluon.bench.egg-info/namespace_packages.txt
 src/autogluon.bench.egg-info/requires.txt
 src/autogluon.bench.egg-info/top_level.txt
 src/autogluon.bench.egg-info/zip-safe
-src/autogluon/bench/Dockerfile
 src/autogluon/bench/__init__.py
-src/autogluon/bench/entrypoint.sh
 src/autogluon/bench/main.py
 src/autogluon/bench/runbenchmark.py
 src/autogluon/bench/version.py
 src/autogluon/bench/cloud/__init__.py
 src/autogluon/bench/cloud/aws/__init__.py
 src/autogluon/bench/cloud/aws/app.py
 src/autogluon/bench/cloud/aws/constants.py
-src/autogluon/bench/cloud/aws/default_config.yaml
-src/autogluon/bench/cloud/aws/deploy.sh
-src/autogluon/bench/cloud/aws/destroy.sh
 src/autogluon/bench/cloud/aws/stack_handler.py
 src/autogluon/bench/cloud/aws/batch_stack/__init__.py
 src/autogluon/bench/cloud/aws/batch_stack/stack.py
 src/autogluon/bench/cloud/aws/batch_stack/constructs/__init__.py
 src/autogluon/bench/cloud/aws/batch_stack/constructs/batch_lambda_function.py
 src/autogluon/bench/cloud/aws/batch_stack/constructs/instance_profile.py
 src/autogluon/bench/cloud/aws/batch_stack/lambdas/__init__.py
 src/autogluon/bench/cloud/aws/batch_stack/lambdas/lambda_function.py
-src/autogluon/bench/cloud/aws/batch_stack/lambdas/requirements.txt
 src/autogluon/bench/datasets/__init__.py
 src/autogluon/bench/datasets/constants.py
 src/autogluon/bench/datasets/dataset_registry.py
 src/autogluon/bench/datasets/multimodal_dataset.py
 src/autogluon/bench/datasets/object_detection_dataset.py
 src/autogluon/bench/datasets/registry.py
 src/autogluon/bench/frameworks/__init__.py
 src/autogluon/bench/frameworks/benchmark.py
 src/autogluon/bench/frameworks/multimodal/__init__.py
 src/autogluon/bench/frameworks/multimodal/exec.py
 src/autogluon/bench/frameworks/multimodal/multimodal_benchmark.py
-src/autogluon/bench/frameworks/multimodal/setup.sh
 src/autogluon/bench/frameworks/tabular/__init__.py
-src/autogluon/bench/frameworks/tabular/exec.sh
-src/autogluon/bench/frameworks/tabular/setup.sh
 src/autogluon/bench/frameworks/tabular/tabular_benchmark.py
 src/autogluon/bench/utils/__init__.py
 src/autogluon/bench/utils/dataset_utils.py
 src/autogluon/bench/utils/general_utils.py
```

