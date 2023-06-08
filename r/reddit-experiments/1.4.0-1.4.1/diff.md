# Comparing `tmp/reddit_experiments-1.4.0.tar.gz` & `tmp/reddit_experiments-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit_experiments-1.4.0.tar", last modified: Thu May 11 21:52:14 2023, max compression
+gzip compressed data, was "reddit_experiments-1.4.1.tar", last modified: Thu Jun  8 15:51:21 2023, max compression
```

## Comparing `reddit_experiments-1.4.0.tar` & `reddit_experiments-1.4.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.922507 reddit_experiments-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.898507 reddit_experiments-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/.github/workflows/python-package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-11 21:52:14.922507 reddit_experiments-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    53651 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/images/ddg-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/images/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/docs/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/legacy/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_decider/
--rw-r--r--   0 runner    (1001) docker     (123)    45454 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_decider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_decider/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_experiments/
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_experiments/providers/
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/forced_variant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/r2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/providers/simple_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_experiments/targeting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/targeting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/targeting/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/targeting/tree_targeting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_experiments/variant_sets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/multi_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/range_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/rollout_variant_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/reddit_experiments/variant_sets/single_variant_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/reddit_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 21:52:14.000000 reddit_experiments-1.4.0/reddit_experiments.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/requirements-transitive.txt
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-11 21:52:14.922507 reddit_experiments-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.902507 reddit_experiments-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    79965 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/decider_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    38015 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/experiment_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.906507 reddit_experiments-1.4.0/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/feature_flag_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/forced_variant_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/r2_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/simple_experiment_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.906507 reddit_experiments-1.4.0/tests/providers/variant_sets/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/variant_sets/multi_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/variant_sets/range_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/variant_sets/rollout_variant_set_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/providers/variant_sets/single_variant_set_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.906507 reddit_experiments-1.4.0/tests/range_variant_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.918507 reddit_experiments-1.4.0/tests/range_variant_tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   154451 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/range_variant_tests/data/original_zk_config.json
--rw-r--r--   0 runner    (1001) docker     (123) 14213529 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/range_variant_tests/data/output.json
--rw-r--r--   0 runner    (1001) docker     (123)   163729 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/range_variant_tests/data/range_variant_zk_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/range_variant_tests/range_variant_parity_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 21:52:14.918507 reddit_experiments-1.4.0/tests/targeting/
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-05-11 21:52:00.000000 reddit_experiments-1.4.0/tests/targeting/tree_targeting_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.067167 reddit_experiments-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.047166 reddit_experiments-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/.github/workflows/python-package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-08 15:51:21.067167 reddit_experiments-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    53651 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/docs/images/ddg-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/docs/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/docs/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/docs/legacy/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/reddit_decider/
+-rw-r--r--   0 runner    (1001) docker     (123)    45652 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_decider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_decider/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/reddit_experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/reddit_experiments/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/providers/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/providers/forced_variant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13980 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/providers/r2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11799 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/providers/simple_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/reddit_experiments/targeting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/targeting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/targeting/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/targeting/tree_targeting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/reddit_experiments/variant_sets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/variant_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/variant_sets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/variant_sets/multi_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/variant_sets/range_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/variant_sets/rollout_variant_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/reddit_experiments/variant_sets/single_variant_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/reddit_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-08 15:51:20.000000 reddit_experiments-1.4.1/reddit_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-08 15:51:21.000000 reddit_experiments-1.4.1/reddit_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:51:20.000000 reddit_experiments-1.4.1/reddit_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-08 15:51:20.000000 reddit_experiments-1.4.1/reddit_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 15:51:20.000000 reddit_experiments-1.4.1/reddit_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:51:20.000000 reddit_experiments-1.4.1/reddit_experiments.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/requirements-transitive.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-08 15:51:21.067167 reddit_experiments-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    79965 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/decider_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38015 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/experiment_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.051167 reddit_experiments-1.4.1/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)    27412 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/providers/feature_flag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/providers/forced_variant_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29866 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/providers/r2_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/providers/simple_experiment_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.055167 reddit_experiments-1.4.1/tests/providers/variant_sets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/providers/variant_sets/multi_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/providers/variant_sets/range_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/providers/variant_sets/rollout_variant_set_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/providers/variant_sets/single_variant_set_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.055167 reddit_experiments-1.4.1/tests/range_variant_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.067167 reddit_experiments-1.4.1/tests/range_variant_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   154451 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/range_variant_tests/data/original_zk_config.json
+-rw-r--r--   0 runner    (1001) docker     (123) 14213529 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/range_variant_tests/data/output.json
+-rw-r--r--   0 runner    (1001) docker     (123)   163729 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/range_variant_tests/data/range_variant_zk_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/range_variant_tests/range_variant_parity_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:51:21.067167 reddit_experiments-1.4.1/tests/targeting/
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-06-08 15:51:07.000000 reddit_experiments-1.4.1/tests/targeting/tree_targeting_tests.py
```

### Comparing `reddit_experiments-1.4.0/.github/workflows/python-package.yaml` & `reddit_experiments-1.4.1/.github/workflows/python-package.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/.github/workflows/python-publish.yaml` & `reddit_experiments-1.4.1/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/.readthedocs.yaml` & `reddit_experiments-1.4.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/LICENSE` & `reddit_experiments-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/Makefile` & `reddit_experiments-1.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/PKG-INFO` & `reddit_experiments-1.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit_experiments
-Version: 1.4.0
+Version: 1.4.1
 Summary: reddit's python experiments framework
 Home-page: https://github.com/reddit/experiments.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-experiments.readthedocs.io/
 Description: # experiments.py
         
@@ -14,20 +14,22 @@
         Documentation: https://reddit-experiments.readthedocs.io/
         
         ## Usage
         
         Install the library:
         
         ```console
-        $ pip install reddit-experiments
+        # `reddit-v2-events` is a Reddit internal package used for emitting exposure events
+        $ pip install reddit-experiments reddit-v2-events>=2.8.2
         ```
         
         Add the client to your application's Baseplate context:
         
         ```python
+         from event_utils.v2_event_utils import ExperimentLogger
          from reddit_decider import decider_client_from_config
         
          decider = decider_client_from_config(
              app_config=app_config,
              event_logger=ExperimentLogger(),
              request_field_extractor=decider_field_extractor,
          )
```

### Comparing `reddit_experiments-1.4.0/README.md` & `reddit_experiments-1.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,22 @@
 Documentation: https://reddit-experiments.readthedocs.io/
 
 ## Usage
 
 Install the library:
 
 ```console
-$ pip install reddit-experiments
+# `reddit-v2-events` is a Reddit internal package used for emitting exposure events
+$ pip install reddit-experiments reddit-v2-events>=2.8.2
 ```
 
 Add the client to your application's Baseplate context:
 
 ```python
+ from event_utils.v2_event_utils import ExperimentLogger
  from reddit_decider import decider_client_from_config
 
  decider = decider_client_from_config(
      app_config=app_config,
      event_logger=ExperimentLogger(),
      request_field_extractor=decider_field_extractor,
  )
```

### Comparing `reddit_experiments-1.4.0/docs/conf.py` & `reddit_experiments-1.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/docs/images/ddg-logo.png` & `reddit_experiments-1.4.1/docs/images/ddg-logo.png`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/docs/images/favicon.png` & `reddit_experiments-1.4.1/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/docs/index.rst` & `reddit_experiments-1.4.1/docs/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,21 @@
 
     reddit-v2-events>=2.8.2
 
 Prerequisite infrastructure
 ---------------------------
 **Zookeeper live-data sidecar**:
 
-Set up your service to pull down & synchronize experiment configurations from Zookeeper via the Baseplate `live-data watcher sidecar
-<https://baseplate.readthedocs.io/en/stable/api/baseplate/lib/live_data.html?highlight=sidecar#watcher-daemon>`_ (minimum v2.5.4).
-You'll have to make sure that your service is authorized to fetch the appropriate secret from Vault.
-See example setup `here
-<https://reddit.atlassian.net/wiki/spaces/EX/pages/343212125/Running+Experiments+at+Reddit#Live-Data-Sidecar>`__.
+Define a **live-data sidecar** in the manifest file to fetch the experiment configuration, see example setup `here
+<https://reddit.atlassian.net/wiki/spaces/EX/pages/343212125/Running+Experiments+at+Reddit#Live-Data-Sidecar>`__
+(make sure that your service is authorized to fetch the appropriate secret from Vault).
 
 **Event publisher sidecar**:
 
-Set up your service to be able to publish v2 exposure events via an `events sidecar <https://baseplate.readthedocs.io/en/stable/api/baseplate/lib/events.html?highlight=sidecar#publishing-events>`_
-. See example setup `here <https://reddit.atlassian.net/wiki/spaces/EX/pages/343212125/Running+Experiments+at+Reddit#Event-Publisher-Sidecar>`__.
+Set up your service to be able to publish v2 exposure events via an **event publisher sidecar**, see example setup `here <https://reddit.atlassian.net/wiki/spaces/EX/pages/343212125/Running+Experiments+at+Reddit#Event-Publisher-Sidecar>`__.
 
 Prerequisite configuration
 ---------------------------
 Setup :code:`reddit-experiments` in your application's configuration file:
 
 .. code-block:: ini
 
@@ -61,15 +58,15 @@
 -----------------------------------------------------------
 
 Upgrade or integrate reddit-experiments package:
 
 .. code-block:: python
 
     # import latest reddit-experiments package in service requirements.txt
-    reddit-experiments>=1.3.14
+    reddit-experiments>=1.4.0
 
 Initialize :code:`decider` instance on Baseplate context
 --------------------------------------------------------
 
 In your service's initialization process, add a :code:`decider` instance to baseplate's context:
 
 .. code-block:: python
```

### Comparing `reddit_experiments-1.4.0/docs/legacy/index.rst` & `reddit_experiments-1.4.1/docs/legacy/index.rst`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_decider/__init__.py` & `reddit_experiments-1.4.1/reddit_decider/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,17 @@
         self._span = server_span
         self._context_name = context_name
         if event_logger:
             self._event_logger = event_logger
         else:
             self._event_logger = DebugLogger()
 
+    def internal_decider(self) -> RustDecider:
+        return self._internal
+
     def _send_expose(self, event: str, exposure_fields: dict) -> None:
         event_fields = deepcopy(exposure_fields)
         try:
             (
                 _event_type,
                 exp_id,
                 name,
@@ -421,15 +424,16 @@
         identifier_type: Literal[
             "user_id", "device_id", "canonical_url", "subreddit_id", "ad_account_id", "business_id"
         ],
         **exposure_kwargs: Optional[Dict[str, Any]],
     ) -> Optional[str]:
         """Return a bucketing variant, if any, with auto-exposure for a given :code:`identifier`.
 
-        Note: If the experiment's :code:`bucket_val` (e.g. "user_id", "device_id", "canonical_url")
+        Note: If the experiment's :code:`bucket_val`
+            (e.g. "user_id", "device_id", "canonical_url", "subreddit_id", "ad_account_id", "business_id")
             does not match the :code:`identifier_type` param,
             the :code:`identifier` will be ignored and not used to bucket (:code:`{identifier_type: identifier}` is
             added to internal :code:`DeciderContext` instance, but doesn't act like a bucketing override).
 
             If the :code:`bucket_val` field exists on the :code:`DeciderContext` instance,
             that field will be used to bucket, since it corresponds to the experiment's config.
 
@@ -482,15 +486,16 @@
         identifier: str,
         identifier_type: Literal[
             "user_id", "device_id", "canonical_url", "subreddit_id", "ad_account_id", "business_id"
         ],
     ) -> Optional[str]:
         """Return a bucketing variant, if any, without emitting exposure event for a given :code:`identifier`.
 
-        Note: If the experiment's :code:`bucket_val` (e.g. "user_id", "device_id", "canonical_url")
+        Note: If the experiment's :code:`bucket_val`
+            (e.g. "user_id", "device_id", "canonical_url", "subreddit_id", "ad_account_id", "business_id")
             does not match the :code:`identifier_type` param,
             the :code:`identifier` will be ignored and not used to bucket (:code:`{identifier_type: identifier}` is
             added to internal :code:`DeciderContext` instance, but doesn't act like a bucketing override).
 
             If the :code:`bucket_val` field exists on the :code:`DeciderContext` instance,
             that field will be used to bucket, since it corresponds to the experiment's config.
```

### Comparing `reddit_experiments-1.4.0/reddit_experiments/__init__.py` & `reddit_experiments-1.4.1/reddit_experiments/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/providers/__init__.py` & `reddit_experiments-1.4.1/reddit_experiments/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/providers/base.py` & `reddit_experiments-1.4.1/reddit_experiments/providers/base.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/providers/feature_flag.py` & `reddit_experiments-1.4.1/reddit_experiments/providers/feature_flag.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/providers/forced_variant.py` & `reddit_experiments-1.4.1/reddit_experiments/providers/forced_variant.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/providers/r2.py` & `reddit_experiments-1.4.1/reddit_experiments/providers/r2.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/providers/simple_experiment.py` & `reddit_experiments-1.4.1/reddit_experiments/providers/simple_experiment.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/targeting/tree_targeting.py` & `reddit_experiments-1.4.1/reddit_experiments/targeting/tree_targeting.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/variant_sets/base.py` & `reddit_experiments-1.4.1/reddit_experiments/variant_sets/base.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/variant_sets/multi_variant_set.py` & `reddit_experiments-1.4.1/reddit_experiments/variant_sets/multi_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/variant_sets/range_variant_set.py` & `reddit_experiments-1.4.1/reddit_experiments/variant_sets/range_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/variant_sets/rollout_variant_set.py` & `reddit_experiments-1.4.1/reddit_experiments/variant_sets/rollout_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments/variant_sets/single_variant_set.py` & `reddit_experiments-1.4.1/reddit_experiments/variant_sets/single_variant_set.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/reddit_experiments.egg-info/PKG-INFO` & `reddit_experiments-1.4.1/reddit_experiments.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-experiments
-Version: 1.4.0
+Version: 1.4.1
 Summary: reddit's python experiments framework
 Home-page: https://github.com/reddit/experiments.py
 Author: reddit
 License: BSD
 Project-URL: Documentation, https://reddit-experiments.readthedocs.io/
 Description: # experiments.py
         
@@ -14,20 +14,22 @@
         Documentation: https://reddit-experiments.readthedocs.io/
         
         ## Usage
         
         Install the library:
         
         ```console
-        $ pip install reddit-experiments
+        # `reddit-v2-events` is a Reddit internal package used for emitting exposure events
+        $ pip install reddit-experiments reddit-v2-events>=2.8.2
         ```
         
         Add the client to your application's Baseplate context:
         
         ```python
+         from event_utils.v2_event_utils import ExperimentLogger
          from reddit_decider import decider_client_from_config
         
          decider = decider_client_from_config(
              app_config=app_config,
              event_logger=ExperimentLogger(),
              request_field_extractor=decider_field_extractor,
          )
```

### Comparing `reddit_experiments-1.4.0/reddit_experiments.egg-info/SOURCES.txt` & `reddit_experiments-1.4.1/reddit_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/requirements-transitive.txt` & `reddit_experiments-1.4.1/requirements-transitive.txt`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/setup.cfg` & `reddit_experiments-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/setup.py` & `reddit_experiments-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/decider_tests.py` & `reddit_experiments-1.4.1/tests/decider_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/experiment_tests.py` & `reddit_experiments-1.4.1/tests/experiment_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/providers/feature_flag_tests.py` & `reddit_experiments-1.4.1/tests/providers/feature_flag_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/providers/forced_variant_tests.py` & `reddit_experiments-1.4.1/tests/providers/forced_variant_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/providers/r2_tests.py` & `reddit_experiments-1.4.1/tests/providers/r2_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/providers/simple_experiment_tests.py` & `reddit_experiments-1.4.1/tests/providers/simple_experiment_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/providers/variant_sets/multi_variant_set_tests.py` & `reddit_experiments-1.4.1/tests/providers/variant_sets/multi_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/providers/variant_sets/range_variant_set_tests.py` & `reddit_experiments-1.4.1/tests/providers/variant_sets/range_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/providers/variant_sets/rollout_variant_set_tests.py` & `reddit_experiments-1.4.1/tests/providers/variant_sets/rollout_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/providers/variant_sets/single_variant_set_tests.py` & `reddit_experiments-1.4.1/tests/providers/variant_sets/single_variant_set_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/range_variant_tests/data/original_zk_config.json` & `reddit_experiments-1.4.1/tests/range_variant_tests/data/original_zk_config.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/range_variant_tests/data/output.json` & `reddit_experiments-1.4.1/tests/range_variant_tests/data/output.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/range_variant_tests/data/range_variant_zk_config.json` & `reddit_experiments-1.4.1/tests/range_variant_tests/data/range_variant_zk_config.json`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/range_variant_tests/range_variant_parity_tests.py` & `reddit_experiments-1.4.1/tests/range_variant_tests/range_variant_parity_tests.py`

 * *Files identical despite different names*

### Comparing `reddit_experiments-1.4.0/tests/targeting/tree_targeting_tests.py` & `reddit_experiments-1.4.1/tests/targeting/tree_targeting_tests.py`

 * *Files identical despite different names*

