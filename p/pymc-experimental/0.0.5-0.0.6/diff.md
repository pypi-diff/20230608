# Comparing `tmp/pymc-experimental-0.0.5.tar.gz` & `tmp/pymc-experimental-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc-experimental-0.0.5.tar", last modified: Mon Jun  5 16:04:57 2023, max compression
+gzip compressed data, was "pymc-experimental-0.0.6.tar", last modified: Thu Jun  8 10:24:44 2023, max compression
```

## Comparing `pymc-experimental-0.0.5.tar` & `pymc-experimental-0.0.6.tar`

### file list

```diff
@@ -1,77 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.155985 pymc-experimental-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-05 16:04:57.155985 pymc-experimental-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.139985 pymc-experimental-0.0.5/pymc_experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.143985 pymc-experimental-0.0.5/pymc_experimental/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/histogram_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.143985 pymc-experimental-0.0.5/pymc_experimental/distributions/multivariate/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/multivariate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/multivariate/r2d2m2cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/distributions/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.143985 pymc-experimental-0.0.5/pymc_experimental/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/gp/latent_approx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.143985 pymc-experimental-0.0.5/pymc_experimental/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/inference/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/inference/pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19997 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    24222 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.147985 pymc-experimental-0.0.5/pymc_experimental/model_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/model_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/model_transform/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/model_transform/conditioning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.147985 pymc-experimental-0.0.5/pymc_experimental/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.151985 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_multivariate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.151985 pymc-experimental-0.0.5/pymc_experimental/tests/model_transform/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/model_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/model_transform/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/model_transform/test_conditioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_histogram_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_linearmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_marginal_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_pathfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_prior_from_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/test_splines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.151985 pymc-experimental-0.0.5/pymc_experimental/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/tests/utils/test_model_fgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.155985 pymc-experimental-0.0.5/pymc_experimental/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/linear_cg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/model_fgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/pivoted_cholesky.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/prior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/pytensorf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/utils/spline.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pymc_experimental/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:04:57.139985 pymc-experimental-0.0.5/pymc_experimental.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-05 16:04:57.000000 pymc-experimental-0.0.5/pymc_experimental.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-05 16:04:57.000000 pymc-experimental-0.0.5/pymc_experimental.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:04:57.000000 pymc-experimental-0.0.5/pymc_experimental.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-05 16:04:57.000000 pymc-experimental-0.0.5/pymc_experimental.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 16:04:57.000000 pymc-experimental-0.0.5/pymc_experimental.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-05 16:04:57.155985 pymc-experimental-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-05 16:04:47.000000 pymc-experimental-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/histogram_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/distributions/multivariate/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/multivariate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10325 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/multivariate/r2d2m2cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/distributions/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/gp/latent_approx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/inference/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/inference/pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19997 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/model_transform/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/model_transform/conditioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/preprocessing/standard_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/pymc_experimental/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7479 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_discrete_markov_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_multivariate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/test_conditioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_histogram_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_linearmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_marginal_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_pathfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_prior_from_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/test_splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/pymc_experimental/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/tests/utils/test_model_fgraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/pymc_experimental/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/linear_cg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12913 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/model_fgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/pivoted_cholesky.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/pytensorf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/utils/spline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pymc_experimental/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:24:44.607944 pymc-experimental-0.0.6/pymc_experimental.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-08 10:24:44.000000 pymc-experimental-0.0.6/pymc_experimental.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-08 10:24:44.000000 pymc-experimental-0.0.6/pymc_experimental.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:24:44.000000 pymc-experimental-0.0.6/pymc_experimental.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-08 10:24:44.000000 pymc-experimental-0.0.6/pymc_experimental.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 10:24:44.000000 pymc-experimental-0.0.6/pymc_experimental.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-08 10:24:44.611944 pymc-experimental-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-08 10:24:35.000000 pymc-experimental-0.0.6/setup.py
```

### Comparing `pymc-experimental-0.0.5/CODE_OF_CONDUCT.md` & `pymc-experimental-0.0.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/LICENSE` & `pymc-experimental-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/PKG-INFO` & `pymc-experimental-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.5
+Version: 0.0.6
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.5 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.6 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `pymc-experimental-0.0.5/README.md` & `pymc-experimental-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/__init__.py` & `pymc-experimental-0.0.6/pymc_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/distributions/__init__.py` & `pymc-experimental-0.0.6/pymc_experimental/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/distributions/continuous.py` & `pymc-experimental-0.0.6/pymc_experimental/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/distributions/discrete.py` & `pymc-experimental-0.0.6/pymc_experimental/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/distributions/histogram_utils.py` & `pymc-experimental-0.0.6/pymc_experimental/distributions/histogram_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/distributions/multivariate/r2d2m2cp.py` & `pymc-experimental-0.0.6/pymc_experimental/distributions/multivariate/r2d2m2cp.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/distributions/timeseries.py` & `pymc-experimental-0.0.6/pymc_experimental/distributions/timeseries.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/gp/__init__.py` & `pymc-experimental-0.0.6/pymc_experimental/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/gp/latent_approx.py` & `pymc-experimental-0.0.6/pymc_experimental/gp/latent_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/inference/__init__.py` & `pymc-experimental-0.0.6/pymc_experimental/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/inference/fit.py` & `pymc-experimental-0.0.6/pymc_experimental/inference/fit.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/inference/pathfinder.py` & `pymc-experimental-0.0.6/pymc_experimental/inference/pathfinder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/linearmodel.py` & `pymc-experimental-0.0.6/pymc_experimental/linearmodel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+from typing import Dict, Optional, Union
+
 import numpy as np
+import pandas as pd
 import pymc as pm
 
 from pymc_experimental.model_builder import ModelBuilder
 
 
 class LinearModel(ModelBuilder):
+    def __init__(self, model_config: Dict = None, sampler_config: Dict = None, nsamples=100):
+        self.nsamples = nsamples
+        super().__init__(model_config, sampler_config)
+
     """
     This class is an implementation of a single-input linear regression model in PYMC using the
     BayesianEstimator base class for interoperability with scikit-learn.
     """
 
     _model_type = "LinearModel"
     version = "0.1"
@@ -26,15 +33,19 @@
         return {
             "draws": 1_000,
             "tune": 1_000,
             "chains": 3,
             "target_accept": 0.95,
         }
 
-    def build_model(self, data=None):
+    @property
+    def output_var(self):
+        return "y_hat"
+
+    def build_model(self, X: pd.DataFrame, y: pd.Series):
         """
         Build the PyMC model.
 
         Returns
         -------
         None
 
@@ -74,24 +85,24 @@
                 "y_hat",
                 y_model,
                 sigma=obs_error,
                 shape=x.shape,
                 observed=y_data,
                 dims="observation",
             )
-            self.output_var = "y_hat"
 
-    def _data_setter(self, X, y=None):
+    def _data_setter(self, X: pd.DataFrame, y: Optional[Union[pd.DataFrame, pd.Series]] = None):
         with self.model:
-            pm.set_data({"x": X[:, 0]})
+            pm.set_data({"x": X.squeeze()})
             if y is not None:
                 pm.set_data({"y_data": y.squeeze()})
 
-    @classmethod
-    def generate_model_data(cls, nsamples=100, data=None):
+    def generate_and_preprocess_model_data(
+        self, X: Union[pd.DataFrame, pd.Series], y: pd.Series
+    ) -> None:
         """
         Generate model data for linear regression.
 
         Parameters
         ----------
         nsamples : int, optional
             The number of samples to generate. Default is 100.
@@ -108,13 +119,8 @@
         >>> import numpy as np
         >>> x, y = cls.generate_model_data()
         >>> assert isinstance(x, np.ndarray)
         >>> assert isinstance(y, np.ndarray)
         >>> assert x.shape == (100, 1)
         >>> assert y.shape == (100,)
         """
-        x = np.linspace(start=0, stop=1, num=nsamples)
-        y = 5 * x + 3
-        y = y + np.random.normal(0, 1, len(x))
-
-        x = np.expand_dims(x, -1)  # scikit assumes a dimension for features.
-        return x, y
+        self.X, self.y = X, y
```

### Comparing `pymc-experimental-0.0.5/pymc_experimental/marginal_model.py` & `pymc-experimental-0.0.6/pymc_experimental/marginal_model.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/model_builder.py` & `pymc-experimental-0.0.6/pymc_experimental/model_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     """
 
     _model_type = "BaseClass"
     version = "None"
 
     def __init__(
         self,
-        data: Union[np.ndarray, pd.DataFrame, pd.Series] = None,
         model_config: Dict = None,
         sampler_config: Dict = None,
     ):
         """
         Initializes model configuration and sampler configuration for the model
 
         Parameters
@@ -73,18 +72,16 @@
         """
         sampler_config = self.default_sampler_config if sampler_config is None else sampler_config
         self.sampler_config = sampler_config
         model_config = self.default_model_config if model_config is None else model_config
 
         self.model_config = model_config  # parameters for priors etc.
         self.model = None  # Set by build_model
-        self.output_var = ""  # Set by build_model
         self.idata: Optional[az.InferenceData] = None  # idata is generated during fitting
         self.is_fitted_ = False
-        self.data = data
 
     def _validate_data(self, X, y=None):
         if y is not None:
             return check_X_y(X, y, accept_sparse=False, y_numeric=True, multi_output=False)
         else:
             return check_array(X, accept_sparse=False)
 
@@ -120,14 +117,27 @@
 
         """
 
         raise NotImplementedError
 
     @property
     @abstractmethod
+    def output_var(self):
+        """
+        Returns the name of the output variable of the model.
+
+        Returns
+        -------
+        output_var : str
+            Name of the output variable of the model.
+        """
+        raise NotImplementedError
+
+    @property
+    @abstractmethod
     def default_model_config(self) -> Dict:
         """
         Returns a class default config dict for model builder if no model_config is provided on class initialization
         Useful for understanding structure of required model_config to allow its customization by users
         Examples
         --------
         >>>     @classmethod
@@ -172,71 +182,82 @@
         -------
         sampler_config : dict
             A set of default settings for used by model in fit process.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def generate_model_data(
-        self, data: Union[np.ndarray, pd.DataFrame, pd.Series] = None
-    ) -> pd.DataFrame:
+    def generate_and_preprocess_model_data(
+        self, X: Union[pd.DataFrame, pd.Series], y: pd.Series
+    ) -> None:
         """
-        Returns a default dataset for a class, can be used as a hint to data formatting required for the class
-        If data is not None, dataset will be created from it's content.
+        Applies preprocessing to the data before fitting the model.
+        if validate is True, it will check if the data is valid for the model.
+        sets self.model_coords based on provided dataset
 
         Parameters:
-        data : Union[np.ndarray, pd.DataFrame, pd.Series], optional
-            dataset that will replace the default sample data
-
+        X : array, shape (n_obs, n_features)
+        y : array, shape (n_obs,)
 
         Examples
         --------
         >>>     @classmethod
-        >>>     def generate_model_data(self):
+        >>>     def generate_and_preprocess_model_data(self, X, y):
         >>>         x = np.linspace(start=1, stop=50, num=100)
         >>>         y = 5 * x + 3 + np.random.normal(0, 1, len(x)) * np.random.rand(100)*10 +  np.random.rand(100)*6.4
-        >>>         data = pd.DataFrame({'input': x, 'output': y})
+        >>>         X = pd.DataFrame(x, columns=['x'])
+        >>>         y = pd.Series(y, name='y')
+        >>>         self.X = X
+        >>>         self.y = y
 
         Returns
         -------
-        data : pd.DataFrame
-            The data we want to train the model on.
+        None
 
         """
         raise NotImplementedError
 
     @abstractmethod
     def build_model(
         self,
-        data: Union[np.ndarray, pd.DataFrame, pd.Series] = None,
-        model_config: Dict = None,
+        X: pd.DataFrame,
+        y: pd.Series,
         **kwargs,
     ) -> None:
         """
         Creates an instance of pm.Model based on provided data and model_config, and
         attaches it to self.
 
         Parameters
         ----------
-        data : dict
-            Preformated data that is going to be used in the model. For efficiency reasons it should contain only the necesary data columns,
-            not entire available dataset since it's going to be encoded into data used to recreate the model.
-            If not provided uses data from self.data
-        model_config : dict
-            Dictionary where keys are strings representing names of parameters of the model, values are dictionaries of parameters
-            needed for creating model parameters. If not provided uses data from self.model_config
+        X : pd.DataFrame
+            The input data that is going to be used in the model. This should be a DataFrame
+            containing the features (predictors) for the model. For efficiency reasons, it should
+            only contain the necessary data columns, not the entire available dataset, as this
+            will be encoded into the data used to recreate the model.
+
+        y : pd.Series
+            The target data for the model. This should be a Series representing the output
+            or dependent variable for the model.
+
+        kwargs : dict
+            Additional keyword arguments that may be used for model configuration.
 
         See Also
         --------
         default_model_config : returns default model config
 
-        Returns:
-        ----------
+        Returns
+        -------
         None
 
+        Raises
+        ------
+        NotImplementedError
+            This is an abstract method and must be implemented in a subclass.
         """
         raise NotImplementedError
 
     def sample_model(self, **kwargs):
         """
         Sample from the PyMC model.
 
@@ -244,15 +265,15 @@
         ----------
         **kwargs : dict
             Additional keyword arguments to pass to the PyMC sampler.
 
         Returns
         -------
         xarray.Dataset
-            The PyMC3 samples dataset.
+            The PyMC samples dataset.
 
         Raises
         ------
         RuntimeError
             If the PyMC model hasn't been built yet.
 
         Examples
@@ -379,33 +400,35 @@
         >>>     ...
         >>> name = './mymodel.nc'
         >>> imported_model = MyModel.load(name)
         """
         filepath = Path(str(fname))
         idata = az.from_netcdf(filepath)
         model = cls(
-            data=idata.fit_data.to_dataframe(),
             model_config=json.loads(idata.attrs["model_config"]),
             sampler_config=json.loads(idata.attrs["sampler_config"]),
         )
         model.idata = idata
-        model.build_model()
+        dataset = idata.fit_data.to_dataframe()
+        X = dataset.drop(columns=[model.output_var])
+        y = dataset[model.output_var]
+        model.build_model(X, y)
         # All previously used data is in idata.
 
         if model.id != idata.attrs["id"]:
             raise ValueError(
                 f"The file '{fname}' does not contain an inference data of the same model or configuration as '{cls._model_type}'"
             )
 
         return model
 
     def fit(
         self,
-        X: Union[np.ndarray, pd.DataFrame, pd.Series],
-        y: Union[np.ndarray, pd.Series],
+        X: pd.DataFrame,
+        y: Optional[pd.Series] = None,
         progressbar: bool = True,
         predictor_names: List[str] = None,
         random_seed: RandomState = None,
         **kwargs: Any,
     ) -> az.InferenceData:
         """
         Fit a model using the data passed as a parameter.
@@ -437,34 +460,29 @@
         >>> model = MyModel()
         >>> idata = model.fit(data)
         Auto-assigning NUTS sampler...
         Initializing NUTS using jitter+adapt_diag...
         """
         if predictor_names is None:
             predictor_names = []
-
-        X, y = X, y
-
-        self.build_model(data=self.data)
-        self._data_setter(X, y)
+        if y is None:
+            y = np.zeros(X.shape[0])
+        y = pd.DataFrame({self.output_var: y})
+        self.generate_and_preprocess_model_data(X, y.values.flatten())
+        self.build_model(self.X, self.y)
 
         sampler_config = self.sampler_config.copy()
         sampler_config["progressbar"] = progressbar
         sampler_config["random_seed"] = random_seed
         sampler_config.update(**kwargs)
-
         self.idata = self.sample_model(**sampler_config)
-        if type(X) is np.ndarray:
-            if len(predictor_names) > 0:
-                X = pd.DataFrame(X, columns=predictor_names)
-            else:
-                X = pd.DataFrame(X, columns=[f"predictor{x}" for x in range(1, X.shape[1] + 1)])
-        if type(y) is np.ndarray:
-            y = pd.Series(y, name="target")
-        combined_data = pd.concat([X, y], axis=1)
+
+        X_df = pd.DataFrame(X, columns=X.columns)
+        combined_data = pd.concat([X_df, y], axis=1)
+        assert all(combined_data.columns), "All columns must have non-empty names"
         self.idata.add_groups(fit_data=combined_data.to_xarray())  # type: ignore
         return self.idata  # type: ignore
 
     def predict(
         self,
         X_pred: Union[np.ndarray, pd.DataFrame, pd.Series],
         extend_idata: bool = True,
@@ -509,14 +527,15 @@
             dim=["chain", "draw"], keep_attrs=True
         )
         return posterior_means.data
 
     def sample_prior_predictive(
         self,
         X_pred,
+        y_pred=None,
         samples: Optional[int] = None,
         extend_idata: bool = False,
         combined: bool = True,
         **kwargs,
     ):
         """
         Sample from the model's prior predictive distribution.
@@ -535,21 +554,23 @@
         **kwargs: Additional arguments to pass to pymc.sample_prior_predictive
 
         Returns
         -------
         prior_predictive_samples : DataArray, shape (n_pred, samples)
             Prior predictive samples for each input X_pred
         """
+        if y_pred is None:
+            y_pred = np.zeros(len(X_pred))
         if samples is None:
             samples = self.sampler_config.get("draws", 500)
 
         if self.model is None:
-            self.build_model()
+            self.build_model(X_pred, y_pred)
 
-        self._data_setter(X_pred)
+        self._data_setter(X_pred, y_pred)
         if self.model is not None:
             with self.model:  # sample with new input data
                 prior_pred: az.InferenceData = pm.sample_prior_predictive(samples, **kwargs)
                 self.set_idata_attrs(prior_pred)
                 if extend_idata:
                     if self.idata is not None:
                         self.idata.extend(prior_pred)
```

### Comparing `pymc-experimental-0.0.5/pymc_experimental/model_transform/basic.py` & `pymc-experimental-0.0.6/pymc_experimental/model_transform/basic.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/model_transform/conditioning.py` & `pymc-experimental-0.0.6/pymc_experimental/model_transform/conditioning.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/__init__.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/distributions/__init__.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_continuous.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_discrete.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_discrete_markov_chain.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_discrete_markov_chain.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/distributions/test_multivariate.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/distributions/test_multivariate.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/model_transform/test_basic.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/test_basic.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/model_transform/test_conditioning.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/model_transform/test_conditioning.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/test_histogram_approximation.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/test_histogram_approximation.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/test_linearmodel.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/test_linearmodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,128 +8,140 @@
 #
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 
+
 import hashlib
 import sys
 import tempfile
 
 import numpy as np
+import pandas as pd
 import pytest
 import xarray as xr
 
 from pymc_experimental.linearmodel import LinearModel
 
 try:
+    from sklearn import set_config
     from sklearn.compose import TransformedTargetRegressor
     from sklearn.pipeline import Pipeline
     from sklearn.preprocessing import StandardScaler
 
+    set_config(transform_output="pandas")
     sklearn_available = True
 except ImportError:
     sklearn_available = False
 
 
 @pytest.fixture(scope="module")
-def sample_input():
-    x, y = LinearModel.generate_model_data()
-    return x, y
+def toy_X():
+    x = np.linspace(start=0, stop=1, num=100)
+    X = pd.DataFrame({"input": x})
+    return X
+
+
+@pytest.fixture(scope="module")
+def toy_y(toy_X):
+    y = 5 * toy_X["input"] + 3
+    y = y + np.random.normal(0, 1, size=len(toy_X))
+    y = pd.Series(y, name="output")
+    return y
 
 
 @pytest.fixture(scope="module")
-def fitted_linear_model_instance(sample_input):
+def fitted_linear_model_instance(toy_X, toy_y):
     sampler_config = {
         "draws": 500,
         "tune": 300,
         "chains": 2,
         "target_accept": 0.95,
     }
-    x, y = sample_input
-    model = LinearModel()
-    model.fit(x, y)
+    model = LinearModel(sampler_config=sampler_config)
+    model.fit(toy_X, toy_y)
     return model
 
 
-def test_save_without_fit_raises_runtime_error():
-    x, y = LinearModel.generate_model_data()
+def test_save_without_fit_raises_runtime_error(toy_X, toy_y):
     test_model = LinearModel()
     with pytest.raises(RuntimeError):
         test_model.save("saved_model")
 
 
 def test_fit(fitted_linear_model_instance):
     model = fitted_linear_model_instance
 
-    x_pred = np.random.uniform(low=0, high=1, size=(100, 1))
-    pred = model.predict(x_pred)
-    assert len(x_pred) == len(pred)
+    new_X_pred = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=100)})
+
+    pred = model.predict(new_X_pred)
+    assert len(new_X_pred) == len(pred)
     assert isinstance(pred, np.ndarray)
-    post_pred = model.predict_posterior(x_pred)
-    assert len(x_pred) == len(post_pred)
+    post_pred = model.predict_posterior(new_X_pred)
+    assert len(new_X_pred) == len(post_pred)
     assert isinstance(post_pred, xr.DataArray)
 
 
 @pytest.mark.skipif(
     sys.platform == "win32", reason="Permissions for temp files not granted on windows CI."
 )
 def test_save_load(fitted_linear_model_instance):
     model = fitted_linear_model_instance
     temp = tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", delete=False)
     model.save(temp.name)
     model2 = LinearModel.load(temp.name)
     assert model.idata.groups() == model2.idata.groups()
 
-    x_pred = np.random.uniform(low=0, high=1, size=(100, 1))
-    pred1 = model.predict(x_pred, random_seed=423)
-    pred2 = model2.predict(x_pred, random_seed=423)
+    X_pred = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=100)})
+    pred1 = model.predict(X_pred, random_seed=423)
+    pred2 = model2.predict(X_pred, random_seed=423)
     # Predictions should be identical
     np.testing.assert_array_equal(pred1, pred2)
     temp.close()
 
 
 def test_predict(fitted_linear_model_instance):
     model = fitted_linear_model_instance
-    x_pred = np.random.uniform(low=0, high=1, size=(100, 1))
-    pred = model.predict(x_pred)
-    assert len(x_pred) == len(pred)
+    X_pred = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=100)})
+    pred = model.predict(X_pred)
+    assert len(X_pred) == len(pred)
     assert np.issubdtype(pred.dtype, np.floating)
 
 
 @pytest.mark.parametrize("combined", [True, False])
 def test_predict_posterior(fitted_linear_model_instance, combined):
     model = fitted_linear_model_instance
     n_pred = 150
-    x_pred = np.random.uniform(low=0, high=1, size=(n_pred, 1))
-    pred = model.predict_posterior(x_pred, combined=combined)
+    X_pred = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=n_pred)})
+    pred = model.predict_posterior(X_pred, combined=combined)
     chains = model.idata.sample_stats.dims["chain"]
     draws = model.idata.sample_stats.dims["draw"]
     expected_shape = (n_pred, chains * draws) if combined else (chains, draws, n_pred)
     assert pred.shape == expected_shape
     assert np.issubdtype(pred.dtype, np.floating)
     # TODO: check that extend_idata has the expected effect
 
 
 @pytest.mark.parametrize("samples", [None, 300])
 @pytest.mark.parametrize("combined", [True, False])
-def test_sample_prior_predictive(samples, combined, sample_input):
-    x, y = sample_input
+def test_sample_prior_predictive(samples, combined, toy_X, toy_y):
     model = LinearModel()
-    prior_pred = model.sample_prior_predictive(x, samples, combined=combined)[model.output_var]
+    prior_pred = model.sample_prior_predictive(toy_X, toy_y, samples, combined=combined)[
+        model.output_var
+    ]
     draws = model.sampler_config["draws"] if samples is None else samples
     chains = 1
-    expected_shape = (len(x), chains * draws) if combined else (chains, draws, len(x))
+    expected_shape = (len(toy_X), chains * draws) if combined else (chains, draws, len(toy_X))
     assert prior_pred.shape == expected_shape
     # TODO: check that extend_idata has the expected effect
 
 
-def test_id(sample_input):
-    x, y = sample_input
+def test_id():
     model_config = {
         "intercept": {"loc": 0, "scale": 10},
         "slope": {"loc": 0, "scale": 10},
         "obs_error": 2,
     }
     sampler_config = {
         "draws": 1_000,
@@ -143,15 +155,15 @@
         str(model_config.values()).encode() + model.version.encode() + model._model_type.encode()
     ).hexdigest()[:16]
 
     assert model.id == expected_id
 
 
 @pytest.mark.skipif(not sklearn_available, reason="scikit-learn package is not available.")
-def test_pipeline_integration(sample_input):
+def test_pipeline_integration(toy_X, toy_y):
     model_config = {
         "intercept": {"loc": 0, "scale": 2},
         "slope": {"loc": 0, "scale": 2},
         "obs_error": 1,
         "default_output_var": "y_hat",
     }
     model = Pipeline(
@@ -159,12 +171,11 @@
             ("input_scaling", StandardScaler()),
             (
                 "linear_model",
                 TransformedTargetRegressor(LinearModel(model_config), transformer=StandardScaler()),
             ),
         ]
     )
-    x, y = sample_input
-    model.fit(x, y)
+    model.fit(toy_X, toy_y)
 
-    x_pred = np.random.uniform(low=0, high=1, size=(100, 1))
-    model.predict(x_pred)
+    X_pred = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=100)})
+    model.predict(X_pred)
```

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/test_marginal_model.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/test_marginal_model.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/test_model_builder.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/test_model_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,61 +21,92 @@
 import pandas as pd
 import pymc as pm
 import pytest
 
 from pymc_experimental.model_builder import ModelBuilder
 
 
+@pytest.fixture(scope="module")
+def toy_X():
+    x = np.linspace(start=0, stop=1, num=100)
+    X = pd.DataFrame({"input": x})
+    return X
+
+
+@pytest.fixture(scope="module")
+def toy_y(toy_X):
+    y = 5 * toy_X["input"] + 3
+    y = y + np.random.normal(0, 1, size=len(toy_X))
+    y = pd.Series(y, name="output")
+    return y
+
+
+@pytest.fixture(scope="module")
+def fitted_model_instance(toy_X, toy_y):
+    sampler_config = {
+        "draws": 500,
+        "tune": 300,
+        "chains": 2,
+        "target_accept": 0.95,
+    }
+    model_config = {
+        "a": {"loc": 0, "scale": 10},
+        "b": {"loc": 0, "scale": 10},
+        "obs_error": 2,
+    }
+    model = test_ModelBuilder(model_config=model_config, sampler_config=sampler_config)
+    model.fit(toy_X)
+    return model
+
+
 class test_ModelBuilder(ModelBuilder):
+
     _model_type = "LinearModel"
     version = "0.1"
 
-    def build_model(self, data=None, model_config=None):
-
+    def build_model(self, X: pd.DataFrame, y: pd.Series, model_config=None):
+        self.generate_and_preprocess_model_data(X, y)
         with pm.Model() as self.model:
-            if data is None:
-                data = test_ModelBuilder.generate_model_data()
             if model_config is None:
                 model_config = self.default_model_config
-            x = pm.MutableData("x", data["input"].values)
-            y_data = pm.MutableData("y_data", data["output"].values)
+            x = pm.MutableData("x", self.X["input"].values)
+            y_data = pm.MutableData("y_data", self.y)
 
             # prior parameters
             a_loc = model_config["a"]["loc"]
             a_scale = model_config["a"]["scale"]
             b_loc = model_config["b"]["loc"]
             b_scale = model_config["b"]["scale"]
             obs_error = model_config["obs_error"]
 
             # priors
             a = pm.Normal("a", a_loc, sigma=a_scale)
             b = pm.Normal("b", b_loc, sigma=b_scale)
             obs_error = pm.HalfNormal("σ_model_fmc", obs_error)
 
             # observed data
-            y_model = pm.Normal("y_model", a + b * x, obs_error, shape=x.shape, observed=y_data)
-            self.output_var = "y_model"
+            output = pm.Normal("output", a + b * x, obs_error, shape=x.shape, observed=y_data)
+
+    @property
+    def output_var(self):
+        return "output"
 
     def _data_setter(self, x: pd.Series, y: pd.Series = None):
         with self.model:
             pm.set_data({"x": x.values})
             if y is not None:
                 pm.set_data({"y_data": y.values})
 
     @property
     def _serializable_model_config(self):
         return self.model_config
 
-    @classmethod
-    def generate_model_data(cls, data=None):
-        x = np.linspace(start=0, stop=1, num=100)
-        y = 5 * x + 3
-        y = y + np.random.normal(0, 1, len(x))
-        data = pd.DataFrame({"input": x, "output": y})
-        return data
+    def generate_and_preprocess_model_data(self, X: pd.DataFrame, y: pd.Series):
+        self.X = X
+        self.y = y
 
     @property
     def default_model_config(self) -> Dict:
         return {
             "a": {"loc": 0, "scale": 10},
             "b": {"loc": 0, "scale": 10},
             "obs_error": 2,
@@ -86,97 +117,95 @@
         return {
             "draws": 1_000,
             "tune": 1_000,
             "chains": 3,
             "target_accept": 0.95,
         }
 
-    @staticmethod
-    def initial_build_and_fit(check_idata=True) -> ModelBuilder:
-        data = test_ModelBuilder.generate_model_data()
-        model_builder = test_ModelBuilder()
-        model_builder.idata = model_builder.fit(X=data["input"], y=data["output"])
-        if check_idata:
-            assert model_builder.idata is not None
-            assert "posterior" in model_builder.idata.groups()
-        return model_builder
+
+def test_initial_build_and_fit(fitted_model_instance, check_idata=True) -> ModelBuilder:
+    if check_idata:
+        assert fitted_model_instance.idata is not None
+        assert "posterior" in fitted_model_instance.idata.groups()
 
 
 def test_save_without_fit_raises_runtime_error():
     model_builder = test_ModelBuilder()
     with pytest.raises(RuntimeError):
         model_builder.save("saved_model")
 
 
-def test_empty_sampler_config_fit():
+def test_empty_sampler_config_fit(toy_X, toy_y):
     sampler_config = {}
     model_builder = test_ModelBuilder(sampler_config=sampler_config)
-    data = test_ModelBuilder.generate_model_data()
-    model_builder.idata = model_builder.fit(X=data["input"], y=data["output"])
+    model_builder.idata = model_builder.fit(X=toy_X, y=toy_y)
     assert model_builder.idata is not None
     assert "posterior" in model_builder.idata.groups()
 
 
-def test_fit():
-    model = test_ModelBuilder.initial_build_and_fit()
-    x_pred = np.random.uniform(low=0, high=1, size=100)
-    prediction_data = pd.DataFrame({"input": x_pred})
-    pred = model.predict(prediction_data["input"])
-    post_pred = model.sample_posterior_predictive(
+def test_fit(fitted_model_instance):
+    prediction_data = pd.DataFrame({"input": np.random.uniform(low=0, high=1, size=100)})
+    pred = fitted_model_instance.predict(prediction_data["input"])
+    post_pred = fitted_model_instance.sample_posterior_predictive(
         prediction_data["input"], extend_idata=True, combined=True
     )
-    post_pred.y_model.shape[0] == prediction_data.input.shape
+    post_pred[fitted_model_instance.output_var].shape[0] == prediction_data.input.shape
+
+
+def test_fit_no_y(toy_X):
+    model_builder = test_ModelBuilder()
+    model_builder.idata = model_builder.fit(X=toy_X)
+    assert model_builder.model is not None
+    assert model_builder.idata is not None
+    assert "posterior" in model_builder.idata.groups()
 
 
 @pytest.mark.skipif(
     sys.platform == "win32", reason="Permissions for temp files not granted on windows CI."
 )
-def test_save_load():
-    test_builder = test_ModelBuilder.initial_build_and_fit()
+def test_save_load(fitted_model_instance):
     temp = tempfile.NamedTemporaryFile(mode="w", encoding="utf-8", delete=False)
-    test_builder.save(temp.name)
+    fitted_model_instance.save(temp.name)
     test_builder2 = test_ModelBuilder.load(temp.name)
-    assert test_builder.idata.groups() == test_builder2.idata.groups()
+    assert fitted_model_instance.idata.groups() == test_builder2.idata.groups()
 
     x_pred = np.random.uniform(low=0, high=1, size=100)
     prediction_data = pd.DataFrame({"input": x_pred})
-    pred1 = test_builder.predict(prediction_data["input"])
+    pred1 = fitted_model_instance.predict(prediction_data["input"])
     pred2 = test_builder2.predict(prediction_data["input"])
     assert pred1.shape == pred2.shape
     temp.close()
 
 
-def test_predict():
-    model = test_ModelBuilder.initial_build_and_fit()
+def test_predict(fitted_model_instance):
     x_pred = np.random.uniform(low=0, high=1, size=100)
     prediction_data = pd.DataFrame({"input": x_pred})
-    pred = model.predict(prediction_data["input"])
+    pred = fitted_model_instance.predict(prediction_data["input"])
     # Perform elementwise comparison using numpy
     assert type(pred) == np.ndarray
     assert len(pred) > 0
 
 
 @pytest.mark.parametrize("combined", [True, False])
-def test_sample_posterior_predictive(combined):
-    model = test_ModelBuilder.initial_build_and_fit()
+def test_sample_posterior_predictive(fitted_model_instance, combined):
     n_pred = 100
     x_pred = np.random.uniform(low=0, high=1, size=n_pred)
     prediction_data = pd.DataFrame({"input": x_pred})
-    pred = model.sample_posterior_predictive(
+    pred = fitted_model_instance.sample_posterior_predictive(
         prediction_data["input"], combined=combined, extend_idata=True
     )
-    chains = model.idata.sample_stats.dims["chain"]
-    draws = model.idata.sample_stats.dims["draw"]
+    chains = fitted_model_instance.idata.sample_stats.dims["chain"]
+    draws = fitted_model_instance.idata.sample_stats.dims["draw"]
     expected_shape = (n_pred, chains * draws) if combined else (chains, draws, n_pred)
-    assert pred["y_model"].shape == expected_shape
-    assert np.issubdtype(pred["y_model"].dtype, np.floating)
+    assert pred[fitted_model_instance.output_var].shape == expected_shape
+    assert np.issubdtype(pred[fitted_model_instance.output_var].dtype, np.floating)
 
 
 def test_id():
-    model = test_ModelBuilder()
+    model_builder = test_ModelBuilder()
     expected_id = hashlib.sha256(
-        str(model.model_config.values()).encode()
-        + model.version.encode()
-        + model._model_type.encode()
+        str(model_builder.model_config.values()).encode()
+        + model_builder.version.encode()
+        + model_builder._model_type.encode()
     ).hexdigest()[:16]
 
-    assert model.id == expected_id
+    assert model_builder.id == expected_id
```

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/test_pathfinder.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/test_pathfinder.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/test_pivoted_cholesky.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/test_pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/test_prior_from_trace.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/test_prior_from_trace.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/test_splines.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/tests/utils/test_model_fgraph.py` & `pymc-experimental-0.0.6/pymc_experimental/tests/utils/test_model_fgraph.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/utils/__init__.py` & `pymc-experimental-0.0.6/pymc_experimental/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/utils/linear_cg.py` & `pymc-experimental-0.0.6/pymc_experimental/utils/linear_cg.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/utils/model_fgraph.py` & `pymc-experimental-0.0.6/pymc_experimental/utils/model_fgraph.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/utils/pivoted_cholesky.py` & `pymc-experimental-0.0.6/pymc_experimental/utils/pivoted_cholesky.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/utils/prior.py` & `pymc-experimental-0.0.6/pymc_experimental/utils/prior.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/utils/pytensorf.py` & `pymc-experimental-0.0.6/pymc_experimental/utils/pytensorf.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental/utils/spline.py` & `pymc-experimental-0.0.6/pymc_experimental/utils/spline.py`

 * *Files identical despite different names*

### Comparing `pymc-experimental-0.0.5/pymc_experimental.egg-info/PKG-INFO` & `pymc-experimental-0.0.6/pymc_experimental.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc-experimental
-Version: 0.0.5
+Version: 0.0.6
 Summary: A home for new additions to PyMC, which may include unusual probability distribitions, advanced model fitting algorithms, or any code that may be inappropriate to include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.5 Summary: A home
+Metadata-Version: 2.1 Name: pymc-experimental Version: 0.0.6 Summary: A home
 for new additions to PyMC, which may include unusual probability distribitions,
 advanced model fitting algorithms, or any code that may be inappropriate to
 include in the pymc repository, but may want to be made available to users.
 Home-page: http://github.com/pymc-devs/pymc-experimental Maintainer: PyMC
 Developers Maintainer-email: pymc.devs@gmail.com License: Apache License,
 Version 2.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

### Comparing `pymc-experimental-0.0.5/pymc_experimental.egg-info/SOURCES.txt` & `pymc-experimental-0.0.6/pymc_experimental.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 pymc_experimental/gp/latent_approx.py
 pymc_experimental/inference/__init__.py
 pymc_experimental/inference/fit.py
 pymc_experimental/inference/pathfinder.py
 pymc_experimental/model_transform/__init__.py
 pymc_experimental/model_transform/basic.py
 pymc_experimental/model_transform/conditioning.py
+pymc_experimental/preprocessing/__init__.py
+pymc_experimental/preprocessing/standard_scaler.py
 pymc_experimental/tests/__init__.py
 pymc_experimental/tests/test_histogram_approximation.py
 pymc_experimental/tests/test_linearmodel.py
 pymc_experimental/tests/test_marginal_model.py
 pymc_experimental/tests/test_model_builder.py
 pymc_experimental/tests/test_pathfinder.py
 pymc_experimental/tests/test_pivoted_cholesky.py
```

### Comparing `pymc-experimental-0.0.5/setup.py` & `pymc-experimental-0.0.6/setup.py`

 * *Files identical despite different names*

