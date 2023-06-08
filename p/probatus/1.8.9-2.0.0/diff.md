# Comparing `tmp/probatus-1.8.9.tar.gz` & `tmp/probatus-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probatus-1.8.9.tar", last modified: Mon Apr 11 11:35:00 2022, max compression
+gzip compressed data, was "probatus-2.0.0.tar", last modified: Thu Jun  8 12:53:18 2023, max compression
```

## Comparing `probatus-1.8.9.tar` & `probatus-2.0.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.322018 probatus-1.8.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-04-11 11:31:43.000000 probatus-1.8.9/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     3236 2022-04-11 11:35:00.322018 probatus-1.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-04-11 11:31:43.000000 probatus-1.8.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.318018 probatus-1.8.9/probatus/
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.318018 probatus-1.8.9/probatus/binning/
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16891 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/binning/binning.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.318018 probatus-1.8.9/probatus/feature_elimination/
--rw-r--r--   0 runner    (1001) docker     (121)     1210 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/feature_elimination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    55750 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/feature_elimination/feature_elimination.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.318018 probatus-1.8.9/probatus/interpret/
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20790 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/interpret/inspector.py
--rw-r--r--   0 runner    (1001) docker     (121)    18851 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/interpret/model_interpret.py
--rw-r--r--   0 runner    (1001) docker     (121)    14050 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/interpret/shap_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.318018 probatus-1.8.9/probatus/metric_volatility/
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/metric_volatility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4723 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/metric_volatility/metric.py
--rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/metric_volatility/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    30005 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/metric_volatility/volatility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.318018 probatus-1.8.9/probatus/missing_values/
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/missing_values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15575 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/missing_values/imputation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.318018 probatus-1.8.9/probatus/sample_similarity/
--rw-r--r--   0 runner    (1001) docker     (121)     1338 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/sample_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28535 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/sample_similarity/resemblance_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.318018 probatus-1.8.9/probatus/stat_tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/stat_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2687 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/stat_tests/ad.py
--rw-r--r--   0 runner    (1001) docker     (121)    17120 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/stat_tests/distribution_statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/stat_tests/es.py
--rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/stat_tests/ks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5692 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/stat_tests/psi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3584 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/stat_tests/sw.py
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/stat_tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.322018 probatus-1.8.9/probatus/utils/
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1860 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10237 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/utils/arrayfuncs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3445 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2245 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/utils/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/utils/missing_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3591 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (121)     5723 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/utils/scoring.py
--rw-r--r--   0 runner    (1001) docker     (121)     7459 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/utils/shap_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-04-11 11:31:43.000000 probatus-1.8.9/probatus/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.318018 probatus-1.8.9/probatus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3236 2022-04-11 11:34:59.000000 probatus-1.8.9/probatus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-04-11 11:35:00.000000 probatus-1.8.9/probatus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-11 11:34:59.000000 probatus-1.8.9/probatus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-11 11:33:19.000000 probatus-1.8.9/probatus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-04-11 11:34:59.000000 probatus-1.8.9/probatus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-11 11:35:00.000000 probatus-1.8.9/probatus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-11 11:35:00.322018 probatus-1.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2568 2022-04-11 11:31:43.000000 probatus-1.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.318018 probatus-1.8.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.322018 probatus-1.8.9/tests/binning/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/binning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10040 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/binning/test_binning.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.322018 probatus-1.8.9/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/docs/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (121)     1576 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/docs/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.322018 probatus-1.8.9/tests/interpret/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    34609 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/interpret/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (121)    10313 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/interpret/test_model_interpret.py
--rw-r--r--   0 runner    (1001) docker     (121)     5858 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/interpret/test_shap_dependence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.322018 probatus-1.8.9/tests/metric_volatility/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/metric_volatility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12382 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/metric_volatility/test_metric_volatility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.322018 probatus-1.8.9/tests/sample_similarity/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/sample_similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9098 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/sample_similarity/test_resemblance_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.322018 probatus-1.8.9/tests/stat_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/stat_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9862 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/stat_tests/test_distribution_statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/stat_tests/test_stat_tests.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/stat_tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 11:35:00.322018 probatus-1.8.9/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7750 2022-04-11 11:31:43.000000 probatus-1.8.9/tests/utils/test_utils_array_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-08 12:49:29.000000 probatus-2.0.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-08 12:53:18.690420 probatus-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-08 12:49:29.000000 probatus-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/binning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/binning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16871 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/binning/binning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/feature_elimination/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/feature_elimination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57143 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/feature_elimination/feature_elimination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/interpret/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/interpret/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/interpret/model_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/interpret/shap_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/metric_volatility/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/metric_volatility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/metric_volatility/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/metric_volatility/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29943 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/metric_volatility/volatility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus/missing_values/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/missing_values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/missing_values/imputation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.686421 probatus-2.0.0/probatus/sample_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/sample_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28520 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/sample_similarity/resemblance_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.686421 probatus-2.0.0/probatus/stat_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/distribution_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/ks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/psi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/sw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/stat_tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.686421 probatus-2.0.0/probatus/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/arrayfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/missing_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/shap_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-08 12:49:29.000000 probatus-2.0.0/probatus/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.682420 probatus-2.0.0/probatus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-08 12:53:18.000000 probatus-2.0.0/probatus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-08 12:53:18.000000 probatus-2.0.0/probatus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:53:18.000000 probatus-2.0.0/probatus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:49:50.000000 probatus-2.0.0/probatus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-08 12:53:18.000000 probatus-2.0.0/probatus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 12:53:18.000000 probatus-2.0.0/probatus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:53:18.690420 probatus-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-08 12:49:29.000000 probatus-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.678420 probatus-2.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.686421 probatus-2.0.0/tests/binning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/binning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/binning/test_binning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.686421 probatus-2.0.0/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/docs/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/docs/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/tests/interpret/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/interpret/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/interpret/test_model_interpret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/interpret/test_shap_dependence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/tests/metric_volatility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/metric_volatility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/metric_volatility/test_metric_volatility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/tests/sample_similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/sample_similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/sample_similarity/test_resemblance_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/tests/stat_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/stat_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/stat_tests/test_distribution_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/stat_tests/test_stat_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/stat_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:53:18.690420 probatus-2.0.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-06-08 12:49:29.000000 probatus-2.0.0/tests/utils/test_utils_array_funcs.py
```

### Comparing `probatus-1.8.9/LICENCE` & `probatus-2.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/PKG-INFO` & `probatus-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: probatus
-Version: 1.8.9
+Version: 2.0.0
 Summary: Validation of binary classifiers and data used to develop them
 Home-page: https://github.com/ing-bank/probatus
 Author: ING Bank N.V.
 Author-email: mateusz.garbacz@ing.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 Provides-Extra: all
 License-File: LICENCE
 
 <img src="https://github.com/ing-bank/probatus/raw/main/docs/img/logo_large.png" width="120" align="right">
 
 [![pytest](https://github.com/ing-bank/probatus/workflows/Development/badge.svg)](https://github.com/ing-bank/probatus/actions?query=workflow%3A%22Development%22)
 [![PyPi Version](https://img.shields.io/pypi/pyversions/probatus)](#)
 [![PyPI](https://img.shields.io/pypi/v/probatus)](#)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/probatus)](#)
 ![GitHub contributors](https://img.shields.io/github/contributors/ing-bank/probatus)
 
-# probatus
+# Probatus
 
 ## Overview
 
 **Probatus** is a python package that helps validate binary classification models and the data used to develop them. Main features:
 
-- [probatus.interpret](https://ing-bank.github.io/probatus/api/model_interpret.html) provides shap-based model interpretation tools 
+- [probatus.interpret](https://ing-bank.github.io/probatus/api/model_interpret.html) provides shap-based model interpretation tools
 - [probatus.metric_volatility](https://ing-bank.github.io/probatus/api/metric_volatility.html) provides tools using bootstrapping and/or different random seeds to assess metric volatility/stability.
 - [probatus.sample_similarity](https://ing-bank.github.io/probatus/api/sample_similarity.html) to compare two datasets using resemblance modelling, f.e. `train` with out-of-time `test`.
 - [probatus.feature_elimination.ShapRFECV](https://ing-bank.github.io/probatus/api/feature_elimination.html) provides cross-validated Recursive Feature Elimination using shap feature importance.
 - [probatus.missing_values](https://ing-bank.github.io/probatus/api/imputation_selector.html) compares performance gains of different missing values imputation strategies for a given model.
 
 ## Installation
 
@@ -50,17 +49,15 @@
 pip install probatus
 ```
 
 ## Documentation
 
 Documentation at [ing-bank.github.io/probatus/](https://ing-bank.github.io/probatus/).
 
-You can also check out blog posts about Probatus: 
+You can also check out blog posts about Probatus:
 
 -  [Open-sourcing ShapRFECV — Improved feature selection powered by SHAP.](https://medium.com/ing-blog/open-sourcing-shaprfecv-improved-feature-selection-powered-by-shap-994fe7861560)
 -  [Model Explainability — How to choose the right tool?](https://medium.com/ing-blog/model-explainability-how-to-choose-the-right-tool-6c5eabd1a46a)
 
 ## Contributing
 
-To learn more about making a contribution to probatus, please see [`CONTRIBUTING.md`](CONTRIBUTING.md).
-
-
+To learn more about making a contribution to Probatus, please see [`CONTRIBUTING.md`](CONTRIBUTING.md).
```

### Comparing `probatus-1.8.9/README.md` & `probatus-2.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 [![pytest](https://github.com/ing-bank/probatus/workflows/Development/badge.svg)](https://github.com/ing-bank/probatus/actions?query=workflow%3A%22Development%22)
 [![PyPi Version](https://img.shields.io/pypi/pyversions/probatus)](#)
 [![PyPI](https://img.shields.io/pypi/v/probatus)](#)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/probatus)](#)
 ![GitHub contributors](https://img.shields.io/github/contributors/ing-bank/probatus)
 
-# probatus
+# Probatus
 
 ## Overview
 
 **Probatus** is a python package that helps validate binary classification models and the data used to develop them. Main features:
 
-- [probatus.interpret](https://ing-bank.github.io/probatus/api/model_interpret.html) provides shap-based model interpretation tools 
+- [probatus.interpret](https://ing-bank.github.io/probatus/api/model_interpret.html) provides shap-based model interpretation tools
 - [probatus.metric_volatility](https://ing-bank.github.io/probatus/api/metric_volatility.html) provides tools using bootstrapping and/or different random seeds to assess metric volatility/stability.
 - [probatus.sample_similarity](https://ing-bank.github.io/probatus/api/sample_similarity.html) to compare two datasets using resemblance modelling, f.e. `train` with out-of-time `test`.
 - [probatus.feature_elimination.ShapRFECV](https://ing-bank.github.io/probatus/api/feature_elimination.html) provides cross-validated Recursive Feature Elimination using shap feature importance.
 - [probatus.missing_values](https://ing-bank.github.io/probatus/api/imputation_selector.html) compares performance gains of different missing values imputation strategies for a given model.
 
 ## Installation
 
@@ -24,15 +24,15 @@
 pip install probatus
 ```
 
 ## Documentation
 
 Documentation at [ing-bank.github.io/probatus/](https://ing-bank.github.io/probatus/).
 
-You can also check out blog posts about Probatus: 
+You can also check out blog posts about Probatus:
 
 -  [Open-sourcing ShapRFECV — Improved feature selection powered by SHAP.](https://medium.com/ing-blog/open-sourcing-shaprfecv-improved-feature-selection-powered-by-shap-994fe7861560)
 -  [Model Explainability — How to choose the right tool?](https://medium.com/ing-blog/model-explainability-how-to-choose-the-right-tool-6c5eabd1a46a)
 
 ## Contributing
 
-To learn more about making a contribution to probatus, please see [`CONTRIBUTING.md`](CONTRIBUTING.md).
+To learn more about making a contribution to Probatus, please see [`CONTRIBUTING.md`](CONTRIBUTING.md).
```

### Comparing `probatus-1.8.9/probatus/__init__.py` & `probatus-2.0.0/probatus/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/binning/__init__.py` & `probatus-2.0.0/probatus/binning/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/binning/binning.py` & `probatus-2.0.0/probatus/binning/binning.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,31 +14,29 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-import pandas as pd
+import warnings
+from abc import abstractmethod
+
 import numpy as np
+import pandas as pd
 from sklearn.cluster import AgglomerativeClustering
 from sklearn.tree import DecisionTreeClassifier, _tree
 from sklearn.utils.validation import check_is_fitted
-from probatus.utils import (
-    assure_numpy_array,
-    ApproximationWarning,
-    BaseFitComputeClass,
-)
-import warnings
-from abc import abstractmethod
+
+from probatus.utils import ApproximationWarning, BaseFitComputeClass, assure_numpy_array
 
 
 class Bucketer(BaseFitComputeClass):
     """
-    Bucket (bin) some datea.
+    Bucket (bin) some data.
     """
 
     def __repr__(self):
         """
         String representation.
         """
         repr_ = f"{self.__class__.__name__}\n\tbincount: {self.bin_count}"
@@ -282,15 +280,15 @@
     def quantile_bins(x, bin_count, inf_edges=True):
         """
         Bins.
         """
         try:
             out, boundaries = pd.qcut(x, q=bin_count, retbins=True, duplicates="raise")
         except ValueError:
-            # If there are too many duplicate values (assume a lot of filled missings)
+            # If there are too many duplicate values (assume a lot of filled missing)
             # this crashes - the exception drops them.
             # This means that it will return approximate quantile bins
             out, boundaries = pd.qcut(x, q=bin_count, retbins=True, duplicates="drop")
             warnings.warn(
                 ApproximationWarning(
                     f"Unable to calculate quantile bins for this feature, because possibly "
                     f"there is too many duplicate values.Approximated quantiles, as a result,"
@@ -346,21 +344,21 @@
     myBucketer.boundaries gives the boundaries of the buckets
 
     Args:
         inf_edges (boolean): Flag to keep the lower and upper boundary as infinite (if set to True).
         If false, the edges will be set to the minimum and maximum value of the fitted
 
         tree (sklearn.tree.DecisionTreeClassifier): decision tree object defined by the user. By default is None, and
-        it will be constructed using tkhe provided **kwargs
+        it will be constructed using the provided **kwargs
 
         **tree_kwargs: kwargs related to the decision tree.
-            For and extensive list of parameteres, please check the sklearn Decision Tree Classifier documentation
+            For and extensive list of parameters, please check the sklearn Decision Tree Classifier documentation
             https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html
 
-            The most relevant parameteres useful for the bucketing, are listed below:
+            The most relevant parameters useful for the bucketing, are listed below:
 
 
                 - criterion : {"gini", "entropy"}, default="gini"
                     The function to measure the quality of a split. Supported criteria are
                     "gini" for the Gini impurity and "entropy" for the information gain.
```

### Comparing `probatus-1.8.9/probatus/feature_elimination/__init__.py` & `probatus-2.0.0/probatus/feature_elimination/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/feature_elimination/feature_elimination.py` & `probatus-2.0.0/probatus/feature_elimination/feature_elimination.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                 order to reach min_features_to_select.
                 If columns_to_keep parameter is specified in the fit method, step is the number of features to remove after
                 keeping those columns.
 
             min_features_to_select (int, optional):
                 Minimum number of features to be kept. This is a stopping criterion of the feature elimination. By
                 default the process stops when one feature is left. If columns_to_keep is specified in the fit method,
-                it may overide this parameter to the maximum between length of columns_to_keep the two.
+                it may override this parameter to the maximum between length of columns_to_keep the two.
 
             cv (int, cross-validation generator or an iterable, optional):
                 Determines the cross-validation splitting strategy. Compatible with sklearn
                 [cv parameter](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.RFECV.html).
                 If None, then cv of 5 is used.
 
             scoring (string or probatus.utils.Scorer, optional):
@@ -401,14 +401,15 @@
     def fit(
         self,
         X,
         y,
         sample_weight=None,
         columns_to_keep=None,
         column_names=None,
+        groups=None,
         **shap_kwargs,
     ):
         """
         Fits the object with the provided data.
 
         The algorithm starts with the entire dataset, and then sequentially
              eliminates features. If sklearn compatible search CV is passed as clf e.g.
@@ -439,14 +440,20 @@
                 However, these feature will used for the calculation of the SHAP values.
 
             column_names (list of str, optional):
                 List of feature names of the provided samples. If provided it will be used to overwrite the existing
                 feature names. If not provided the existing feature names are used or default feature names are
                 generated.
 
+            groups (pd.Series, np.ndarray, list, optional):
+                array-like of shape (n_samples,)
+                Group labels for the samples used while splitting the dataset into train/test set.
+                Only used in conjunction with a "Group" `cv` instance.
+                (e.g. `sklearn.model_selection.GroupKFold`).
+
             **shap_kwargs:
                 keyword arguments passed to
                 [shap.Explainer](https://shap.readthedocs.io/en/latest/generated/shap.Explainer.html#shap.Explainer).
                 It also enables `approximate` and `check_additivity` parameters, passed while calculating SHAP values.
                 The `approximate=True` causes less accurate, but faster SHAP values calculation, while
                 `check_additivity=False` disables the additivity check inside SHAP.
 
@@ -472,15 +479,15 @@
                 )
 
         # If the columns_to_keep parameter is provided, check if they match the column names in the X.
         if column_names is not None:
             if all(x in column_names for x in list(X.columns)):
                 pass
             else:
-                raise (ValueError("The column names in parameter columns_to_keep and column_names are not macthing."))
+                raise (ValueError("The column names in parameter columns_to_keep and column_names are not matching."))
 
         # Check that the total number of columns to select is less than total number of columns in the data.
         # only when both parameters are provided.
         if column_names is not None and columns_to_keep is not None:
             if (self.min_features_to_select + len_columns_to_keep) > len(self.column_names):
                 raise ValueError(
                     "Minimum features to select is greater than number of features."
@@ -515,17 +522,20 @@
 
         while len(current_features_set) > stopping_criteria:
             round_number += 1
 
             # Get current dataset info
             current_features_set = remaining_features
             if columns_to_keep is None:
-                remaining_removeable_features = list(set(current_features_set))
+                # Keeps the original order, while removing duplicate elements
+                remaining_removeable_features = pd.Series(current_features_set).unique()
             else:
-                remaining_removeable_features = list(set(current_features_set) | set(columns_to_keep))
+                # Keeps the original order, while removing duplicate elements
+                remaining_removeable_features = pd.Series(list(current_features_set) + columns_to_keep).unique()
+
             current_X = self.X[remaining_removeable_features]
 
             # Set seed for results reproducibility
             if self.random_state is not None:
                 np.random.seed(self.random_state)
 
             # Optimize parameters
@@ -542,30 +552,36 @@
                     y=self.y,
                     clf=current_clf,
                     train_index=train_index,
                     val_index=val_index,
                     sample_weight=sample_weight,
                     **shap_kwargs,
                 )
-                for train_index, val_index in self.cv.split(current_X, self.y)
+                for train_index, val_index in self.cv.split(current_X, self.y, groups)
             )
 
             shap_values = np.vstack([current_result[0] for current_result in results_per_fold])
             scores_train = [current_result[1] for current_result in results_per_fold]
             scores_val = [current_result[2] for current_result in results_per_fold]
 
             # Calculate the shap features with remaining features and features to keep.
 
             shap_importance_df = calculate_shap_importance(shap_values, remaining_removeable_features)
 
             # Get features to remove
             features_to_remove = self._get_current_features_to_remove(
                 shap_importance_df, columns_to_keep=columns_to_keep
             )
-            remaining_features = list(set(current_features_set) - set(features_to_remove))
+            # Ensures the order of the first list is kept as it was originally,
+            # while removing elements which are present in both lists.
+            remaining_features = np.setdiff1d(
+                pd.Series(current_features_set).unique(),
+                pd.Series(features_to_remove).unique(),
+                assume_unique=True,
+            )
 
             # Report results
             self._report_current_results(
                 round_number=round_number,
                 current_features_set=current_features_set,
                 features_to_remove=features_to_remove,
                 train_metric_mean=np.round(np.mean(scores_train), 3),
@@ -586,15 +602,15 @@
         self.fitted = True
         return self
 
     def compute(self):
         """
         Checks if fit() method has been run.
 
-        and computes the DataFrame with results of feature elimintation for each round.
+        and computes the DataFrame with results of feature elimination for each round.
 
         Returns:
             (pd.DataFrame):
                 DataFrame with results of feature elimination for each round.
         """
         self._check_if_fitted()
 
@@ -857,15 +873,15 @@
                 order to reach min_features_to_select.
                 If columns_to_keep parameter is specified in the fit method, step is the number of features to remove after
                 keeping those columns.
 
             min_features_to_select (int, optional):
                 Minimum number of features to be kept. This is a stopping criterion of the feature elimination. By
                 default the process stops when one feature is left. If columns_to_keep is specified in the fit method,
-                it may overide this parameter to the maximum between length of columns_to_keep the two.
+                it may override this parameter to the maximum between length of columns_to_keep the two.
 
             cv (int, cross-validation generator or an iterable, optional):
                 Determines the cross-validation splitting strategy. Compatible with sklearn
                 [cv parameter](https://scikit-learn.org/stable/modules/generated/sklearn.feature_selection.RFECV.html).
                 If None, then cv of 5 is used.
 
             scoring (string or probatus.utils.Scorer, optional):
@@ -898,15 +914,15 @@
             eval_metric (str, optional):
                 Metric for scoring fitting rounds and activating early stopping. This is passed to the
                 fit method of the model for Shapley values estimation, but not for hyperparameter search. Only
                 supported by some models, such as [XGBoost](https://xgboost.readthedocs.io/en/latest/parameter.html#learning-task-parameters)
                  and [LightGBM](https://lightgbm.readthedocs.io/en/latest/Parameters.html#metric-parameters).
                 Note that `eval_metric` is an argument of the model's fit method and it is different from `scoring`.
         """  # noqa
-        super(EarlyStoppingShapRFECV, self).__init__(
+        super().__init__(
             clf,
             step=step,
             min_features_to_select=min_features_to_select,
             cv=cv,
             scoring=scoring,
             n_jobs=n_jobs,
             verbose=verbose,
@@ -974,15 +990,14 @@
         """
         from lightgbm import early_stopping, log_evaluation
 
         fit_params = {
             "X": X_train,
             "y": y_train,
             "eval_set": [(X_val, y_val)],
-            "eval_metric": self.eval_metric,
             "callbacks": [early_stopping(self.early_stopping_rounds, first_metric_only=True)],
         }
         if self.verbose >= 100:
             fit_params["callbacks"].append(log_evaluation(1))
         else:
             fit_params["callbacks"].append(log_evaluation(0))
         if sample_weight is not None:
@@ -1028,16 +1043,14 @@
         Returns:
             dict: fit parameters
         """
         fit_params = {
             "X": X_train,
             "y": y_train,
             "eval_set": [(X_val, y_val)],
-            "eval_metric": self.eval_metric,
-            "early_stopping_rounds": self.early_stopping_rounds,
         }
         if sample_weight is not None:
             fit_params["sample_weight"] = sample_weight.iloc[train_index]
             fit_params["eval_sample_weight"] = [sample_weight.iloc[val_index]]
         return fit_params
 
     def _get_fit_params_CatBoost(
@@ -1080,15 +1093,14 @@
         """
         from catboost import Pool
 
         cat_features = [col for col in X_train.select_dtypes(include=["category"]).columns]
         fit_params = {
             "X": Pool(X_train, y_train, cat_features=cat_features),
             "eval_set": Pool(X_val, y_val, cat_features=cat_features),
-            "early_stopping_rounds": self.early_stopping_rounds,
             # Evaluation metric should be passed during initialization
         }
         if sample_weight is not None:
             fit_params["X"].set_weight(sample_weight.iloc[train_index])
             fit_params["eval_set"].set_weight(sample_weight.iloc[val_index])
         return fit_params
 
@@ -1233,14 +1245,40 @@
             X_val=X_val,
             y_val=y_val,
             sample_weight=sample_weight,
             train_index=train_index,
             val_index=val_index,
         )
 
+        # Due to deprecation issues (compatibility with Sklearn) set some params
+        # like below, instead of through fit().
+        try:
+            from lightgbm import LGBMModel
+
+            if isinstance(clf, LGBMModel):
+                clf.set_params(eval_metric=self.eval_metric)
+        except ImportError:
+            pass
+
+        try:
+            from xgboost.sklearn import XGBModel
+
+            if isinstance(clf, XGBModel):
+                clf.set_params(eval_metric=self.eval_metric, early_stopping_rounds=self.early_stopping_rounds)
+        except ImportError:
+            pass
+
+        try:
+            from catboost import CatBoost
+
+            if isinstance(clf, CatBoost):
+                clf.set_params(early_stopping_rounds=self.early_stopping_rounds)
+        except ImportError:
+            pass
+
         # Train the model
         clf = clf.fit(**fit_params)
 
         # Score the model
         score_train = self.scorer.scorer(clf, X_train, y_train)
         score_val = self.scorer.scorer(clf, X_val, y_val)
```

### Comparing `probatus-1.8.9/probatus/interpret/__init__.py` & `probatus-2.0.0/probatus/interpret/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/interpret/inspector.py` & `probatus-2.0.0/probatus/interpret/inspector.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from ..utils import NotFittedError, UnsupportedModelError, BaseFitComputeClass
-import numpy as np
-import pandas as pd
 import copy
 
+import numpy as np
+import pandas as pd
 from sklearn.cluster import KMeans
+
 from probatus.utils import shap_helpers
 
+from ..utils import BaseFitComputeClass, NotFittedError, UnsupportedModelError
+
 
 def return_confusion_metric(y_true, y_score, normalize=False):
     """
     Computes a confusion metric as absolute difference between the y_true and y_score.
 
     If normalize is set to true, it will normalize y_score to the maximum value in the array
 
@@ -54,29 +56,26 @@
     """
 
     def __init__(self, algotype, **kwargs):
         """
         Init.
         """
         self.algotype = algotype
-        # TODO fix compilatiopn issue on  for hdbscan
-        # if algotype =='dbscan':
-        #     self.clusterer = hdbscan.HDBSCAN(prediction_data=True,**kwargs)
         if algotype == "kmeans":
             self.clusterer = KMeans(**kwargs)
         else:
-            raise UnsupportedModelError("The algorithm {} is not supported".format(algotype))
+            raise UnsupportedModelError(f"The algorithm {algotype} is not supported")
 
     def __repr__(self):
         """
         String representation.
         """
-        repr_ = "{},\n\t{}".format(self.__class__.__name__, self.algotype)
+        repr_ = f"{self.__class__.__name__},\n\t{self.algotype}"
         if self.fitted:
-            repr_ += "\n\tTotal clusters {}".format(np.unique(self.clusterer.labels_).shape[0])
+            repr_ += f"\n\tTotal clusters {np.unique(self.clusterer.labels_).shape[0]}"
         return repr_
 
     def fit_clusters(self, X):
         """
         Perform the fit of the clusters with the algorithm specified in the constructor.
 
         Args:
@@ -128,51 +127,51 @@
             return series
         elif isinstance(series, pd.DataFrame) and series.shape[1] == 1:
             return pd.Series(series.values.ravel(), index=series.index)
         elif isinstance(series, np.ndarray) and len(series.shape) == 1 and index is not None:
             return pd.Series(series, index=index)
         else:
             raise TypeError(
-                "The object should be a pd.Series, a dataframe with one collumn or a 1 dimensional numpy array"
+                "The object should be a pd.Series, a dataframe with one column or a 1 dimensional numpy array"
             )
 
 
 class InspectorShap(BaseInspector):
     """
     Class to perform inspection of the model prediction based on Shapley values.
 
-    It uses the calculated Shapley values for the train model to build clusters in the shap space.
+    It uses the calculated Shapley values for the train model to build clusters in the SHAP space.
     For each cluster, an average confusion, average predicted probability and observed rate of a single class is
     calculated.
     Every sub cluster can be retrieved with the function slice_cluster to perform deeper analysis.
 
     The original dataframe indexing is used in slicing the dataframe, ensuring easy filtering
 
     Args:
             model: (obj) pretrained model (with sklearn-like API)
             algotype: (str) clustering algorithm (supported are kmeans and hdbscan)
             confusion_metric: (str) Confusion metric to use:
                 - "proba": it will calculate the confusion metric as the absolute value of the target minus
                     the predicted probability. This provides a continuous measure of confusion, where 0 indicated
                     correct predictions and the closer the number is to 1, the higher the confusion
-            normalize_probability: (boolean) if true, it will normalize the probabilities to the max value when computing
-                the confusion metric
+            normalize_probability: (boolean) if true, it will normalize the probabilities to the max value when
+                computing the confusion metric
             cluster_probabilities: (boolean) if true, uses the model prediction as an input for the cluster prediction
             **kwargs: keyword arguments for the clustering algorithm
 
-    """  # noqa
+    """
 
     def __init__(
         self,
         model,
         algotype="kmeans",
         confusion_metric="proba",
         normalize_probability=False,
         cluster_probability=False,
-        **kwargs
+        **kwargs,
     ):
         """
         Init.
         """
         super().__init__(algotype, **kwargs)
         self.model = model
         self.isinspected = False
@@ -187,23 +186,23 @@
         self.predicted_proba = None
         self.X_shap = None
         self.clusters = None
         self.init_eval_set_report_variables()
 
         if confusion_metric not in ["proba"]:
             # TODO implement the target method
-            raise NotImplementedError("confusion metric {} not supported. See docstrings".format(confusion_metric))
+            raise NotImplementedError(f"confusion metric {confusion_metric} not supported. See docstrings")
 
     def __repr__(self):
         """
         String representation.
         """
-        repr_ = "{},\n\t{}".format(self.__class__.__name__, self.algotype)
+        repr_ = f"{self.__class__.__name__},\n\t{self.algotype}"
         if self.fitted:
-            repr_ += "\n\tTotal clusters {}".format(np.unique(self.clusterer.labels_).shape[0])
+            repr_ += f"\n\tTotal clusters {np.unique(self.clusterer.labels_).shape[0]}"
         return repr_
 
     def init_eval_set_report_variables(self):
         """
         Init report values.
         """
         self.X_shaps = list()
@@ -329,15 +328,14 @@
         """
         self.summary_df = self.create_summary_df(
             self.clusters, self.y, self.predicted_proba, normalize=self.normalize_proba
         )
         self.agg_summary_df = self.aggregate_summary_df(self.summary_df)
 
         if self.hasmultiple_dfs:
-
             self.summary_dfs = [
                 self.create_summary_df(clust, y, pred_proba, normalize=self.normalize_proba)
                 for clust, y, pred_proba in zip(self.clusters_list, self.ys, self.predicted_probas)
             ]
 
             self.agg_summary_dfs = [self.aggregate_summary_df(df) for df in self.summary_dfs]
 
@@ -346,43 +344,42 @@
         Calculates a report containing the information per cluster.
 
         Includes the following:
             - cluster id
             - total number of observations in the cluster
             - total number of target 1 in the cluster
             - target 1 rate (ration of target 1 counts/observations)
-            - average predicted probabilitites
+            - average predicted probabilities
             - average confusion
 
-        If multiple eval_sets were passed in the inspect() functions, the output will contain those aggregations as well.
-        The output names will use the sample names provided in the inspect function. Otherwise they will be labelled by
-        the suffix sample_{i}, where i is the index of the sample
+        If multiple eval_sets were passed in the inspect() functions, the output will contain those aggregations as
+            well. The output names will use the sample names provided in the inspect function. Otherwise they will be
+            labelled by the suffix sample_{i}, where i is the index of the sample.
 
         Returns: (pd.DataFrame) with above mentioned aggregations.
         """
         if self.cluster_report is not None:
             return self.cluster_report
 
         self._compute_report()
         out = copy.deepcopy(self.agg_summary_df)
 
         if self.hasmultiple_dfs:
-
             for ix, agg_summary_df in enumerate(self.agg_summary_dfs):
                 if self.set_names is None:
-                    sample_suffix = "sample_{}".format(ix + 1)
+                    sample_suffix = f"sample_{ix + 1}"
                 else:
                     sample_suffix = self.set_names[ix]
 
                 out = pd.merge(
                     out,
                     agg_summary_df,
                     how="left",
                     on="cluster_id",
-                    suffixes=("", "_{}".format(sample_suffix)),
+                    suffixes=("", f"_{sample_suffix}"),
                 )
 
         self.cluster_report = out
         return self.cluster_report
 
     def slice_cluster(
         self,
@@ -529,17 +526,17 @@
 
         Args:
             X: (pd.DataFrame) with the features set used to train the model
             y: (pd.Series, default=None): targets used to train the model
             eval_set: (list, default=None). list of tuples in the shape (X,y) containing evaluation samples, for example
                 a test sample, validation sample etc... X corresponds to the feature set of the sample, y corresponds
                 to the targets of the samples
-            sample_names: (list of strings, default=None): list of suffixed for the samples. If none, it will be labelled with
-                sample_{i}, where i corresponds to the index of the sample.
+            sample_names: (list of strings, default=None): list of suffixed for the samples. If none, it will be
+                labelled with sample_{i}, where i corresponds to the index of the sample.
                 List length must match that of eval_set
             **shap_kwargs:  kwargs to pass to the Shapley Tree Explained
 
         Returns:
             (pd.DataFrame) Report with aggregations described in compute() method.
-        """  # noqa
+        """
         self.fit(X, y, eval_set, sample_names, **shap_kwargs)
         return self.compute()
```

### Comparing `probatus-1.8.9/probatus/interpret/model_interpret.py` & `probatus-2.0.0/probatus/interpret/model_interpret.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+from shap import summary_plot
+from shap.plots._waterfall import waterfall_legacy
+
 from probatus.interpret import DependencePlotter
 from probatus.utils import (
-    preprocess_data,
-    preprocess_labels,
-    shap_calc,
-    calculate_shap_importance,
     BaseFitComputePlotClass,
     assure_list_of_strings,
+    calculate_shap_importance,
     get_single_scorer,
+    preprocess_data,
+    preprocess_labels,
+    shap_calc,
 )
-import numpy as np
-from shap import summary_plot
-from shap.plots._waterfall import waterfall_legacy
-import matplotlib.pyplot as plt
-import pandas as pd
 
 
 class ShapModelInterpreter(BaseFitComputePlotClass):
     """
     This class is a wrapper that allows to easily analyse a model's features.
 
     It allows us to plot SHAP feature importance,
@@ -154,25 +155,33 @@
         self.test_score = self.scorer.score(self.clf, self.X_test, self.y_test)
 
         self.results_text = (
             f"Train {self.scorer.metric_name}: {np.round(self.train_score, 3)},\n"
             f"Test {self.scorer.metric_name}: {np.round(self.test_score, 3)}."
         )
 
-        (self.shap_values_train, self.expected_value_train, self.tdp_train,) = self._prep_shap_related_variables(
+        (
+            self.shap_values_train,
+            self.expected_value_train,
+            self.tdp_train,
+        ) = self._prep_shap_related_variables(
             clf=self.clf,
             X=self.X_train,
             y=self.y_train,
             column_names=self.column_names,
             class_names=self.class_names,
             verbose=self.verbose,
             **shap_kwargs,
         )
 
-        (self.shap_values_test, self.expected_value_test, self.tdp_test,) = self._prep_shap_related_variables(
+        (
+            self.shap_values_test,
+            self.expected_value_test,
+            self.tdp_test,
+        ) = self._prep_shap_related_variables(
             clf=self.clf,
             X=self.X_test,
             y=self.y_test,
             column_names=self.column_names,
             class_names=self.class_names,
             verbose=self.verbose,
             **shap_kwargs,
```

### Comparing `probatus-1.8.9/probatus/interpret/shap_dependence.py` & `probatus-2.0.0/probatus/interpret/shap_dependence.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,24 +14,20 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-import pandas as pd
-import numpy as np
 import matplotlib.pyplot as plt
-from probatus.binning import SimpleBucketer, AgglomerativeBucketer, QuantileBucketer
-from probatus.utils import (
-    BaseFitComputePlotClass,
-    shap_to_df,
-    preprocess_data,
-    preprocess_labels,
-)
+import numpy as np
+import pandas as pd
+
+from probatus.binning import AgglomerativeBucketer, QuantileBucketer, SimpleBucketer
+from probatus.utils import BaseFitComputePlotClass, preprocess_data, preprocess_labels, shap_to_df
 
 
 class DependencePlotter(BaseFitComputePlotClass):
     """
     Plotter used to plot SHAP dependence plot together with the target rates.
 
     Currently it supports tree-based and linear models.
@@ -75,15 +71,15 @@
         self.clf = clf
         self.verbose = verbose
 
     def __repr__(self):
         """
         Represent string method.
         """
-        return "Shap dependence plotter for {}".format(self.clf.__class__.__name__)
+        return f"Shap dependence plotter for {self.clf.__class__.__name__}"
 
     def fit(self, X, y, column_names=None, class_names=None, precalc_shap=None, **shap_kwargs):
         """
         Fits the plotter to the model and data by computing the shap values.
 
         If the shap_values are passed, they do not need to be computed.
 
@@ -218,15 +214,15 @@
         if min_q >= max_q:
             raise ValueError("min_q must be smaller than max_q")
         if feature not in self.X.columns:
             raise ValueError("Feature not recognized")
         if type_binning not in ["simple", "agglomerative", "quantile"]:
             raise ValueError("Select one of the following binning methods: 'simple', 'agglomerative', 'quantile'")
         if (alpha < 0) or (alpha > 1):
-            raise ValueError("alpha must be a float value betwee 0 and 1")
+            raise ValueError("alpha must be a float value between 0 and 1")
 
         self.min_q, self.max_q, self.alpha = min_q, max_q, alpha
 
         _ = plt.figure(1, figsize=figsize)
         ax1 = plt.subplot2grid((3, 1), (0, 0), rowspan=2)
         ax2 = plt.subplot2grid((3, 1), (2, 0))
```

### Comparing `probatus-1.8.9/probatus/metric_volatility/__init__.py` & `probatus-2.0.0/probatus/metric_volatility/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     BaseVolatilityEstimator,
     TrainTestVolatility,
     BootstrappedVolatility,
     SplitSeedVolatility,
 )
 from .utils import sample_data, check_sampling_input
 
-
 __all__ = [
     "get_metric",
     "BaseVolatilityEstimator",
     "TrainTestVolatility",
     "BootstrappedVolatility",
     "SplitSeedVolatility",
     "sample_data",
```

### Comparing `probatus-1.8.9/probatus/metric_volatility/metric.py` & `probatus-2.0.0/probatus/metric_volatility/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,21 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-import pandas as pd
 import numpy as np
-from probatus.utils import assure_numpy_array
-from probatus.metric_volatility.utils import sample_data
+import pandas as pd
 from sklearn.model_selection import train_test_split
 
+from probatus.metric_volatility.utils import sample_data
+from probatus.utils import assure_numpy_array
+
 
 def get_metric(
     X,
     y,
     clf,
     test_size,
     split_seed,
@@ -77,15 +78,16 @@
             Fraction of train data sampled, if sample_train_type is not None. Default value is 1.
 
         test_sampling_fraction (float, optional):
             Fraction of test data sampled, if sample_test_type is not None. Default value is 1.
 
     Returns:
         (pd.Dataframe):
-            Dataframe with results for a given model trained. Rows indicate the metric measured and columns ther results
+            Dataframe with results for a given model trained. Rows indicate the metric measured and columns their
+                results.
     """
 
     if not (isinstance(X, np.ndarray) or isinstance(X, pd.DataFrame)):
         X = assure_numpy_array(X)
     if not (isinstance(X, np.ndarray) or isinstance(X, pd.Series)):
         y = assure_numpy_array(y)
```

### Comparing `probatus-1.8.9/probatus/metric_volatility/utils.py` & `probatus-2.0.0/probatus/metric_volatility/utils.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/metric_volatility/volatility.py` & `probatus-2.0.0/probatus/metric_volatility/volatility.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,31 +14,33 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
+import warnings
+
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
-from probatus.metric_volatility.metric import get_metric
 from joblib import Parallel, delayed
 from tqdm.auto import tqdm
+
+from probatus.metric_volatility.metric import get_metric
+from probatus.metric_volatility.utils import check_sampling_input
+from probatus.stat_tests import DistributionStatistics
 from probatus.utils import (
-    get_scorers,
+    BaseFitComputePlotClass,
     assure_list_of_strings,
     assure_list_values_allowed,
-    BaseFitComputePlotClass,
+    get_scorers,
     preprocess_data,
     preprocess_labels,
 )
-from probatus.metric_volatility.utils import check_sampling_input
-from probatus.stat_tests import DistributionStatistics
-import warnings
 
 
 class BaseVolatilityEstimator(BaseFitComputePlotClass):
     """
     Base object for estimating volatility estimation.
 
     This class is a base class, therefore cannot be used on its
@@ -225,27 +227,27 @@
             # Enable traversing the axs
             axs = axs.flatten()
             axis_index = 0
 
             for metric, row in target_report.iterrows():
                 train, test, delta = self._get_samples_to_plot(metric_name=metric)
 
-                axs[axis_index].hist(train, alpha=0.5, label="Train {}".format(metric), bins=bins)
-                axs[axis_index].hist(test, alpha=0.5, label="Test {}".format(metric), bins=bins)
-                axs[axis_index].set_title("Distributions {}".format(metric))
+                axs[axis_index].hist(train, alpha=0.5, label=f"Train {metric}", bins=bins)
+                axs[axis_index].hist(test, alpha=0.5, label=f"Test {metric}", bins=bins)
+                axs[axis_index].set_title(f"Distributions {metric}")
                 axs[axis_index].legend(loc="upper right")
 
-                axs[axis_index + 1].hist(delta, alpha=0.5, label="Delta {}".format(metric), bins=bins)
-                axs[axis_index + 1].set_title("Distributions delta {}".format(metric))
+                axs[axis_index + 1].hist(delta, alpha=0.5, label=f"Delta {metric}", bins=bins)
+                axs[axis_index + 1].set_title(f"Distributions delta {metric}")
                 axs[axis_index + 1].legend(loc="upper right")
 
                 axis_index += 2
 
             for ax in axs.flat:
-                ax.set(xlabel="{} score".format(metric), ylabel="Results count")
+                ax.set(xlabel=f"{metric} score", ylabel="Results count")
 
             if show:
                 plt.show()
             else:
                 plt.close()
 
             return axs
@@ -273,16 +275,16 @@
         store them as report.
         """
         unique_metrics = self.iterations_results["metric_name"].unique()
 
         # Get columns which will be filled
         stats_tests_columns = []
         for stats_tests_object in self.stats_tests_objects:
-            stats_tests_columns.append("{} statistic".format(stats_tests_object.statistical_test_name))
-            stats_tests_columns.append("{} p-value".format(stats_tests_object.statistical_test_name))
+            stats_tests_columns.append(f"{stats_tests_object.statistical_test_name} statistic")
+            stats_tests_columns.append(f"{stats_tests_object.statistical_test_name} p-value")
         stats_columns = [
             "train_mean",
             "train_std",
             "test_mean",
             "test_std",
             "delta_mean",
             "delta_std",
```

### Comparing `probatus-1.8.9/probatus/missing_values/__init__.py` & `probatus-2.0.0/probatus/missing_values/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/missing_values/imputation.py` & `probatus-2.0.0/probatus/missing_values/imputation.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,36 +13,32 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-from probatus.utils import (
-    preprocess_data,
-    preprocess_labels,
-    BaseFitComputePlotClass,
-    get_single_scorer,
-)
-from sklearn.model_selection import cross_validate
-from sklearn.pipeline import Pipeline
-from sklearn.impute import SimpleImputer
-from sklearn.compose import ColumnTransformer
-from sklearn.preprocessing import OneHotEncoder
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from sklearn.compose import ColumnTransformer
+from sklearn.impute import SimpleImputer
+from sklearn.model_selection import cross_validate
+from sklearn.pipeline import Pipeline
+from sklearn.preprocessing import OneHotEncoder
+
+from probatus.utils import BaseFitComputePlotClass, get_single_scorer, preprocess_data, preprocess_labels
 
 
 class ImputationSelector(BaseFitComputePlotClass):
     """
     Comparison of various imputation strategies that can be used for imputing missing values.
 
     The aim of this class is to present the model performance based on imputation
-    strategies and a choosen model.
+    strategies and a chosen model.
     For models like XGBoost & LighGBM which have capabilities to handle missing values by default
     the model performance with no imputation will be shown as well.
     The missing values categorical features are imputed with the value `missing` and an missing indicator is
     added.
 
     Example:
     ```python
@@ -69,30 +65,30 @@
        'Simple Median Imputer' : SimpleImputer(strategy='median',add_indicator=True),
        'Simple Mean Imputer' : SimpleImputer(strategy='mean',add_indicator=True),
        'Iterative Imputer'  : IterativeImputer(add_indicator=True,n_nearest_features=5,
        sample_posterior=True),
        'KNN' : KNNImputer(n_neighbors=3)}
     #Create a classifier.
     clf = LogisticRegression()
-    #Create the comparision of the imputation strategies.
+    #Create the comparison of the imputation strategies.
     cmp = ImputationSelector(
         clf=clf,
         strategies=strategies,
         cv=5,
         model_na_support=False)
 
     cmp.fit_compute(X_missing,y)
     #Plot the results.
     performance_plot=cmp.plot()
 
     ```
 
-    <img src="../img/imputation_comparision.png" width="500" />
+    <img src="../img/imputation_comparison.png" width="500" />
 
-    """ # noqa
+    """
 
     def __init__(
         self,
         clf,
         strategies,
         scoring="roc_auc",
         cv=5,
@@ -115,20 +111,22 @@
                 'Simple Median Imputer' : SimpleImputer(strategy='median',add_indicator=True),
                 'Iterative Imputer'  : IterativeImputer(add_indicator=True,n_nearest_features=5,
                 sample_posterior=True)}
                 This allows you to have fine grained control over the imputation method.
 
             scoring (string, list of strings, probatus.utils.Scorer or list of probatus.utils.Scorers, optional):
                 Metrics for which the score is calculated. It can be either a name or list of names metric names and
-                needs to be aligned with predefined [classification scorers names in sklearn](https://scikit-learn.org/stable/modules/model_evaluation.html).
+                needs to be aligned with predefined
+                [classification scorers names in sklearn](https://scikit-learn.org/stable/modules/model_evaluation.html).
                 Another option is using probatus.utils.Scorer to define a custom metric.
 
             model_na_support (boolean): default False
                 If the classifier supports missing values by default e.g. LightGBM,XGBoost etc.
-                If True an default comparison `No Imputation`  result will be added indicating the model performance without any explict imputation.
+                If True an default comparison `No Imputation`  result will be added indicating the model performance
+                    without any explicit imputation.
                 If False only the provided strategies will be used.
 
             n_jobs (int, optional):
                 Number of cores to run in parallel while fitting across folds. None means 1 unless in a
                 `joblib.parallel_backend` context. -1 means using all processors.
 
             verbose (int, optional):
@@ -155,15 +153,15 @@
         self.fitted = False
         self.report_df = pd.DataFrame([])
 
     def __repr__(self):
         """
         String representation.
         """
-        return "Imputation comparision for {}".format(self.clf.__class__.__name__)
+        return f"Imputation comparison for {self.clf.__class__.__name__}"
 
     def fit(self, X, y, column_names=None):
         """
         Calculates the cross validated results for various imputation strategies.
 
         Args:
             X (pd.DataFrame):
@@ -187,15 +185,14 @@
 
         # Identify categorical features.
         categorical_columns = X.select_dtypes(include=["category", "object"]).columns
         # Identify the numeric columns.Numeric columns are all columns expect the categorical columns
         numeric_columns = X.select_dtypes("number").columns
 
         for strategy in self.strategies:
-
             numeric_transformer = Pipeline(steps=[("imputer", self.strategies[strategy])])
 
             categorical_transformer = Pipeline(
                 steps=[
                     (
                         "imp_cat",
                         SimpleImputer(
@@ -221,15 +218,14 @@
             temp_results = self._calculate_results(X, y, clf=model_pipeline, strategy=strategy)
 
             results.append(temp_results)
 
         # If model supports missing values by default, then calculate the scores
         # on raw data without any imputation.
         if self.model_na_support:
-
             categorical_transformer = Pipeline(
                 steps=[
                     ("ohe_cat", OneHotEncoder(handle_unknown="ignore")),
                 ]
             )
 
             preprocessor = ColumnTransformer(
@@ -240,15 +236,15 @@
             model_pipeline = Pipeline(steps=[("preprocessor", preprocessor), ("classifier", self.clf)])
 
             temp_results = self._calculate_results(X, y, clf=model_pipeline, strategy="No Imputation")
             results.append(temp_results)
 
         self.report_df = pd.DataFrame(results)
         # Set the index of the dataframe to the imputation methods.
-        self.report_df = self.report_df.set_index(self.report_df.strategy, "strategy")
+        self.report_df = self.report_df.set_index(self.report_df.strategy)
         self.report_df.drop(columns=["strategy"], inplace=True)
         self.report_df.sort_values(by="mean_test_score", inplace=True)
         self.fitted = True
         return self
 
     def _calculate_results(self, X, y, clf, strategy):
         """
@@ -278,20 +274,20 @@
             y,
             scoring=self.scorer.scorer,
             cv=self.cv,
             n_jobs=self.n_jobs,
             return_train_score=True,
         )
         # Calculate the mean of the results.
-        imp_agg_results = dict((k, np.mean(v)) for k, v in imputation_cv_results.items())
+        imp_agg_results = {k: np.mean(v) for k, v in imputation_cv_results.items()}
         imp_agg_results = {"mean_" + str(key): val for key, val in imp_agg_results.items()}
         imp_agg_results["test_score_std"] = np.std(imputation_cv_results["test_score"])
         imp_agg_results["train_score_std"] = np.std(imputation_cv_results["train_score"])
         # Round off all calculations to 3 decimal places
-        imp_agg_results = dict((k, np.round(v, 3)) for k, v in imp_agg_results.items())
+        imp_agg_results = {k: np.round(v, 3) for k, v in imp_agg_results.items()}
         imp_agg_results["strategy"] = strategy
 
         return imp_agg_results
 
     def compute(self):
         """
         Checks if fit() method has been run.
@@ -360,15 +356,15 @@
         def _autolabel(rects):
             """
             Label the bars of the plot.
             """
             for rect in rects:
                 width = rect.get_width()
                 ax.annotate(
-                    "{}".format(width),
+                    f"{width}",
                     xy=((width + 0.05 * width), rect.get_y() + rect.get_height() / 2),
                     xytext=(4, 0),  # 4 points horizontal offset
                     textcoords="offset points",
                     ha="center",
                     va="bottom",
                     fontsize="small",
                 )
@@ -389,15 +385,15 @@
             align="center",
             label="CV-Test",
         )
         _autolabel(train_rect)
         _autolabel(test_rect)
 
         ax.set_xlabel(f'{self.scorer.metric_name.replace("_"," ").upper()} Score')
-        ax.set_title("Imputation Techniques Comparision")
+        ax.set_title("Imputation Techniques Comparison")
         ax.set_yticks(y)
         ax.set_yticklabels(imp_methods, rotation=45)
         plt.margins(0.2)
         plt.legend(loc="best", ncol=2)
         fig.tight_layout()
 
         if show:
```

### Comparing `probatus-1.8.9/probatus/sample_similarity/__init__.py` & `probatus-2.0.0/probatus/sample_similarity/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/sample_similarity/resemblance_model.py` & `probatus-2.0.0/probatus/sample_similarity/resemblance_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,28 +14,25 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-import pandas as pd
-import numpy as np
-from sklearn.model_selection import train_test_split
-from probatus.utils import (
-    preprocess_labels,
-    get_single_scorer,
-    preprocess_data,
-    BaseFitComputePlotClass,
-)
-from probatus.utils.shap_helpers import shap_calc, calculate_shap_importance
-from sklearn.inspection import permutation_importance
+import warnings
+
 import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
 from shap import summary_plot
-import warnings
+from sklearn.inspection import permutation_importance
+from sklearn.model_selection import train_test_split
+
+from probatus.utils import BaseFitComputePlotClass, get_single_scorer, preprocess_data, preprocess_labels
+from probatus.utils.shap_helpers import calculate_shap_importance, shap_calc
 
 
 class BaseResemblanceModel(BaseFitComputePlotClass):
     """
     This model checks for the similarity of two samples.
 
     A possible use case is analysis of whether th train sample differs
@@ -510,22 +507,22 @@
 class SHAPImportanceResemblance(BaseResemblanceModel):
     """
     This model checks for similarity of two samples.
 
     A possible use case is analysis of whether the train sample differs
         from the test sample, due to e.g. non-stationarity.
 
-    It assigns labels to each sample, 0 to the first sample, 1 to the second. Then, it randomly selects a portion of data
-        to train on. The resulting model tries to distinguish which sample a given test row comes from. This
+    It assigns labels to each sample, 0 to the first sample, 1 to the second. Then, it randomly selects a portion of
+        data to train on. The resulting model tries to distinguish which sample a given test row comes from. This
         provides insights on how distinguishable these samples are and which features contribute to that. The feature
         importance is calculated using SHAP feature importance.
 
     If the model achieves test AUC significantly different than 0.5, it indicates that it is possible to distinguish
-    between the samples, and therefore, the samples differ. Features with a high permutation importance contribute to that
-        effect the most. Thus, their distribution might differ between two samples.
+        between the samples, and therefore, the samples differ. Features with a high permutation importance contribute
+        to that effect the most. Thus, their distribution might differ between two samples.
 
     This class currently works only with the Tree based models.
 
     Examples:
     ```python
     from sklearn.datasets import make_classification
     from sklearn.ensemble import RandomForestClassifier
```

### Comparing `probatus-1.8.9/probatus/stat_tests/__init__.py` & `probatus-2.0.0/probatus/stat_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/stat_tests/ad.py` & `probatus-2.0.0/probatus/stat_tests/ad.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-from ..utils import assure_numpy_array
 from probatus.stat_tests.utils import verbose_p_vals
 from probatus.utils import NotInstalledError
 
+from ..utils import assure_numpy_array
+
 try:
     from scipy import stats
 except ModuleNotFoundError:
     stats = NotInstalledError("scipy", "extras")
 
 
 @verbose_p_vals
```

### Comparing `probatus-1.8.9/probatus/stat_tests/distribution_statistics.py` & `probatus-2.0.0/probatus/stat_tests/distribution_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 import itertools
 import warnings
 
-import pandas as pd
 import numpy as np
+import pandas as pd
 from tqdm import tqdm
 
-from probatus.binning import SimpleBucketer, AgglomerativeBucketer, QuantileBucketer
-from probatus.stat_tests import es, ks, psi, ad, sw
+from probatus.binning import AgglomerativeBucketer, QuantileBucketer, SimpleBucketer
+from probatus.stat_tests import ad, es, ks, psi, sw
 from probatus.utils.arrayfuncs import check_numeric_dtypes
 
 
-class DistributionStatistics(object):
+class DistributionStatistics:
     """
     Wrapper that applies a statistical test to compare two distributions.
 
     Details on the available tests can be found [here](/probatus/api/stat_tests.html#available-tests).
 
     For some tests, default data binning strategies are also provided.
 
@@ -103,62 +103,60 @@
             binning_strategy (string, optional):
                 Binning strategy to apply, binning strategies implemented:
 
                 - `'simplebucketer'`: equally spaced bins,
                 - `'agglomerativebucketer'`: binning by applying the Scikit-learn implementation of Agglomerative
                     Clustering,
                 - `'quantilebucketer'`: bins with equal number of elements,
-                - `'default'`: applies a default binning for a given stats_test. For all tests appart from PSI, no
+                - `'default'`: applies a default binning for a given stats_test. For all tests apart from PSI, no
                     binning (None) is used. For PSI by default quantilebucketer is used,
                 - `None`: no binning is applied. The test is computed based on original distribution.
 
             bin_count (int, optional): In case binning_strategy is not None, specify the number of bins to be used by
                 the binning strategy. By default 10 bins are used.
         """
         self.statistical_test = statistical_test.upper()
         self.binning_strategy = binning_strategy
         self.bin_count = bin_count
         self.fitted = False
 
         # Initialize the statistical test
         if self.statistical_test not in self.statistical_test_dict:
-            raise NotImplementedError(
-                "The statistical test should be one of {}".format(self.statistical_test_dict.keys())
-            )
+            raise NotImplementedError(f"The statistical test should be one of {self.statistical_test_dict.keys()}")
         else:
             self.statistical_test_name = self.statistical_test_dict[self.statistical_test]["name"]
             self._statistical_test_function = self.statistical_test_dict[self.statistical_test]["func"]
 
         # Initialize the binning strategy
         if self.binning_strategy:
             self.binning_strategy = self.binning_strategy.lower()
             if self.binning_strategy == "default":
                 self.binning_strategy = self.statistical_test_dict[self.statistical_test]["default_binning"]
             if self.binning_strategy not in self.binning_strategy_dict:
                 raise NotImplementedError(
-                    "The binning strategy should be one of {}".format(list(self.binning_strategy_dict.keys()))
+                    f"The binning strategy should be one of {list(self.binning_strategy_dict.keys())}"
                 )
             else:
                 binner = self.binning_strategy_dict[self.binning_strategy]
                 if binner is not None:
                     self.binner = binner(bin_count=self.bin_count)
 
     def __repr__(self):
         """
         String representation.
         """
-        repr_ = "DistributionStatistics object\n\tstatistical_test: {}".format(self.statistical_test)
+        repr_ = f"DistributionStatistics object\n\tstatistical_test: {self.statistical_test}"
         if self.binning_strategy:
-            repr_ += "\n\tbinning_strategy: {}\n\tbin_count: {}".format(self.binning_strategy, self.bin_count)
+            repr_ += f"\n\tbinning_strategy: {self.binning_strategy}\n\tbin_count: {self.bin_count}"
         else:
             repr_ += "\n\tNo binning applied"
         if self.fitted:
-            repr_ += "\nResults\n\tvalue {}-statistic: {}".format(self.statistical_test, self.statistic)
+            repr_ += f"\nResults\n\tvalue {self.statistical_test}-statistic: {self.statistic}"
         if hasattr(self, "p_value"):
-            repr_ += "\n\tp-value: {}".format(self.p_value)
+            repr_ += f"\n\tp-value: {self.p_value}"
         return repr_
 
     def compute(self, d1, d2, verbose=False):
         """
         Apply the statistical test and compute statistic value and p-value.
 
         Args:
@@ -195,15 +193,15 @@
             self.statistic, self.p_value = res
             return self.statistic, self.p_value
         else:
             self.statistic = res
             return self.statistic
 
 
-class AutoDist(object):
+class AutoDist:
     """Apply stat tests and binning strategies.
 
     Class to automatically apply all implemented statistical distribution tests and binning strategies
     to (a selection of) features in two dataframes.
 
     Details on the available tests can be found [here](/probatus/api/stat_tests.html#available-tests).
 
@@ -243,15 +241,15 @@
 
                 - `'SimpleBucketer'`: equally spaced bins,
                 - `'AgglomerativeBucketer'`: binning by applying the Scikit-learn implementation of Agglomerative
                     Clustering,
                 - `'QuantileBucketer'`: bins with equal number of elements,
                 - `None`: no binning is applied. Note that not all statistical tests will be performed since some of
                     them require binning strategies.
-                - `'default'`: applies a default binning for a given stats_test. For all tests appart from PSI, no
+                - `'default'`: applies a default binning for a given stats_test. For all tests apart from PSI, no
                     binning (None) is used. For PSI by default quantilebucketer is used.
                 - `'all'`: each binning strategy is used for each statistical test
 
             bin_count (integer, None or list of integers, optional):
                 bin_count value(s) to be used, note that None can only be used when no bucketing strategy is applied.
         """
         self.fitted = False
@@ -283,17 +281,17 @@
         String representation.
         """
         repr_ = "AutoDist object"
         if not self.fitted:
             repr_ += "\n\tAutoDist not fitted"
         if self.fitted:
             repr_ += "\n\tAutoDist fitted"
-        repr_ += "\n\tstatistical_tests: {}".format(self.statistical_tests)
-        repr_ += "\n\tbinning_strategies: {}".format(self.binning_strategies)
-        repr_ += "\n\tbin_count: {}".format(self.bin_count)
+        repr_ += f"\n\tstatistical_tests: {self.statistical_tests}"
+        repr_ += f"\n\tbinning_strategies: {self.binning_strategies}"
+        repr_ += f"\n\tbin_count: {self.bin_count}"
         return repr_
 
     def compute(
         self,
         df1,
         df2,
         column_names=None,
```

### Comparing `probatus-1.8.9/probatus/stat_tests/es.py` & `probatus-2.0.0/probatus/stat_tests/es.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,17 +21,18 @@
 from probatus.utils import NotInstalledError
 
 try:
     from scipy import stats
 except ModuleNotFoundError:
     stats = NotInstalledError("scipy", "extras")
 
-from ..utils import assure_numpy_array
 from probatus.stat_tests.utils import verbose_p_vals
 
+from ..utils import assure_numpy_array
+
 
 @verbose_p_vals
 def es(d1, d2, verbose=False):
     """
     Calculates the Epps-Singleton test statistic on 2 distributions.
 
     Can be used on continuous or discrete distributions.
```

### Comparing `probatus-1.8.9/probatus/stat_tests/ks.py` & `probatus-2.0.0/probatus/stat_tests/ks.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,28 +21,29 @@
 from probatus.utils import NotInstalledError
 
 try:
     from scipy import stats
 except ModuleNotFoundError:
     stats = NotInstalledError("scipy", "extras")
 
-from ..utils import assure_numpy_array
 from probatus.stat_tests.utils import verbose_p_vals
 
+from ..utils import assure_numpy_array
+
 
 @verbose_p_vals
 def ks(d1, d2, verbose=False):
     """
     Calculates the Kolmogorov-Smirnov test statistic on 2 samples.
 
     Any binning/bucketing of the distributions/samples should be done before passing them to this function.
 
     References:
 
-    - [Wikipedia article about the Kolmogorov-Smirnov test](https://en.wikipedia.org/wiki/Kolmogorov%E2%80%93Smirnov_test)
+    - [Wikipedia article about Kolmogorov-Smirnov test](https://en.wikipedia.org/wiki/Kolmogorov%E2%80%93Smirnov_test)
     - [SciPy documentation](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ks_2samp.html)
 
     Args:
         d1 (np.ndarray or pandas.Series): First sample.
 
         d2 (np.ndarray or pandas.Series): Second sample.
```

### Comparing `probatus-1.8.9/probatus/stat_tests/psi.py` & `probatus-2.0.0/probatus/stat_tests/psi.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         verbose (bool): If True, useful interpretation info is printed to stdout.
 
 
     Returns:
         float: Measure of the similarity between d1 & d2. (range 0-inf, with 0 indicating identical
         distributions and > 0.25 indicating significantly different distributions)
         float: p-value for rejecting null hypothesis (that the two distributions are identical)
-    """
+    """  # noqa
     # Perform data checks
     d1 = assure_numpy_array(d1)
     d2 = assure_numpy_array(d2)
 
     if len(d1) < 10:
         warnings.warn("PSI is not well-behaved when using less than 10 bins.")
     if len(d1) > 20:
```

### Comparing `probatus-1.8.9/probatus/stat_tests/sw.py` & `probatus-2.0.0/probatus/stat_tests/sw.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,30 +14,33 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
-import pandas as pd
 import random
-from ..utils import assure_numpy_array
+
+import pandas as pd
 
 from probatus.utils import NotInstalledError
 
+from ..utils import assure_numpy_array
+
 try:
     from scipy import stats
 except ModuleNotFoundError:
     stats = NotInstalledError("scipy", "extras")
 
 
 def sw(d1, d2, verbose=False):
     """
-    Calculates the Shapiro-Wilk test statistic on 2 distributions,
-    which examines whether deviation from normality of two distributions are significantly different.
+    Calculates the Shapiro-Wilk test statistic on 2 distributions.
+
+    This examines whether deviation from normality of two distributions are significantly different.
 
     References:
 
     - [Wikipedia article about the Shapiro-Wilk test](https://en.wikipedia.org/wiki/Shapiro%E2%80%93Wilk_test)
     - [SciPy documentation](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.shapiro.html)
 
 
@@ -67,32 +70,27 @@
 
     MOT = pd.concat([d1, d2])
     n1 = d1.shape[0]
     n2 = d2.shape[0]
 
     def ran_delta(n1, n2):
         take_ran = lambda n: random.sample(range(MOT.shape[0]), n)
-        ran_1 = MOT.iloc[
-            take_ran(n1),
-        ]
-        ran_2 = MOT.iloc[
-            take_ran(n2),
-        ]
+        ran_1 = MOT.iloc[take_ran(n1),]
+        ran_2 = MOT.iloc[take_ran(n2),]
         delta_ran = stats.shapiro(ran_1)[0] - stats.shapiro(ran_2)[0]
         return delta_ran
 
     collect = [ran_delta(n1, n2) for a in range(100)]
     collect = pd.Series(list(collect))
     delta_p_value = 1 - stats.percentileofscore(collect, delta) / 100
 
     quants = [0.025, 0.975]
     sig_vals = list(collect.quantile(quants))
 
     if verbose:
-
         if delta < sig_vals[0] or delta > sig_vals[1]:
             print("\nShapiro_Difference | Null hypothesis : <delta is not different from zero> REJECTED.")
             print("\nDelta is outside 95% CI -> Distributions very different.")
         else:
             print("\nShapiro_Difference | Null hypothesis : <delta is not different from zero> NOT REJECTED.")
             print("\nDelta is inside 95% CI -> Distributions are not different.")
```

### Comparing `probatus-1.8.9/probatus/stat_tests/utils.py` & `probatus-2.0.0/probatus/stat_tests/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,23 +29,23 @@
     @functools.wraps(func)
     def wrapper_verbose_p_vals(*args, **kwargs):
         test_name = func.__name__.upper()
 
         stat, pvalue = func(*args, **kwargs)
 
         if "verbose" in kwargs and kwargs["verbose"] is True:
-            print("\n{}: pvalue =".format(test_name), pvalue)
+            print(f"\n{test_name}: pvalue =", pvalue)
             if pvalue < 0.01:
                 print(
                     "\n{}: Null hypothesis rejected with 99% confidence. Distributions very different.".format(
                         test_name
                     )
                 )
             elif pvalue < 0.05:
-                print("\n{}: Null hypothesis rejected with 95% confidence. Distributions different.".format(test_name))
+                print(f"\n{test_name}: Null hypothesis rejected with 95% confidence. Distributions different.")
             else:
                 print(
                     "\n{}: Null hypothesis cannot be rejected. Distributions not statistically different.".format(
                         test_name
                     )
                 )
```

### Comparing `probatus-1.8.9/probatus/utils/__init__.py` & `probatus-2.0.0/probatus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/utils/_utils.py` & `probatus-2.0.0/probatus/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/utils/arrayfuncs.py` & `probatus-2.0.0/probatus/utils/arrayfuncs.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
+import numbers
+import warnings
+
 import numpy as np
 import pandas as pd
-import numbers
+
 from probatus.utils import DimensionalityError
-import warnings
 
 
 def check_1d(x):
     """
     Checks whether or not a list, numpy array, pandas dataframe, pandas series are one-dimensional.
 
     Returns True when check is ok, otherwise throws a `DimensionalityError`
```

### Comparing `probatus-1.8.9/probatus/utils/exceptions.py` & `probatus-2.0.0/probatus/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/utils/interface.py` & `probatus-2.0.0/probatus/utils/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
 # COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
 # IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 
 from abc import ABC, abstractmethod
+
 from probatus.utils import NotFittedError
 
 
 class BaseFitComputeClass(ABC):
     """
     Placeholder that must be overwritten by subclass.
     """
```

### Comparing `probatus-1.8.9/probatus/utils/missing_helpers.py` & `probatus-2.0.0/probatus/utils/missing_helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def generate_MCAR(df, missing):
     """
     Generate missing values completely at random for dataframe df.
 
     Args:
         df: input dataframe where some values will be masked
-        missings: (float or dict)
+        missing: (float or dict)
             - float ( must be a fraction between 0 and 1 - both inclusive), then it will apply this
             fraction of missing values on the whole dataset.
             - dict:
                 - keys: column names to mask values
                 - values: fraction of missing values for this column
 
     Returns:
```

### Comparing `probatus-1.8.9/probatus/utils/plots.py` & `probatus-2.0.0/probatus/utils/plots.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/utils/scoring.py` & `probatus-2.0.0/probatus/utils/scoring.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/utils/shap_helpers.py` & `probatus-2.0.0/probatus/utils/shap_helpers.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus/utils/warnings.py` & `probatus-2.0.0/probatus/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/probatus.egg-info/PKG-INFO` & `probatus-2.0.0/probatus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: probatus
-Version: 1.8.9
+Version: 2.0.0
 Summary: Validation of binary classifiers and data used to develop them
 Home-page: https://github.com/ing-bank/probatus
 Author: ING Bank N.V.
 Author-email: mateusz.garbacz@ing.com
 License: MIT License
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: extras
 Provides-Extra: all
 License-File: LICENCE
 
 <img src="https://github.com/ing-bank/probatus/raw/main/docs/img/logo_large.png" width="120" align="right">
 
 [![pytest](https://github.com/ing-bank/probatus/workflows/Development/badge.svg)](https://github.com/ing-bank/probatus/actions?query=workflow%3A%22Development%22)
 [![PyPi Version](https://img.shields.io/pypi/pyversions/probatus)](#)
 [![PyPI](https://img.shields.io/pypi/v/probatus)](#)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/probatus)](#)
 ![GitHub contributors](https://img.shields.io/github/contributors/ing-bank/probatus)
 
-# probatus
+# Probatus
 
 ## Overview
 
 **Probatus** is a python package that helps validate binary classification models and the data used to develop them. Main features:
 
-- [probatus.interpret](https://ing-bank.github.io/probatus/api/model_interpret.html) provides shap-based model interpretation tools 
+- [probatus.interpret](https://ing-bank.github.io/probatus/api/model_interpret.html) provides shap-based model interpretation tools
 - [probatus.metric_volatility](https://ing-bank.github.io/probatus/api/metric_volatility.html) provides tools using bootstrapping and/or different random seeds to assess metric volatility/stability.
 - [probatus.sample_similarity](https://ing-bank.github.io/probatus/api/sample_similarity.html) to compare two datasets using resemblance modelling, f.e. `train` with out-of-time `test`.
 - [probatus.feature_elimination.ShapRFECV](https://ing-bank.github.io/probatus/api/feature_elimination.html) provides cross-validated Recursive Feature Elimination using shap feature importance.
 - [probatus.missing_values](https://ing-bank.github.io/probatus/api/imputation_selector.html) compares performance gains of different missing values imputation strategies for a given model.
 
 ## Installation
 
@@ -50,17 +49,15 @@
 pip install probatus
 ```
 
 ## Documentation
 
 Documentation at [ing-bank.github.io/probatus/](https://ing-bank.github.io/probatus/).
 
-You can also check out blog posts about Probatus: 
+You can also check out blog posts about Probatus:
 
 -  [Open-sourcing ShapRFECV — Improved feature selection powered by SHAP.](https://medium.com/ing-blog/open-sourcing-shaprfecv-improved-feature-selection-powered-by-shap-994fe7861560)
 -  [Model Explainability — How to choose the right tool?](https://medium.com/ing-blog/model-explainability-how-to-choose-the-right-tool-6c5eabd1a46a)
 
 ## Contributing
 
-To learn more about making a contribution to probatus, please see [`CONTRIBUTING.md`](CONTRIBUTING.md).
-
-
+To learn more about making a contribution to Probatus, please see [`CONTRIBUTING.md`](CONTRIBUTING.md).
```

### Comparing `probatus-1.8.9/probatus.egg-info/SOURCES.txt` & `probatus-2.0.0/probatus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `probatus-1.8.9/setup.py` & `probatus-2.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,49 @@
 import os
+import sys
+import platform
 
 import setuptools
 
 
 def read(fname):
     """
     Read contents of file as a string.
     """
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
+def python_ver():
+    """
+    Returns the python version as a string. e.g.: "3.8"
+    """
+    return str(sys.version_info.major) + "." + str(sys.version_info.minor)
+
+def system():
+    """
+    Returns the system os as a string. e.g.: "darwin"
+    """
+    return platform.system().lower()
+
 
 base_packages = [
     "scikit-learn>=0.22.2",
     "pandas>=1.0.0",
     "matplotlib>=3.1.1",
     "scipy>=1.4.0",
     "joblib>=0.13.2",
     "tqdm>=4.41.0",
-    "shap >= 0.38.1, < 0.39.0",  # 0.40.0 causes issues in certain plots. For now it is excluded
-    "numpy>=1.19.0",
+    "shap==0.41.0",  # 0.40.0 causes issues in certain plots.
+    "numpy==1.23.2" if python_ver() == "3.11" else "numpy==1.23.0", # wait for SHAP to upgrade.
+    "numba==0.57.0" if python_ver() == "3.11" else "numba>=0.56.4", # wait for SHAP to upgrade.
 ]
 
 extra_dep = [
     "lightgbm>=3.3.0",
-    "catboost>=1.0.0",
+    # https://github.com/catboost/catboost/issues/2371
+    "catboost<1.2" if python_ver() == "3.8" and system() == "darwin" else "catboost>=1.1",
     "xgboost>=1.5.0",
     "scipy>=1.4.0",
 ]
 
 dev_dep = [
     "flake8>=3.8.3",
     "black>=19.10b0",
@@ -39,14 +55,16 @@
     "pyflakes",
     "seaborn>=0.9.0",
     "joblib>=0.13.2",
     "jupyter>=1.0.0",
     "tabulate>=0.8.7",
     "nbconvert>=6.0.7",
     "pre-commit>=2.7.1",
+    "isort>=5.12.0",
+    "codespell>=2.2.4",
 ]
 
 docs_dep = [
     "mkdocs-material>=6.1.0",
     "mkdocs-git-revision-date-localized-plugin>=0.7.2",
     "mkdocs-git-authors-plugin>=0.3.2",
     "mkdocs-table-reader-plugin>=0.4.1",
@@ -57,31 +75,31 @@
     "mkdocstrings>=0.13.6",
     "mkdocs-print-site-plugin>=0.8.2",
     "mkdocs-markdownextradata-plugin>=0.1.9",
 ]
 
 setuptools.setup(
     name="probatus",
-    version="1.8.9",
+    version="2.0.0",
     description="Validation of binary classifiers and data used to develop them",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="ING Bank N.V.",
     author_email="mateusz.garbacz@ing.com",
     license="MIT License",
     packages=setuptools.find_packages(exclude=["tests"]),
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=base_packages,
     extras_require={
```

### Comparing `probatus-1.8.9/tests/binning/test_binning.py` & `probatus-2.0.0/tests/binning/test_binning.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import pytest
-
-from probatus.binning import SimpleBucketer, QuantileBucketer, AgglomerativeBucketer, TreeBucketer, Bucketer
 from sklearn.exceptions import NotFittedError
 
+from probatus.binning import AgglomerativeBucketer, Bucketer, QuantileBucketer, SimpleBucketer, TreeBucketer
+
 
 @pytest.mark.filterwarnings("ignore:")
 def test_deprecations():
     """
     Test.
     """
     x = [1, 2, 1]
```

### Comparing `probatus-1.8.9/tests/docs/test_docstring.py` & `probatus-2.0.0/tests/docs/test_docstring.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This approach is adapted from, and explained in: https://calmcode.io/docs/epic.html
 
-import pytest
-import matplotlib.pyplot as plt
-import matplotlib
 import os
+from typing import List
+
+import matplotlib
+import matplotlib.pyplot as plt
+import pytest
 
 import probatus.binning
 import probatus.feature_elimination
 import probatus.interpret
 import probatus.metric_volatility
+import probatus.missing_values
 import probatus.sample_similarity
 import probatus.stat_tests
 import probatus.utils
-import probatus.missing_values
-
-from typing import List
 
 # Turn off interactive mode in plots
 plt.ioff()
 matplotlib.use("Agg")
 
 CLASSES_TO_TEST = [
     probatus.binning.SimpleBucketer,
```

### Comparing `probatus-1.8.9/tests/docs/test_notebooks.py` & `probatus-2.0.0/tests/docs/test_notebooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # This approach is adapted from, and explained in: https://calmcode.io/docs/epic.html
 
-import pytest
 import os
 
+import pytest
+
 # Turn off interactive mode in plots
 
 plots_disable = "import matplotlib \n" "import matplotlib.pyplot as plt \n" "plt.ioff() \n" "matplotlib.use('Agg') \n"
 NOTEBOOKS_PATH = "./docs/tutorials/"
 
 NOTEBOOKS_TO_TEST_LGBM = [
     "./docs/tutorials/nb_shap_feature_elimination",
```

### Comparing `probatus-1.8.9/tests/interpret/test_inspector.py` & `probatus-2.0.0/tests/interpret/test_inspector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from probatus.interpret.inspector import return_confusion_metric, InspectorShap, BaseInspector
-from tests.mocks import MockClusterer, MockModel
 from unittest.mock import patch
-from probatus.utils import NotFittedError, UnsupportedModelError
 
 import numpy as np
 import pandas as pd
 import pytest
 
+from probatus.interpret.inspector import BaseInspector, InspectorShap, return_confusion_metric
+from probatus.utils import NotFittedError, UnsupportedModelError
+from tests.mocks import MockClusterer, MockModel
+
 test_sensitivity = 0.0000000001
 
 
 @pytest.mark.skip(reason="Not currently implemented")
 def test_after_implementation_completed():
     """
     Test.
@@ -721,15 +722,14 @@
         global_clusters,
         global_Xs,
         global_ys,
         global_predicted_probas,
         global_clusters_eval_set,
         global_X_shaps,
     ):
-
         inspector = InspectorShap(model=MockModel(), algotype="kmeans")
         input_eval_set = [(global_Xs[0], global_ys[0]), (global_Xs[1], global_ys[1])]
         input_sample_names = ["set1", "set2"]
         input_X = global_X
         input_y = global_y
 
         with patch.object(InspectorShap, "perform_fit_calc") as mock_perform_fit_calc:
```

### Comparing `probatus-1.8.9/tests/interpret/test_model_interpret.py` & `probatus-2.0.0/tests/interpret/test_model_interpret.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 
 import numpy as np
 import pandas as pd
 import pytest
-from probatus.interpret import ShapModelInterpreter
 from sklearn.linear_model import LogisticRegression
 from sklearn.tree import DecisionTreeClassifier
 
+from probatus.interpret import ShapModelInterpreter
+
 
 @pytest.fixture(scope="function")
 def X_train():
     """
     Fixture.
     """
     return pd.DataFrame({"col_1": [1, 1, 1, 1], "col_2": [0, 0, 0, 0], "col_3": [1, 0, 1, 0]}, index=[1, 2, 3, 4])
@@ -240,26 +241,23 @@
     """
     Test lightgbm.
     """
     class_names = ["neg", "pos"]
     X_train, X_test, y_train, y_test = complex_data_split
 
     shap_interpret = ShapModelInterpreter(complex_fitted_lightgbm, verbose=50)
-    with pytest.warns(None) as record:
-        importance_df = shap_interpret.fit_compute(
-            X_train, X_test, y_train, y_test, class_names=class_names, approximate=False, check_additivity=False
-        )
+    importance_df = shap_interpret.fit_compute(
+        X_train, X_test, y_train, y_test, class_names=class_names, approximate=False, check_additivity=False
+    )
 
     # Check parameters
     assert shap_interpret.fitted
     shap_interpret._check_if_fitted
 
     assert shap_interpret.class_names == class_names
-    assert len(record) > 4
-
     assert importance_df.shape[0] == X_train.shape[1]
 
     # Check if plots work for such dataset
     ax1 = shap_interpret.plot("importance", target_set="test", show=False)
     ax2 = shap_interpret.plot("summary", target_set="test", show=False)
     ax3 = shap_interpret.plot("dependence", target_columns="f2_missing", target_set="test", show=False)
     ax4 = shap_interpret.plot("sample", samples_index=X_test.index.tolist()[0:2], target_set="test", show=False)
```

### Comparing `probatus-1.8.9/tests/interpret/test_shap_dependence.py` & `probatus-2.0.0/tests/interpret/test_shap_dependence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import pytest
+import os
 
+import matplotlib
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import pytest
 from sklearn.ensemble import RandomForestClassifier
+
 from probatus.interpret.shap_dependence import DependencePlotter
 from probatus.utils.exceptions import NotFittedError
-import os
-import matplotlib.pyplot as plt
-import matplotlib
 
 # Turn off interactive mode in plots
 plt.ioff()
 matplotlib.use("Agg")
 
 
 @pytest.fixture(scope="function")
@@ -115,15 +116,15 @@
 
     plotter.fit(X_test, y_test)
 
     pd.testing.assert_frame_equal(plotter.X, X_test)
     pd.testing.assert_series_equal(plotter.y, pd.Series(y_test, index=X_test.index))
     assert plotter.fitted is True
 
-    # Check if plotting doesnt cause errors
+    # Check if plotting does not cause errors
     for binning in ["simple", "agglomerative", "quantile"]:
         _ = plotter.plot(feature="f2_missing", type_binning=binning, show=False)
 
 
 def test_get_X_y_shap_with_q_cut_normal(X_y, clf):
     """
     Test.
```

### Comparing `probatus-1.8.9/tests/metric_volatility/test_metric_volatility.py` & `probatus-2.0.0/tests/metric_volatility/test_metric_volatility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+import os
+from unittest.mock import patch
+
+import matplotlib
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import pytest
+from sklearn.tree import DecisionTreeClassifier
+
 from probatus.metric_volatility import (
     BaseVolatilityEstimator,
-    TrainTestVolatility,
-    SplitSeedVolatility,
     BootstrappedVolatility,
+    SplitSeedVolatility,
+    TrainTestVolatility,
+    check_sampling_input,
     get_metric,
     sample_data,
-    check_sampling_input,
 )
-from sklearn.tree import DecisionTreeClassifier
-import pytest
-import numpy as np
-import pandas as pd
-from unittest.mock import patch
 from probatus.stat_tests.distribution_statistics import DistributionStatistics
-from probatus.utils import Scorer, NotFittedError
-import os
-import matplotlib.pyplot as plt
-import matplotlib
+from probatus.utils import NotFittedError, Scorer
 
 # Turn off interactive mode in plots
 plt.ioff()
 matplotlib.use("Agg")
 
 
 @pytest.fixture(scope="function")
@@ -198,15 +200,14 @@
     """
     with patch.object(BaseVolatilityEstimator, "compute", return_value=report.loc[["roc_auc"]]) as mock_compute:
         with patch.object(
             BaseVolatilityEstimator,
             "_get_samples_to_plot",
             return_value=(iterations_train, iterations_test, iterations_delta),
         ) as mock_get_samples:
-
             vol = BaseVolatilityEstimator(mock_model)
             vol.fitted = True
 
             vol.plot(metrics="roc_auc")
             mock_compute.assert_called_with(metrics="roc_auc")
             mock_get_samples.assert_called_with(metric_name="roc_auc")
 
@@ -230,15 +231,15 @@
     Test.
     """
     vol = BaseVolatilityEstimator(mock_model)
     vol.fitted = True
     vol.iterations_results = iteration_results
 
     vol._create_report()
-    pd.testing.assert_frame_equal(vol.report, report, check_less_precise=3)
+    pd.testing.assert_frame_equal(vol.report, report, atol=1e-3)
 
 
 def test_compute_mean_std_from_runs(mock_model, iteration_results):
     """
     Test.
     """
     vol = BaseVolatilityEstimator(mock_model)
@@ -285,15 +286,14 @@
 
     with patch.object(BaseVolatilityEstimator, "fit") as mock_base_fit:
         with patch.object(TrainTestVolatility, "_create_report") as mock_create_report:
             with patch(
                 "probatus.metric_volatility.volatility.get_metric",
                 side_effect=[iteration_results.iloc[[0]], iteration_results.iloc[[1]], iteration_results.iloc[[2]]],
             ):
-
                 vol.fit(X_df, y_series)
 
                 mock_base_fit.assert_called_once()
                 mock_create_report.assert_called_once()
 
     pd.testing.assert_frame_equal(vol.iterations_results, iteration_results.iloc[[0, 1, 2]])
```

### Comparing `probatus-1.8.9/tests/sample_similarity/test_resemblance_model.py` & `probatus-2.0.0/tests/sample_similarity/test_resemblance_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from probatus.sample_similarity import BaseResemblanceModel, SHAPImportanceResemblance, PermutationImportanceResemblance
-from probatus.utils import NotFittedError
+import os
 
-import pytest
+import matplotlib
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from sklearn.tree import DecisionTreeClassifier
-from sklearn.linear_model import LogisticRegression
-import os
+import pytest
 from pandas.api.types import is_numeric_dtype
-import matplotlib.pyplot as plt
-import matplotlib
+from sklearn.linear_model import LogisticRegression
+from sklearn.tree import DecisionTreeClassifier
+
+from probatus.sample_similarity import BaseResemblanceModel, PermutationImportanceResemblance, SHAPImportanceResemblance
+from probatus.utils import NotFittedError
 
 # Turn off interactive mode in plots
 plt.ioff()
 matplotlib.use("Agg")
 
 
 @pytest.fixture(scope="function")
```

### Comparing `probatus-1.8.9/tests/stat_tests/test_distribution_statistics.py` & `probatus-2.0.0/tests/stat_tests/test_distribution_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import numpy as np
-import pandas as pd
 import numbers
 
+import numpy as np
+import pandas as pd
 import pytest
-
 from sklearn.datasets import make_classification
 from sklearn.model_selection import train_test_split
 
-from probatus.stat_tests import ks, psi, DistributionStatistics, AutoDist
+from probatus.stat_tests import AutoDist, DistributionStatistics, ks, psi
 
 
 def test_distribution_statistics_base():
     """
     Test.
     """
     with pytest.raises(NotImplementedError):
```

### Comparing `probatus-1.8.9/tests/stat_tests/test_stat_tests.py` & `probatus-2.0.0/tests/stat_tests/test_stat_tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
-from probatus.stat_tests import ks, psi, es, ad, sw
 
 from probatus.binning import binning
+from probatus.stat_tests import ad, es, ks, psi, sw
 
 
 def test_psi_returns_zero():
     """
     Test.
     """
     x = np.random.normal(size=1000)
```

### Comparing `probatus-1.8.9/tests/stat_tests/test_utils.py` & `probatus-2.0.0/tests/stat_tests/test_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from probatus.stat_tests import ks, es
+from probatus.stat_tests import es, ks
 
 
 def test_verbosity_true_(capsys):
     """
     Test.
     """
     d1 = np.random.normal(size=1000)
```

### Comparing `probatus-1.8.9/tests/utils/test_utils_array_funcs.py` & `probatus-2.0.0/tests/utils/test_utils_array_funcs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import numpy as np
 import pandas as pd
-
 import pytest
 
 from probatus.utils import (
+    DimensionalityError,
     assure_numpy_array,
     assure_pandas_df,
     check_1d,
-    DimensionalityError,
     check_numeric_dtypes,
-    preprocess_labels,
     preprocess_data,
+    preprocess_labels,
 )
 
 
 @pytest.fixture(scope="function")
 def expected_df_2d():
     """
     Fixture.
@@ -215,73 +214,48 @@
 def test_preprocess_labels():
     """
     Test.
     """
     y1 = pd.Series([1, 0, 1, 0, 1])
     index_1 = np.array([5, 4, 3, 2, 1])
 
-    with pytest.warns(None) as record:
-        y1_output = preprocess_labels(y1, y_name="y1", index=index_1, verbose=150)
-
+    y1_output = preprocess_labels(y1, y_name="y1", index=index_1, verbose=150)
     pd.testing.assert_series_equal(y1_output, pd.Series([1, 0, 1, 0, 1], index=index_1))
-    # Ensure that number of warnings is correct
-    assert len(record) == 0
 
     y2 = [False, False, False, False, False]
-
-    with pytest.warns(None) as record:
-        y2_output = preprocess_labels(y2, y_name="y2", verbose=150)
-
+    y2_output = preprocess_labels(y2, y_name="y2", verbose=150)
     pd.testing.assert_series_equal(y2_output, pd.Series(y2))
-    # Ensure that number of warnings is correct
-    assert len(record) == 1
 
     y3 = np.array([0, 1, 2, 3, 4])
-    with pytest.warns(None) as record:
-        y3_output = preprocess_labels(y3, y_name="y3", verbose=150)
-
+    y3_output = preprocess_labels(y3, y_name="y3", verbose=150)
     pd.testing.assert_series_equal(y3_output, pd.Series(y3))
-    # Ensure that number of warnings is correct
-    assert len(record) == 1
 
     y4 = pd.Series(["2", "1", "3", "2", "1"])
     index4 = pd.Index([0, 2, 1, 3, 4])
-    with pytest.warns(None) as record:
-        y4_output = preprocess_labels(y4, y_name="y4", index=index4, verbose=0)
+    y4_output = preprocess_labels(y4, y_name="y4", index=index4, verbose=0)
     pd.testing.assert_series_equal(y4_output, pd.Series(["2", "3", "1", "2", "1"], index=index4))
-    # Ensure that number of warnings is correct
-    assert len(record) == 0
 
 
 def test_preprocess_data():
     """
     Test.
     """
     X1 = pd.DataFrame({"cat": ["a", "b", "c"], "missing": [1, np.nan, 2], "num_1": [1, 2, 3]})
 
     target_column_names_X1 = ["1", "2", "3"]
     X1_expected_output = pd.DataFrame({"1": ["a", "b", "c"], "2": [1, np.nan, 2], "3": [1, 2, 3]})
 
     X1_expected_output["1"] = X1_expected_output["1"].astype("category")
-
-    with pytest.warns(None) as record:
-        X1_output, output_column_names_X1 = preprocess_data(
-            X1, X_name="X1", column_names=target_column_names_X1, verbose=150
-        )
-
+    X1_output, output_column_names_X1 = preprocess_data(
+        X1, X_name="X1", column_names=target_column_names_X1, verbose=150
+    )
     assert target_column_names_X1 == output_column_names_X1
     pd.testing.assert_frame_equal(X1_output, X1_expected_output)
-    # Ensure that number of warnings is correct
-    assert len(record) == 2
 
     X2 = np.array([[1, 3, 2], [1, 2, 2], [1, 2, 3]])
 
     target_column_names_X1 = [0, 1, 2]
     X2_expected_output = pd.DataFrame(X2, columns=target_column_names_X1)
-
-    with pytest.warns(None) as record:
-        X2_output, output_column_names_X2 = preprocess_data(X2, X_name="X2", column_names=None, verbose=150)
+    X2_output, output_column_names_X2 = preprocess_data(X2, X_name="X2", column_names=None, verbose=150)
 
     assert target_column_names_X1 == output_column_names_X2
     pd.testing.assert_frame_equal(X2_output, X2_expected_output)
-    # Ensure that number of warnings is correct
-    assert len(record) == 0
```

