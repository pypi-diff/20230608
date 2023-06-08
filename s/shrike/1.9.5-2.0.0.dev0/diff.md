# Comparing `tmp/shrike-1.9.5.tar.gz` & `tmp/shrike-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrike-1.9.5.tar", last modified: Wed Aug 11 15:45:43 2021, max compression
+gzip compressed data, was "shrike-2.0.0.dev0.tar", last modified: Thu Jun  8 20:41:44 2023, max compression
```

## Comparing `shrike-1.9.5.tar` & `shrike-2.0.0.dev0.tar`

### file list

```diff
@@ -1,53 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2021-08-11 15:43:54.000000 shrike-1.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)   627957 2021-08-11 15:43:54.000000 shrike-1.9.5/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7186 2021-08-11 15:45:43.127162 shrike-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5637 2021-08-11 15:43:54.000000 shrike-1.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-11 15:45:43.127162 shrike-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2021-08-11 15:43:54.000000 shrike-1.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.123162 shrike-1.9.5/shrike/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.123162 shrike-1.9.5/shrike/build/
--rw-r--r--   0 runner    (1001) docker     (121)      427 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.123162 shrike-1.9.5/shrike/build/commands/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40962 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/commands/prepare.py
--rw-r--r--   0 runner    (1001) docker     (121)     7142 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/commands/register.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.123162 shrike-1.9.5/shrike/build/core/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12518 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/core/command_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     7594 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/core/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/shrike/build/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5526 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/build/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/shrike/compliant_logging/
--rw-r--r--   0 runner    (1001) docker     (121)      932 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    10327 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (121)    13617 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    37911 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     4875 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/stack_trace_extractor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/compliant_logging/system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/shrike/pipeline/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4900 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/aml_connect.py
--rw-r--r--   0 runner    (1001) docker     (121)     7143 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/canary_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    13162 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/module_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3277 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    63121 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/pipeline_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/telemetry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/shrike/pipeline/testing/
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24363 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/testing/components.py
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/testing/importer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/testing/module_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     7855 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/pipeline/testing/pipeline_class_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.127162 shrike-1.9.5/shrike/spark/
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4870 2021-08-11 15:43:54.000000 shrike-1.9.5/shrike/spark/spark_net.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-11 15:45:43.123162 shrike-1.9.5/shrike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7186 2021-08-11 15:45:42.000000 shrike-1.9.5/shrike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-08-11 15:45:42.000000 shrike-1.9.5/shrike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-11 15:45:42.000000 shrike-1.9.5/shrike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      848 2021-08-11 15:45:42.000000 shrike-1.9.5/shrike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-08-11 15:45:42.000000 shrike-1.9.5/shrike.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.914792 shrike-2.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)   252717 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-06-08 20:41:44.914792 shrike-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6977 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-08 20:41:44.914792 shrike-2.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2318 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.898791 shrike-2.0.0.dev0/shrike/
+-rw-r--r--   0 runner    (1001) docker     (122)      399 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.902791 shrike-2.0.0.dev0/shrike/_core/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4102 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/_core/eyesoff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/_core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1048 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.902791 shrike-2.0.0.dev0/shrike/build/
+-rw-r--r--   0 runner    (1001) docker     (122)      427 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.902791 shrike-2.0.0.dev0/shrike/build/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61555 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/build/commands/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8229 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/build/commands/register.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.902791 shrike-2.0.0.dev0/shrike/build/core/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/build/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13960 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/build/core/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8499 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/build/core/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.902791 shrike-2.0.0.dev0/shrike/build/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5526 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/build/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.906791 shrike-2.0.0.dev0/shrike/compliant_logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/compliant_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6036 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/compliant_logging/argparser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      429 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/compliant_logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10327 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/compliant_logging/data_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16169 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/compliant_logging/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41145 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/compliant_logging/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10311 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/compliant_logging/progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/compliant_logging/stack_trace_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1967 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/compliant_logging/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.906791 shrike-2.0.0.dev0/shrike/distributed/
+-rw-r--r--   0 runner    (1001) docker     (122)      254 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/distributed/cluster_auto_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9829 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/distributed/dask.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4130 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/distributed/mpi_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/distributed/ray.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.910791 shrike-2.0.0.dev0/shrike/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (122)      537 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/argparser_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7223 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/canary_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.898791 shrike-2.0.0.dev0/shrike/pipeline/components/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.910791 shrike-2.0.0.dev0/shrike/pipeline/components/fedavg/
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/components/fedavg/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     2616 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/components/fedavg/run.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2389 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/components/fedavg/spec.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    35499 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/federated_learning.py
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20048 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/module_helper_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16294 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      206 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/pipeline_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42898 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/pipeline_helper_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2561 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/ray_actor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2685 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/telemetry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.910791 shrike-2.0.0.dev0/shrike/pipeline/testing/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24460 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/testing/components.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/testing/importer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1837 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/testing/module_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7894 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/testing/pipeline_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7520 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/testing/pipeline_class_test_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.914792 shrike-2.0.0.dev0/shrike/pipeline/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5039 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/v1/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3565 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/v1/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    75640 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/v1/pipeline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.914792 shrike-2.0.0.dev0/shrike/pipeline/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/v2/aml_connect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/v2/module_helper.py
+-rw-r--r--   0 runner    (1001) docker     (122)    68222 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/pipeline/v2/pipeline_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.914792 shrike-2.0.0.dev0/shrike/spark/
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4936 2023-06-08 20:37:09.000000 shrike-2.0.0.dev0/shrike/spark/spark_net.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 20:41:44.902791 shrike-2.0.0.dev0/shrike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8629 2023-06-08 20:41:44.000000 shrike-2.0.0.dev0/shrike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2238 2023-06-08 20:41:44.000000 shrike-2.0.0.dev0/shrike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 20:41:44.000000 shrike-2.0.0.dev0/shrike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-06-08 20:41:44.000000 shrike-2.0.0.dev0/shrike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-08 20:41:44.000000 shrike-2.0.0.dev0/shrike.egg-info/top_level.txt
```

### Comparing `shrike-1.9.5/LICENSE` & `shrike-2.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `shrike-1.9.5/README.md` & `shrike-2.0.0.dev0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Shrike: Compliant Azure ML Utilities
+# Shrike: incubation for Azure ML
 
-[![CodeQL](https://github.com/Azure/shrike/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Azure/shrike/actions/workflows/codeql-analysis.yml)
-[![docs](https://github.com/Azure/shrike/actions/workflows/docs.yml/badge.svg)](https://github.com/Azure/shrike/actions/workflows/docs.yml)
-[![python](https://github.com/Azure/shrike/actions/workflows/python.yml/badge.svg)](https://github.com/Azure/shrike/actions/workflows/python.yml)
+[![CodeQL](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/codeql-analysis.yml)
+[![docs](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/docs.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/docs.yml)
+[![python](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/python.yml/badge.svg)](https://github.com/ai-platform-ml-platform/shrike/actions/workflows/python.yml)
 [![Component Governance](https://dev.azure.com/msdata/Vienna/_apis/build/status/aml-ds/Azure.shrike%20Component%20Governance?branchName=main)](https://dev.azure.com/msdata/Vienna/_build/latest?definitionId=16088&branchName=main)
 [![Python versions](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/downloads/)
 [![code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-[![codecov](https://codecov.io/gh/Azure/shrike/branch/main/graph/badge.svg?token=sSq0BKlfTu)](https://codecov.io/gh/Azure/shrike)
+[![codecov](https://codecov.io/gh/ai-platform-ml-platform/shrike/branch/main/graph/badge.svg?token=sSq0BKlfTu)](https://codecov.io/gh/ai-platform-ml-platform/shrike)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/shrike)](https://pypi.org/project/shrike/)
 [![PyPI version](https://badge.fury.io/py/shrike.svg)](https://badge.fury.io/py/shrike)
 [![license: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](LICENSE)
 
 The `shrike` library is a set of Python utilities for running experiments in the 
 [Azure Machine Learning](https://github.com/Azure/azureml-examples) platform (_a.k.a._ Azure ML). This
 library contains four elements, which are:
@@ -19,19 +19,24 @@
 exception handling;
 -  `shrike.pipeline`: helper code for managing, validating and submitting Azure
 ML pipelines based on 
 [azure-ml-component](https://aka.ms/azure-ml-component-reference) (_a.k.a._ the Component SDK);
 -  `shrike.build`: helper code for packaging, building, validating, signing and
 registering Azure ML components.
 - `shrike.spark`: utilities for running jobs, especially those leveraging Spark
-  .NET, in HDInsight.
+  .NET, in HDInsight and later Synapse.
 
 ## Documentation
 For the full documentation of `shrike` with detailed examples and API reference, 
-please see the [docs page](http://azure.github.io/shrike).
+please see the [docs page](https://shrike-docs.com/).
+
+For a list of problems (along with guidance and solutions) designed specifically
+to help you learn how to use shrike, please refer to the information in
+[this README file](https://github.com/Azure/azure-ml-problem-sets/blob/main/README.md#azure-ml-problems-aimed-at-learning-shrike)
+(located in another GitHub repository).
 
 ## Installation
 
 The `shrike` library is publicly available in PyPi. There are three optional extra dependencies: `pipeline`, `build`, and `dev`.
 The `pipeline` dependency is for submitting Azure ML pipelines, `build` is for signing and registering components, 
 and `dev` is for the development environment of `shrike`.
 
@@ -48,42 +53,56 @@
 pip install shrike[pipeline]
 ```
 - If you would like to contribute to the source code, please `pip install` with all the dependencies:
 ```pwsh
 pip install shrike[pipeline,build,dev]
 ```
 
+Alternatively, for local development, you may use the Conda environment defined
+in [environment.yml](./environment.yml). It pins the appropriate versions of
+pip, Python, and installs all shrike together with all extras as an editable
+package.
+
+:warning: If you are using a ZSH terminal, please consider adding quotes,
+e.g., `pip install "shrike[pipeline,build,dev]"` to avoid the accidental shell expansion.
+
 ## Migration from `aml-build-tooling`, `aml-ds-pipeline-contrib`, and `confidential-ml-utils`
 If you have been using the `aml-build-tooling`, `aml-ds-pipeline-contrib`, or `confidential-ml-utils` libraries, 
-please use the migration script ([migration.py](https://github.com/Azure/shrike/blob/main/migration.py)) to convert your repo or files and
+please use the migration script ([migration.py](https://github.com/ai-platform-ml-platform/shrike/blob/main/migration.py)) to convert your repo or files and
 adopt the `shrike` package with one simple command:
 ```pwsh
 python migraton.py --input_path PATH/TO/YOUR/REPO/OR/FILE
 ```
 :warning: This command will update files **in-place**. Please make a copy of your repo/file if you do not want to do so.
 
 ## Need Support?
 If you have any feature requests, technical questions, or find
 any bugs, please do not hesitate to reach out to us.
 
-- For bug reports and feature requests, you are welcome to open an [issue](https://github.com/Azure/shrike/issues). 
+- For bug reports and feature requests, you are welcome to open an [issue](https://github.com/ai-platform-ml-platform/shrike/issues). 
 - If you are a Microsoft employee, please refer to the 
 [support page](https://aka.ms/aml/support) for details;
 - If you are outside Microsoft, please send an email
-to [aml-ds@microsoft.com](mailto:aml-ds@microsoft.com). 
+to [aims-team@microsoft.com](mailto:aims-team@microsoft.com). 
 
 
 ## Contributing
 
 This project welcomes contributions and suggestions. Most contributions require
 you to agree to a Contributor License Agreement (CLA) declaring that you have
 the right to, and actually do, grant us the rights to use your contribution.
 For details, visit https://cla.opensource.microsoft.com.
 
-When you submit a pull request, a CLA bot will automatically determine whether
+To contribute, please start by creating a self-assigned [issue](https://github.com/ai-platform-ml-platform/shrike/issues/new/choose)
+giving a high-level overview of what you'd like to do.
+Once any discussion there concludes, follow up with a PR.
+
+Please join the security group "aml-ds-guests" on [IDweb](https://idweb.microsoft.com/IdentityManagement/default.aspx), if you have difficulty
+in creating a branch. When you submit a pull request, 
+a CLA bot will automatically determine whether
 you need to provide a CLA and decorate the PR appropriately (e.g., status check,
 comment). Simply follow the instructions provided by the bot. You will only need
 to do this once across all repos using our CLA.
 
 This project has adopted the
 [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the
```

### Comparing `shrike-1.9.5/setup.py` & `shrike-2.0.0.dev0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 https://docs.python.org/3/distutils/setupscript.html
 """
 
 
 import pathlib
 from setuptools import setup, find_packages
 from shrike import __version__
+import glob
 
 
 def versions_in_requirements(file):
     lines = file.read().splitlines()
     versions = [
         line
         for line in lines
@@ -30,43 +31,51 @@
 
 with open(HERE / "requirements/requirements-logging.txt") as f:
     required_logging = versions_in_requirements(f)
 
 with open(HERE / "requirements/requirements-pipeline.txt") as f:
     required_pipeline = versions_in_requirements(f)
 
+with open(HERE / "requirements/requirements-distributed.txt") as f:
+    required_distributed = versions_in_requirements(f)
+
 with open(HERE / "requirements/requirements-build.txt") as f:
     required_build = versions_in_requirements(f)
 
 with open(HERE / "requirements/requirements-dev.txt") as f:
     required_dev = versions_in_requirements(f)
 
+
+def component_files():
+    return glob.glob("shrike/components/**/**")
+
+
 setup(
     name="shrike",
     version=__version__,
     description="Python utilities for compliant Azure machine learning",
     long_description=README,
     long_description_content_type="text/markdown",
-    url="https://github.com/azure/shrike",
+    url="https://github.com/ai-platform-ml-platform/shrike",
     author="AML Data Science",
     author_email="aml-ds@microsoft.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
     packages=find_packages(include=["shrike*"]),
     include_package_data=True,
     install_requires=required_logging,
     extras_require={
         "pipeline": required_pipeline,
+        "distributed": required_distributed,
         "build": required_build,
         "dev": required_dev,
     },
     # https://stackoverflow.com/a/48777286
     python_requires="~=3.6",
+    package_data={"components": component_files()},
 )
```

### Comparing `shrike-1.9.5/shrike/build/commands/register.py` & `shrike-2.0.0.dev0/shrike/build/commands/register.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
 import logging
 import re
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 from packaging.version import parse
 from ruamel.yaml import YAML
 import os
+import multiprocessing
 
 from shrike.build.core.command_line import Command
 
 log = logging.getLogger(__name__)
 
 
 class Register(Command):
@@ -38,103 +39,119 @@
         absolute paths of these components in the format of a list of string.
         """
         if dir is None:
             dir = self.config.working_directory
 
         signed_component_spec_files = []
         # Find the path of spec files in the '.build' folders
-        for spec_path in Path(dir).glob(
-            "**/.build/" + Path(self.config.component_specification_glob).name
-        ):
+        for spec_path in Path(dir).glob(f'{Path(self.config.component_specification_glob).parent}/.build/{Path(self.config.component_specification_glob).name}'):
+
             # Check whether the component is signed by examining catalog files
             if (
                 spec_path.parent.joinpath("catalog.json").exists()
                 and spec_path.parent.joinpath("catalog.json.sig").exists()
             ):
                 signed_component_spec_files.append(os.path.abspath(spec_path))
-                log.info(f"Find a signed component for AML: {spec_path}")
+                log.info(f"Found a signed component for AML: {spec_path}")
             elif spec_path.parent.joinpath(".build.cat").exists():
-                log.info(f"Find a signed component for Aether: {spec_path}")
+                log.info(f"Found a signed component for Aether: {spec_path}")
             else:
-                log.warning(f"Find an unsigned component: {spec_path}")
+                log.warning(f"Found an unsigned component: {spec_path}")
             log.info(str(spec_path.parent.joinpath("catalog.json")))
 
         if len(signed_component_spec_files) == 0:
             log.info("Cannot find any signed components for AML.")
         else:
             log.info(
-                f"Find {len(signed_component_spec_files)} signed components for AML."
+                f"Found {len(signed_component_spec_files)} signed components for AML."
             )
 
         return signed_component_spec_files
 
     def list_registered_component(self) -> None:
         """
         Log all registered component in the attached workspace by using az ml command.
         """
         list_registered_component_success = self.execute_azure_cli_command(
-            f"ml component list -o table"
+            f"ml component list -o table", ignore_blowfish=True
         )
         if not list_registered_component_success:
             self.register_error(f"Error when listing registered components.")
 
-    def register_all_signed_components(self, files: List[str]) -> None:
+    def register_all_signed_components(self, files: List[str], registry: Optional[str] = None) -> None:
         """
-        For each signed component specification file, run `az ml component create`,
-        and register the status (+ register error if registration failed).
+        Run register_component_with_status() in parallel with nb_cores threads
         """
-        for component in files:
-
-            register_command, stderr_is_failure = self.register_component_command(
-                component
-            )
+        if files:
+            nb_cores = self.nb_cores
 
-            register_component_success = self.execute_azure_cli_command(
-                command=register_command,
-                stderr_is_failure=stderr_is_failure,
-            )
-            if register_component_success:
-                log.info(f"Component {component} is registered.")
-                self.register_component_status(component, "register", "succeeded")
+            if nb_cores == 1:
+                for component in files:
+                    self.register_component_with_status(component, registry)
             else:
-                self.register_component_status(component, "register", "failed")
-                self.register_error(f"Error when registering component {component}.")
+                log.info(f"Batch register with {nb_cores} threads.")
+                files_with_registry = [(f, registry) for f in files]
+                pool = multiprocessing.Pool(processes=nb_cores)
+                pool.starmap(self.register_component_with_status, files_with_registry)
+                pool.close()
+                pool.join()
+
+    def register_component_with_status(self, component, registry: Optional[str] = None) -> None:
+        """
+        For one of the signed component specification file, run `az ml component create`,
+        and register the status (+ register error if registration failed).
+        """
+        register_command = self.register_component_command(component, registry)
 
-    def register_component_command(self, component):
+        register_component_success = self.execute_azure_cli_command(
+            command=register_command,
+            stderr_is_failure=False,
+            fail_if_version_exists=self.config.fail_if_version_exists,
+        )
+        if register_component_success:
+            log.info(f"Component {component} is registered.")
+            self.register_component_status(component, "register", "succeeded")
+        else:
+            self.register_component_status(component, "register", "failed")
+            self.register_error(f"Error when registering component {component}.")
+
+    def register_component_command(self, component, registry: Optional[str] = None):
         register_command = f"ml component create --file {component}"
         set_default_version = False
         component_raw_version = self.read_component_version(component)
 
         if self.config.all_component_version:
             register_command += f" --version {self.config.all_component_version}"
             component_raw_version = self.config.all_component_version
             log.info(
                 f"Overwrite the component version with the specified value {self.config.all_component_version}"
             )
+
+        if registry:
+            register_command += f" --registry {registry}"
+
         try:
-            component_version = parse(component_raw_version)
+            component_version = parse(str(component_raw_version))
             set_default_version = (
-                component_version.base_version == component_raw_version
+                component_version.base_version == str(component_raw_version)
             )
         except:
             log.error(f"{component_raw_version} is not a valid version number.")
-        stderr_is_failure = self.config.fail_if_version_exists
         if set_default_version:
             log.info(
                 f"Component {component} version {component_raw_version} is production-ready. Setting as default."
             )
             register_command += f" --label default"
         else:
             log.info(
                 f"Component {component} version {component_raw_version} is not production-ready. NOT setting as default."
             )
-            stderr_is_failure = False
 
         log.info(f"Register command is {register_command}")
-        return register_command, stderr_is_failure
+        return register_command
 
     def read_component_version(self, yaml_file: str) -> str:
         yaml = YAML(typ="safe")
         with open(yaml_file, "r") as file:
             spec = yaml.load(file)
         try:
             version = spec["version"]
@@ -164,11 +181,14 @@
                 log.info("List of components in workspace before current registration.")
                 self.list_registered_component()
 
                 self.register_all_signed_components(files=component_path)
 
                 log.info("List of components in workspace after current registration.")
                 self.list_registered_component()
+            for registry in self.config.registries:
+                log.info(f"Start registering signed components in {registry}")
+                self.register_all_signed_components(files=component_path, registry=registry)
 
 
 if __name__ == "__main__":
     Register().run()
```

### Comparing `shrike-1.9.5/shrike/build/core/command_line.py` & `shrike-2.0.0.dev0/shrike/build/core/command_line.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from abc import ABC, abstractmethod
 import base64
 import logging
 from omegaconf import OmegaConf
 from pathlib import Path
 import subprocess
 import sys
+import os
 from typing import Any, Dict, List, Optional, Tuple, Union
 from dataclasses import asdict
 
 from shrike import __version__
 from shrike.build.core.configuration import Configuration, load_configuration
 from shrike.build.utils.utils import TelemetryLogger
 
@@ -37,38 +38,46 @@
     """
 
     @abstractmethod
     def __init__(self) -> None:
         self.config: Configuration = None  # type: ignore
         self._component_statuses: Dict[str, Dict[str, str]] = {}
         self._errors: List[str] = []
+        self.nb_cores = 1
 
     def attach_workspace(self, workspace_id: str = None) -> None:
         """
         Run `az ml folder attach` to the configured workspace ID. Default to the
         first configured workspace if none is provided.
         """
         working_direcotry = self.config.working_directory
         if workspace_id is None:
-            try:
-                workspace_id = self.config.workspaces[0]
-            except IndexError:
-                self.register_error(
-                    f"No workspaces are configured. Please include them in your configuration file and ensure the path to your configuration file is correct relative to the working directory {working_direcotry} using `--configuration-file PATH/TO/CONFIGURATION_FILE`."
-                )
-                return
+            if not self.config.workspaces and self.config.registries:
+                workspace_id = self.config.validation_workspace
+                if not workspace_id:
+                    self.register_error("No workspaces are configured. If you want to publish to registries only, please specify one workspace string in `validation_workspace` for validating components.")
+                    return
+            else:
+                try:
+                    workspace_id = self.config.workspaces[0]
+                except IndexError:
+                    self.register_error(
+                        f"No workspaces are configured. Please include them in your configuration file and ensure the path to your configuration file is correct relative to the working directory {working_direcotry} using `--configuration-file PATH/TO/CONFIGURATION_FILE`."
+                    )
+                    return
 
         (subscription_id, resource_group, workspace) = self.parse_workspace_arm_id(
             workspace_id
         )
         success = self.execute_azure_cli_command(
             f"account set --subscription {subscription_id}"
         )
         success = success and self.execute_azure_cli_command(
-            f"ml folder attach --workspace-name {workspace} --resource-group {resource_group}"
+            f"ml folder attach --workspace-name {workspace} --resource-group {resource_group}",
+            ignore_blowfish = True
         )
         if not success:
             self.register_error(f"Error!! Failed to attach to {workspace_id}!")
 
     def display_all_statuses(self) -> None:
         """
         Display all component statuses in an easily readable format.
@@ -97,17 +106,17 @@
         )
 
         if component_cli_exists:
             log.info("component CLI exists. Skipping installation.")
             return True
         else:
             log.info(
-                f"installing component CLI version 0.1.0.{self.config.component_cli_version}."
+                f"installing component CLI version {self.config.component_cli_version}."
             )
-            cli_install_command = f"extension add --source https://azuremlsdktestpypi.blob.core.windows.net/wheels/modulesdkpreview/azure_cli_ml-0.1.0.{self.config.component_cli_version}-py3-none-any.whl --pip-extra-index-urls https://azuremlsdktestpypi.azureedge.net/CLI-SDK-Runners-Validation/{self.config.component_cli_version} --yes"
+            cli_install_command = f"extension add --source https://azuremlsdktestpypi.blob.core.windows.net/wheels/componentsdk/azure_cli_ml-{self.config.component_cli_version}-py3-none-any.whl --pip-extra-index-urls https://azuremlsdktestpypi.azureedge.net/componentsdk/{self.config.component_cli_version} --yes"
             if self.config.verbose:
                 cli_install_command += " --verbose"
 
             is_installed = self.execute_azure_cli_command(
                 command=cli_install_command,
                 # installation may show time to install
                 stderr_is_failure=False,
@@ -121,15 +130,17 @@
             return is_installed
 
     def execute_azure_cli_command(
         self,
         command: str,
         working_dir: Optional[str] = None,
         stderr_is_failure: bool = True,
+        fail_if_version_exists: bool = False,
         log_error: bool = True,
+        ignore_blowfish: bool = False,
     ) -> bool:
         """
         Use this method, NOT `execute_command`, for running Azure CLI commands.
         The `command` string should contain everything AFTER the `az`.
 
         This does NOT use the `azure-cli-core` Python package
         ( https://stackoverflow.com/a/55960725 ) because it takes a long time
@@ -139,30 +150,32 @@
         exposes commands. The "naive approach" doesn't work.
         """
         log.debug(f"Executing: az {command}")
         az_command_bytes = bytes(f"az {command}", "utf-16le")
         az_command_b64 = base64.b64encode(az_command_bytes).decode("ascii")
         pwsh_command = ["pwsh", "-EncodedCommand", az_command_b64]
         success = self.execute_command(
-            pwsh_command, working_dir, stderr_is_failure, log_error
+            pwsh_command, working_dir, stderr_is_failure, fail_if_version_exists, log_error, ignore_blowfish
         )
         return success
 
     def execute_command(
         self,
         command: List[str],
         working_dir: Optional[str] = None,
         stderr_is_failure: bool = True,
+        fail_if_version_exists: bool = False,
         log_error: bool = True,
+        ignore_blowfish: bool = False,
     ) -> bool:
         """
         Execute the provided shell command using the configured timeout. Working
         directory defaults to the configured one. If `stderr_is_failure` is
         set to false, stderr from the command will be converted to "vanilla"
-        logs and will not affect success.
+        logs and will not affect success; 
 
         Logs are NOT streamed realtime - they are "bundled together" after the
         command executes or times out.
 
         Warning: running `az *` naively via this function will not work, since
         the Azure CLI is not, by default, discoverable via `subprocess.run`.
         """
@@ -172,15 +185,15 @@
         if len(command) > 0 and command[0] == "az":
             raise ValueError(
                 "Do not run Azure CLI commands with this function. Use execute_azure_cli_command instead."
             )
 
         kwargs = {}
 
-        if stderr_is_failure:
+        if stderr_is_failure or fail_if_version_exists:
             kwargs["stderr"] = subprocess.PIPE
 
         log.debug(f"Executing {command} in {working_dir}")
 
         timeout = self.config.shell_command_timeout_in_seconds
 
         try:
@@ -214,24 +227,32 @@
                     line = str(line, encoding="utf-8", errors="ignore")  # type: ignore
                 except:
                     log.debug(
                         "Failed to convert the following stdout line into String (utf-8)"
                     )
                 log.info(line)
         if stderr:
+            stderr = stderr.decode() if isinstance(stderr, bytes) else stderr
+            if ignore_blowfish and "Blowfish" in stderr:
+                log.info("Ignoring Blowfish error.")
+                return True
+                
             for line in stderr.splitlines():
                 try:
                     line = str(line, encoding="utf-8", errors="ignore")  # type: ignore
                 except:
                     log.debug(
                         "Failed to convert the following stdout line into String (utf-8)"
                     )
                 if stderr_is_failure:
                     log.error(line)
                     success = False
+                elif fail_if_version_exists and "Error" in line and "already exists in" in line:
+                    log.error(line)
+                    success = False                       
                 else:
                     log.info(line)
 
         return success
 
     def normalize_path(self, path: Union[str, Path], directory=False) -> str:
         """
@@ -305,14 +326,20 @@
         appropriate exit code. This should be the entrypoint inside a command's
         `if __name__ == "__main__"` block.
         """
         config = load_configuration()
 
         log_level = "DEBUG" if config.verbose else "INFO"
         logging.basicConfig(level=log_level, format=config.log_format)
+        
+        max_nb_cores = max(os.cpu_count() - 1, 1) # type: ignore
+        if config.number_of_cores_parallel <= 0 or config.number_of_cores_parallel > max_nb_cores:
+            self.nb_cores = max_nb_cores
+        else:
+            self.nb_cores = config.number_of_cores_parallel
 
         with self.emphasize():
             config_yaml = OmegaConf.to_yaml(config)
             log.info("Final configuration being used:\n")
             log.info(config_yaml)
 
         self.config = config
```

### Comparing `shrike-1.9.5/shrike/build/core/configuration.py` & `shrike-2.0.0.dev0/shrike/build/core/configuration.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,42 +9,57 @@
 from typing import Any, Dict, List
 import warnings
 
 
 log = logging.getLogger(__name__)
 
 
+# Freeze single "empty list" so by-reference comparison of default values works.
+_EMPTY_LIST = []
+
+
 @dataclass(frozen=True)
 class Configuration:
     # TODO: should this be handled via enum?
     activation_method: str = field(default="all")
     compliant_branch: str = field(default="^refs/heads/main$")
     source_branch: str = field(default="")
-    component_cli_version: str = field(default="42428082")
+    component_cli_version: str = field(default="0.9.18")
     component_specification_glob: str = field(default="**/spec.yaml")
     # TODO: consider a way of supporting both this and `*.yaml` as defaults.
     configuration_file: str = field(default="aml-build-configuration.yml")
     log_format: str = field(default="%(message)s")
-    shell_command_timeout_in_seconds: int = field(default=240)
+    # Registration in registries is surprisingly slow.
+    shell_command_timeout_in_seconds: int = field(default=1000)
+    number_of_cores_parallel: int = field(default=0)
     # TODO: should this be handled via enum?
     signing_mode: str = field(default="aml")
     verbose: bool = field(default=False)
     working_directory: str = field(default_factory=lambda: os.getcwd())
-    workspaces: List[str] = field(default_factory=lambda: [])
+    workspaces: List[str] = field(
+        default_factory=lambda: _EMPTY_LIST, metadata={"nargs": "*"}
+    )
     makecat_directory: str = field(default=r"C:\Program Files (x86)\Windows Kits")
     makecat_default: str = field(default=r"10\bin\x64\makecat.exe")
     # allow_duplicate_versions is on path to deprecation. Please avoid using it
     allow_duplicate_versions: bool = field(default=False)
     fail_if_version_exists: bool = field(default=False)
     use_build_number: bool = field(default=False)
     all_component_version: str = field(default="")
     disable_telemetry: bool = field(default=False)
     suppress_adding_repo_pr_tags: bool = field(default=False)
     enable_component_validation: bool = field(default=False)
+    fail_if_pattern_not_found_in_component_validation: bool = field(default=False)
     component_validation: dict = field(default_factory=dict)
+    dependency_hints: dict = field(default_factory=dict)
+    registries: List[str] = field(
+        default_factory=lambda: _EMPTY_LIST, metadata={"nargs": "*"}
+    )
+    detect_changes_in_unzipped_folder: bool = field(default=False)
+    validation_workspace: str = field(default="")
 
 
 def load_configuration() -> Configuration:
     """
     Create configuration object from "implicit" command line arguments and
     environment variables.
     """
@@ -64,21 +79,26 @@
     """
     from argparse_dataclass import ArgumentParser
 
     default_config = Configuration()
     parser = ArgumentParser(Configuration)
 
     cli_config = parser.parse_args(args)
-    cli_config = asdict(cli_config)
-
-    for key in list(cli_config.keys()):
-        if cli_config[key] == getattr(default_config, key):
-            del cli_config[key]
+    # Strangely, calling `asdict` changes the object reference for the value
+    # if it is an empty array.
+    cli_config_vars = asdict(cli_config)
+
+    for key in list(cli_config_vars.keys()):
+
+        # Compare by reference so that you can override with default values like
+        # the empty list: https://stackoverflow.com/a/14080980.
+        if getattr(cli_config, key) is getattr(default_config, key):
+            del cli_config_vars[key]
 
-    return cli_config
+    return cli_config_vars
 
 
 def load_configuration_from_args_and_env(
     args: List[str], env: Dict[str, Any]
 ) -> Configuration:
     """
     Load configuration file from provided command line arguments and environment
```

### Comparing `shrike-1.9.5/shrike/build/utils/utils.py` & `shrike-2.0.0.dev0/shrike/build/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.5/shrike/compliant_logging/__init__.py` & `shrike-2.0.0.dev0/shrike/compliant_logging/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,11 +24,17 @@
     pandas_dataframe_schema,
     pandas_series_to_list,
     numpy_array_to_list,
     spark_dataframe_schema,
     vaex_dataframe_schema,
 )
 
-from .logging import enable_compliant_logging  # noqa: F401
-from .logging import enable_confidential_logging  # noqa: F401
+from .logging import (  # noqa: F401
+    enable_compliant_logging,
+    enable_confidential_logging,
+    is_eyesoff,
+)
+from .progress import compliant_tqdm  # noqa: F401
 from .system_info import provide_system_info  # noqa: F401
 from .exceptions import prefix_stack_trace  # noqa: F401
+
+from .argparser_utils import get_args_from_component_spec  # noqa: F401
```

### Comparing `shrike-1.9.5/shrike/compliant_logging/data_conversions.py` & `shrike-2.0.0.dev0/shrike/compliant_logging/data_conversions.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.5/shrike/compliant_logging/exceptions.py` & `shrike-2.0.0.dev0/shrike/compliant_logging/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 # https://stackoverflow.com/a/38569536
 from typing import Callable, Optional, Set, TextIO, Union
 
 
 PREFIX = "SystemLog:"
 SCRUB_MESSAGE = "**Exception message scrubbed**"
+LATEST_EXCEPTION = None
 
 
 class PublicValueError(ValueError):
     """
     Value error with public message. Exceptions of this type raised under
     `prefix_stack_trace` or `print_prefixed_stack_trace_and_raise` will have
     the message prefixed with `PREFIX` in both the printed stack trace and the
@@ -46,14 +47,23 @@
     Argument error with public message. Exceptions of this type raised under
     `prefix_stack_trace` or `print_prefixed_stack_trace_and_raise` will have
     the message prefixed with `PREFIX` in both the printed stack trace and the
     re-raised exception.
     """
 
 
+class PublicArgumentTypeError(argparse.ArgumentTypeError):
+    """
+    Argument type error with public message. Exceptions of this type raised under
+    `prefix_stack_trace` or `print_prefixed_stack_trace_and_raise` will have
+    the message prefixed with `PREFIX` in both the printed stack trace and the
+    re-raised exception.
+    """
+
+
 class PublicKeyError(KeyError):
     """
     Key error with public message. Exceptions of this type raised under
     `prefix_stack_trace` or `print_prefixed_stack_trace_and_raise` will have
     the message prefixed with `PREFIX` in both the printed stack trace and the
     re-raised exception.
     """
@@ -100,32 +110,84 @@
         I/O error with public message. Exceptions of this type raised
     under `prefix_stack_trace` or `print_prefixed_stack_trace_and_raise` will
         have the message prefixed with `PREFIX` in both the printed stack trace and
         the re-raised exception.
     """
 
 
+class PublicEnvironmentError(EnvironmentError):
+    """
+    Environment error with public message. Exceptions of this type raised
+    under `prefix_stack_trace` or `print_prefixed_stack_trace_and_raise` will
+    have the message prefixed with `PREFIX` in both the printed stack trace and
+    the re-raised exception.
+    """
+
+
+class PublicImportError(ImportError):
+    """
+    Import error with public message. Exceptions of this type raised
+    under `prefix_stack_trace` or `print_prefixed_stack_trace_and_raise` will
+    have the message prefixed with `PREFIX` in both the printed stack trace and
+    the re-raised exception.
+    """
+
+
+class PublicStopIteration(StopIteration):
+    """
+    Stop iteration error with public message. Exceptions of this type raised
+    under `prefix_stack_trace` or `print_prefixed_stack_trace_and_raise` will
+    have the message prefixed with `PREFIX` in both the printed stack trace and
+    the re-raised exception.
+    """
+
+
+class PublicSystemError(SystemError):
+    """
+    System error with public message. Exceptions of this type raised
+    under `prefix_stack_trace` or `print_prefixed_stack_trace_and_raise` will
+    have the message prefixed with `PREFIX` in both the printed stack trace and
+    the re-raised exception.
+    """
+
+
+class PublicDeprecationWarning(DeprecationWarning):
+    """
+    Deprecation warning with public message. Exceptions of this type raised
+    under `prefix_stack_trace` or `print_prefixed_stack_trace_and_raise` will
+    have the message prefixed with `PREFIX` in both the printed stack trace and
+    the re-raised exception.
+    """
+
+
 default_allow_list = [
     PublicValueError.__name__,
     PublicRuntimeError.__name__,
     PublicArgumentError.__name__,
+    PublicArgumentTypeError.__name__,
     PublicKeyError.__name__,
     PublicTypeError.__name__,
     PublicIndexError.__name__,
     PublicNotImplementedError.__name__,
     PublicFileNotFoundError.__name__,
     PublicIOError.__name__,
+    PublicEnvironmentError.__name__,
+    PublicImportError.__name__,
+    PublicStopIteration.__name__,
+    PublicSystemError.__name__,
+    PublicDeprecationWarning.__name__,
 ]
 
 
 def _attribute_transformer(prefix: str, scrub_message: str, keep: bool) -> Callable:
     """
     Create a function which may be used to transform exception attributes.
 
-    If an attribute is string-valued, apply the logic keep? prefix + attr: prefix
+    If an attribute is string-valued or int-valued,
+    apply the logic keep? prefix + attr: prefix
     + scrub_message.
 
     If the attribute is iterable, apply this logic to each member of the
     attribute.
 
     If the attribute is callable, don't change it.
 
@@ -135,14 +197,17 @@
     def inner(o):
         rv = o
         if isinstance(o, str):
             if keep:
                 rv = prefix + o
             else:
                 rv = prefix + scrub_message
+        elif isinstance(o, int):
+            # handling SystemExit
+            rv = inner(str(o))
         elif isinstance(o, Iterable):
             rv = type(o)(map(inner, o))  # type: ignore
         elif callable(o):
             rv = rv
         elif not keep:
             rv = None
 
@@ -197,38 +262,39 @@
             allow_list,
             _seen,
         )
 
     keep = keep_message or is_exception_allowed(exception, allow_list)
     transformer = _attribute_transformer(prefix, scrub_message, keep)
 
-    for attr in dir(exception):
-        if attr and not attr.startswith("__"):
-            try:
-                value = getattr(exception, attr)
-            except AttributeError:
-                # In some cases, e.g. FileNotFoundError, there are attributes
-                # which show up in dir(e), but for which an AttributeError is
-                # thrown when attempting to access the value. See, e.g.:
-                # https://stackoverflow.com/q/47775772 .
-                continue
-            try:
-                # If unable to transform or set the attribute, replace the
-                # entire exception since the attribute value is readable, but
-                # we are unable to scrub it.
-                new_value = transformer(value)
-                setattr(exception, attr, new_value)
-            except BaseException as e:
-                new_exception = PublicRuntimeError(
-                    f"{prefix} Obtained {type(e).__name__} when trying to scrub {attr} from {type(exception).__name__}"  # noqa: E501
-                )
-                new_exception.__cause__ = exception.__cause__
-                new_exception.__context__ = exception.__context__
-                exception = new_exception
-                break
+    if not keep:
+        for attr in dir(exception):
+            if attr and not attr.startswith("__"):
+                try:
+                    value = getattr(exception, attr)
+                except AttributeError:
+                    # In some cases, e.g. FileNotFoundError, there are attributes
+                    # which show up in dir(e), but for which an AttributeError is
+                    # thrown when attempting to access the value. See, e.g.:
+                    # https://stackoverflow.com/q/47775772 .
+                    continue
+                try:
+                    # If unable to transform or set the attribute, replace the
+                    # entire exception since the attribute value is readable, but
+                    # we are unable to scrub it.
+                    new_value = transformer(value)
+                    setattr(exception, attr, new_value)
+                except BaseException as e:
+                    new_exception = PublicRuntimeError(
+                        f"{prefix} Obtained {type(e).__name__} when trying to scrub {attr} from {type(exception).__name__}"  # noqa: E501
+                    )
+                    new_exception.__cause__ = exception.__cause__
+                    new_exception.__context__ = exception.__context__
+                    exception = new_exception
+                    break
 
     return exception
 
 
 def is_exception_allowed(
     exception: Union[BaseException, TracebackException], allow_list: list
 ) -> bool:
@@ -270,17 +336,23 @@
     Args:
         keep_message (bool): if True, don't scrub message. If false, scrub (unless
             allowed).
         allow_list (list): exception allow_list. Ignored if keep_message is True. If
             empty all messages will be srubbed.
         err: the error that was thrown. None accepted for backwards compatibility.
     """
+    global LATEST_EXCEPTION
     if err is None:
         err = sys.exc_info()[1]
-    scrubbed_err = scrub_exception(err, scrub_message, prefix, keep_message, allow_list)
+    scrubbed_err = err
+    if err != LATEST_EXCEPTION:
+        scrubbed_err = scrub_exception(
+            err, scrub_message, prefix, keep_message, allow_list
+        )
+        LATEST_EXCEPTION = err
 
     tb_exception = TracebackException.from_exception(scrubbed_err)  # type: ignore
 
     for execution in tb_exception.format():
         if "return function(*func_args, **func_kwargs)" in execution:
             # Do not show the stack trace for our decorator.
             continue
@@ -364,15 +436,14 @@
     scrubbed (replaced with `scrub_message`). To use this, just add
     `@prefix_stack_trace()` above your function definition, e.g.
 
         @prefix_stack_trace()
         def foo(x):
             pass
     """
-
     return _PrefixStackTraceWrapper(
         file, disable, prefix, scrub_message, keep_message, allow_list, add_timestamp
     )
 
 
 class PrefixStackTrace:
     def __init__(
```

### Comparing `shrike-1.9.5/shrike/compliant_logging/logging.py` & `shrike-2.0.0.dev0/shrike/compliant_logging/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,44 +22,85 @@
     get_pandas_dataframe_info,
     get_pandas_series_info,
     get_spark_dataframe_info,
     get_vaex_dataframe_info,
     numpy_array_to_list,
     pandas_series_to_list,
 )
+from shrike._core import is_eyesoff_helper
 from datetime import datetime
 import logging
 import sys
+import os
 from threading import Lock
-
+from azureml.exceptions import ServiceException
 
 _LOCK = Lock()
 _PREFIX = None
+_SCRUB_MESSAGE = "**Log message scrubbed**"
+_SCRUB_LOGGING = False
 _AML_RUN = None
 
 
+def set_scrubbed_logging(value: bool) -> None:
+    """
+    Set the global scrubbed logging functionality settings.
+
+    This method is thread-safe.
+    """
+    with _LOCK:
+        global _SCRUB_LOGGING
+        _SCRUB_LOGGING = value
+
+
 def set_prefix(prefix: str) -> None:
     """
-    Set the global prefix to use when logging public (non-private) data.
+    Set the global prefix to use when logging data.
 
     This method is thread-safe.
     """
     with _LOCK:
         global _PREFIX
         _PREFIX = prefix
 
 
+def set_scrub_message(scrub_message: str) -> None:
+    """
+    Set the global scrub message to use when logging private (non-public) data.
+
+    This method is thread-safe.
+    """
+    with _LOCK:
+        global _SCRUB_MESSAGE
+        # Make the passed in value string as dditional safety measure
+        _SCRUB_MESSAGE = str(scrub_message)
+
+
+def get_scrubbed_logging() -> bool:
+    """
+    Obtain the current global scrubbed logging functionality settings.
+    """
+    return _SCRUB_LOGGING
+
+
 def get_prefix() -> Optional[str]:
     """
-    Obtain the current global prefix to use when logging public (non-private)
-    data.
+    Obtain the current global prefix to use when logging data.
     """
     return _PREFIX
 
 
+def get_scrub_message() -> str:
+    """
+    Obtain the current global scrub message to use when logging private (non-public)
+    data.
+    """
+    return _SCRUB_MESSAGE
+
+
 def set_aml_context() -> None:
     """
     Retrieves the AML Context, should be bundled in a try-catch.
     """
     global _AML_RUN
     from azureml.core.run import Run
 
@@ -95,30 +136,33 @@
 
     The default value for data `category` is `PRIVATE` for all methods.
 
     Implementation is inspired by:
     https://github.com/python/cpython/blob/3.8/Lib/logging/__init__.py
     """
 
-    def __init__(self, name: str, use_aml_metrics: bool = False):
+    def __init__(self, name: str, use_aml_metrics: bool = False, handlers=None):
         super().__init__(name)  # type: ignore
+
+        if handlers:
+            self.handlers = handlers
+
         self.start_time = datetime.now()
         self.metric_count = 1
         # number of iterable items that are logged
         self.max_iter_items = 10
 
         # check for azure context
         if use_aml_metrics:
             run = get_aml_context()
             if run is None:
                 try:
                     set_aml_context()
                     self.info(
-                        "AML Metrics:"
-                        + f"{get_aml_context().get_status()}",  # type: ignore
+                        "AML Metrics:" + f"{get_aml_context().id}",  # type: ignore
                         category=DataCategory.PUBLIC,
                     )
                 except Exception:
                     self.warning(
                         "AML writer failed to initialize.", category=DataCategory.PUBLIC
                     )
 
@@ -201,17 +245,25 @@
         exc_info=None,
         extra=None,
         stack_info=False,
         stacklevel=1,
         items=None,
         category=DataCategory.PRIVATE,
     ):
-        p = ""
-        if category == DataCategory.PUBLIC:
+        if not get_scrubbed_logging() and category == DataCategory.PRIVATE:
+            p = ""
+        else:
             p = get_prefix()
+
+        if get_scrubbed_logging() and category == DataCategory.PRIVATE:
+            msg = get_scrub_message()
+            items = None
+            stack_info = False
+            exc_info = None
+
         if extra:
             extra.update({"prefix": p})
         else:
             extra = {"prefix": p}
 
         # update message accordingly to items
         if items is not None:
@@ -282,31 +334,31 @@
 
         # retrieve AML Context
         run = self._get_aml_context()
 
         # check if value provided
         if value is None:
             self.error(
-                f"Value provided for metric {name} is None, skipping (step: {step})"
+                f"Value provided for metric {name} is None, skipping (step: {step})",
+                category=category,
             )
             return
 
         # check different data-types
         if isinstance(value, (float, int)):
             # log the data
             if run is not None and category == DataCategory.PUBLIC:
                 if step:
                     run.log(name=name, value=value, description=description, step=step)
                 else:
                     run.log(name=name, value=value, description=description)
-            else:
-                self.info(
-                    f"NumbericMetric  | {name}:{step} | {value}",
-                    category=category,
-                )
+            self.info(
+                f"NumbericMetric  | {name}:{step} | {value}",
+                category=category,
+            )
 
             return
 
         # collect dataframes
         if is_vaex_dataframe(value):
             value = collect_vaex_dataframe(value)
         elif is_spark_dataframe(value):
@@ -314,15 +366,18 @@
         elif is_pandas_dataframe(value):
             value = collect_pandas_dataframe(value)
 
         # log dictionary data
         if isinstance(value, dict):
             # check if values are present
             if len(value) == 0:
-                self.warning(f"Dictionary Value for Metric {name} is empty. Skipping.")
+                self.warning(
+                    f"Dictionary Value for Metric {name} is empty. Skipping.",
+                    category=category,
+                )
                 return
 
             # check the value types of the dict
             type_set = list(set([type(v) for v in value.values()]))
 
             # check for mixed types
             if len(type_set) > 1:
@@ -330,33 +385,32 @@
             else:
                 type_set = type_set[0]
 
             # check types
             if type_set == list:
                 if run is not None and category == DataCategory.PUBLIC:
                     run.log_table(name, value, description)
-                else:
-                    # log the matrix manually
-                    col_names = " | ".join(
-                        [f"{('' if col is None else col):15}" for col in value.keys()]
-                    )
-                    header = f"TableMetric     | Index | {col_names} |"
-                    self.info(f"TableMetric     | {name}", category=category)
-                    self.info(header, category=category)
-                    self.info("-" * len(header), category=category)
-
-                    # generate the rows
-                    max_rows = max([len(value[col]) for col in value])
-                    for i in range(max_rows):
-                        row_str = f"TableMetric     | {i:05}"
-                        for key in value:
-                            col = value[key]
-                            col = col[i] if i < len(col) and col[i] else ""
-                            row_str += f" | {str(col):15}"
-                        self.info(row_str, category=category)
+                # log the matrix manually
+                col_names = " | ".join(
+                    [f"{('' if col is None else col):15}" for col in value.keys()]
+                )
+                header = f"TableMetric     | Index | {col_names} |"
+                self.info(f"TableMetric     | {name}", category=category)
+                self.info(header, category=category)
+                self.info("-" * len(header), category=category)
+
+                # generate the rows
+                max_rows = max([len(value[col]) for col in value])
+                for i in range(max_rows):
+                    row_str = f"TableMetric     | {i:05}"
+                    for key in value:
+                        col = value[key]
+                        col = col[i] if i < len(col) and col[i] is not None else ""
+                        row_str += f" | {str(col):15}"
+                    self.info(row_str, category=category)
             elif type_set in [int, float]:
                 for key, val in value.items():
                     key = name + "/" + key
                     self.metric(val, step, key, description, category)
             else:
                 self.warning(
                     (
@@ -376,22 +430,24 @@
 
         # log list data
         if isinstance(value, (list, tuple)):
             value = list(value)
 
             # check if values are present
             if len(value) == 0:
-                self.warning(f"List Value for Metric {name} is empty. Skipping.")
+                self.warning(
+                    f"List Value for Metric {name} is empty. Skipping.",
+                    category=category,
+                )
                 return
 
             # log data to run context
             if run is not None and category == DataCategory.PUBLIC:
                 run.log_list(name=name, value=value, description=description)
-            else:
-                self.info(f"ListMetric      | {name} | {value}")
+            self.info(f"ListMetric      | {name} | {value}", category=category)
 
             return
 
         self.warning(
             f"Value {value} of the provided metric {name} has an unkown type",
             category=category,
         )
@@ -439,28 +495,43 @@
                 Defaults to DataCategory.PRIVATE.
         """
         # retrieve the run context
         run = self._get_aml_context()
 
         # check if parameters are correct
         if category != DataCategory.PUBLIC:
-            self.warning(f"Unable to log image metric {name} as private, skipping.")
+            self.warning(
+                f"Unable to log image metric {name} as private, skipping.",
+                category=DataCategory.PUBLIC,
+            )
+            return
+        elif run is None:
+            self.warning(
+                f"Unable to log image metric {name} without AML Run Context, skipping.",
+                category=category,
+            )
             return
 
         # check for name
         if name is None:
             name = f"metric_{self.metric_count}"
             self.metric_count += 1
         if description is None:
             description = ""
 
         # log the image
-        run.log_image(  # type: ignore
-            name=name, path=path, plot=plot, description=description
-        )
+        try:
+            run.log_image(  # type: ignore
+                name=name, path=path, plot=plot, description=description
+            )
+        except ServiceException:
+            self.warning(
+                "log_image is not available for detonation chamber, skipping.",
+                category=category,
+            )
 
     def metric_list(self, name, value, description=None, category=DataCategory.PRIVATE):
         """
         Equivalent to the `Run.log_list`.
         Logs a list of values for a single metric.
 
         Note: Private Data will not be send to metrics!
@@ -622,15 +693,18 @@
                     + "correct data is passed."
                 )
 
         # log the data
         if category == DataCategory.PUBLIC and run is not None:
             run.log_accuracy_table(name, value, description)
         else:
-            self.warning("Logging Accuracy Tables to text is not yet implemented")
+            self.warning(
+                "Logging Accuracy Tables to text is not yet implemented",
+                category=DataCategory.PUBLIC,
+            )
 
     def metric_confusion_matrix(
         self,
         name,
         value,
         idx_true=None,
         idx_pred=None,
@@ -721,15 +795,18 @@
                     + "data is passed."
                 )
 
         # log the data
         if category == DataCategory.PUBLIC and run is not None:
             run.log_confusion_matrix(name, value, description)
         else:
-            self.warning("Logging Confusion Matrices to text is not yet implemented")
+            self.warning(
+                "Logging Confusion Matrices to text is not yet implemented",
+                category=DataCategory.PUBLIC,
+            )
 
     def metric_predictions(
         self,
         name,
         value,
         description=None,
         col_predict=None,
@@ -821,15 +898,18 @@
                     + "data is passed."
                 )
 
         # log the data
         if category == DataCategory.PUBLIC and run is not None:
             run.log_predictions(name, value, description)
         else:
-            self.warning("Logging Predictions to text is not yet implemented")
+            self.warning(
+                "Logging Predictions to text is not yet implemented",
+                category=DataCategory.PUBLIC,
+            )
 
     def metric_residual(
         self,
         name,
         value,
         description=None,
         col_predict=None,
@@ -918,15 +998,18 @@
                     + "data is passed."
                 )
 
         # log the data
         if category == DataCategory.PUBLIC and run is not None:
             run.log_residuals(name, value, description)
         else:
-            self.warning("Logging Residuals to text is not yet implemented")
+            self.warning(
+                "Logging Residuals to text is not yet implemented",
+                category=DataCategory.PUBLIC,
+            )
 
     def metric_row(
         self, name, description=None, category=DataCategory.PRIVATE, **kwargs
     ):
         """
         Equivalent of the `Run.log_row` function.
         Logs a single row of a table to the metrics.
@@ -941,18 +1024,17 @@
         """
         # check run context
         run = self._get_aml_context()
 
         # log the data
         if category == DataCategory.PUBLIC and run is not None:
             run.log_row(name=name, description=description, **kwargs)
-        else:
-            row_str = f"RowMetric      | {name} | "
-            row_str += " | ".join([f"{r}:{c}" for r, c in kwargs.items()])
-            self.info(row_str, category=category)
+        row_str = f"RowMetric      | {name} | "
+        row_str += " | ".join([f"{r}:{c}" for r, c in kwargs.items()])
+        self.info(row_str, category=category)
 
     def metric_table(
         self, name, value, description=None, category=DataCategory.PRIVATE
     ):
         """
         Equivalent to the `Run.log_table` function.
         Logs a table in dict format {rows: [values]} to metrics.
@@ -965,27 +1047,48 @@
             description (str, optional): Description of the metric. Defaults to None.
             category (DataCategory, optional): Category to log the data.
                 Default to DataCategory.PRIVATE.
         """
         self.metric(value=value, name=name, description=description, category=category)
 
 
+def is_eyesoff() -> bool:
+    """
+    Returns a boolean of whether current workspace is eyes-off.
+    First check if the user-defined "EYESOFF_ENV" environment variable is provided.
+    """
+    if os.environ.get("EYESOFF_ENV", ""):
+        print(
+            "SystemLog: WARNING: you are manually setting the environment via `EYESOFF_ENV`. \
+            Please be cautious as incorrect settings could cause privacy incidents."
+        )
+        return os.environ.get("EYESOFF_ENV", "").lower() == "true"
+    else:
+        tenant_id = os.environ.get("AZ_BATCHAI_CLUSTER_TENANT_ID", "")
+        subscription_id = os.environ.get("AZUREML_ARM_SUBSCRIPTION", "")
+        return is_eyesoff_helper(tenant_id, subscription_id)
+
+
 _logging_basic_config_set_warning = """
 ********************************************************************************
 The root logger already has handlers set! As a result, the behavior of this
 library is undefined. If running in Python >= 3.8, this library will attempt to
 call logging.basicConfig(force=True), which will remove all existing root
 handlers. See https://stackoverflow.com/q/20240464 and
 https://github.com/Azure/confidential-ml-utils/issues/33 for more information.
 ********************************************************************************
 """
 
 
 def enable_compliant_logging(
-    prefix: str = "SystemLog:", use_aml_metrics: bool = False, **kwargs
+    prefix: str = "SystemLog:",
+    scrub_message: str = "**Log message scrubbed**",
+    use_aml_metrics: bool = False,
+    enable_scrubbed_logging: bool = False,
+    **kwargs,
 ) -> None:
     """
     The default format is `logging.BASIC_FORMAT` (`%(levelname)s:%(name)s:%(message)s`).
     All other kwargs are passed to `logging.basicConfig`. Sets the default
     logger class and root logger to be compliant. This means the format
     string `%(prefix)` will work.
 
@@ -999,14 +1102,18 @@
     if no changes are made to an existing set of log statements, the log output
     should be the same.
 
     The standard implementation of the logging API is a good reference:
     https://github.com/python/cpython/blob/3.9/Lib/logging/__init__.py
     """
     set_prefix(prefix)
+    set_scrub_message(scrub_message)
+
+    if enable_scrubbed_logging:
+        set_scrubbed_logging(True)
 
     if "format" not in kwargs:
         kwargs["format"] = f"%(prefix)s{logging.BASIC_FORMAT}"
 
     # Ensure that all loggers created via `logging.getLogger` are instances of
     # the `CompliantLogger` class.
     logging.setLoggerClass(CompliantLogger)
@@ -1015,33 +1122,38 @@
         p = get_prefix()
         for line in _logging_basic_config_set_warning.splitlines():
             print(f"{p}{line}", file=sys.stderr)
 
     if "force" not in kwargs and sys.version_info >= (3, 8):
         kwargs["force"] = True
 
-    old_root = logging.root
-
-    root = CompliantLogger(logging.root.name, use_aml_metrics)
-    root.handlers = old_root.handlers
+    root = CompliantLogger(
+        logging.root.name, use_aml_metrics, handlers=logging.root.handlers
+    )
 
     logging.root = root
     logging.Logger.root = root  # type: ignore
     logging.Logger.manager = logging.Manager(root)  # type: ignore
 
     # https://github.com/kivy/kivy/issues/6733
     logging.basicConfig(**kwargs)
 
 
 def enable_confidential_logging(
-    prefix: str = "SystemLog:", use_aml_metrics: bool = False, **kwargs
+    prefix: str = "SystemLog:",
+    scrub_message: str = "**Log message scrubbed**",
+    use_aml_metrics: bool = False,
+    enable_scrubbed_logging: bool = False,
+    **kwargs,
 ) -> None:
     """
     This function is a duplicate of the function `enable_compliant_logging`.
     We encourage users to use `enable_compliant_logging`.
     """
     print(
         f"{prefix} The function enable_confidential_logging() is on the way"
         " to deprecation. Please use enable_compliant_logging() instead.",
         file=sys.stderr,
     )
-    enable_compliant_logging(prefix, use_aml_metrics, **kwargs)
+    enable_compliant_logging(
+        prefix, scrub_message, use_aml_metrics, enable_scrubbed_logging, **kwargs
+    )
```

### Comparing `shrike-1.9.5/shrike/compliant_logging/stack_trace_extractor.py` & `shrike-2.0.0.dev0/shrike/compliant_logging/stack_trace_extractor.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.5/shrike/compliant_logging/system_info.py` & `shrike-2.0.0.dev0/shrike/compliant_logging/system_info.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.5/shrike/pipeline/aml_connect.py` & `shrike-2.0.0.dev0/shrike/pipeline/v1/aml_connect.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
-""" Helper code for connecting to AzureML and sharing one workspace accross code. """
-import os
-import argparse
+"""
+Helper code for connecting to AzureML and sharing one workspace accross code.
+"""
+
 
-from azureml.core import Workspace
+import argparse
+from azureml.core import Workspace, Run
 from collections import namedtuple
+import logging
+import os
+
+
+log = logging.getLogger(__name__)
+
 
 CURRENT_AML_WORKSPACE = None
 
 
 def current_workspace(workspace=None):
     """Sets/Gets the current AML workspace used all accross code.
 
@@ -66,15 +74,15 @@
         help="path to aml config.json file",
     )
 
     parser.add_argument(
         "--aml-auth",
         dest="aml_auth",
         type=str,
-        choices=["azurecli", "msi", "interactive"],
+        choices=["azurecli", "msi", "interactive", "aml_job"],
         default="interactive",
     )
     parser.add_argument(
         "--aml-tenant",
         dest="aml_tenant",
         type=str,
         default=None,
@@ -134,51 +142,50 @@
 
         auth = InteractiveLoginAuthentication(
             tenant_id=args.aml_tenant, force=args.aml_force
         )
     else:
         auth = None
 
-    if args.aml_config:
+    if args.aml_auth == "aml_job":
+        aml_ws = Run.get_context().experiment.workspace
+    elif args.aml_config:
         config_dir = os.path.dirname(args.aml_config)
         config_file_name = os.path.basename(args.aml_config)
 
         aml_ws = Workspace.from_config(
             path=config_dir, _file_name=config_file_name, auth=auth
         )
     else:
         aml_ws = Workspace.get(
             subscription_id=args.aml_subscription_id,
             name=args.aml_workspace_name,
             resource_group=args.aml_resource_group,
             auth=auth,
         )
 
-    print(
-        "Connected to Workspace",
-        "-- subscription:" + aml_ws.subscription_id,
-        "-- name: " + aml_ws.name,
-        "-- Azure region: " + aml_ws.location,
-        "-- Resource group: " + aml_ws.resource_group,
-        sep="\n",
-    )
+    log.info("Connected to workspace:")
+    log.info(f"\tsubscription: {aml_ws.subscription_id}")
+    log.info(f"\tname: {aml_ws.name}")
+    log.info(f"\tAzure region: {aml_ws.location}")
+    log.info(f"\tresource group: {aml_ws.resource_group}")
 
     return current_workspace(aml_ws)
 
 
 def main():
     """Main function (for testing)"""
     parser = argparse.ArgumentParser(description=__doc__)
 
     group = parser.add_argument_group("AzureML connect arguments")
     add_cli_args(group)
 
     args, unknown_args = parser.parse_known_args()
 
     if unknown_args:
-        print("WARNING: you have provided unknown arguments {}".format(unknown_args))
+        log.warning(f"You have provided unknown arguments {unknown_args}")
 
     return azureml_connect_cli(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shrike-1.9.5/shrike/pipeline/canary_helper.py` & `shrike-2.0.0.dev0/shrike/pipeline/canary_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
 """
 Canary helper code
 """
-import os
 
-from azureml.core.workspace import Workspace
+
 from azureml.core import Dataset
 from azureml.data.datapath import DataPath
+import logging
+
+
+log = logging.getLogger(__name__)
 
 
 def get_repo_info():
     """[EXPERIMENTAL] Obtains info on the current repo the code is in.
 
     Returns:
         dict: git meta data"""
@@ -22,15 +25,17 @@
         repo = git.Repo(search_parent_directories=True)
         branch = repo.active_branch
         head = repo.head
         return {
             "git": repo.remotes.origin.url,
             "branch": branch.name,
             "commit": head.commit.hexsha,
-            "last_known_author": head.commit.author.name,
+            "last_known_author": head.commit.author.name.encode(
+                "ascii", "ignore"
+            ).decode(),
         }
     except:
         return {"git": "n/a"}
 
 
 def test_pipeline_step_metrics(pipeline_run, expected_metrics):
     """Tests a pipeline run against a set of expected metrics.
@@ -49,29 +54,29 @@
         tests module "SelectJsonField" for a metric row named "output", checks key "size" must have value 369559
 
         "tokenizerparallel" : [{"metric" : {"key" : "Failed Items", "value" : 0}}],
         tests module "tokenizerparallel" for a metric named "Failed Items", value must be 0
     """
     errors = []
 
-    print("Looping through PipelineRun steps to test metrics...")
+    log.info("Looping through PipelineRun steps to test metrics...")
     for step in pipeline_run.get_steps():
-        print(f"Checking status of step {step.name}...")
+        log.info(f"Checking status of step {step.name}...")
 
         observed_metrics = step.get_metrics()
-        print(f"Step Metrics: {observed_metrics}")
+        log.info(f"Step Metrics: {observed_metrics}")
 
         status = step.get_status()
         if status != "Finished":
             errors.append(f"Pipeline step {step.name} status is {status} != Finished")
 
         if step.name in expected_metrics:
             for expected_metric_test in expected_metrics[step.name]:
                 if "row" in expected_metric_test:
-                    print(f"Checking metrics, looking for {expected_metric_test}")
+                    log.info(f"Checking metrics, looking for {expected_metric_test}")
                     row_key = expected_metric_test["row"]["name"]
                     metric_key = expected_metric_test["row"]["key"]
                     expected_value = expected_metric_test["row"]["value"]
                     if row_key not in observed_metrics:
                         errors.append(
                             f"Step {step.name} metric row '{row_key}' not available in observed metrics {observed_metrics}"
                         )
@@ -80,15 +85,15 @@
                             f"Step {step.name} metric row '{row_key}' does not have a metric '{metric_key}' in observed metrics {observed_metrics[row_key]}"
                         )
                     elif observed_metrics[row_key][metric_key] != expected_value:
                         errors.append(
                             f"Step {step.name} metric row '{row_key}' - metric '{metric_key}' - does not have expected value {expected_value} in observed metrics {observed_metrics[row_key]}"
                         )
                 if "metric" in expected_metric_test:
-                    print(f"Checking metrics, looking for {expected_metric_test}")
+                    log.info(f"Checking metrics, looking for {expected_metric_test}")
                     metric_key = expected_metric_test["metric"]["key"]
                     expected_value = expected_metric_test["metric"]["value"]
                     if metric_key not in observed_metrics:
                         errors.append(
                             f"Step {step.name} metric '{metric_key}' not available in observed metrics {observed_metrics}"
                         )
                     elif observed_metrics[metric_key] != expected_value:
@@ -136,15 +141,15 @@
         datastore=data_reference.datastore,
         path_on_datastore=data_reference.path_on_datastore,
         name=data_reference.data_reference_name,
     )
 
     if kwargs.get("length"):
         expected_length = kwargs.get("length")
-        print(
+        log.info(
             f"Checking count={expected_length} of files for step {step_name} output {output_name}..."
         )
         data_set = Dataset.File.from_files(data_path)
 
         files_list = data_set.to_path()
 
         if expected_length < 0:
```

### Comparing `shrike-1.9.5/shrike/pipeline/module_helper.py` & `shrike-2.0.0.dev0/shrike/pipeline/module_helper_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
 """
 Pipeline helper class to create pipelines loading modules from a flexible manifest.
 """
+from abc import abstractmethod, ABC
+from dataclasses import dataclass, field
 import os
+import logging
+from typing import Optional, List, Tuple
 
-from azure.ml.component import Component
-
-from shrike.pipeline.aml_connect import current_workspace
-
-from dataclasses import dataclass, field
-from omegaconf import MISSING
-from typing import Optional, List
-from enum import Enum
+log = logging.getLogger(__name__)
 
 
 @dataclass
 class module_reference:
     key: Optional[
         str
     ] = None  # use as internal key to reference module (if None, use name)
     name: Optional[str] = None  # None if module exists only locally?
-    source: Optional[str] = "registered"  # or "local"
+    source: Optional[str] = None  # This config is deprecated. Please do not use.
     yaml: Optional[str] = None
     version: Optional[str] = None
+    from_workspace: Optional[
+        bool
+    ] = False  # If set to True and it's a remote component, shrike will only attempt to load it from workspace (not from registry or feed)
 
 
 @dataclass
 class module_manifest:
     manifest: List[module_reference] = field(default_factory=list)
+    feeds: List[str] = field(default_factory=list)
+    registries: List[str] = field(default_factory=list)
 
 
 @dataclass
 class module_loader_config:  # pylint: disable=invalid-name
     """Config for the AMLModuleLoader class"""
 
     use_local: Optional[str] = None
@@ -47,17 +49,19 @@
             "..",
             "tests",
             "tests_pipeline",
             "sample",
             "steps",
         )
     )
+    use_remote_when_component_not_in_manifest: Optional[bool] = False
+    loading_order: Optional[str] = "registry, feed, workspace"
 
 
-class AMLModuleLoader:
+class AMLModuleLoaderBase(ABC):
     """Helper class to load modules from within an AMLPipelineHelper."""
 
     def __init__(self, config):
         """Creates module instances for AMLPipelineHelper.
 
         Args:
             config (DictConfig): configuration options
@@ -73,15 +77,15 @@
             self.use_local = []
         elif config.module_loader.use_local == "*":
             self.use_local = "*"
         elif isinstance(config.module_loader.use_local, str):
             self.use_local = [
                 x.strip() for x in config.module_loader.use_local.split(",")
             ]
-            if not _check_use_local_syntax_valid(self.use_local):
+            if not self._check_use_local_syntax_valid(self.use_local):
                 raise ValueError(
                     f'Invalid value for `use_local`. Please follow one of the four patterns: \n1) use_local="", all modules are remote\n2) use_local="*", all modules are local\n3) use_local="MODULE_KEY_1, MODULE_KEY_2", only MODULE_KEY_1, MODULE_KEY_2 are local, everything else is remote\n4) use_local="!MODULE_KEY_1, !MODULE_KEY_2", all except for MODULE_KEY_1, MODULE_KEY_2 are local'
                 )
             self.use_local_except_for = self.use_local[0].startswith("!")
 
         self.force_default_module_version = (
             config.module_loader.force_default_module_version
@@ -90,23 +94,72 @@
         )
         self.force_all_module_version = (
             config.module_loader.force_all_module_version
             if "force_all_module_version" in config.module_loader
             else None
         )
         self.local_steps_folder = config.module_loader.local_steps_folder
+        self.use_remote_when_component_not_in_manifest = (
+            config.module_loader.use_remote_when_component_not_in_manifest
+            if "use_remote_when_component_not_in_manifest" in config.module_loader
+            else None
+        )
         self.module_cache = {}
 
+        self.feeds: List[str] = []
+        self.registries: List[str] = []
+
+        self.loading_order = (
+            [x.strip().lower() for x in config.module_loader.loading_order.split(",")]
+            if "loading_order" in config.module_loader
+            else ["registry", "feed", "workspace"]
+        )
+
         # internal manifest built from yaml config
         self.modules_manifest = {}
         self.load_config_manifest(config)
 
-        print(
-            f"AMLModuleLoader initialized (use_local={self.use_local}, force_default_module_version={self.force_default_module_version}, force_all_module_version={self.force_all_module_version}, local_steps_folder={self.local_steps_folder}, manifest={list(self.modules_manifest.keys())})"
+        initialization_info_string = (
+            "AMLModuleLoader initialized ("
+            f"use_local={self.use_local}"
+            f", force_default_module_version={self.force_default_module_version}"
+            f", force_all_module_version={self.force_all_module_version}"
+            f", local_steps_folder={self.local_steps_folder}"
+            f", use_remote_when_component_not_in_manifest={self.use_remote_when_component_not_in_manifest}"
+            f", manifest={list(self.modules_manifest.keys())}"
+            f", loading_order={self.loading_order}"
+            ")"
         )
+        log.info(initialization_info_string)
+
+    @abstractmethod
+    def load_local_module(self, module_spec_path):
+        """Creates one module instance.
+
+        Args:
+            module_spec_path (str): path to local module yaml spec
+
+        Returns:
+            object: module class loaded
+        """
+        pass
+
+    @abstractmethod
+    def solve_module_version_and_load(
+        self, module_name, module_version, module_cache_key, registry=None
+    ):
+        """Loads module class if exists
+
+        Args:
+            module_name (str): name of the module to load
+            module_version (str): version of the module to load
+            module_cache_key (str): cache key of the module after loading
+            registy (str): registry name if loading from a registry
+        """
+        pass
 
     def load_config_manifest(self, config):
         """Fills the internal module manifest based on config object"""
         for entry in config.modules.manifest:
             if entry.key:
                 module_key = entry.key
             elif entry.name:
@@ -114,14 +167,20 @@
             else:
                 raise Exception(
                     "In module manifest, you have to provide at least key or name."
                 )
 
             self.modules_manifest[module_key] = entry
 
+        for feed in config.modules.get("feeds", []):
+            self.feeds.append(feed)
+
+        for registry in config.modules.get("registries", []):
+            self.registries.append(registry)
+
     def is_local(self, module_name):
         """Tests is module is in local list"""
         if self.use_local == "*":
             return True
         if self.use_local_except_for:
             return "!" + module_name not in self.use_local
         else:
@@ -129,26 +188,26 @@
 
     def module_in_cache(self, module_cache_key):
         """Tests if module in internal cache (dict)"""
         return module_cache_key in self.module_cache
 
     def get_from_cache(self, module_cache_key):
         """Gets module class from internal cache (dict)"""
-        print(f"--- Using cached module {module_cache_key}")
+        log.debug(f"Using cached module {module_cache_key}")
         return self.module_cache.get(module_cache_key, None)
 
     def put_in_cache(self, module_cache_key, module_class):
         """Puts module class in internal cache (dict)"""
         self.module_cache[module_cache_key] = module_class
 
     def verify_manifest(self, modules_manifest):
         """Tests a module manifest schema"""
         errors = []
 
-        for (k, module_entry) in modules_manifest.items():
+        for k, module_entry in modules_manifest.items():
             # TODO: merge error checking code with processing code so we do all this in one pass
             if self.is_local(k):
                 if "yaml_spec" not in module_entry:
                     errors.append(
                         f"{k}: You need to specify a yaml_spec for your module to use_local=['{k}']"
                     )
                 elif not os.path.isfile(
@@ -175,172 +234,274 @@
                 ):
                     errors.append(
                         f"{k}: You need to specify a version for your module to use_local=False, or use either force_default_module_version or force_all_module_version in config"
                     )
 
         return errors
 
+    @abstractmethod
+    def load_local_module_helper(self, module_spec_path):
+        """Calls SDK to load a local component.
+
+        Args:
+            module_spec_path (str): path to local module yaml spec
+
+        Returns:
+            object: module class loaded"""
+        pass
+
     def load_local_module(self, module_spec_path):
         """Creates one module instance.
 
         Args:
             module_spec_path (str): path to local module yaml spec
 
         Returns:
             object: module class loaded
         """
         module_cache_key = module_spec_path
         if self.module_in_cache(module_cache_key):
             return self.get_from_cache(module_cache_key)
 
-        print("--- Building module from local code at {}".format(module_spec_path))
+        log.info("Building module from local code at {}".format(module_spec_path))
         if not os.path.isfile(module_spec_path):
             module_spec_path = os.path.join(self.local_steps_folder, module_spec_path)
-        loaded_module_class = Component.from_yaml(current_workspace(), module_spec_path)
+        loaded_module_class = self.load_local_module_helper(module_spec_path)
         self.put_in_cache(module_cache_key, loaded_module_class)
 
         return loaded_module_class
 
-    def load_prod_module(self, module_name, module_version, module_namespace=None):
+    def load_prod_module_helper(
+        self,
+        module_name,
+        module_version,
+        module_cache_key,
+        module_namespace=None,
+        loading_order=None,
+    ):
+        """Loads module from available sources
+
+        Args:
+            module_name (str): name of the module to load
+            module_version (str): version of the module to load
+            module_cache_key (str): cache key of the module after loading
+            module_namespace (str): namespace of the module if applicable
+            loading_order (list[str]): custom loading order, if not specified loading order from config is used
+        """
+
+        if loading_order is None:
+            loading_order = self.loading_order
+
+        for source in loading_order:
+            if source == "registry":
+                log.info(f"Attempting to load {module_name} from registries...")
+                for registry in self.registries:
+                    try:
+                        log.info(
+                            f"Loading component {module_name} from registry {registry}"
+                        )
+
+                        loaded_module_class = self.solve_module_version_and_load(
+                            module_name, module_version, module_cache_key, registry
+                        )
+                        return loaded_module_class
+
+                    except BaseException as e:
+                        log.debug(f"Exception: {e}")
+
+            elif source == "feed":
+                log.info(f"Attempting to load {module_name} from feeds...")
+                for feed in self.feeds:
+                    try:
+                        log.info(f"Loading component {module_name} from feed {feed}")
+
+                        module_name = f"azureml.feed://{feed}/{module_name}"
+
+                        loaded_module_class = self.solve_module_version_and_load(
+                            module_name, module_version, module_cache_key
+                        )
+                        return loaded_module_class
+
+                    except BaseException as e:
+                        log.debug(f"Exception: {e}")
+
+            elif source == "workspace":
+                log.info(f"Attempting to load {module_name} from workspace...")
+                try:
+                    # try without namespace first
+                    return self.solve_module_version_and_load(
+                        module_name, module_version, module_cache_key
+                    )
+                except BaseException as e:
+                    log.debug(f"Exception: {e}")
+
+                if module_namespace is not None:
+                    log.info(
+                        f"    Trying to load module {module_name} with namespace {module_namespace}."
+                    )
+                    module_name = module_namespace + "://" + module_name
+
+                    try:
+                        return self.solve_module_version_and_load(
+                            module_name, module_version, module_cache_key
+                        )
+                    except BaseException as e:
+                        log.debug(f"Exception: {e}")
+
+            else:
+                raise ValueError(
+                    f"Loading order contains incorrect key {source}. Please use a comma-separated str to order 'registry', 'feed', and 'workspace'."
+                )
+
+        raise ValueError(
+            f"Module {module_name} with version {module_version} not found in neither of the following sources: {loading_order}."
+        )
+
+    def load_prod_module(
+        self, module_name, module_version, from_workspace=False, module_namespace=None
+    ):
         """Creates one module instance.
 
         Args:
             module_name (str) : module name
             module_version (str) : module version
+            from_workspace (bool) : attempt to load from workspace only
 
         Returns:
             object: module class loaded
         """
         if self.force_all_module_version:
             module_version = self.force_all_module_version
         else:
             module_version = module_version or self.force_default_module_version
 
         module_cache_key = f"{module_name}:{module_version}"
         if self.module_in_cache(module_cache_key):
             return self.get_from_cache(module_cache_key)
 
-        print(
-            f"--- Loading remote module {module_cache_key} (name={module_name}, version={module_version}, namespace={module_namespace})"
+        log.info(
+            f"Loading remote module {module_cache_key} (name={module_name}, version={module_version}, namespace={module_namespace})"
         )
-        loading_raised_exception = None
 
-        try:
-            # try without namespace first
-            loaded_module_class = Component.load(
-                current_workspace(),
-                name=module_name,
-                version=module_version,
-            )
-        except BaseException as e:
-            # save the exception to raise it if namespace not provided
-            if not module_namespace:
-                raise e
-
-        if module_namespace:
-            print(
-                f"    Trying to load module {module_name} with namespace {module_namespace}."
+        if from_workspace:
+            return self.load_prod_module_helper(
+                module_name,
+                module_version,
+                module_cache_key,
+                module_namespace,
+                loading_order=["workspace"],
             )
-            module_name = module_namespace + "://" + module_name
-            loaded_module_class = Component.load(
-                current_workspace(),
-                name=module_name,
-                version=module_version,
-            )
-
-        self.put_in_cache(module_cache_key, loaded_module_class)
-
-        return loaded_module_class
+        return self.load_prod_module_helper(
+            module_name, module_version, module_cache_key, module_namespace
+        )
 
-    def get_module_manifest_entry(self, module_key, modules_manifest=None):
+    def get_module_manifest_entry(
+        self, module_key, modules_manifest=None
+    ) -> Tuple[dict, Optional[str], bool]:
         """Gets a particular entry in the module manifest.
 
         Args:
             module_key (str): module key from the manifest
             modules_manifest (dict): manifest from required_modules() [DEPRECATED]
 
         Returns:
-            dict: module manifest entry
+            module_entry (dict): module manifest entry (if no entry for this module key in the manifest, only the module key is returned)
+            module_namespace (str | None): module namespace for legacy modules
+            is_in_manifest (bool): true if the module key can be found in the manifest
         """
         if module_key in self.modules_manifest:
             module_entry = self.modules_manifest[module_key]
             module_namespace = None
+            is_in_manifest = True
         elif modules_manifest and module_key in modules_manifest:
-            print(
-                f"WARNING: We highly recommend substituting the required_modules() method by the modules.manifest configuration."
+            log.warning(
+                f"We highly recommend substituting the `required_modules` method by the modules.manifest configuration."
             )
             module_entry = modules_manifest[module_key]
             # map to new format
             module_entry["yaml"] = module_entry["yaml_spec"]
             module_entry["name"] = module_entry["remote_module_name"]
             module_namespace = module_entry.get("namespace", None)
+            is_in_manifest = True
         else:
-            raise Exception(
-                f"Module key '{module_key}' could not be found in modules.manifest configuration or in required_modules() method."
-            )
+            module_entry = {}
+            module_entry["name"] = module_key
+            module_namespace = None
+            is_in_manifest = False
+            if not (self.use_remote_when_component_not_in_manifest):
+                log.warning(
+                    f"Module key '{module_key}' could not be found in modules.manifest configuration or in required_modules() method. If you want to try and load it from the workspace, set 'module_loader.use_remote_when_component_not_in_manifest' to True in the config."
+                )
 
-        return module_entry, module_namespace
+        return module_entry, module_namespace, is_in_manifest
 
     def load_module(self, module_key, modules_manifest=None):
         """Loads a particular module from the manifest.
 
         Args:
             module_key (str): module key from the manifest
             modules_manifest (dict): manifest from required_modules() [DEPRECATED]
 
         Returns:
             object: module class loaded
         """
-        module_entry, module_namespace = self.get_module_manifest_entry(
+        module_entry, module_namespace, is_in_manifest = self.get_module_manifest_entry(
             module_key, modules_manifest
         )
-
-        if self.is_local(module_key):
-            loaded_module = self.load_local_module(module_entry["yaml"])
+        if is_in_manifest:
+            if self.is_local(module_key):
+                loaded_module = self.load_local_module(module_entry["yaml"])
+            else:
+                loaded_module = self.load_prod_module(
+                    module_entry["name"],
+                    module_entry["version"],
+                    from_workspace=module_entry["from_workspace"]
+                    if "from_workspace" in module_entry
+                    else False,
+                    module_namespace=module_namespace,
+                )
         else:
-            loaded_module = self.load_prod_module(
-                module_entry["name"],
-                module_entry["version"],
-                module_namespace=module_namespace,
+            log.warning(
+                f"The component '{module_key}' cannot be found in the manifest. Attempting to load the remote copy."
             )
+            loaded_module = self.load_prod_module(module_entry["name"], None)
         return loaded_module
 
     def load_modules_manifest(self, modules_manifest):
         """Creates module instances from modules_manifest.
 
         Args:
             modules_manifest (dict): manifest of modules to load
 
         Returns:
             dict: modules loaded, keys are taken from module_manifest.
 
         Raises:
             Exception: if loading module has an error or manifest is wrong.
         """
-        print(f"Loading module manifest (use_local={self.use_local})")
+        log.info(f"Loading module manifest (use_local={self.use_local})")
         test_results = self.verify_manifest(modules_manifest)
         if test_results:
             raise Exception(
                 "Loading modules from manifest raised errors:\n\nMANIFEST: {}\n\nERRORS: {}".format(
                     modules_manifest, "\n".join(test_results)
                 )
             )
 
         loaded_modules = {}
         for module_key in modules_manifest:
-            print(f"Loading module {module_key} from manifest")
+            log.info(f"Loading module {module_key} from manifest")
             loaded_modules[module_key] = self.load_module(module_key, modules_manifest)
 
         return loaded_modules
 
-
-def _check_use_local_syntax_valid(use_local_list) -> bool:
-    use_local_except_for = True if use_local_list[0].startswith("!") else False
-    if use_local_except_for:
-        for module_key in use_local_list:
-            if not module_key.startswith("!"):
-                return False
-    else:
-        for module_key in use_local_list:
-            if module_key.startswith("!"):
-                return False
-    return True
+    def _check_use_local_syntax_valid(self, use_local_list) -> bool:
+        use_local_except_for = True if use_local_list[0].startswith("!") else False
+        if use_local_except_for:
+            for module_key in use_local_list:
+                if not module_key.startswith("!"):
+                    return False
+        else:
+            for module_key in use_local_list:
+                if module_key.startswith("!"):
+                    return False
+        return True
```

### Comparing `shrike-1.9.5/shrike/pipeline/pipeline_helper.py` & `shrike-2.0.0.dev0/shrike/pipeline/v1/pipeline_helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,338 +1,674 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
 """
-Pipeline helper class to create pipelines loading modules from a flexible manifest.
+V1 Pipeline helper class to create pipelines loading modules from a flexible manifest.
 """
+from __future__ import annotations
+import argparse
+from abc import ABC
 import os
 import json
 import logging
-import argparse
-from posixpath import splitext
-import re
-import webbrowser
 import uuid
-import shutil
+from typing import Callable, Optional
+from toposort import toposort_flatten
 import yaml
-import jsonpath_ng
-import sys
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+from toposort import toposort_flatten, CircularDependencyError
+from dataclasses import dataclass, fields, asdict
+from functools import lru_cache, wraps
+from itertools import groupby
 
 try:
-    from dataclasses import dataclass
     import hydra
-    from hydra.core.config_store import ConfigStore
     from hydra.core.hydra_config import HydraConfig
-    from omegaconf import DictConfig, OmegaConf
+    from omegaconf import DictConfig, OmegaConf, MISSING
     from flatten_dict import flatten
 
     import azureml
     from azureml.core import Datastore
-    from azureml.core import Experiment
     from azureml.core import Dataset
     from azureml.pipeline.core import PipelineRun
-    from azure.ml.component.component import Input, Output
-    from azure.ml.component._core._component_definition import (
-        ComponentDefinition,
-        ComponentType,
-    )
+    from azure.ml.component.component import Component, Input, Output
+    from azure.ml.component.pipeline import Pipeline
+    from azure.ml.component._pipeline_parameters import PipelineParameter
+    from azureml.exceptions._azureml_exception import UserErrorException
 except ImportError as error:
     raise ImportError(
         f"{error.msg}. Please install using `pip install shrike[pipeline]`."
     )
 
 from shrike import __version__
-from shrike.pipeline.aml_connect import azureml_connect, current_workspace
-from shrike.pipeline.canary_helper import get_repo_info
-from shrike.pipeline.module_helper import AMLModuleLoader, module_loader_config
-from shrike.pipeline.pipeline_config import default_config_dict, HDI_DEFAULT_CONF
-from shrike.pipeline.telemetry_utils import TelemetryLogger
+from shrike.pipeline.pipeline_helper_base import AMLPipelineHelperBase
+from shrike.pipeline.v1.aml_connect import azureml_connect, current_workspace
+from shrike.pipeline.v1.module_helper import AMLModuleLoader
+from shrike.pipeline.pipeline_config import (
+    HDI_DEFAULT_CONF,
+    pipeline_compute_config,
+    uw_compute_config,
+)
 
+log = logging.getLogger(__name__)
 
-class AMLPipelineHelper:
-    """Helper class for building pipelines"""
-
-    BUILT_PIPELINE = None  # the hydra run decorator doesn't allow for return, we're using this variable instead (hack)
 
+class AMLPipelineHelper(AMLPipelineHelperBase, ABC):
     def __init__(self, config, module_loader=None):
         """Constructs the pipeline helper.
 
         Args:
             config (DictConfig): config for this object
             module_loader (AMLModuleLoader): which module loader to (re)use
         """
-        self.config = config
-
         if module_loader is None:
-            print(f"Creating instance of AMLModuleLoader for {self.__class__.__name__}")
-            self.module_loader = AMLModuleLoader(self.config)
-        else:
-            self.module_loader = module_loader
+            log.info(
+                f"Creating instance of AMLModuleLoader for {self.__class__.__name__}"
+            )
+            module_loader = AMLModuleLoader(config)
+        super(AMLPipelineHelper, self).__init__(
+            config=config, module_loader=module_loader
+        )
 
-    ######################
-    ### CUSTOM METHODS ###
-    ######################
+    def _get_job_status(self, job):
+        return job.get_status()
 
-    @classmethod
-    def get_config_class(cls):
-        """Returns a dataclass containing config for this pipeline"""
-        pass
+    def _wait_for_job_completion(self, job):
+        return job.wait_for_completion(show_output=True)
 
-    @classmethod
-    def required_subgraphs(cls):
-        """Dependencies on other subgraphs
-        Returns:
-            dict[str, AMLPipelineHelper]: dictionary of subgraphs used for building this one.
-                keys are whatever string you want for building your graph
-                values should be classes inherinting from AMLPipelineHelper.
-        """
-        return {}
+    ##################################
+    ### USER FACING HELPER METHODS ###
+    ##################################
+    @lru_cache()
+    def component_load(self, component_key) -> Callable[..., "Component"]:
+        """Loads one component from the manifest"""
+        component_func = self.module_loader.load_module(
+            component_key, self.required_modules()
+        )
 
-    @classmethod
-    def required_modules(cls):
-        """Dependencies on modules/components
+        @wraps(component_func)
+        def wrapper(*args, **kwargs):
+            component_step = component_func(*args, **kwargs)
+            if not self.unified_workspace:
+                # In unified workspace, we don't know which location/environment to use
+                # so we will not call apply_smart_runsettings by default
+                log.info(
+                    f"Now try applying the smart runsettting as component post load operation after component initialize: "
+                )
+                self.apply_smart_runsettings(component_step)
+                log.info(f"Successfully applied the smart runsettting. ")
+            return component_step
 
-        Returns:
-            dict[str, dict]: manifest
-        """
-        return {}
+        return wrapper
 
-    def build(self, config):
-        """Builds a pipeline function for this pipeline.
+    @lru_cache()
+    def module_load(self, module_key):
+        """Loads one module from the manifest"""
+        module_func = self.module_loader.load_module(
+            module_key, self.required_modules()
+        )
 
-        Args:
-            config (DictConfig): configuration object (see get_config_class())
+        @wraps(module_func)
+        def wrapper(*args, **kwargs):
+            module_step = module_func(*args, **kwargs)
+            if not self.unified_workspace:
+                log.info(
+                    f"Now try applying the smart runsettting as component post load operation after component initialize: "
+                )
+                self.apply_smart_runsettings(module_step)
+                log.info(f"Successfully applied the smart runsettting. ")
+            return module_step
 
-        Returns:
-            pipeline_function: the function to create your pipeline
-        """
-        raise NotImplementedError("You need to implement your build() method.")
+        return wrapper
 
-    def pipeline_instance(self, pipeline_function, config):
-        """Creates an instance of the pipeline using arguments.
+    @lru_cache()
+    def dataset_load(
+        self,
+        name,
+        version="latest",
+        datastore=None,
+        path_on_datastore=None,
+        description=None,
+    ):
+        """Loads a dataset by either id or name. If the workspace does not contain this dataset and path is given, create the dataset.
 
         Args:
-            pipeline_function (function): the pipeline function obtained from self.build()
-            config (DictConfig): configuration object (see get_config_class())
-
-        Returns:
-            pipeline: the instance constructed using build() function
+            name (str): name or uuid of dataset to load
+            version (str): if loading by name, used to specify version (default "latest")
+            datastore (str): datastore for registering the dataset as <name>
+            path_on_datastore (str): path for registering the dataset as <name>
+            description (str): description of dataset to register
         """
-        raise NotImplementedError(
-            "You need to implement your pipeline_instance() method."
-        )
-
-    def canary(self, args, experiment, pipeline_run):
-        """Tests the output of the pipeline"""
-        pass
-
-    ##################################
-    ### USER FACING HELPER METHODS ###
-    ##################################
+        try:
+            return self._dataset_load_by_name_or_id(name, version)
+        except UserErrorException:
+            log.info(
+                f"Dataset {name} not found. Try registering from {path_on_datastore} on {datastore}..."
+            )
+            dataset = Dataset.File.from_files(
+                path=[(Datastore(self.workspace(), datastore), path_on_datastore)],
+                validate=False,
+            )
+            dataset = dataset.register(
+                workspace=self.workspace(),
+                name=name,
+                description=description,
+                create_new_version=True,
+            )
+            return dataset
 
+    @lru_cache()
     def workspace(self):
         """Gets the current workspace"""
         return current_workspace()
 
-    def component_load(self, component_key):
-        """Loads one component from the manifest"""
-        return self.module_loader.load_module(component_key, self.required_modules())
+    def connect(self):
+        """Connect to the AML workspace using internal config"""
+        # Only call azureml_connect if there is not an already a pre-existing workspace
+        try:
+            return self.workspace()
+        except:
+            return azureml_connect(
+                aml_subscription_id=self.config.aml.subscription_id,
+                aml_resource_group=self.config.aml.resource_group,
+                aml_workspace_name=self.config.aml.workspace_name,
+                aml_auth=self.config.aml.auth,
+                aml_tenant=self.config.aml.tenant,
+                aml_force=self.config.aml.force,
+            )  # NOTE: this also stores aml workspace in internal global variable
 
-    def module_load(self, module_key):
-        """Loads one module from the manifest"""
-        return self.module_loader.load_module(module_key, self.required_modules())
+    ################
+    ### MAIN/RUN ###
+    ################
+    def apply_recommended_runsettings(
+        self,
+        module_name,
+        module_instance,
+        gpu=False,  # can't autodetect that
+        hdi="auto",
+        windows="auto",
+        parallel="auto",
+        mpi="auto",
+        scope="auto",
+        datatransfer="auto",
+        sweep="auto",
+        synapse="auto",
+        location=None,
+        environment=None,
+        **custom_runtime_arguments,
+    ):
+        """Applies regular settings for a given module.
+
+        Args:
+            module_name (str): name of the module from the module manifest (required_modules() method)
+            module_instance (Module): the AML module we need to add settings to
+            gpu (bool): is the module using GPU?
+            hdi (bool): is the module using HDI/Spark?
+            windows (bool): is the module using Windows compute?
+            parallel (bool): is the module using ParallelRunStep?
+            mpi (bool): is the module using Mpi?
+            scope (bool): is the component using scope?
+            datatransfer (bool): is the component using datatransfer?
+            sweep (bool): is the component using sweep?
+            synapse (bool): is the component using Synapse?
+            location (str): location of the silo to use in unified workspace setting
+            environment (str): environment of the silo to use in unified workspace setting
+            custom_runtime_arguments (dict): any additional custom args
+        """
+        # Verifies if module_name corresponds to module_instance
+        self._check_module_runsettings_consistency(module_name, module_instance)
+
+        # Skips if this is a PipelineComponent
+        if str(module_instance.type) == "PipelineComponent":
+            log.info(f"Component {module_name} detected as PipelineComponent.")
+            return
+
+        if environment:
+            assert environment.lower() in [
+                "cloverport",
+                "msit",
+                "mdp",
+            ]  # TODO: what else allowed?
+
+            # Manually add env var because we can't identify the environment in a unified workspace based on subscription
+            environment_variable = {
+                "EYESOFF_ENV": "false"
+                if environment.lower() == "cloverport"
+                else "true"
+            }
+            if str(module_instance.type) not in [
+                "HDInsightComponent",
+                "ScopeComponent",
+                "DataTransferComponent",
+                "SparkComponent",
+            ]:
+                module_instance.runsettings.environment_variables = environment_variable
+
+        # Auto detects runsettings
+        if hdi == "auto":
+            hdi = str(module_instance.type) == "HDInsightComponent"
+            if hdi:
+                log.info(f"Module {module_name} detected as HDI: {hdi}")
+                if environment:
+                    custom_runtime_arguments["eyesoff_conf"] = {
+                        "spark.EYESOFF_ENV": environment_variable["EYESOFF_ENV"]
+                    }
+
+        if parallel == "auto":
+            parallel = str(module_instance.type) == "ParallelComponent"
+            if parallel:
+                log.info(f"Module {module_name} detected as PARALLEL: {parallel}")
+
+        if mpi == "auto":
+            mpi = str(module_instance.type) == "DistributedComponent"
+            if mpi:
+                log.info(f"Module {module_name} detected as MPI: {mpi}")
+
+        if scope == "auto":
+            scope = str(module_instance.type) == "ScopeComponent"
+            if scope:
+                log.info(f"Module {module_name} detected as SCOPE: {scope}")
+
+        if sweep == "auto":
+            sweep = str(module_instance.type) == "SweepComponent"
+            if sweep:
+                log.info(f"Module {module_name} detected as SweepComponent: {sweep}")
+
+        if synapse == "auto":
+            synapse = str(module_instance.type) in ["SparkComponent", "spark"]
+            if synapse:
+                log.info(f"Module {module_name} detected as spark (Synapse): {synapse}")
+                if environment:
+                    custom_runtime_arguments["eyesoff_conf"] = {
+                        "spark.EYESOFF_ENV": environment_variable["EYESOFF_ENV"]
+                    }
+
+        if windows == "auto":
+            if (
+                str(module_instance.type) == "HDInsightComponent"
+                or str(module_instance.type) == "ScopeComponent"
+                or str(module_instance.type) == "DataTransferComponent"
+                or str(module_instance.type) == "SweepComponent"
+                or str(module_instance.type) == "SparkComponent"
+            ):
+                # HDI/scope/datatransfer/sweep modules might not have that environment object
+                windows = False
+            else:
+                windows = (
+                    module_instance._definition.environment.os.lower() == "windows"
+                )
+                if windows:
+                    log.info(f"Module {module_name} detected as WINDOWS: {windows}")
+
+        if datatransfer == "auto":
+            datatransfer = str(module_instance.type) == "DataTransferComponent"
+            if datatransfer:
+                log.info(
+                    f"Module {module_name} detected as DATATRANSFER: {datatransfer}"
+                )
 
-    def subgraph_load(self, subgraph_key):
-        """Loads one subgraph from the manifest"""
-        subgraph_class = self.required_subgraphs()[subgraph_key]
+        if parallel:
+            self._apply_parallel_runsettings(
+                module_name,
+                module_instance,
+                windows=windows,
+                gpu=gpu,
+                location=location,
+                environment=environment,
+                **custom_runtime_arguments,
+            )
+            return
+
+        if sweep:
+            self._apply_sweep_runsettings(
+                module_name,
+                module_instance,
+                windows=windows,
+                gpu=gpu,
+                location=location,
+                environment=environment,
+                **custom_runtime_arguments,
+            )
+            return
 
-        print(f"Building subgraph [{subgraph_key} as {subgraph_class.__name__}]...")
-        # NOTE: below creates subgraph with same pipeline_config
-        subgraph_instance = subgraph_class(
-            config=self.config, module_loader=self.module_loader
+        if windows:
+            self._apply_windows_runsettings(
+                module_name,
+                module_instance,
+                mpi=mpi,
+                location=location,
+                environment=environment,
+                **custom_runtime_arguments,
+            )
+            return
+
+        if hdi:
+            self._apply_hdi_runsettings(
+                module_name,
+                module_instance,
+                location=location,
+                environment=environment,
+                **custom_runtime_arguments,
+            )
+            return
+
+        if scope:
+            self._apply_scope_runsettings(
+                module_name,
+                module_instance,
+                location=location,
+                environment=environment,
+                **custom_runtime_arguments,
+            )
+            return
+
+        if datatransfer:
+            self._apply_datatransfer_runsettings(
+                module_name,
+                module_instance,
+                location=location,
+                environment=environment,
+                **custom_runtime_arguments,
+            )
+            return
+
+        if synapse:
+            self._apply_synapse_runsettings(
+                module_name,
+                module_instance,
+                location=location,
+                environment=environment,
+                **custom_runtime_arguments,
+            )
+            return
+
+        self._apply_linux_runsettings(
+            module_name,
+            module_instance,
+            mpi=mpi,
+            gpu=gpu,
+            location=location,
+            environment=environment,
+            **custom_runtime_arguments,
+        )
+
+    def apply_smart_runsettings(
+        self,
+        component_instance,
+        gpu=False,  # can't autodetect that
+        hdi="auto",
+        windows="auto",
+        parallel="auto",
+        mpi="auto",
+        scope="auto",
+        datatransfer="auto",
+        sweep="auto",
+        synapse="auto",
+        location=None,
+        environment=None,
+        **custom_runtime_arguments,
+    ):
+        """Applies regular settings for a given component.
+
+        Args:
+            component_instance (Component): the AML component we need to add settings to
+            gpu (bool): is the component using GPU?
+            hdi (bool): is the component using HDI?
+            windows (bool): is the component using Windows compute?
+            parallel (bool): is the component using ParallelRunStep?
+            mpi (bool): is the component using Mpi?
+            scope (bool): is the component using scope?
+            datatransfer (bool): is the component using datatransfer?
+            sweep (bool): is the component using sweep?
+            synapse (bool): is the component using Synapse?
+            location (str): location of the silo to use in unified workspace setting
+            environment (str): environment of the silo to use in unified workspace setting
+            custom_runtime_arguments (dict): any additional custom args
+        """
+        # infer component_name
+        component_name = self._get_component_name_from_instance(component_instance)
+        self.apply_recommended_runsettings(
+            component_name,
+            component_instance,
+            gpu,
+            hdi,
+            windows,
+            parallel,
+            mpi,
+            scope,
+            datatransfer,
+            sweep,
+            synapse,
+            location,
+            environment,
+            **custom_runtime_arguments,
         )
-        # subgraph_instance.setup(self.pipeline_config)
-        return subgraph_instance.build(self.config)
 
-    def dataset_load(self, name, version="latest"):
+    def _get_pipeline_run(self, run_id, experiment):
+        return PipelineRun(experiment, self.config.run.pipeline_run_id)
+
+    def _get_run_url(self, pipeline_run):
+        return pipeline_run.get_portal_url()
+
+    def _dataset_load_by_name_or_id(self, name, version):
         """Loads a dataset by either id or name.
 
         Args:
             name (str): name or uuid of dataset to load
             version (str): if loading by name, used to specify version (default "latest")
 
         NOTE: in AzureML SDK there are 2 different methods for loading dataset
         one for id, one for name. This method just wraps them up in one."""
         # test if given name is a uuid
         try:
             parsed_uuid = uuid.UUID(name)
-            print(f"Getting a dataset handle [id={name}]...")
+            log.info(f"Getting a dataset handle [id={name}]...")
             return Dataset.get_by_id(self.workspace(), id=name)
         except ValueError:
-            print(f"Getting a dataset handle [name={name} version={version}]...")
+            log.info(f"Getting a dataset handle [name={name} version={version}]...")
             return Dataset.get_by_name(self.workspace(), name=name, version=version)
 
-    @staticmethod
-    def validate_experiment_name(name):
-        """
-        Check whether the experiment name is valid. It's required that
-        experiment names must be between 1 to 250 characters, start with
-        letters or numbers. Valid characters are letters, numbers, "_",
-        and the "-" character.
-        """
-        if len(name) < 1 or len(name) > 250:
-            raise ValueError("Experiment names must be between 1 to 250 characters!")
-        if not re.match("^[a-zA-Z0-9]$", name[0]):
-            raise ValueError("Experiment names must start with letters or numbers!")
-        if not re.match("^[a-zA-Z0-9_-]*$", name):
-            raise ValueError(
-                "Valid experiment names must only contain letters, numbers, underscore and dash!"
-            )
-        return True
-
-    #######################
-    ### HELPER BACKEND  ###
-    #######################
-
-    @classmethod
-    def _default_config(cls):
-        """Builds the default config for the pipeline class"""
-        config_store = ConfigStore.instance()
-
-        config_dict = default_config_dict()
-        cls._build_config(config_dict)
-
-        config_store.store(name="default", node=config_dict)
-        return OmegaConf.structured(config_dict)
-
-    @classmethod
-    def _build_config(cls, config_dict, modules_config=None):
-        """Builds the entire configuration object for this graph and all subgraphs."""
-        self_config_class = cls.get_config_class()
-        if self_config_class:
-            config_dict[self_config_class.__name__] = self_config_class
-
-        for subgraph_key, subgraph_class in cls.required_subgraphs().items():
-            subgraph_class._build_config(config_dict)
-
     def _set_all_inputs_to(self, module_instance, input_mode):
         """Sets all module inputs to a given intput mode"""
         input_names = [
             a
             for a in dir(module_instance.inputs)
             if isinstance(getattr(module_instance.inputs, a), Input)
         ]
         for input_key in input_names:
             input_instance = getattr(module_instance.inputs, input_key)
             input_instance.configure(mode=input_mode)
-            print(f"-- configured input {input_key} to use mode {input_mode}")
+            log.info(f"Configured input {input_key} to use mode {input_mode}")
 
-    def _set_all_outputs_to(self, module_instance, output_mode, compliant=True):
+    def _set_all_outputs_to(
+        self, module_instance, output_mode, compliant=True, datastore_name=None
+    ):
         """Sets all module outputs to a given output mode"""
         output_names = [
             a
             for a in dir(module_instance.outputs)
             if isinstance(getattr(module_instance.outputs, a), Output)
         ]
-        datastore_name = (
-            self.config.compute.compliant_datastore
-            if compliant
-            else self.config.compute.noncompliant_datastore
-        )
+        if not datastore_name:
+            datastore_name = self._get_datastore_name(module_instance, compliant)
         for output_key in output_names:
             output_instance = getattr(module_instance.outputs, output_key)
-            if output_mode is None:
-                output_instance.configure(
-                    datastore=Datastore(
-                        current_workspace(),
-                        name=datastore_name,
-                    )  # datastore name for storing outputs
-                )
-            else:
-                output_instance.configure(
-                    datastore=Datastore(
-                        current_workspace(),
-                        name=datastore_name,
-                    ),  # datastore name for storing outputs
-                    output_mode=output_mode,
-                )
-            print(
-                f"-- configured output {output_key} to use mode {output_mode} and datastore {datastore_name}"
+            if output_mode:
+                output_instance.configure(output_mode=output_mode)
+            output_instance.configure(datastore=datastore_name)
+            log.info(
+                f"Configured output {output_key} to use mode {output_mode} and datastore {datastore_name}"
             )
 
+    @lru_cache()
+    def _get_uw_configs(self, assets, key_func):
+        assets_dict = {}
+        for key, group in groupby(assets, key_func):
+            for x in group:
+                pass
+            assets_dict[key] = x["name"]  # list(x["name"] for x in group)
+        return assets_dict
+
+    @lru_cache()
+    def _get_uw_datastores(self, location: str, environment: str, dc: bool):
+        environment = environment.lower()
+        if environment == "cloverport":
+            # no DC concept for eyes-on workspace
+            key_func = lambda x: (x["location"].lower(), x["environment"].lower())
+            return self._get_uw_configs(self.config.uw_config.datastores, key_func)[
+                location, environment
+            ]
+        else:
+            key_func = lambda x: (
+                x["location"].lower(),
+                x["environment"].lower(),
+                x["DC"],
+            )
+            return self._get_uw_configs(self.config.uw_config.datastores, key_func)[
+                location, environment, dc
+            ]
+
+    @lru_cache()
+    def _get_uw_computes(
+        self,
+        location: str,
+        environment: str,
+        type: str,
+        os: str = None,
+        gpu: bool = None,
+        dc: bool = None,
+    ):
+        location = location.lower()
+        environment = environment.lower()
+        type = type.lower()
+        if type == "datafactory":
+            key_func = lambda x: (
+                x["location"].lower(),
+                x["environment"].lower(),
+                x["type"].lower(),
+            )
+        elif environment == "cloverport":
+            key_func = lambda x: (
+                x["location"].lower(),
+                x["environment"].lower(),
+                x["type"].lower(),
+                x["os"].lower(),
+                x["gpu"],
+            )
+        else:
+            key_func = lambda x: (
+                x["location"].lower(),
+                x["environment"].lower(),
+                x["type"].lower(),
+                x["os"].lower(),
+                x["gpu"],
+                x["DC"],
+            )
+        uw_computes = self._get_uw_configs(self.config.uw_config.computes, key_func)
+        if type == "datafactory":
+            return uw_computes[location, environment, type]
+        elif environment == "cloverport":
+            return uw_computes[location, environment, type, os.lower(), gpu]
+        else:
+            return uw_computes[location, environment, type, os.lower(), gpu, dc]
+
     def _apply_windows_runsettings(
         self,
         module_name,
         module_instance,
         mpi=False,
         target=None,
         node_count=None,
         process_count_per_node=None,
         input_mode=None,
         output_mode=None,
+        datastore_name=None,
+        location=None,
+        environment=None,
         **custom_runtime_arguments,
     ):
         """Applies settings for a windows module.
 
         Args:
             module_name (str): name of the module from the module manifest (required_modules() method)
             module_instance (Module): the AML module we need to add settings to
             mpi (bool): is job mpi ?
             target (str): force target compute over hydra conf
             node_count (int): force node_count over hydra conf
             process_count_per_node (int): force process_count_per_node over hydra conf
             input_mode (str): force input_mode over hydra conf
             output_mode (str): force output_mode over hydra conf
+            datastore_name (str): output datastore. This will override the datastore based on silo
+            location (str): location of the silo to use in unified workspace setting
+            environment (str): environment of the silo to use in unified workspace setting
             custom_runtime_arguments (dict): any additional custom args
         """
-        if self.module_loader.is_local(module_name):
-            target = (
-                target
-                if target is not None
-                else self.config.compute.windows_cpu_dc_target
-            )
+        if self.unified_workspace:
+            target = target or self._get_uw_computes(
+                location,
+                environment,
+                "amlcompute",
+                "windows",
+                False,
+                self.module_loader.is_local(module_name),
+            )
+            datastore_name = self._get_uw_datastores(
+                location, environment, self.module_loader.is_local(module_name)
+            )  # TODO: how does hdi/spark dc work?
         else:
-            target = (
-                target
-                if target is not None
-                else self.config.compute.windows_cpu_prod_target
-            )
+            if self.module_loader.is_local(module_name):
+                target = (
+                    target
+                    if target is not None
+                    else self.config.compute.windows_cpu_dc_target
+                )
+            else:
+                target = (
+                    target
+                    if target is not None
+                    else self.config.compute.windows_cpu_prod_target
+                )
 
-        print(
+        log.info(
             f"Using windows compute target {target} to run {module_name} from pipeline class {self.__class__.__name__}"
         )
         if custom_runtime_arguments:
-            print(f"Adding custom runtime arguments {custom_runtime_arguments}")
+            log.info(f"Adding custom runtime arguments {custom_runtime_arguments}")
 
         module_instance.runsettings.configure(target=target, **custom_runtime_arguments)
         if mpi:
             node_count = node_count if node_count is not None else 1
             process_count_per_node = (
                 process_count_per_node if process_count_per_node is not None else 1
             )
-            print(
+            log.info(
                 f"Using mpi with node_count={node_count} process_count_per_node={process_count_per_node}"
             )
             module_instance.runsettings.resource_layout.configure(
                 node_count=node_count,
                 process_count_per_node=process_count_per_node,
             )
 
         if input_mode:
             self._set_all_inputs_to(module_instance, input_mode)
         else:
             self._set_all_inputs_to(
-                module_instance, self.config.compute.windows_input_mode
+                module_instance,
+                self.config.compute.windows_input_mode,  # TODO: verify if this works in uw
             )
 
         if output_mode:
-            self._set_all_outputs_to(module_instance, output_mode)
+            self._set_all_outputs_to(
+                module_instance, output_mode, datastore_name=datastore_name
+            )
         else:
             self._set_all_outputs_to(
-                module_instance, self.config.compute.windows_output_mode
+                module_instance,
+                self.config.compute.windows_output_mode,
+                datastore_name=datastore_name,
             )
 
     def _apply_hdi_runsettings(
         self,
         module_name,
         module_instance,
         target=None,
@@ -340,14 +676,17 @@
         driver_memory=None,
         executor_memory=None,
         executor_cores=None,
         number_executors=None,
         conf=None,
         input_mode=None,
         output_mode=None,
+        datastore_name=None,
+        location=None,
+        environment=None,
         **custom_runtime_arguments,
     ):
         """Applies settings for a HDI module.
 
         Args:
             module_name (str): name of the module from the module manifest (required_modules() method)
             module_instance (Module): the AML module we need to add settings to
@@ -356,21 +695,52 @@
             driver_memory (str): force driver_memory over hydra conf
             executor_memory (int): force executor_memory over hydra conf
             executor_cores (int): force executor_cores over hydra conf
             number_executors (int): force number_executors over hydra conf
             conf (str): force conf over hydra conf
             input_mode (str): force input_mode over hydra conf
             output_mode (str): force output_mode over hydra conf
+            datastore_name (str): output datastore. This will override the datastore based on silo
+            location (str): location of the silo to use in unified workspace setting
+            environment (str): environment of the silo to use in unified workspace setting
             custom_runtime_arguments (dict): any additional custom args
         """
-        print(
-            f"Using HDI compute target {self.config.compute.hdi_prod_target} to run {module_name} from pipeline class {self.__class__.__name__}"
+        merged_conf = json.loads(HDI_DEFAULT_CONF)
+        if self.unified_workspace:
+            target = target or self._get_uw_computes(
+                location,
+                environment,
+                "hdinsight",
+                "linux",
+                False,
+                self.module_loader.is_local(module_name),
+            )
+            datastore_name = datastore_name or self._get_uw_datastores(
+                location, environment, self.module_loader.is_local(module_name)
+            )  # TODO: how does hdi/spark dc work?
+        else:
+            if self.module_loader.is_local(module_name):
+                target = (
+                    target if target is not None else self.config.compute.hdi_dc_target
+                )
+                if not self.config.compute.hdi_dc_target:
+                    raise Exception(
+                        f"Your HDI component {module_name} is using local version. Please specify hdi_dc_target"
+                    )
+            else:
+                target = (
+                    target
+                    if target is not None
+                    else self.config.compute.hdi_prod_target
+                )
+        log.info(
+            f"Using HDI compute target {target} to run {module_name} from pipeline class {self.__class__.__name__}"
         )
         if custom_runtime_arguments:
-            print(f"Adding custom runtime arguments {custom_runtime_arguments}")
+            log.info(f"Adding custom runtime arguments {custom_runtime_arguments}")
 
         merged_conf = json.loads(HDI_DEFAULT_CONF)
         new_conf = (
             self.config.compute.hdi_conf if "hdi_conf" in self.config.compute else None
         )
         if conf is not None:
             new_conf = conf
@@ -380,20 +750,18 @@
             elif isinstance(new_conf, DictConfig):
                 new_conf = flatten(dict(new_conf), reducer="dot")
             else:
                 raise ValueError(
                     "computed.hdi_conf is not a valid json string or a single tested configuration."
                 )
             merged_conf.update(new_conf)
+            if "eyesoff_conf" in custom_runtime_arguments:
+                merged_conf.update(custom_runtime_arguments.pop("eyesoff_conf"))
 
-        module_instance.runsettings.configure(
-            target=target
-            if target is not None
-            else self.config.compute.hdi_prod_target,
-        )
+        module_instance.runsettings.configure(target=target)
 
         module_instance.runsettings.hdinsight.configure(
             driver_memory=driver_memory
             if driver_memory is not None
             else self.config.compute.hdi_driver_memory,
             driver_cores=driver_cores
             if driver_cores is not None
@@ -409,15 +777,155 @@
             else self.config.compute.hdi_number_executors,
             conf=merged_conf,
             **custom_runtime_arguments,
         )
 
         if input_mode:
             self._set_all_inputs_to(module_instance, input_mode)
-        self._set_all_outputs_to(module_instance, output_mode)
+        self._set_all_outputs_to(
+            module_instance, output_mode, datastore_name=datastore_name
+        )
+
+    def _apply_synapse_runsettings(
+        self,
+        module_name,
+        module_instance,
+        target=None,
+        driver_cores=None,
+        driver_memory=None,
+        executor_memory=None,
+        executor_cores=None,
+        number_executors=None,
+        conf=None,
+        input_mode=None,
+        output_mode=None,
+        datastore_name=None,
+        location=None,
+        environment=None,
+        **custom_runtime_arguments,
+    ):
+        """Applies settings for a Synapse component. Shrike will not set default runsettings except for spark_identity.
+
+        Args:
+            module_name (str): name of the module from the module manifest (required_modules() method)
+            module_instance (Module): the AML module we need to add settings to
+            target (str): force target compute over hydra conf
+            driver_cores (int): force driver_cores over hydra conf
+            driver_memory (str): force driver_memory over hydra conf
+            executor_memory (int): force executor_memory over hydra conf
+            executor_cores (int): force executor_cores over hydra conf
+            number_executors (int): force number_executors over hydra conf
+            conf (str): force conf over hydra conf
+            input_mode (str): force input_mode over hydra conf
+            output_mode (str): force output_mode over hydra conf
+            datastore_name (str): output datastore. This will override the datastore based on silo
+            location (str): location of the silo to use in unified workspace setting
+            environment (str): environment of the silo to use in unified workspace setting
+            custom_runtime_arguments (dict): any additional custom args
+        """
+
+        if self.unified_workspace:
+            target = target or self._get_uw_computes(
+                location,
+                environment,
+                "synapse",
+                "linux",
+                False,
+                self.module_loader.is_local(module_name),
+            )
+            datastore_name = datastore_name or self._get_uw_datastores(
+                location, environment, self.module_loader.is_local(module_name)
+            )  # TODO: how does hdi/spark dc work?
+        else:
+            if self.module_loader.is_local(module_name):
+                target = (
+                    target
+                    if target is not None
+                    else self.config.compute.synapse_dc_target
+                )
+            else:
+                target = (
+                    target
+                    if target is not None
+                    else self.config.compute.synapse_prod_target
+                )
+        log.info(
+            f"Using Synapse compute target {target} to run {module_name} from pipeline class {self.__class__.__name__}"
+        )
+        if custom_runtime_arguments:
+            log.info(f"Adding custom runtime arguments {custom_runtime_arguments}")
+
+        new_conf = (
+            self.config.compute.synapse_conf
+            if "synapse_conf" in self.config.compute
+            else None
+        )
+        if conf is not None:
+            new_conf = conf
+        if "eyesoff_conf" in custom_runtime_arguments:
+            if new_conf:
+                new_conf.update(custom_runtime_arguments.pop("eyesoff_conf"))
+            else:
+                new_conf = custom_runtime_arguments.pop("eyesoff_conf")
+        if new_conf is not None:
+            if isinstance(new_conf, str):
+                new_conf = json.loads(new_conf)
+            elif isinstance(new_conf, DictConfig) or isinstance(new_conf, dict):
+                new_conf = flatten(dict(new_conf), reducer="dot")
+            else:
+                raise TypeError(
+                    f"compute.synapse_conf of type {type(new_conf)} is not a valid json string or a single tested configuration."
+                )
+            if self.module_loader.is_local(module_name):
+                # https://msdata.visualstudio.com/Vienna/_workitems/edit/1918995
+                new_conf = json.dumps(new_conf)
+
+            module_instance.runsettings.spark.configure(
+                conf=new_conf,
+            )
+
+        module_instance.runsettings.configure(target=target)
+        module_instance.runsettings.spark_identity.configure(type="managed")
+
+        if "synapse_driver_memory" in self.config.compute:
+            driver_memory = driver_memory or self.config.compute.synapse_driver_memory
+        if driver_memory:
+            module_instance.runsettings.spark.configure(driver_memory=driver_memory)
+        if "synapse_driver_cores" in self.config.compute:
+            driver_cores = driver_cores or self.config.compute.synapse_driver_cores
+        if driver_cores:
+            module_instance.runsettings.spark.configure(driver_cores=driver_cores)
+        if "synapse_executor_memory" in self.config.compute:
+            executor_memory = (
+                executor_memory or self.config.compute.synapse_executor_memory
+            )
+        if executor_memory:
+            module_instance.runsettings.spark.configure(executor_memory=executor_memory)
+        if "synapse_number_executors" in self.config.compute:
+            number_executors = (
+                number_executors or self.config.compute.synapse_number_executors
+            )
+        if number_executors:
+            module_instance.runsettings.spark.configure(
+                number_executors=number_executors
+            )
+        if "synapse_executor_cores" in self.config.compute:
+            executor_cores = (
+                executor_cores or self.config.compute.synapse_executor_cores
+            )
+        if executor_cores:
+            module_instance.runsettings.spark.configure(executor_cores=executor_cores)
+        module_instance.runsettings.spark.configure(
+            **custom_runtime_arguments,
+        )
+        if input_mode:
+            self._set_all_inputs_to(module_instance, input_mode)
+        self._set_all_outputs_to(
+            module_instance, output_mode, datastore_name=datastore_name
+        )
 
     def _apply_parallel_runsettings(
         self,
         module_name,
         module_instance,
         windows=False,
         gpu=False,
@@ -426,14 +934,17 @@
         process_count_per_node=None,
         mini_batch_size=None,
         run_invocation_timeout=None,
         run_max_try=None,
         error_threshold=None,
         input_mode=None,
         output_mode=None,
+        datastore_name=None,
+        location=None,
+        environment=None,
         **custom_runtime_arguments,
     ):
         """Applies settings for a ParallelRunStep linux module.
 
         Args:
             module_name (str): name of the module from the module manifest (required_modules() method)
             module_instance (Module): the AML module we need to add settings to
@@ -447,50 +958,70 @@
             run_max_try (int): force run_max_try over hydra conf
             error_threshold (int): The number of file failures for the input FileDataset that should be ignored during processing.
                 If the error count goes above this value, then the job will be aborted.
                 Error threshold is for the entire input and not for individual mini-batches sent to run() method.
                 The range is [-1, int.max]. -1 indicates ignoring all failures during processing.
             input_mode (str): force input_mode over hydra conf
             output_mode (str): force output_mode over hydra conf
+            datastore_name (str): output datastore. This will override the datastore based on silo
+            location (str): location of the silo to use in unified workspace setting
+            environment (str): environment of the silo to use in unified workspace setting
             custom_runtime_arguments (dict): any additional custom args
         """
-        if self.module_loader.is_local(module_name):
-            if windows:
-                if gpu:
-                    raise ValueError(
-                        "A GPU compute target with Windows OS is not available yet!"
-                    )
-                else:
-                    _target = self.config.compute.windows_cpu_dc_target
-            else:
-                if gpu:
-                    _target = self.config.compute.linux_gpu_dc_target
-                else:
-                    _target = self.config.compute.linux_cpu_dc_target
+        if self.unified_workspace:
+            if windows and gpu:
+                raise ValueError(
+                    "A GPU compute target with Windows OS is not available yet!"
+                )
+            target = target or self._get_uw_computes(
+                location,
+                environment,
+                "amlcompute",
+                "windows" if windows else "linux",
+                gpu,
+                self.module_loader.is_local(module_name),
+            )
+            datastore_name = datastore_name or self._get_uw_datastores(
+                location, environment, self.module_loader.is_local(module_name)
+            )  # TODO: how does hdi/spark dc work?
         else:
-            if windows:
-                if gpu:
-                    raise ValueError(
-                        "A GPU compute target with Windows OS is not available yet!"
-                    )
+            if self.module_loader.is_local(module_name):
+                if windows:
+                    if gpu:
+                        raise ValueError(
+                            "A GPU compute target with Windows OS is not available yet!"
+                        )
+                    else:
+                        _target = self.config.compute.windows_cpu_dc_target
                 else:
-                    _target = self.config.compute.windows_cpu_prod_target
+                    if gpu:
+                        _target = self.config.compute.linux_gpu_dc_target
+                    else:
+                        _target = self.config.compute.linux_cpu_dc_target
             else:
-                if gpu:
-                    _target = self.config.compute.linux_gpu_prod_target
+                if windows:
+                    if gpu:
+                        raise ValueError(
+                            "A GPU compute target with Windows OS is not available yet!"
+                        )
+                    else:
+                        _target = self.config.compute.windows_cpu_prod_target
                 else:
-                    _target = self.config.compute.linux_cpu_prod_target
+                    if gpu:
+                        _target = self.config.compute.linux_gpu_prod_target
+                    else:
+                        _target = self.config.compute.linux_cpu_prod_target
 
-        target = target if target is not None else _target
+            target = target if target is not None else _target
 
-        print(
+        log.info(
             f"Using parallelrunstep compute target {target} to run {module_name} from pipeline class {self.__class__.__name__}"
         )
         if custom_runtime_arguments:
-            print(f"Adding custom runtime arguments {custom_runtime_arguments}")
+            log.info(f"Adding custom runtime arguments {custom_runtime_arguments}")
 
         module_instance.runsettings.configure(target=target)
 
         module_instance.runsettings.parallel.configure(
             node_count=node_count
             if node_count is not None
             else self.config.compute.parallel_node_count,
@@ -516,210 +1047,255 @@
             if error_threshold is not None
             else self.config.compute.parallel_error_threshold,
             **custom_runtime_arguments,
         )
 
         if input_mode:
             self._set_all_inputs_to(module_instance, input_mode)
-        if output_mode:
-            self._set_all_outputs_to(module_instance, output_mode)
+        self._set_all_outputs_to(
+            module_instance, output_mode, datastore_name=datastore_name
+        )
 
     def _apply_linux_runsettings(
         self,
         module_name,
         module_instance,
         mpi=False,
         gpu=False,
         target=None,
         node_count=None,
         process_count_per_node=None,
         input_mode=None,
         output_mode=None,
+        datastore_name=None,
+        location=None,
+        environment=None,
         **custom_runtime_arguments,
     ):
         """Applies settings for linux module.
 
         Args:
             module_name (str): name of the module from the module manifest (required_modules() method)
             module_instance (Module): the AML module we need to add settings to
             mpi (bool): is the job mpi?
             gpu (bool): is the job using GPU?
             target (str): force target compute over hydra conf
             node_count (int): force node_count over hydra conf
             process_count_per_node (int): force process_count_per_node over hydra conf
             input_mode (str): force input_mode over hydra conf
             output_mode (str): force output_mode over hydra conf
+            datastore_name (str): output datastore. This will override the datastore based on silo
+            location (str): location of the silo to use in unified workspace setting
+            environment (str): environment of the silo to use in unified workspace setting
             custom_runtime_arguments (dict): any additional custom args
         """
-        if self.module_loader.is_local(module_name) and gpu:
-            target = (
-                target
-                if target is not None
-                else self.config.compute.linux_gpu_dc_target
-            )
-            print(
-                f"Using target {target} for local code GPU module {module_name} from pipeline class {self.__class__.__name__}"
-            )
-        elif not self.module_loader.is_local(module_name) and gpu:
-            target = (
-                target
-                if target is not None
-                else self.config.compute.linux_gpu_prod_target
-            )
-            print(
-                f"Using target {target} for registered GPU module {module_name} from pipeline class {self.__class__.__name__}"
-            )
-        elif self.module_loader.is_local(module_name) and not gpu:
-            target = (
-                target
-                if target is not None
-                else self.config.compute.linux_cpu_dc_target
-            )
-            print(
-                f"Using target {target} for local CPU module {module_name} from pipeline class {self.__class__.__name__}"
-            )
-        elif not self.module_loader.is_local(module_name) and not gpu:
-            target = (
-                target
-                if target is not None
-                else self.config.compute.linux_cpu_prod_target
-            )
-            print(
-                f"Using target {target} for registered CPU module {module_name} from pipeline class {self.__class__.__name__}"
-            )
+        if self.unified_workspace:
+            target = target or self._get_uw_computes(
+                location,
+                environment,
+                "amlcompute",
+                "linux",
+                gpu,
+                self.module_loader.is_local(module_name),
+            )
+            datastore_name = datastore_name or self._get_uw_datastores(
+                location, environment, self.module_loader.is_local(module_name)
+            )  # TODO: how does hdi/spark dc work?
+        else:
+            if self.module_loader.is_local(module_name) and gpu:
+                target = (
+                    target
+                    if target is not None
+                    else self.config.compute.linux_gpu_dc_target
+                )
+            elif not self.module_loader.is_local(module_name) and gpu:
+                target = (
+                    target
+                    if target is not None
+                    else self.config.compute.linux_gpu_prod_target
+                )
+            elif self.module_loader.is_local(module_name) and not gpu:
+                target = (
+                    target
+                    if target is not None
+                    else self.config.compute.linux_cpu_dc_target
+                )
+            elif not self.module_loader.is_local(module_name) and not gpu:
+                target = (
+                    target
+                    if target is not None
+                    else self.config.compute.linux_cpu_prod_target
+                )
+        processor = "GPU" if gpu else "CPU"
+        source = "local" if self.module_loader.is_local(module_name) else "registered"
+        log.info(
+            f"Using target {target} for {source} {processor} module {module_name} from pipeline class {self.__class__.__name__}"
+        )
 
         if custom_runtime_arguments:
-            print(f"Adding custom runtime arguments {custom_runtime_arguments}")
+            log.info(f"Adding custom runtime arguments {custom_runtime_arguments}")
 
         module_instance.runsettings.configure(target=target, **custom_runtime_arguments)
 
         if mpi:
             node_count = node_count if node_count is not None else 1
             process_count_per_node = (
                 process_count_per_node if process_count_per_node is not None else 1
             )
-            print(
+            log.info(
                 f"Using mpi with node_count={node_count} process_count_per_node={process_count_per_node}"
             )
             module_instance.runsettings.resource_layout.configure(
                 node_count=node_count,
                 process_count_per_node=process_count_per_node,
             )
 
         if input_mode:
             self._set_all_inputs_to(module_instance, input_mode)
         else:
             self._set_all_inputs_to(
                 module_instance, self.config.compute.linux_input_mode
             )
-
         if output_mode:
-            self._set_all_outputs_to(module_instance, output_mode)
+            self._set_all_outputs_to(
+                module_instance, output_mode, datastore_name=datastore_name
+            )
         else:
             self._set_all_outputs_to(
-                module_instance, self.config.compute.linux_output_mode
+                module_instance,
+                self.config.compute.linux_output_mode,
+                datastore_name=datastore_name,
             )
 
     def _apply_scope_runsettings(
         self,
         module_name,
         module_instance,
         input_mode=None,
         output_mode=None,
         scope_param=None,
         custom_job_name_suffix=None,
         adla_account_name=None,
+        priority=None,
         **custom_runtime_arguments,
     ):
         """Applies settings for a scope module.
 
         Args:
             module_name (str): name of the module from the module manifest (required_modules() method)
             module_instance (Module): the AML module we need to add settings to
             input_mode (str): force input_mode over hydra conf
             output_mode (str): force output_mode over hydra conf
             scope_param (str): Parameters to pass to scope e.g. Nebula parameters, VC allocation parameters etc.
             custom_job_name_suffix (str): Optional parameter defining custom string to append to job name
             adla_account_name (str): The name of the Cosmos-migrated Azure Data Lake Analytics account to submit scope job
+            priority (int): Scope job priority. Default is 1000.
             custom_runtime_arguments (dict): any additional custom args
         """
-        print(
+        log.info(
             f"Using scope compute target to run {module_name} from pipeline class {self.__class__.__name__}"
         )
         if custom_runtime_arguments:
-            print(f"Adding custom runtime arguments {custom_runtime_arguments}")
+            log.info(f"Adding custom runtime arguments {custom_runtime_arguments}")
 
         if input_mode:
             self._set_all_inputs_to(module_instance, input_mode)
         self._set_all_outputs_to(module_instance, output_mode, compliant=False)
 
         module_instance.runsettings.scope.configure(
             adla_account_name=adla_account_name,
             scope_param=scope_param,
             custom_job_name_suffix=custom_job_name_suffix,
+            priority=priority,
         )
 
     def _apply_datatransfer_runsettings(
         self,
         module_name,
         module_instance,
         compliant=True,
         target=None,
         input_mode=None,
         output_mode=None,
+        datastore_name=None,
+        location=None,
+        environment=None,
         **custom_runtime_arguments,
     ):
         """Applies settings for a HDI module.
 
         Args:
             module_name (str): name of the module from the module manifest (required_modules() method)
             module_instance (Module): the AML module we need to add settings to
             compliant (bool): destination datastore, `compliant_datastore` if True, else `noncompliant_datastore`
             target (str): force target compute over hydra conf
             input_mode (str): force input_mode over hydra conf
             output_mode (str): force output_mode over hydra conf
+            datastore_name (str): output datastore. This will override the datastore based on silo
+            location (str): location of the silo to use in unified workspace setting
+            environment (str): environment of the silo to use in unified workspace setting
             custom_runtime_arguments (dict): any additional custom args
         """
-        print(
-            f"Using datatransfer compute target {self.config.compute.datatransfer_target} to run {module_name} from pipeline class {self.__class__.__name__}"
-        )
         if custom_runtime_arguments:
-            print(f"Adding custom runtime arguments {custom_runtime_arguments}")
+            log.info(f"Adding custom runtime arguments {custom_runtime_arguments}")
 
-        module_instance.runsettings.configure(
-            target=target
-            if target is not None
-            else self.config.compute.datatransfer_target,
+        if self.unified_workspace:
+            target = target or self._get_uw_computes(
+                location, environment, "datafactory"
+            )
+            if compliant:
+                datastore_name = datastore_name or self._get_uw_datastores(
+                    location, environment, False
+                )
+            else:
+                datastore_name = (
+                    datastore_name or self.config.compute.noncompliant_datastore
+                )
+            self._set_all_outputs_to(
+                module_instance, output_mode, datastore_name=datastore_name
+            )
+        else:
+            target = target or self.config.compute.datatransfer_target
+            self._set_all_outputs_to(
+                module_instance, output_mode, compliant, datastore_name
+            )
+        log.info(
+            f"Using datatransfer compute target {target} to run {module_name} from pipeline class {self.__class__.__name__}"
         )
+        module_instance.runsettings.configure(target=target)
 
         if input_mode:
             self._set_all_inputs_to(module_instance, input_mode)
-        self._set_all_outputs_to(module_instance, output_mode, compliant)
 
     def _apply_sweep_runsettings(
         self,
         module_name,
         module_instance,
         windows=False,
         gpu=False,
         target=None,
         input_mode=None,
         output_mode=None,
+        node_count=None,
+        process_count_per_node=None,
         algorithm=None,
         primary_metric=None,
         goal=None,
         policy_type=None,
         evaluation_interval=None,
         delay_evaluation=None,
         slack_factor=None,
         slack_amount=None,
         truncation_percentage=None,
         max_total_trials=None,
         max_concurrent_trials=None,
         timeout_minutes=None,
+        datastore_name=None,
+        location=None,
+        environment=None,
         **custom_runtime_arguments,
     ):
         """Applies settings for a sweep component.
 
         Args:
             module_name (str): name of the module from the module manifest (required_modules() method)
             module_instance (Module): the AML module we need to add settings to
@@ -738,54 +1314,82 @@
             slack_factor (float): the slack allowed with respect to the best performing training run, as a ratio
             slack_amount (float): the slack allowed with respect to the best performing training run, as an absolute ampunt. You should only specify either slack_factor or slack_amount, but not both.
             truncation_percentage (int): the percentage of lowest performing runs to terminate at each evaluation interval. An integer value between 1 and 99.
             max_total_trials (int): maximum number of trial runs. Must be an integer between 1 and 1000.
             max_concurrent_trials (int): maximum number of runs that can run concurrently. If not specified, all runs launch in parallel. If specified, must be an integer between 1 and 100.
             timeout_minutes (int): maximum duration, in minutes, of the hyperparameter tuning experiment. Runs after this duration are canceled.
 
+            datastore_name (str): output datastore
+            location (str): location of the silo to use in unified workspace setting
+            environment (str): environment of the silo to use in unified workspace setting
+
             custom_runtime_arguments (dict): any additional custom args
         """
-        if target is not None:
-            target = target
-        elif self.module_loader.is_local(module_name):
-            if windows:
-                if gpu:
-                    raise ValueError(
-                        "A GPU compute target with Windows OS is not available yet!"
-                    )
-                else:
-                    target = self.config.compute.windows_cpu_dc_target
-            else:
-                if gpu:
-                    target = self.config.compute.linux_gpu_dc_target
-                else:
-                    target = self.config.compute.linux_cpu_dc_target
+        if self.unified_workspace:
+            target = target or self._get_uw_computes(
+                location,
+                environment,
+                "amlcompute",
+                "windows" if windows else "linux",
+                gpu,
+                self.module_loader.is_local(module_name),
+            )
+            datastore_name = datastore_name or self._get_uw_datastores(
+                location, environment, self.module_loader.is_local(module_name)
+            )  # TODO: how does hdi/spark dc work?
         else:
-            if windows:
-                if gpu:
-                    raise ValueError(
-                        "A GPU compute target with Windows OS is not available yet!"
-                    )
+            if target is not None:
+                target = target
+            elif self.module_loader.is_local(module_name):
+                if windows:
+                    if gpu:
+                        raise ValueError(
+                            "A GPU compute target with Windows OS is not available yet!"
+                        )
+                    else:
+                        target = self.config.compute.windows_cpu_dc_target
                 else:
-                    target = self.config.compute.windows_cpu_prod_target
+                    if gpu:
+                        target = self.config.compute.linux_gpu_dc_target
+                    else:
+                        target = self.config.compute.linux_cpu_dc_target
             else:
-                if gpu:
-                    target = self.config.compute.linux_gpu_prod_target
+                if windows:
+                    if gpu:
+                        raise ValueError(
+                            "A GPU compute target with Windows OS is not available yet!"
+                        )
+                    else:
+                        target = self.config.compute.windows_cpu_prod_target
                 else:
-                    target = self.config.compute.linux_cpu_prod_target
-        print(
+                    if gpu:
+                        target = self.config.compute.linux_gpu_prod_target
+                    else:
+                        target = self.config.compute.linux_cpu_prod_target
+        log.info(
             f"Using target {target} to run sweep component {module_name} from pipeline class {self.__class__.__name__}"
         )
         if custom_runtime_arguments:
-            print(f"Adding custom runtime arguments {custom_runtime_arguments}")
+            log.info(f"Adding custom runtime arguments {custom_runtime_arguments}")
+
+        module_instance.runsettings.configure(target=target, **custom_runtime_arguments)
+
+        if node_count:
+            log.info(
+                f"Setting node_count={node_count} and process_count_per_node={process_count_per_node} as run settings for sweep component {module_name} from pipeline class {self.__class__.__name__}"
+            )
+            module_instance.runsettings.resource_layout.configure(
+                node_count=node_count, process_count_per_node=process_count_per_node
+            )
 
         if input_mode:
             self._set_all_inputs_to(module_instance, input_mode)
-        if output_mode:
-            self._set_all_outputs_to(module_instance, output_mode)
+        self._set_all_outputs_to(
+            module_instance, output_mode, datastore_name=datastore_name
+        )
 
         if algorithm:
             module_instance.runsettings.sweep.algorithm = algorithm
         if primary_metric:
             module_instance.runsettings.sweep.objective.configure(
                 primary_metric=primary_metric
             )
@@ -824,680 +1428,254 @@
                 max_concurrent_trials=max_concurrent_trials
             )
         if timeout_minutes:
             module_instance.runsettings.sweep.limits.configure(
                 timeout_minutes=timeout_minutes
             )
 
-    def _check_module_runsettings_consistency(self, module_key, module_instance):
-        """Verifies if entry at module_key matches the module instance description"""
-        module_manifest_entry, _ = self.module_loader.get_module_manifest_entry(
-            module_key, modules_manifest=self.required_modules()
-        )
-
-        if "name" in module_manifest_entry:
-            if module_manifest_entry["name"] == module_instance.name:
-                return
-            if "namespace" in module_manifest_entry:
-                module_entry_name = (
-                    module_manifest_entry["namespace"]
-                    + "://"
-                    + module_manifest_entry["name"]
-                )
-                if module_entry_name == module_instance.name:
-                    return
-            raise Exception(
-                f"During build() of graph class {self.__class__.__name__}, call to self.apply_recommended_runsettings() is wrong: key used as first argument ('{module_key}') maps to a module reference {module_manifest_entry} which name is different from the module instance provided as 2nd argument (name={module_instance.name}), did you use the wrong module key as first argument?"
-            )
-
-    def _get_component_name_from_instance(self, component_instance):
-        component_manifest_list = self.config.modules.manifest
-        component_name = component_instance.name
-        for component_manifest_entry in component_manifest_list:
-            try:
-                if component_manifest_entry["name"] == component_name:
-                    return component_manifest_entry["key"] or component_name
-                if "namespace" in component_manifest_entry:
-                    component_entry_name = (
-                        component_manifest_entry["namespace"]
-                        + "://"
-                        + component_manifest_entry["name"]
-                    )
-                    if component_entry_name == component_name:
-                        return component_manifest_entry["key"] or component_name
-            except:
-                pass
-        raise ValueError(
-            f"Could not find component matching {component_name}. Please check your spelling."
-        )
-
-    def apply_smart_runsettings(
-        self,
-        component_instance,
-        gpu=False,  # can't autodetect that
-        hdi="auto",
-        windows="auto",
-        parallel="auto",
-        mpi="auto",
-        scope="auto",
-        datatransfer="auto",
-        sweep="auto",
-        **custom_runtime_arguments,
-    ):
-        """Applies regular settings for a given component.
-
-        Args:
-            component_instance (Component): the AML component we need to add settings to
-            gpu (bool): is the component using GPU?
-            hdi (bool): is the component using HDI/Spark?
-            windows (bool): is the component using Windows compute?
-            parallel (bool): is the component using ParallelRunStep?
-            mpi (bool): is the component using Mpi?
-            scope (bool): is the component using scope?
-            datatransfer (bool): is the component using datatransfer?
-            sweep (bool): is the component using sweep?
-            custom_runtime_arguments (dict): any additional custom args
-        """
-        # infer component_name
-        component_name = self._get_component_name_from_instance(component_instance)
-        self.apply_recommended_runsettings(
-            component_name,
-            component_instance,
-            gpu,
-            hdi,
-            windows,
-            parallel,
-            mpi,
-            scope,
-            datatransfer,
-            sweep,
-            **custom_runtime_arguments,
-        )
-
-    def apply_recommended_runsettings(
-        self,
-        module_name,
-        module_instance,
-        gpu=False,  # can't autodetect that
-        hdi="auto",
-        windows="auto",
-        parallel="auto",
-        mpi="auto",
-        scope="auto",
-        datatransfer="auto",
-        sweep="auto",
-        **custom_runtime_arguments,
-    ):
-        """Applies regular settings for a given module.
-
-        Args:
-            module_name (str): name of the module from the module manifest (required_modules() method)
-            module_instance (Module): the AML module we need to add settings to
-            gpu (bool): is the module using GPU?
-            hdi (bool): is the module using HDI/Spark?
-            windows (bool): is the module using Windows compute?
-            parallel (bool): is the module using ParallelRunStep?
-            mpi (bool): is the module using Mpi?
-            custom_runtime_arguments (dict): any additional custom args
-        """
-        # verifies if module_name corresponds to module_instance
-        self._check_module_runsettings_consistency(module_name, module_instance)
-
-        # Auto detect runsettings
-        if hdi == "auto":
-            hdi = str(module_instance.type) == "HDInsightComponent"
-            if hdi:
-                print(f"Module {module_name} detected as HDI: {hdi}")
-
-        if parallel == "auto":
-            parallel = str(module_instance.type) == "ParallelComponent"
-            if parallel:
-                print(f"Module {module_name} detected as PARALLEL: {parallel}")
-
-        if mpi == "auto":
-            mpi = str(module_instance.type) == "DistributedComponent"
-            if mpi:
-                print(f"Module {module_name} detected as MPI: {mpi}")
-
-        if scope == "auto":
-            scope = str(module_instance.type) == "ScopeComponent"
-            if scope:
-                print(f"Module {module_name} detected as SCOPE: {scope}")
-
-        if sweep == "auto":
-            sweep = str(module_instance.type) == "SweepComponent"
-            if sweep:
-                print(f"Module {module_name} detected as SweepComponent: {sweep}")
-
-        if windows == "auto":
-            if (
-                str(module_instance.type) == "HDInsightComponent"
-                or str(module_instance.type) == "ScopeComponent"
-                or str(module_instance.type) == "DataTransferComponent"
-                or str(module_instance.type) == "SweepComponent"
-            ):
-                # HDI/scope/datatransfer/sweep modules might not have that environment object
-                windows = False
-            else:
-                windows = (
-                    module_instance._definition.environment.os.lower() == "windows"
-                )
-                if windows:
-                    print(f"Module {module_name} detected as WINDOWS: {windows}")
-
-        if datatransfer == "auto":
-            datatransfer = str(module_instance.type) == "DataTransferComponent"
-            if datatransfer:
-                print(f"Module {module_name} detected as DATATRANSFER: {datatransfer}")
-
-        if parallel:
-            self._apply_parallel_runsettings(
-                module_name,
-                module_instance,
-                windows=windows,
-                gpu=gpu,
-                **custom_runtime_arguments,
-            )
-            return
-
-        if sweep:
-            self._apply_sweep_runsettings(
-                module_name,
-                module_instance,
-                windows=windows,
-                gpu=gpu,
-                **custom_runtime_arguments,
-            )
-            return
+    def _get_component_name_helper(self, component_instance):
+        return component_instance.name
 
-        if windows:
-            # no detonation chamber, we an't use "use_local" here
-            self._apply_windows_runsettings(
-                module_name, module_instance, mpi=mpi, **custom_runtime_arguments
-            )
-            return
-
-        if hdi:
-            # no detonation chamber, we an't use "use_local" here
-            self._apply_hdi_runsettings(
-                module_name, module_instance, **custom_runtime_arguments
+    def _update_dc_configs(self, pipeline: Pipeline, debug: bool = False) -> Pipeline:
+        # collect the known DC targets
+        dc_datastore = None
+        if not self.unified_workspace:
+            # workaround for missing "throw_on_missing" in currently used omegaconf
+            compute_config_as_dict = yaml.safe_load(
+                OmegaConf.to_yaml(self.config.compute)
             )
-            return
-
-        if scope:
-            self._apply_scope_runsettings(
-                module_name, module_instance, **custom_runtime_arguments
-            )
-            return
-
-        if datatransfer:
-            self._apply_datatransfer_runsettings(
-                module_name, module_instance, **custom_runtime_arguments
-            )
-            return
-
-        self._apply_linux_runsettings(
-            module_name, module_instance, mpi=mpi, gpu=gpu, **custom_runtime_arguments
-        )
-
-    def _parse_pipeline_tags(self):
-        """Parse the tags specified in the pipeline yaml"""
-        pipeline_tags = {}
-        if self.config.run.tags:
-            if isinstance(self.config.run.tags, str):
-                try:
-                    # json.load the tags string in the config
-                    pipeline_tags = json.loads(self.config.run.tags)
-                except ValueError:
-                    print(
-                        f"The pipeline tags {self.config.run.tags} is not a valid json-style string."
-                    )
-            elif isinstance(self.config.run.tags, DictConfig):
-                pipeline_tags.update(self.config.run.tags)
-            else:
-                print(
-                    f"The pipeline tags {self.config.run.tags} is not a valid DictConfig or json-style string."
+            dc_targets: Set[str] = {
+                target
+                for key, target in compute_config_as_dict.items()
+                if key.endswith("_dc_target") and target and target != str(MISSING)
+            }
+            dc_datastore = self.config.compute.dc_datastore
+        else:
+            log.warn(
+                """
+                Updating for DC is not fully supported for multi-region pipelines 
+                in the unified workspace mode and is subject to error. 
+                Strongly recommend to skip this by setting `run.skip_update_dc`. 
+                If you need to test on DC, please try `module_loader.use_local='!<data_transfer>'`
+                """
+            )
+            dc_targets: Set[str] = {
+                target["name"]
+                for target in self.config.uw_config.computes
+                if target["DC"]
+            }
+        if not dc_targets:
+            # This is kind of pointless because if one local component exists
+            # then one of the `apply_*` methods wil fail if no dc target is not
+            # specified. And if no local component exists, then there is no
+            # point in outputting this. But let's do it anyway:
+            log.info("The compute config does not contain any DC targets.")
+            return pipeline
+
+        log.info("Overriding compute target if upstream steps use DC...")
+
+        # build and parse the dependency graph
+        dependency_graph = _DependencyGraph.from_pipeline(
+            pipeline=pipeline, debug=debug
+        )
+
+        should_use_dc = dependency_graph.determine_dc_nodes(dc_targets=dc_targets)
+
+        log.info(f"Need to configure the following for DC: {sorted(should_use_dc)}")
+
+        # prepare a mapping from known prod targets to (their corresponding
+        # key in the shrike config and) the corresponding DC target
+        target_map: Dict[str, Tuple[str, Optional[str]]] = {}
+        if self.unified_workspace:
+            for prod_target_info in self.config.uw_config.computes:
+                if (
+                    prod_target_info.DC
+                    or prod_target_info.type.lower() == "datafactory"
+                ):
+                    continue
+                prod_target = prod_target_info.name
+                dc_target = self._get_uw_computes(
+                    prod_target_info.location,
+                    prod_target_info.environment,
+                    prod_target_info.type,
+                    prod_target_info.os,
+                    prod_target_info.gpu,
+                    True,
                 )
-        return pipeline_tags
+                target_map[prod_target] = [prod_target, dc_target]
+        else:
+            for prod_target in [
+                "hdi_prod_target",
+                "linux_cpu_prod_target",
+                "linux_gpu_prod_target",
+                "windows_cpu_prod_target",
+                "synapse_prod_target",
+            ]:
+                if prod_target not in self.config.compute:
+                    continue
+                target_map[self.config.compute[prod_target]] = [
+                    prod_target,
+                    self.config.compute.get(
+                        prod_target.replace("_prod_", "_dc_"), None
+                    ),
+                ]
 
-    def _check_if_spec_yaml_override_is_needed(self):
-        if self.config.module_loader.use_local == "":
-            print(
-                "All components are using remote copy, so override will not be executed. For components you want submission-time override of images/tags/etc., please specify them in `use_local`."
-            )
-            return False, None
-        if not self.config.tenant_overrides.allow_override:
-            print(
-                "Spec yaml file override is not allowed. If you want to use this feature, please set `tenant_overrides.allow_override` to True in your pipeline yaml."
-            )
-            return False, None
-        cur_tenant = self.config.aml.tenant
-        for tenant in self.config.tenant_overrides.mapping.keys():
-            if tenant == cur_tenant:
-                print(
-                    f"Your tenant is inconsistent with spec yaml, We will override relevant fields in your spec yaml files based on entry `{tenant}` in your pipeline yaml file."
-                )
-                return True, self.config.tenant_overrides.mapping[tenant]
-            if self.config.run.config_dir:
-                config_file_path = os.path.join(
-                    self.config.run.config_dir, "aml", tenant + ".yaml"
-                )
-                print(f"config_file_path is {config_file_path}")
-                if os.path.exists(config_file_path):
-                    with open(config_file_path, "r") as file:
-                        config = yaml.safe_load(file)
-                    if config["tenant"] == cur_tenant:
-                        print(
-                            f"Your tenant is inconsistent with spec yaml, We will override relevant fields in your spec yaml files based on entry `{config_file_path}` in your pipeline yaml file."
-                        )
-                        return True, self.config.tenant_overrides.mapping[tenant]
-        return False, None
+        # move to DC!
+        for node_id in should_use_dc:
+            node = dependency_graph.nodes[node_id]
+
+            if isinstance(node, Output):
+
+                if node._owner.type == "ScopeComponent":
+                    # output datastore has to be cosmos (ADLSg1), while dc_datastore is ADLSg2
+                    continue
+                if self.unified_workspace:
+                    dc_datastore = None
+                    prod_datastore = node._datastore
+                    for datastore in self.config.uw_config.datastores:
+                        if datastore.name == prod_datastore:
+                            dc_datastore = self._get_uw_datastores(
+                                datastore.location,
+                                datastore.environment,
+                                True,
+                            )
+                            break
+                if dc_datastore:
+                    node.configure(
+                        datastore=dc_datastore,
+                        output_mode=None,
+                    )
+                    log.info(f"Configured {node_id} to use datastore {dc_datastore}.")
 
-    def _override_spec_yaml(self, spec_mapping):
-        module_keys = self.module_loader.modules_manifest
-        yaml_to_be_recovered = []
-        env_yaml_override_is_needed = (
-            spec_mapping.remove_polymer_pkg_idx
-            if "remove_polymer_pkg_idx" in spec_mapping
-            else False
-        )
-        for module_key in module_keys:
-            if not self.module_loader.is_local(module_key):
-                print(
-                    f"Component {module_key} is using the remote copy. Skipping overrides."
+            elif not hasattr(node.runsettings, "target"):
+                # e.g. scope component doesn't need to configure compute target
+                log.info(f"Node {node.name} does not have `target`.")
+                continue
+            elif not isinstance(node.runsettings.target, str):
+                log.warn(
+                    f"The compute target of node {node.name} is a PipelineParameter. Shrike will not update even if this or the upstream steps use DC. Please update manually."
                 )
                 continue
-            print(f"Overriding for component: {module_key}.")
-            module_entry = self.module_loader.modules_manifest[module_key]
-            spec_path = os.path.join(
-                self.module_loader.local_steps_folder, module_entry["yaml"]
-            )
-            (
-                old_spec_path,
-                old_env_file_path,
-                new_env_file_path,
-            ) = self._override_single_spec_yaml(
-                spec_path, spec_mapping, env_yaml_override_is_needed
-            )
-
-            yaml_to_be_recovered.append(
-                [old_spec_path, spec_path, old_env_file_path, new_env_file_path]
-            )
-        return yaml_to_be_recovered
-
-    def _update_value_given_flattened_key(self, nested_dict, dot_key, new_val):
-        print(f"Updating key {dot_key}")
-        split_key = dot_key.split(".")
-        res = nested_dict
-        path = ""
-        for key in split_key[:-1]:
-            path += key + "."
-            if not isinstance(res, dict) or key not in res:
-                raise KeyError(
-                    f"Key {dot_key} not in {nested_dict}. It failed at {path}."
-                )
-            res = res[key]
-        if isinstance(res, dict) and split_key[-1] in res:
-            res[split_key[-1]] = new_val
-            print(f"The field {dot_key} has been updated to {new_val} successfully.")
-        else:
-            raise KeyError(f"Key {dot_key} not in {nested_dict}.")
-
-    def _override_single_spec_yaml(
-        self, spec_path, spec_mapping, env_yaml_override_is_needed
-    ):
-        spec_filename, spec_ext = os.path.splitext(spec_path)
-        old_spec_path = (
-            spec_filename + ".not_used"
-        )  # remove ".yaml" extension to avoid confusion
-        shutil.copyfile(
-            spec_path, old_spec_path
-        )  # need to recover after pipeline submission
-
-        with open(spec_path) as file:
-            spec = yaml.safe_load(file)
-        for key in spec_mapping:
-            match = jsonpath_ng.parse(key).find(spec)
-            if match:
-                try:
-                    print(f"Find a matching field to override: {key}.")
-                    original_val = match[0].value
-                    print(
-                        f"Original value is {original_val}. Looking for new value now..."
-                    )
-                    spec_mapping_to_use = spec_mapping[key]
-                    if isinstance(original_val, str):
-                        print(f"The field to be updated is str.")
-                        if original_val in spec_mapping_to_use:
-                            new_val = spec_mapping_to_use[original_val]
-                            print(f"The new value is: {new_val}.")
-                            self._update_value_given_flattened_key(spec, key, new_val)
-                        else:
-                            for pattern in spec_mapping_to_use:
-                                if re.match(pattern, original_val):
-                                    new_val = spec_mapping_to_use[pattern]
-                                    print(f"The new pattern is: {new_val}.")
-                                    self._update_value_given_flattened_key(
-                                        spec,
-                                        key,
-                                        re.sub(pattern, new_val, original_val),
-                                    )
-                    elif isinstance(original_val, dict):
-                        print("The field to be updated is dict")
-                        for spec_mapping_key in spec_mapping_to_use:
-                            self._update_value_given_flattened_key(
-                                spec,
-                                ".".join([key, spec_mapping_key]),
-                                spec_mapping_to_use[spec_mapping_key],
-                            )
-                    else:
-                        print(
-                            f"Override for key {key} is not supported yet. Please open a [feature request](https://github.com/Azure/shrike/issues) if necessary."
-                        )
-                except KeyError:
-                    print(f"Key {key} does not in file {spec_path}. Skip overrides.")
-        new_env_file_path = None
-        old_env_file_path = None
-        if env_yaml_override_is_needed:
-            spec_dirname = os.path.dirname(spec_path)
-            polymer_pkg_idx = "--index-url https://o365exchange.pkgs.visualstudio.com/_packaging/PolymerPythonPackages/pypi/simple/"
-            print(f"Will remove {polymer_pkg_idx} from environment.conda.")
-            try:
-                conda_dependencies_file = spec["environment"]["conda"][
-                    "conda_dependencies_file"
-                ]
-                print("conda_dependencies_file exists.")
-                (
-                    found_index_url,
-                    new_file,
-                    new_env_file_path,
-                    old_env_file_path,
-                ) = self._remove_polymer_pkg_idx_if_exists_and_save_new(
-                    spec_dirname, conda_dependencies_file, polymer_pkg_idx
-                )
-                if found_index_url:
-                    spec["environment"]["conda"]["conda_dependencies_file"] = new_file
-            except KeyError:
-                # conda_dependencies_file does not exist
-                pass
-            try:
-                conda_dependencies = spec["environment"]["conda"]["conda_dependencies"][
-                    "dependencies"
-                ]
-                print("conda_dependencies_file exists.")
-                for idx, dependency in enumerate(conda_dependencies):
-                    if isinstance(dependency, dict) and "pip" in dependency:
-                        pip_dependencies = dependency["pip"]
-                        if polymer_pkg_idx in pip_dependencies:
-                            pip_dependencies.remove(polymer_pkg_idx)
-                            dependency["pip"] = pip_dependencies
-                            conda_dependencies[idx] = dependency
-                spec["environment"]["conda"]["conda_dependencies"][
-                    "dependencies"
-                ] = conda_dependencies
-            except KeyError:
-                # conda_dependencies does not exist
-                pass
-            try:
-                pip_requirements_file = spec["environment"]["conda"][
-                    "pip_requirements_file"
-                ]
-                print("pip_requirements_file exists.")
-                (
-                    found_index_url,
-                    new_file,
-                    new_env_file_path,
-                    old_env_file_path,
-                ) = self._remove_polymer_pkg_idx_if_exists_and_save_new(
-                    spec_dirname, pip_requirements_file, polymer_pkg_idx
-                )
-                if found_index_url:
-                    spec["environment"]["conda"]["pip_requirements_file"] = new_file
-            except KeyError:
-                # pip_requirements_file does not exist
+            elif node.runsettings.target in dc_targets:
+                # nothing to do here
                 pass
 
-        with open(spec_path, "w") as file:
-            yaml.safe_dump(spec, file)
-        return old_spec_path, old_env_file_path, new_env_file_path
+            elif node.runsettings.target not in target_map:
+                log.error(
+                    f"Node {node} is using an unknown target: "
+                    f"{node.runsettings.target}. "
+                    f"Please move this to DC manually, or re-run "
+                    f"this after adding the target to the compute config."
+                )
 
-    def _remove_polymer_pkg_idx_if_exists_and_save_new(
-        self, spec_dirname, file, polymer_pkg_idx
-    ):
-        found_index_url = False
-        new_file = ""
-        new_file_path = ""
-        old_file_path = ""
-        with open(os.path.join(spec_dirname, file), "r") as f:
-            lines = f.readlines()
-        for line in lines:
-            if polymer_pkg_idx in line:
-                found_index_url = True
-                lines.remove(line)
-        if found_index_url:
-            file_name, file_ext = os.path.splitext(file)
-            new_file = file_name + "_" + self.config.aml.tenant + file_ext
-            new_file_path = os.path.join(spec_dirname, new_file)
-            with open(new_file_path, "w") as f:
-                f.writelines(lines)
-            old_file_path = os.path.join(
-                spec_dirname, os.path.splitext(file)[0] + ".not_used"
-            )
-            shutil.move(os.path.join(spec_dirname, file), old_file_path)
-        return found_index_url, new_file, new_file_path, old_file_path
-
-    def _recover_spec_yaml(self, spec_file_pairs, keep_modified_files):
-        print(
-            f"Reverting changes to spec yaml files. Keeping modified spec yaml files: {keep_modified_files}."
-        )
-        for (
-            old_spec_path,
-            new_spec_path,
-            old_env_file_path,
-            new_env_file_path,
-        ) in spec_file_pairs:
-            # Question: do we want to keep a copy of the modified files?
-            if keep_modified_files:
-                filename, ext = os.path.splitext(new_spec_path)
-                shutil.move(
-                    new_spec_path, filename + "_" + self.config.aml.tenant + ext
-                )
-                if os.path.exists(filename + ".additional_includes"):
-                    shutil.copyfile(
-                        filename + ".additional_includes",
-                        filename
-                        + "_"
-                        + self.config.aml.tenant
-                        + ".additional_includes",
-                    )
             else:
-                if new_env_file_path:
-                    os.remove(new_env_file_path)
-            shutil.move(old_spec_path, new_spec_path)
-            if old_env_file_path:
-                shutil.move(
-                    old_env_file_path, os.path.splitext(old_env_file_path)[0] + ".yaml"
+                prod_target_key, dc_target = target_map[node.runsettings.target]
+                if dc_target is None:
+                    log.error(
+                        f"No corresponding DC target is defined for "
+                        f"prod target {prod_target_key}. "
+                        f"Please move this to DC manually, or re-run "
+                        f"this after adding the DC target to the compute config."
+                    )
+                    continue
+
+                node.runsettings.configure(target=dc_target)
+                log.info(
+                    f"Updating compute target for {node_id} to {node.runsettings.target}"
                 )
+        return pipeline
 
     ################
     ### MAIN/RUN ###
     ################
 
     def connect(self):
         """Connect to the AML workspace using internal config"""
-        return azureml_connect(
-            aml_subscription_id=self.config.aml.subscription_id,
-            aml_resource_group=self.config.aml.resource_group,
-            aml_workspace_name=self.config.aml.workspace_name,
-            aml_auth=self.config.aml.auth,
-            aml_tenant=self.config.aml.tenant,
-            aml_force=self.config.aml.force,
-        )  # NOTE: this also stores aml workspace in internal global variable
+        # Only call azureml_connect if there is not an already a pre-existing workspace
+        try:
+            return self.workspace()
+        except:
+            return azureml_connect(
+                aml_subscription_id=self.config.aml.subscription_id,
+                aml_resource_group=self.config.aml.resource_group,
+                aml_workspace_name=self.config.aml.workspace_name,
+                aml_auth=self.config.aml.auth,
+                aml_tenant=self.config.aml.tenant,
+                aml_force=self.config.aml.force,
+            )  # NOTE: this also stores aml workspace in internal global variable
 
-    def build_and_submit_new_pipeline(self):
-        print(f"Building Pipeline [{self.__class__.__name__}]...")
+    def _build_pipeline(self) -> Pipeline:
+        log.info(f"Building Pipeline [{self.__class__.__name__}]...")
         pipeline_function = self.build(self.config)
 
-        print("Creating Pipeline Instance...")
+        log.info("Creating Pipeline Instance...")
         pipeline = self.pipeline_instance(pipeline_function, self.config)
 
-        print("Validating...")
-        pipeline.validate()
+        if not self.config.run.skip_update_dc and self.is_eyesoff():
+            log.info("Overriding compute target if upstream steps use DC...")
+            pipeline = self._update_dc_configs(pipeline)
+
+        if not self.config.run.skip_validation:
+            log.info("Validating...")
+            pipeline.validate(workspace=self.workspace())
 
         if self.config.run.export:
-            print(f"Exporting to {self.config.run.export}...")
+            log.info(f"Exporting to {self.config.run.export}...")
             with open(self.config.run.export, "w") as export_file:
-                export_file.write(pipeline._get_graph_json())
+                export_file.write(pipeline._get_graph_json(workspace=self.workspace()))
+        return pipeline
+
+    def _submit_pipeline(self, pipeline: Pipeline) -> Optional[PipelineRun]:
+        """Publish and submit the given pipeline.
+
+        Args:
+            pipeline: pipeline to be submitted
+        """
+        if self.config.run.publish:
+            self._publish_to_endpoint(pipeline)
 
         if self.config.run.submit:
             pipeline_tags = self._parse_pipeline_tags()
+            pipeline_tags.update({"shrike": __version__})
             pipeline_tags.update(self.repository_info)
-            print(f"Submitting Experiment... [tags={pipeline_tags}]")
+            pipeline_tags.update(self._validate_tags(self.extra_tags()))
+            log.info(f"Submitting Experiment... [tags={pipeline_tags}]")
 
             # pipeline_run is of the class "azure.ml.component.run", which
             # is different from "azureml.pipeline.core.PipelineRun"
             pipeline_run = pipeline.submit(
+                workspace=self.workspace(),
                 experiment_name=self.config.run.experiment_name,
+                description=self.config.run.experiment_description,
+                display_name=self.config.run.display_name,
                 tags=pipeline_tags,
-                default_compute_target=self.config.compute.default_compute_target,
+                default_compute_target=None
+                if self.unified_workspace
+                else self.config.compute.default_compute_target,
                 regenerate_outputs=self.config.run.regenerate_outputs,
                 continue_on_step_failure=self.config.run.continue_on_failure,
+                skip_validation=self.config.run.skip_validation,
             )
 
             # Forece pipeline_run to be of the class "azureml.pipeline.core.PipelineRun"
             pipeline_run = PipelineRun(
                 experiment=pipeline_run._experiment,
                 run_id=pipeline_run._id,
             )
             return pipeline_run
 
         else:
-            print("Exiting now, if you want to submit please override run.submit=True")
+            log.info(
+                "Exiting now, if you want to submit please override run.submit=True"
+            )
             self.__class__.BUILT_PIPELINE = (
                 pipeline  # return so we can have some unit tests done
             )
             return
 
-    def run(self):
-        """Run pipeline using arguments"""
-        # Log the telemetry information in the Azure Application Insights
-        telemetry_logger = TelemetryLogger(
-            enable_telemetry=not self.config.run.disable_telemetry
-        )
-        telemetry_logger.log_trace(
-            message=f"shrike.pipeline=={__version__}",
-            properties={"custom_dimensions": {"configuration": str(self.config)}},
-        )
-
-        # Check whether the experiment name is valid
-        self.validate_experiment_name(self.config.run.experiment_name)
-
-        self.repository_info = get_repo_info()
-        print(f"Running from repository: {self.repository_info}")
-
-        print("azureml.core.VERSION = {}".format(azureml.core.VERSION))
-        self.connect()
-
-        if self.config.run.verbose:
-            logging.getLogger().setLevel(logging.DEBUG)
-
-        pipeline_run = None
-        if self.config.run.resume:
-            if not self.config.run.pipeline_run_id:
-                raise Exception(
-                    "To be able to use --resume you need to provide both --experiment-name and --run-id."
-                )
-
-            print(f"Resuming Experiment {self.config.run.experiment_name}...")
-            experiment = Experiment(
-                current_workspace(), self.config.run.experiment_name
-            )
-            print(f"Resuming PipelineRun {self.config.run.pipeline_run_id}...")
-            # pipeline_run is of the class "azureml.pipeline.core.PipelineRun"
-            pipeline_run = PipelineRun(experiment, self.config.run.pipeline_run_id)
-        else:
-            keep_modified_files = False
-            if self.config.tenant_overrides.allow_override:
-                print("Check if tenant is consistent with spec yaml")
-                yaml_to_be_recovered = []
-                override, mapping = self._check_if_spec_yaml_override_is_needed()
-                if override:
-                    try:
-                        tenant = self.config.aml.tenant
-                        print(
-                            f"Performing spec yaml override to adapt to tenant: {tenant}."
-                        )
-                        yaml_to_be_recovered = self._override_spec_yaml(mapping)
-                        keep_modified_files = (
-                            self.config.tenant_overrides.keep_modified_files
-                        )
-
-                        pipeline_run = self.build_and_submit_new_pipeline()
-                        self._recover_spec_yaml(
-                            yaml_to_be_recovered, keep_modified_files
-                        )
-                    except:
-                        print("An error occured, override is not successful.")
-
-            else:
-                pipeline_run = self.build_and_submit_new_pipeline()
-
-        if not pipeline_run:
-            # not submitting code, exit now
-            return
-        # launch the pipeline execution
-        print(f"Pipeline Run Id: {pipeline_run.id}")
-        print(
-            f"""
-#################################
-#################################
-#################################
-
-Follow link below to access your pipeline run directly:
--------------------------------------------------------
-
-{pipeline_run.get_portal_url()}
-
-#################################
-#################################
-#################################
-        """
-        )
-
-        if self.config.run.canary:
-            print(
-                "*** CANARY MODE ***\n----------------------------------------------------------"
-            )
-            pipeline_run.wait_for_completion(show_output=True)
-
-            # azureml.pipeline.core.PipelineRun.get_status(): ["Running", "Finished", "Failed"]
-            # azureml.core.run.get_status(): ["Running", "Completed", "Failed"]
-            if pipeline_run.get_status() in ["Finished", "Completed"]:
-                print("*** PIPELINE FINISHED, TESTING WITH canary() METHOD ***")
-                self.canary(self.config, pipeline_run.experiment, pipeline_run)
-                print("OK")
-            elif pipeline_run.get_status() == "Failed":
-                print("*** PIPELINE FAILED ***")
-                raise Exception("Pipeline failed.")
-            else:
-                print("*** PIPELINE STATUS {} UNKNOWN ***")
-                raise Exception("Pipeline status is unknown.")
-
-        else:
-            if not self.config.run.silent:
-                webbrowser.open(url=pipeline_run.get_portal_url())
-
-            # This will wait for the completion of the pipeline execution
-            # and show the full logs in the meantime
-            if self.config.run.resume or self.config.run.wait:
-                print(
-                    "Below are the raw debug logs from your pipeline execution:\n----------------------------------------------------------"
-                )
-                pipeline_run.wait_for_completion(show_output=True)
-
     @classmethod
     def main(cls):
         """Pipeline helper main function, parses arguments and run pipeline."""
         config_dict = cls._default_config()
 
         @hydra.main(config_name="default")
         def hydra_run(cfg: DictConfig):
@@ -1507,19 +1685,160 @@
             arg_parser = argparse.ArgumentParser()
             arg_parser.add_argument("--config-dir")
             args, _ = arg_parser.parse_known_args()
             cfg.run.config_dir = os.path.join(
                 HydraConfig.get().runtime.cwd, args.config_dir
             )
 
-            print("*** CONFIGURATION ***")
-            print(OmegaConf.to_yaml(cfg))
+            log.info("*** CONFIGURATION ***")
+            log.info(OmegaConf.to_yaml(cfg))
 
             # create class instance
             main_instance = cls(cfg)
 
             # run
             main_instance.run()
 
         hydra_run()
 
         return cls.BUILT_PIPELINE  # return so we can have some unit tests done
+
+
+class _DependencyGraph:
+    NodeType = Union[Component, Output]
+
+    graph: Dict[str, List[str]] = {}
+    nodes: Dict[str, NodeType] = {}
+    debug: bool = False
+
+    def map_to_id(self, item: Union[Pipeline, Component, Output]) -> Optional[str]:
+        """Maps the given item to an id."""
+        # Reminder: class-wise, pipelines are also components
+        extra = f"{item.comment}, " if self.debug and hasattr(item, "comment") else ""
+        if isinstance(item, Pipeline):
+            return f"pipeline `{item.display_name.replace(' ', '-')}` ({extra}{item._instance_id})"
+        if isinstance(item, Component):
+            return f"component `{item.display_name.replace(' ', '-')}` ({extra}{item._instance_id})"
+        if isinstance(item, Output):
+            return f"output `{item.port_name}` of {self.map_to_id(item._owner)}"
+        raise ValueError(
+            f"Please report this. Could not map {item} to dependency graph id."
+        )
+
+    def add_edge(
+        self,
+        from_node: NodeType,
+        to_node: NodeType,
+    ) -> None:
+        """Add an edge from a dependent node its dependency."""
+        for node in [from_node, to_node]:
+            if not isinstance(node, (Component, Output)):
+                raise ValueError(
+                    f"Please report this. "
+                    f"Expected a valid node type but was given {node} as node."
+                )
+            node_id = self.map_to_id(node)
+            known_node = self.nodes.get(node_id)
+            if known_node is not None and node is not known_node:
+                raise ValueError("Report this. Two different nodes with same id.")
+            self.nodes[node_id] = node
+
+        ids = [self.map_to_id(node) for node in [from_node, to_node]]
+        if ids[0] == ids[1]:
+            return
+        to_nodes = self.graph.setdefault(ids[0], [])
+        if ids[1] not in to_nodes:  # yeah it's a list but short
+            to_nodes.append(ids[1])
+        self.assert_acyclic()
+        log.debug(f"Add edge {ids})")
+
+    def topsorted_ids(self) -> List[str]:
+        return toposort_flatten(self.graph)
+
+    def assert_acyclic(self) -> None:
+        try:
+            self.topsorted_ids()
+        except CircularDependencyError as e:
+            raise ValueError(
+                "Error while constructing dependency graph for DC management."
+            ) from e
+
+    @classmethod
+    def from_pipeline(cls, pipeline: Pipeline, debug: bool) -> _DependencyGraph:
+        graph = _DependencyGraph()
+        graph.debug = debug
+
+        def resolve(node: Any) -> Optional[_DependencyGraph.NodeType]:
+            if isinstance(node, Output) or isinstance(node, Component):
+                return node
+            if isinstance(node, Input):
+                input_dset = node._dset
+                if input_dset is None:
+                    return None
+                return resolve(input_dset)
+            if isinstance(node, PipelineParameter):
+                default_value = node.default_value
+                if default_value is None or default_value is node:
+                    # can't resolve this
+                    return None
+                return resolve(default_value)
+            return None
+
+        for subpipeline in pipeline._expand_pipeline_to_pipelines():
+            # For DC, we only need to adapt `Output` and `Component`
+            # components. The `Output`s of pipelines do not coincide
+            # with the `Output`s of components, hence we have to
+            # insert those into our dependency graph:
+            for output_name, output in subpipeline.outputs.items():
+                linked_output = subpipeline._outputs_mapping[output_name]
+                graph.add_edge(output, linked_output)
+            # However, it seems we can skip the pipeline inputs.
+
+        for component in pipeline._expand_pipeline_nodes():
+            for output in component.outputs.values():
+                graph.add_edge(output, component)
+            for input_ in component.inputs.values():
+                corresponding_node = resolve(input_)
+                if corresponding_node is not None:
+                    graph.add_edge(component, corresponding_node)
+        return graph
+
+    def determine_dc_nodes(self, dc_targets: List[str]) -> Set[str]:
+        """Determine which downstream components/outputs should be configured for DC.
+
+        Args:
+            dc_targets: known DC targets (used to determine which nodes
+               are already configured for DC)
+        Returns:
+            list of node ids for all nodes that should be configured for
+            dc (or have already been configured for dc)
+        """
+        should_use_dc: Set[str] = set()
+        for node_id in self.topsorted_ids():
+
+            # use dc, if upstream used dc
+            for dependency in self.graph.get(node_id, []):
+                if dependency in should_use_dc:
+                    should_use_dc.add(node_id)
+                    continue
+
+            item = self.nodes[node_id]
+
+            if not isinstance(item, Component):
+                # If users choose to move an output to iso datastore out of
+                # nowhere, we ignore this. We're only caring about cases where
+                # the (`apply_*` method caused the) run settings of components
+                # to be configured for DC - and fix downstream components.
+                continue
+
+            if not hasattr(item.runsettings, "target") or not isinstance(
+                item.runsettings.target, str
+            ):
+                # e.g. Scope components do not configure compute targets
+                # e.g. if `target` is a PipelineParameter, it returns None
+                # and no need to update
+                continue
+
+            if item.runsettings.target in dc_targets:
+                should_use_dc.add(node_id)
+
+        return should_use_dc
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `shrike-1.9.5/shrike/pipeline/telemetry_utils.py` & `shrike-2.0.0.dev0/shrike/pipeline/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.5/shrike/pipeline/testing/components.py` & `shrike-2.0.0.dev0/shrike/pipeline/testing/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,46 +2,50 @@
 # Licensed under the MIT license.
 
 """
 PyTest suite for testing if run.py is aligned with module specification:
 
 > Status: this code relates to the _recipe_ and is a _proposition_
 """
+import argparse
+import logging
 import os
 import sys
-from pathlib import Path
-import traceback
-import argparse
-from collections import namedtuple
-import warnings
 import pytest
+import traceback
 
 from ruamel import yaml
 
 from azure.ml.component._core._component_definition import (
     ComponentDefinition,
     ComponentType,
 )
 
 from shrike.pipeline.testing.importer import (
     import_and_test_class,
     dynamic_import_module,
 )
 
 
+log = logging.getLogger(__name__)
+
+
 def component_spec_yaml_exists_and_is_parsable(component_spec_path):
     """Checks component spec file"""
     assert os.path.isfile(
         component_spec_path
     ), f"Component spec file under path {component_spec_path} could not be found"
 
     # opens file for testing schema
     with open(component_spec_path, "r") as ifile:
         component_spec_content = ifile.read()
-        if "$schema: http://azureml/" in component_spec_content:
+        if (
+            "$schema: http://" in component_spec_content
+            or "$schema: https://" in component_spec_content
+        ):
             use_component_sdk = True
         else:
             use_component_sdk = False
 
     # Block unit tests from working with module sdk if not enabled
     if not os.environ.get("MODULE_SDK_ENABLE"):
         assert (
@@ -431,26 +435,26 @@
         component_spec (dict): module specification in yaml
         arg (list or str or dict) : argument specification
         output_script_arguments (list) : output
 
     Returns:
         list: output_script_arguments
     """
-    print(f"generate_component_arguments(spec, {arg}, ...)")
+    log.info(f"generate_component_arguments(spec, {arg}, ...)")
     if isinstance(arg, list):  # optional argument or root list
         for entry in arg:
             generate_component_arguments_componentsdk(
                 component_spec, entry, output_script_arguments
             )
     elif isinstance(arg, str) and arg.startswith("{"):
         io_key = arg.lstrip("{").rstrip("}")
         if io_key.startswith("inputs."):
             input_key = io_key[7:]
-            print("inputs keys: " + " ".join([key for key in component_spec.inputs]))
-            print(
+            log.info("inputs keys: " + " ".join([key for key in component_spec.inputs]))
+            log.info(
                 "parameter keys: "
                 + " ".join([key for key in component_spec.parameters])
             )
             if input_key in component_spec.inputs:
                 output_script_arguments.append(
                     str(
                         _generate_fake_input_arg_componentsdk(
@@ -468,15 +472,17 @@
                 )
             else:
                 raise Exception(
                     f"Input key {input_key} is neither an input or a parameter"
                 )
         elif io_key.startswith("outputs."):
             output_key = io_key[8:]
-            print("outputs keys: " + " ".join([key for key in component_spec.outputs]))
+            log.info(
+                "outputs keys: " + " ".join([key for key in component_spec.outputs])
+            )
             output_script_arguments.append(
                 str(
                     _generate_fake_input_arg_componentsdk(
                         component_spec.outputs[output_key]
                     )
                 )
             )
@@ -668,14 +674,14 @@
         module_spec["jobType"].lower() != "scopecomponent"
         and module_spec["jobType"].lower() != "datatransfercomponent"
     ):
         arguments_spec = module_spec["implementation"]["container"]["args"]
     script_arguments = []
     generate_argument(module_spec, arguments_spec, script_arguments)
 
-    print(script_arguments)
+    log.info(script_arguments)
     # https://medium.com/python-pandemonium/testing-sys-exit-with-pytest-10c6e5f7726f
     with pytest.raises(SystemExit) as pytest_wrapped_e:
         mod.main(script_arguments + ["-h"])
 
     assert pytest_wrapped_e.type == SystemExit
     assert pytest_wrapped_e.value.code == 0
```

### Comparing `shrike-1.9.5/shrike/pipeline/testing/importer.py` & `shrike-2.0.0.dev0/shrike/pipeline/testing/importer.py`

 * *Files identical despite different names*

### Comparing `shrike-1.9.5/shrike/pipeline/testing/module_run_tests.py` & `shrike-2.0.0.dev0/shrike/pipeline/testing/module_run_tests.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
 """
 PyTest suite for testing if run.py is aligned with module specification:
 """
 import os
-import sys
-from pathlib import Path
-import traceback
-import argparse
-from collections import namedtuple
-import warnings
-import pytest
-
-from ruamel import yaml
-from azure.ml.component._core._component_definition import CommandComponentDefinition
 
 from shrike.pipeline.testing.importer import (
     import_and_test_class,
     dynamic_import_module,
 )
 from shrike.pipeline.testing.components import (
     component_spec_yaml_exists_and_is_parsable,
```

### Comparing `shrike-1.9.5/shrike/pipeline/testing/pipeline_class_test.py` & `shrike-2.0.0.dev0/shrike/pipeline/testing/pipeline_class_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT license.
 
 """
 PyTest suite for testing all module specification:
 """
-import traceback
-import pytest
 import json
 import os
+import logging
+import traceback
+
+from shrike.pipeline import AMLPipelineHelper
+
 
-from shrike.pipeline.pipeline_helper import AMLPipelineHelper
+log = logging.getLogger(__name__)
 
 
 def get_config_class(pipeline_class):
     """Test if the get_arg_parser() method is in there and behaves correctly"""
 
     try:
         config_class = pipeline_class.get_config_class()
@@ -135,36 +138,36 @@
         path (str): current path of the comparison (in the json tree)
 
     Returns:
         None
     """
     if definition is None:
         # no definition provided, let's stop inspection at this path
-        print(f"deeptest_graph @ {path}: nop, definition is None")
+        log.info(f"deeptest_graph @ {path}: nop, definition is None")
         return
 
     # is inspecting a dictionary structure, iterate on keys
     if isinstance(pipeline, dict) and isinstance(definition, dict):
-        print(f"deeptest_graph @ {path}: checking dictionary")
+        log.info(f"deeptest_graph @ {path}: checking dictionary")
         for key in definition:
             assert (
                 key in pipeline
             ), f"pipeline graph does not have key {key} at level @ {path}"
 
             # ignoring all ids
             if key in {"id", "node_id", "module_id", "dataset_id"}:
-                print(f"deeptest_graph @ {path}: ignore id key {key}")
+                log.info(f"deeptest_graph @ {path}: ignore id key {key}")
                 return
 
             if (
                 key in {"run_settings", "compute_run_settings"}
                 and definition[key] is not None
             ):
                 # this is a specific kind of key containing a list we're transforming into a dict
-                print(f"deeptest_graph @ {path}: refactoring key {key} as dict")
+                log.info(f"deeptest_graph @ {path}: refactoring key {key} as dict")
                 pipeline_run_settings = dict(
                     [(entry["name"], entry) for entry in pipeline[key]]
                 )
                 definition_run_settings = dict(
                     [(entry["name"], entry) for entry in definition[key]]
                 )
                 deeptest_graph(
@@ -175,15 +178,15 @@
             else:
                 deeptest_graph(pipeline[key], definition[key], path + "." + key)
         return
 
     # is inspecting a list structure, each element MUST passed
     # NOTE: this should be improved in case list can be shuffled ?
     if isinstance(pipeline, list) and isinstance(definition, list):
-        print(f"deeptest_graph @ {path}: checking list")
+        log.info(f"deeptest_graph @ {path}: checking list")
         for key, entry in enumerate(definition):
             deeptest_graph(pipeline[key], entry, path + "[" + str(key) + "]")
         return
 
     # if anything else (int, str, unknown), just test plain equality
-    print(f"deeptest_graph @ {path}: checking equality {pipeline} == {definition}")
+    log.info(f"deeptest_graph @ {path}: checking equality {pipeline} == {definition}")
     assert pipeline == definition, f"values mismatch @ {path}"
```

### Comparing `shrike-1.9.5/shrike/spark/spark_net.py` & `shrike-2.0.0.dev0/shrike/spark/spark_net.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,16 @@
     raise PublicValueError(f"py_files do not contain {py_file_name}: {py_files}")
 
 
 def java_args(spark: SparkSession, args: List[str]):
     """
     Convert a Python list into the corresponding Java argument array.
     """
-    rv = SparkContext._gateway.new_array(spark._jvm.java.lang.String, len(args))
+    s = spark._jvm.java.lang.String  # type: ignore
+    rv = SparkContext._gateway.new_array(s, len(args))  # type: ignore
 
     # https://stackoverflow.com/a/522578
     for index, arg in enumerate(args):
         rv[index] = arg
 
     return rv
 
@@ -100,15 +101,15 @@
         f"Calling dotnet with arguments: {dotnet_args}", category=DataCategory.PUBLIC
     )
     dotnet_args_java = java_args(spark, dotnet_args)
 
     message = None
 
     try:
-        spark._jvm.org.apache.spark.deploy.dotnet.DotnetRunner.main(dotnet_args_java)
+        spark._jvm.org.apache.spark.deploy.dotnet.DotnetRunner.main(dotnet_args_java)  # type: ignore  # noqa
     except py4j.protocol.Py4JJavaError as err:
         log.error("Dotnet failed", category=DataCategory.PUBLIC)
         for line in err.java_exception.getStackTrace():
             log.error(str(line), category=DataCategory.PUBLIC)
 
         message = f"{err.errmsg} {err.java_exception}"
```

