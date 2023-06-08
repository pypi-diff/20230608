# Comparing `tmp/gurobi-machinelearning-1.2.3.tar.gz` & `tmp/gurobi-machinelearning-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gurobi-machinelearning-1.2.3.tar", last modified: Thu May 25 10:39:55 2023, max compression
+gzip compressed data, was "gurobi-machinelearning-1.3.0rc1.tar", last modified: Thu Jun  8 08:21:16 2023, max compression
```

## Comparing `gurobi-machinelearning-1.2.3.tar` & `gurobi-machinelearning-1.3.0rc1.tar`

### file list

```diff
@@ -1,52 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.109146 gurobi-machinelearning-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-25 10:39:55.109146 gurobi-machinelearning-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 10:39:55.109146 gurobi-machinelearning-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.101146 gurobi-machinelearning-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.101146 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6709 2023-05-25 10:39:55.000000 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-25 10:39:55.000000 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 10:39:55.000000 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-25 10:39:55.000000 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 10:39:55.000000 gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.101146 gurobi-machinelearning-1.2.3/src/gurobi_ml/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-25 10:39:48.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/add_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.105146 gurobi-machinelearning-1.2.3/src/gurobi_ml/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/keras/keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.105146 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/_var_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/base_predictor_constr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/get_convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.105146 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/neural_net.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/submodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/register_user_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/registered_predictors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.105146 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/base_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/column_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/linear_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/mlpregressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/pls_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/predictors_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/skgetter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 10:39:55.109146 gurobi-machinelearning-1.2.3/src/gurobi_ml/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-25 10:39:46.000000 gurobi-machinelearning-1.2.3/src/gurobi_ml/torch/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.267817 gurobi-machinelearning-1.3.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.271817 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-06-08 08:21:16.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-08 08:21:16.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:21:16.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 08:21:16.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 08:21:16.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.271817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-08 08:21:09.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/add_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.271817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/keras/keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.271817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/_var_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8545 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/base_predictor_constr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.271817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/decision_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/decision_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/decision_tree/decision_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/get_convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/neural_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/submodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/register_user_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/registered_predictors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/base_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/column_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4597 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/linear_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/mlpregressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/pls_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/predictors_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/skgetter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/torch/sequential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.275817 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/xgboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9472 2023-06-08 08:21:07.000000 gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/xgboost/xgboost_regressor.py
```

### Comparing `gurobi-machinelearning-1.2.3/LICENSE` & `gurobi-machinelearning-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.3/PKG-INFO` & `gurobi-machinelearning-1.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.2.3
+Version: 1.3.0rc1
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
```

### Comparing `gurobi-machinelearning-1.2.3/README.md` & `gurobi-machinelearning-1.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `gurobi-machinelearning-1.2.3/pyproject.toml` & `gurobi-machinelearning-1.3.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gurobi-machinelearning"
-version = "1.2.3"
+version = "1.3.0rc1"
 description = "package to insert ML models in Gurobi"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="Apache-2.0"}
 keywords = ["mathematical optimization", "gurobi", "scikit-learn", "pytorch", "tensorflow", "ml"]
 authors = [
   {name = "Gurobi Optimization LLC"}
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/PKG-INFO` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gurobi-machinelearning
-Version: 1.2.3
+Version: 1.3.0rc1
 Summary: package to insert ML models in Gurobi
 Author: Gurobi Optimization LLC
 Maintainer: Pierre Bonami
 Maintainer-email: bonami@gurobi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/Gurobi/gurobi-machinelearning
 Project-URL: Documentation, https://gurobi-optimization-gurobi-machine-learning.readthedocs-hosted.com
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_machinelearning.egg-info/SOURCES.txt` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_machinelearning.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 src/gurobi_ml/keras/__init__.py
 src/gurobi_ml/keras/keras.py
 src/gurobi_ml/modeling/__init__.py
 src/gurobi_ml/modeling/_var_utils.py
 src/gurobi_ml/modeling/base_predictor_constr.py
 src/gurobi_ml/modeling/get_convertor.py
 src/gurobi_ml/modeling/submodel.py
+src/gurobi_ml/modeling/decision_tree/__init__.py
+src/gurobi_ml/modeling/decision_tree/decision_tree_model.py
 src/gurobi_ml/modeling/neuralnet/__init__.py
 src/gurobi_ml/modeling/neuralnet/activations.py
 src/gurobi_ml/modeling/neuralnet/layers.py
 src/gurobi_ml/modeling/neuralnet/neural_net.py
 src/gurobi_ml/sklearn/__init__.py
 src/gurobi_ml/sklearn/base_regressions.py
 src/gurobi_ml/sklearn/column_transformer.py
@@ -35,8 +37,10 @@
 src/gurobi_ml/sklearn/pipeline.py
 src/gurobi_ml/sklearn/pls_regression.py
 src/gurobi_ml/sklearn/predictors_list.py
 src/gurobi_ml/sklearn/preprocessing.py
 src/gurobi_ml/sklearn/random_forest_regressor.py
 src/gurobi_ml/sklearn/skgetter.py
 src/gurobi_ml/torch/__init__.py
-src/gurobi_ml/torch/sequential.py
+src/gurobi_ml/torch/sequential.py
+src/gurobi_ml/xgboost/__init__.py
+src/gurobi_ml/xgboost/xgboost_regressor.py
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/__init__.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/_version.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/_version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,15 +17,15 @@
 from importlib import metadata
 
 try:
     __version__ = metadata.version("gurobi_machinelearning")
 except metadata.PackageNotFoundError:
     __version__ = "dev"
 
-GIT_HASH = "dec8b6055b1d6cd38bcfb24a0c7d9510b6e4cca1"
+GIT_HASH = "f6a98a0a6ffe194679d00661f204c6204d55f882"
 
 
 def get_versions():
     """Get package version."""
     # Downloaded package with inserted git hash.
     if "Format" not in GIT_HASH:
         git_hash = f"-{GIT_HASH}"
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/add_predictor.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/add_predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/exceptions.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/keras/__init__.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/xgboost/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from .keras import KerasNetworkConstr, add_keras_constr
+from .xgboost_regressor import add_xgboost_regressor_constr, add_xgbrfregressor_constr
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/keras/keras.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/keras/keras.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -130,11 +130,16 @@
                     name=f"dense{i}",
                     **kwargs,
                 )
                 _input = layer.output
         if self._output is None:
             self._output = layer.output
 
-    def get_error(self):
+    def get_error(self, eps=None):
         if self._has_solution:
-            return np.abs(self.predictor.predict(self.input_values) - self.output.X)
+            r_val = np.abs(
+                self.predictor.predict(self.input_values) - self.output_values
+            )
+            if eps is not None and np.max(r_val) > eps:
+                print(f"{self.input_values} != {self.output_values}")
+            return r_val
         raise NoSolution()
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/__init__.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/_var_utils.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/_var_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/base_predictor_constr.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/base_predictor_constr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -156,15 +156,15 @@
             self.input_values
             return True
         except gp.GurobiError:
             pass
         return False
 
     @abstractmethod
-    def get_error(self):
+    def get_error(self, eps):
         """Returns error in Gurobi's solution with respect to prediction from input.
 
         Returns
         -------
         error : ndarray of same shape as :py:attr:`gurobi_ml.modeling.base_predictor_constr.AbstractPredictorConstr.output`
             Assuming that we have a solution for the input and output variables
             `x, y`. Returns the absolute value of the differences between `predictor.predict(x)` and
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/get_convertor.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/get_convertor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/__init__.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/activations.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/activations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/layers.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -37,15 +37,16 @@
         **kwargs,
     ):
         self.activation = activation_function
         AbstractPredictorConstr.__init__(
             self, gp_model, input_vars, output_vars, **kwargs
         )
 
-    def get_error(self):
+    def get_error(self, eps=None):
+        # We can't compute externally the error of a layer
         assert False
 
     def print_stats(self, abbrev=False, file=None):
         """Print statistics about submodel created.
 
         Parameters
         ----------
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/neuralnet/neural_net.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/neuralnet/neural_net.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/modeling/submodel.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/modeling/submodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/register_user_predictor.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/register_user_predictor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/registered_predictors.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/registered_predictors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,15 +24,17 @@
     if "sklearn" in sys.modules:
         from .sklearn import (  # pylint: disable=import-outside-toplevel
             add_pipeline_constr,
         )
         from .sklearn.predictors_list import (  # pylint: disable=import-outside-toplevel
             sklearn_predictors,
         )
-        from .sklearn.preprocessing import sklearn_transformers
+        from .sklearn.preprocessing import (
+            sklearn_transformers,  # pylint: disable-import-outside-toplevel
+        )
 
         return (
             sklearn_predictors()
             | sklearn_transformers()
             | {
                 "Pipeline": add_pipeline_constr,
             }
@@ -49,14 +51,31 @@
             add_sequential_constr,
         )
 
         return {torch.nn.Sequential: add_sequential_constr}
     return {}
 
 
+def xgboost_convertors():
+    """Collect known PyTorch objects that can be formulated and the conversion class."""
+    if "xgboost" in sys.modules:
+        import xgboost as xgb  # pylint: disable=import-outside-toplevel
+
+        from .xgboost import (  # pylint: disable=import-outside-toplevel
+            add_xgboost_regressor_constr,
+            add_xgbrfregressor_constr,
+        )
+
+        return {
+            xgb.core.Booster: add_xgboost_regressor_constr,
+            xgb.XGBRFRegressor: add_xgbrfregressor_constr,
+        }
+    return {}
+
+
 def keras_convertors():
     """Collect known Keras objects that can be embedded and the conversion class."""
     if "tensorflow" in sys.modules:
         from keras.engine.functional import (  # pylint: disable=import-outside-toplevel
             Functional,
         )
         from keras.engine.training import (  # pylint: disable=import-outside-toplevel
@@ -76,9 +95,10 @@
 
 def registered_predictors():
     """Return the list of registered predictors."""
     convertors = {}
     convertors |= sklearn_convertors()
     convertors |= pytorch_convertors()
     convertors |= keras_convertors()
+    convertors |= xgboost_convertors()
     convertors |= user_predictors()
     return convertors
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/__init__.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/base_regressions.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/base_regressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/column_transformer.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/column_transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/decision_tree_regressor.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/xgboost/xgboost_regressor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -10,290 +10,272 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 """Module for formulating a
-:external+sklearn:py:class:`sklearn.tree.DecisionTreeRegressor`
-in a :gurobipy:`model`.
+XGBoost gradient boosting regressor
+into a :gurobipy:`model`.
 """
 
 
+import json
+
 import numpy as np
+import xgboost as xgb
 from gurobipy import GRB
 
+from ..exceptions import NoModel, NoSolution
 from ..modeling import AbstractPredictorConstr
-from .skgetter import SKgetter
+from ..modeling.decision_tree import leaf_formulation
 
 
-def add_decision_tree_regressor_constr(
-    gp_model,
-    decision_tree_regressor,
-    input_vars,
-    output_vars=None,
-    epsilon=0.0,
-    **kwargs,
+def add_xgbrfregressor_constr(
+    gp_model, xgboost_regressor, input_vars, output_vars=None, epsilon=0.0, **kwargs
 ):
-    """Formulate decision_tree_regressor into gp_model.
+    """Formulate xgboost_regressor into gp_model.
 
     The formulation predicts the values of output_vars using input_vars
-    according to decision_tree_regressor. See our :ref:`User's Guide <Decision
-    Tree Regression>` for details on the mip formulation used.
+    according to xgboost_regressor. See our :ref:`User's Guide
+    <Gradient Boosting Regression>` for details on the mip formulation used.
+
+    This version is for using directly with the Scikit-Learn wrapper of XGBoost.
+    Note that only "gbtree" regressors are supported at this point.
 
     Parameters
     ----------
     gp_model : :gurobipy:`model`
         The gurobipy model where the predictor should be inserted.
-    decision_tree_regressor : :external+sklearn:py:class:`sklearn.tree.DecisionTreeRegressor`
-        The decision tree regressor to insert as predictor.
+    xgboost_regressor : :external+xgb:py:class:`xgboost.XGBRFRegressor`
+        The gradient boosting regressor to insert as predictor.
     input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
-        Decision variables used as input for decision tree in model.
+        Decision variables used as input for gradient boosting regressor in model.
     output_vars : :gurobipy:`mvar` or :gurobipy:`var` array like, optional
-        Decision variables used as output for decision tree in model.
-    epsilon : float, optional
-        Small value used to impose strict inequalities for splitting nodes in
-        MIP formulations.
+        Decision variables used as output for gradient boosting regressor in model.
+
     Returns
     -------
-    DecisionTreeRegressorConstr
-        Object containing information about what was added to gp_model to
-        formulate decision_tree_regressor
+    XGBoostRegressorConstr
+        Object containing information about what was added to gp_model to formulate
+        gradient_boosting_regressor.
 
     Note
     ----
-
     |VariablesDimensionsWarn|
 
-    Warning
-    -------
-
-    Although decision trees with multiple outputs are tested they were never
-    used in a non-trivial optimization model. It should be used with care at
-    this point.
+    Also see
+    :py:func:`gurobi_ml.sklearn.decision_tree_regressor.add_decision_tree_regressor`
+    for specific parameters to model decision tree estimators.
+
+    Raises
+    ------
+    NoModel
+        If the booster is not of type "gbtree".
     """
-    return DecisionTreeRegressorConstr(
-        gp_model, decision_tree_regressor, input_vars, output_vars, epsilon, **kwargs
+    return XGBoostRegressorConstr(
+        gp_model,
+        xgboost_regressor.get_booster(),
+        input_vars,
+        output_vars,
+        epsilon=epsilon,
+        **kwargs,
     )
 
 
-class DecisionTreeRegressorConstr(SKgetter, AbstractPredictorConstr):
-    """Class to model trained
-    :external+sklearn:py:class:`sklearn.tree.DecisionTreeRegressor` with
-    gurobipy.
+def add_xgboost_regressor_constr(
+    gp_model, xgboost_regressor, input_vars, output_vars=None, epsilon=0.0, **kwargs
+):
+    """Formulate xgboost_regressor into gp_model.
 
-    |ClassShort|
+    The formulation predicts the values of output_vars using input_vars
+    according to xgboost_regressor. See our :ref:`User's Guide
+    <Gradient Boosting Regression>` for details on the mip formulation used.
+
+    Note that only "gbtree" regressors are supported at this point.
+
+    Parameters
+    ----------
+    gp_model : :gurobipy:`model`
+        The gurobipy model where the predictor should be inserted.
+    xgboost_regressor : :external+xgb:py:class:`xgboost.Booster`
+        The gradient boosting regressor to insert as predictor.
+    input_vars : :gurobipy:`mvar` or :gurobipy:`var` array like
+        Decision variables used as input for gradient boosting regressor in model.
+    output_vars : :gurobipy:`mvar` or :gurobipy:`var` array like, optional
+        Decision variables used as output for gradient boosting regressor in model.
+
+    Returns
+    -------
+    XGBoostRegressorConstr
+        Object containing information about what was added to gp_model to formulate
+        gradient_boosting_regressor.
+
+    Note
+    ----
+    |VariablesDimensionsWarn|
+
+    Also see
+    :py:func:`gurobi_ml.sklearn.decision_tree_regressor.add_decision_tree_regressor`
+    for specific parameters to model decision tree estimators.
+
+    Raises
+    ------
+    NoModel
+        If the booster is not of type "gbtree".
     """
+    return XGBoostRegressorConstr(
+        gp_model, xgboost_regressor, input_vars, output_vars, epsilon=epsilon, **kwargs
+    )
 
+
+class TreeEstimator(AbstractPredictorConstr):
     def __init__(
-        self,
-        gp_model,
-        predictor,
-        input_vars,
-        output_vars=None,
-        epsilon=0.0,
-        scale=1.0,
-        float_type=np.float32,
-        formulation="leafs",
-        **kwargs,
+        self, gp_model, tree, input_vars, output_vars, epsilon, timer, verbose, **kwargs
     ):
-        self.epsilon = epsilon
-        self.scale = scale
-        self.float_type = float_type
-        self._default_name = "tree_reg"
-
-        formulations = ("leafs", "paths")
-        if formulation not in formulations:
-            raise ValueError(
-                "Wrong value for formulation should be one of {}.".format(formulations)
-            )
-        self._formulation = formulation
-        SKgetter.__init__(self, predictor, input_vars)
+        self._default_name = "tree"
+        self._tree = tree
+        self._epsilon = epsilon
+        self._timer = timer
+        self._verbose = verbose
         AbstractPredictorConstr.__init__(
             self, gp_model, input_vars, output_vars, **kwargs
         )
 
-    def _compute_leafs_bounds(self):
+    def _mip_model(self, **kwargs):
+        leaf_formulation(
+            self._gp_model,
+            self.input,
+            self.output,
+            self._tree,
+            self._epsilon,
+            self._name_var,
+            self._verbose,
+            self._timer,
+        )
 
-        tree = self.predictor.tree_
+    def get_error(self, eps):
+        assert False
 
-        node_lb = -np.ones((tree.n_features, tree.capacity)) * GRB.INFINITY
-        node_ub = np.ones((tree.n_features, tree.capacity)) * GRB.INFINITY
 
-        children_left = tree.children_left
-        children_right = tree.children_right
-        feature = tree.feature
-        threshold = tree.threshold
-
-        stack = [
-            0,
-        ]
-        while len(stack):
-            node = stack.pop()
-            left = children_left[node]
-            if left < 0:
-                continue
-            right = children_right[node]
-            assert left not in stack
-            assert right not in stack
-            node_ub[:, right] = node_ub[:, node]
-            node_lb[:, right] = node_lb[:, node]
-            node_ub[:, left] = node_ub[:, node]
-            node_lb[:, left] = node_lb[:, node]
-
-            node_ub[feature[node], left] = threshold[node]
-            node_lb[feature[node], right] = threshold[node] + self.epsilon
-            stack.append(right)
-            stack.append(left)
-        return (node_lb, node_ub)
+class XGBoostRegressorConstr(AbstractPredictorConstr):
+    """Class to model trained :external+xgb:py:class:`xgboost.Booster`
+    with gurobipy.
 
-    def _leaf_mip_model(self, **kwargs):
-        tree = self.predictor.tree_
-        model = self._gp_model
-
-        _input = self._input
-        output = self._output
-        outdim = output.shape[1]
-        nex = _input.shape[0]
-
-        verbose = self.verbose
-
-        timer = AbstractPredictorConstr._ModelingTimer()
+    |ClassShort|
+    """
 
-        # Collect leaf nodes
-        leafs = tree.children_left < 0
-        leafs_vars = model.addMVar(
-            (nex, sum(leafs)), vtype=GRB.BINARY, name=self._name_var("leafs")
+    def __init__(
+        self, gp_model, xgb_regressor, input_vars, output_vars, epsilon=0.0, **kwargs
+    ):
+        self._output_shape = 1
+        self.estimators_ = []
+        self.xgb_regressor = xgb_regressor
+        self._default_name = "xgb_reg"
+        self.epsilon = epsilon
+        AbstractPredictorConstr.__init__(
+            self, gp_model, input_vars, output_vars, **kwargs
         )
 
-        if verbose:
-            timer.timing(f"Added {nex*sum(leafs)} leafs vars")
-        (node_lb, node_ub) = self._compute_leafs_bounds()
-        input_ub = _input.getAttr(GRB.Attr.UB)
-        input_lb = _input.getAttr(GRB.Attr.LB)
-
-        for i, node in enumerate(leafs.nonzero()[0]):
-            reachable = (input_ub >= node_lb[:, node]).all(axis=1) & (
-                input_lb <= node_ub[:, node]
-            ).all(axis=1)
-            # Non reachable nodes
-            leafs_vars[~reachable, i].setAttr(GRB.Attr.UB, 0.0)
-            # Leaf node:
-            rhs = output[reachable, :].tolist()
-            lhs = leafs_vars[reachable, i].tolist()
-            values = tree.value[node, :, 0]
-            n_indicators = sum(reachable)
-            for l_var, r_vars in zip(lhs, rhs):
-                for r_var, value in zip(r_vars, values):
-                    model.addGenConstrIndicator(l_var, 1, r_var, GRB.EQUAL, value)
-
-            for feature in range(tree.n_features):
-                lb = node_lb[feature, node]
-                ub = node_ub[feature, node]
-
-                if lb > -GRB.INFINITY:
-                    tight = (input_lb[:, feature] < lb) & reachable
-                    lhs = leafs_vars[tight, i].tolist()
-                    rhs = _input[tight, feature].tolist()
-                    n_indicators += sum(tight)
-                    for l_var, r_var in zip(lhs, rhs):
-                        model.addGenConstrIndicator(
-                            l_var, 1, r_var, GRB.GREATER_EQUAL, lb
-                        )
-
-                if ub < GRB.INFINITY:
-                    tight = (input_ub[:, feature] > ub) & reachable
-                    lhs = leafs_vars[tight, i].tolist()
-                    rhs = _input[tight, feature].tolist()
-                    n_indicators += sum(tight)
-                    for l_var, r_var in zip(lhs, rhs):
-                        model.addGenConstrIndicator(l_var, 1, r_var, GRB.LESS_EQUAL, ub)
-            if verbose:
-                timer.timing(f"Added leaf {node} using {n_indicators} indicators")
-
-        # We should attain 1 leaf
-        model.addConstr(leafs_vars.sum(axis=1) == 1)
-
-        if verbose:
-            timer.timing(f"Added {nex} linear constraints")
-
-        output.setAttr(GRB.Attr.LB, np.min(tree.value))
-        output.setAttr(GRB.Attr.UB, np.max(tree.value))
+    def _mip_model(self, **kwargs):
+        """Predict output variables y from input variables X using the
+        decision tree.
 
-    def _paths_mip_model(self, **kwargs):
-        tree = self.predictor.tree_
+        Both X and y should be array or list of variables of conforming dimensions.
+        """
         model = self._gp_model
+        xgb_regressor = self.xgb_regressor
 
         _input = self._input
         output = self._output
-        outdim = output.shape[1]
         nex = _input.shape[0]
-        nodes = model.addMVar(
-            (nex, tree.capacity), vtype=GRB.BINARY, name=self._name_var("node")
-        )
-
-        # Collect leafs and non-leafs nodes
-        notleafs = tree.children_left >= 0
-        leafs = tree.children_left < 0
-
-        # Connectivity constraint
-        model.addConstr(
-            nodes[:, notleafs]
-            == nodes[:, tree.children_right[notleafs]]
-            + nodes[:, tree.children_left[notleafs]]
+        timer = AbstractPredictorConstr._ModelingTimer()
+        outdim = output.shape[1]
+        assert (
+            outdim == 1
+        ), "Output dimension of gradient boosting regressor should be 1"
+
+        xgb_raw = json.loads(xgb_regressor.save_raw(raw_format="json"))
+        booster_type = xgb_raw["learner"]["gradient_booster"]["name"]
+        if booster_type != "gbtree":
+            raise NoModel(xgb_regressor, f"model not implemented for {booster_type}")
+        trees = xgb_raw["learner"]["gradient_booster"]["model"]["trees"]
+        n_estimators = len(trees)
+
+        estimators = []
+        if self._no_debug:
+            kwargs["no_record"] = True
+
+        tree_vars = model.addMVar(
+            (nex, n_estimators, 1),
+            lb=-GRB.INFINITY,
+            name=self._name_var("esimator"),
         )
 
-        # The value of the root is always 1
-        nodes[:, 0].LB = 1.0
-
-        # Node splitting
-        for node in notleafs.nonzero()[0]:
-            left = tree.children_left[node]
-            right = tree.children_right[node]
-            threshold = tree.threshold[node]
-            threshold = self.float_type(threshold)
-            scale = max(abs(1 / threshold), self.scale)
-            # Intermediate node
-            feature = tree.feature[node]
-            feat_var = _input[:, feature]
-
-            fixed_input = (feat_var.UB == feat_var.LB).all()
-
-            if fixed_input:
-                # Special case where we have an MVarPlusConst object
-                # If that feature is a constant we can directly fix it.
-                value = _input[:, feature].LB
-                fixed_left = value <= threshold
-                nodes[fixed_left, right].UB = 0.0
-                nodes[~fixed_left, left].UB = 0.0
-            else:
-                lhs = _input[:, feature].tolist()
-                rhs = nodes[:, left].tolist()
-                threshold *= scale
-                model.addConstrs(
-                    ((rhs[k] == 1) >> (scale * lhs[k] <= threshold)) for k in range(nex)
-                )
-                rhs = nodes[:, right].tolist()
-                model.addConstrs(
-                    ((rhs[k] == 1) >> (scale * lhs[k] >= threshold + self.epsilon))
-                    for k in range(nex)
+        for i, tree in enumerate(trees):
+            if self.verbose:
+                self._timer.timing(f"Estimator {i}")
+            tree["threshold"] = (
+                np.array(tree["split_conditions"], dtype=np.float32) - self.epsilon
+            )
+            tree["children_left"] = np.array(tree["left_children"])
+            tree["children_right"] = np.array(tree["right_children"])
+            tree["feature"] = np.array(tree["split_indices"])
+            tree["value"] = tree["threshold"].reshape(-1, 1)
+            tree["capacity"] = len(tree["split_conditions"])
+            tree["n_features"] = int(tree["tree_param"]["num_feature"])
+
+            def _name_tree_var(name):
+                rval = self._name_var(name)
+                if rval is None:
+                    return None
+                return rval + f"_{i}"
+
+            estimators.append(
+                TreeEstimator(
+                    self.gp_model,
+                    tree,
+                    self.input,
+                    tree_vars[:, i, :],
+                    self.epsilon,
+                    timer,
+                    self.verbose,
+                    **kwargs,
                 )
-
-        for node in leafs.nonzero()[0]:
-            # Leaf node:
-            lhs = output.tolist()
-            rhs = nodes[:, node].tolist()
-            value = tree.value[node, :, 0]
-            model.addConstrs(
-                (rhs[k] == 1) >> (lhs[k][i] == value[i])
-                for k in range(nex)
-                for i in range(outdim)
             )
 
-        output.LB = np.min(tree.value)
-        output.UB = np.max(tree.value)
+        self.estimators_ = estimators
 
-    def _mip_model(self, **kwargs):
-        if self._formulation == "leafs":
-            return self._leaf_mip_model(**kwargs)
-        else:
-            return self._paths_mip_model(**kwargs)
+        constant = float(xgb_raw["learner"]["learner_model_param"]["base_score"])
+        learning_rate = 1.0
+        model.addConstr(output == learning_rate * tree_vars.sum(axis=1) + constant)
+
+    def print_stats(self, abbrev=False, file=None):
+        """Print statistics on model additions stored by this class.
+
+        This function prints detailed statistics on the variables
+        and constraints that where added to the model.
+
+        Includes a summary of the estimators that it contains.
+
+        Arguments
+        ---------
+
+        file: None, optional
+            Text stream to which output should be redirected. By default sys.stdout.
+        """
+        super().print_stats(abbrev=abbrev, file=file)
+        if abbrev or self._no_debug:
+            return
+        print(file=file)
+
+        # self._print_container_steps("Estimator", self.estimators_, file=file)
+
+    def get_error(self, eps=None):
+        if self._has_solution:
+            xgb_in = xgb.DMatrix(self.input_values)
+            xgb_out = self.xgb_regressor.predict(xgb_in)
+            r_val = np.abs(xgb_out.reshape(-1, 1) - self.output.X)
+            if eps is not None and np.max(r_val) > eps:
+                print(f"{self.output.X} != {xgb_out.reshape(-1, 1)}")
+            return r_val
+        raise NoSolution()
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/gradient_boosting_regressor.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/gradient_boosting_regressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/linear_regression.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/linear_regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/logistic_regression.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/logistic_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/mlpregressor.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/mlpregressor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/pipeline.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/pls_regression.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/pls_regression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/predictors_list.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/predictors_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/preprocessing.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/random_forest_regressor.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/random_forest_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/sklearn/skgetter.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/sklearn/skgetter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -39,15 +39,15 @@
         predictor._check_feature_names(input_vars, reset=False)
         self.output_type = output_type
         if hasattr(predictor, "n_features_in_"):
             self._input_shape = predictor.n_features_in_
         if hasattr(predictor, "n_outputs_"):
             self._output_shape = predictor.n_outputs_
 
-    def get_error(self):
+    def get_error(self, eps=None):
         """Return error in Gurobi's solution with respect to prediction from input.
 
         Returns
         -------
         error : ndarray of same shape as :py:attr:`gurobi_ml.modeling.base_predictor_constr.AbstractPredictorConstr.output`
             Assuming that we have a solution for the input and output variables
             `x, y`. Returns the absolute value of the differences between `predictor.predict(x)` and
@@ -65,15 +65,19 @@
             elif self.output_type == "probability":
                 predicted = self.predictor.predict_proba(X)
             else:
                 predicted = self.predictor.predict(X)
             output_values = self.output_values
             if len(predicted.shape) == 1 and len(output_values.shape) == 2:
                 predicted = predicted.reshape(-1, 1)
-            return np.abs(predicted - output_values)
+            r_val = np.abs(predicted - output_values)
+            if eps is not None and np.max(r_val) > eps:
+                print(f"{predicted} != {output_values}")
+            return r_val
+
         raise NoSolution()
 
 
 class SKtransformer(AbstractPredictorConstr):
     """Utility class for sklearn preprocessing models convertors.
 
     Implement some common functionalities.
@@ -89,15 +93,15 @@
         if hasattr(transformer, "n_features_in_"):
             self._input_shape = transformer.n_features_in_
         if hasattr(transformer, "n_output_features_"):
             self._output_shape = transformer.n_output_features_
         check_is_fitted(transformer)
         super().__init__(gp_model, input_vars, **kwargs)
 
-    def get_error(self):
+    def get_error(self, eps=None):
         """Return error in Gurobi's solution with respect to preprocessing from input.
 
         Returns
         -------
         error : ndarray of same shape as :py:attr:`gurobi_ml.modeling.base_predictor_constr.AbstractPredictorConstr.output`
             Assuming that we have a solution for the input and output variables
             `x, y`. Returns the absolute value of the differences between `transformer.transform(x)` and
@@ -111,9 +115,14 @@
         if self._has_solution:
             transformer = self.transformer
             input_values = self.input_values
 
             transformed = transformer.transform(input_values)
             if len(transformed.shape) == 1:
                 transformed = transformed.reshape(-1, 1)
-            return np.abs(transformed - self.output_values)
+
+            r_val = np.abs(transformed - self.output_values)
+            if eps is not None and np.max(r_val) > eps:
+                print(f"{transformed} != {self.output_values}")
+            return r_val
+
         raise NoSolution()
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/torch/__init__.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/torch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `gurobi-machinelearning-1.2.3/src/gurobi_ml/torch/sequential.py` & `gurobi-machinelearning-1.3.0rc1/src/gurobi_ml/torch/sequential.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright © 2022 Gurobi Optimization, LLC
+# Copyright © 2023 Gurobi Optimization, LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -115,13 +115,16 @@
                     name=f"linear_{i}",
                     **kwargs,
                 )
                 _input = layer.output
         if self._output is None:
             self._output = layer.output
 
-    def get_error(self):
+    def get_error(self, eps=None):
         if self._has_solution:
             t_in = torch.from_numpy(self.input_values).float()
             t_out = self.predictor.forward(t_in)
-            return np.abs(t_out.detach().numpy() - self.output.X)
+            r_val = np.abs(t_out.detach().numpy() - self.output_values)
+            if eps is not None and np.max(r_val) > eps:
+                print(f"{t_out} != {self.output_values}")
+            return r_val
         raise NoSolution()
```

