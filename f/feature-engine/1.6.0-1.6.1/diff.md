# Comparing `tmp/feature_engine-1.6.0.tar.gz` & `tmp/feature_engine-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/feature_engine-1.6.0.tar", last modified: Mon Mar 27 17:12:58 2023, max compression
+gzip compressed data, was "dist/feature_engine-1.6.1.tar", last modified: Thu Jun  8 06:34:08 2023, max compression
```

## Comparing `feature_engine-1.6.0.tar` & `feature_engine-1.6.1.tar`

### file list

```diff
@@ -1,272 +1,274 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.795604 feature_engine-1.6.0/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1541 2023-03-27 17:12:47.000000 feature_engine-1.6.0/LICENSE.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      245 2023-03-27 17:12:47.000000 feature_engine-1.6.0/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10502 2023-03-27 17:12:58.795604 feature_engine-1.6.0/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7998 2023-03-27 17:12:47.000000 feature_engine-1.6.0/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.767604 feature_engine-1.6.0/feature_engine/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/VERSION
--rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.767604 feature_engine-1.6.0/feature_engine/_base_transformers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_base_transformers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3742 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_base_transformers/base_numerical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6114 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_base_transformers/mixins.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.767604 feature_engine-1.6.0/feature_engine/_check_input_parameters/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_check_input_parameters/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      493 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_check_input_parameters/check_init_input_params.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      916 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_check_input_parameters/check_input_dictionary.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.767604 feature_engine-1.6.0/feature_engine/_docstrings/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_docstrings/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1457 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_docstrings/fit_attributes.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.767604 feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1245 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/all_trasnformers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      714 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/discretisers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1095 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/encoders.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1464 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/outliers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      605 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1284 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_docstrings/methods.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      725 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_docstrings/substitute.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.771604 feature_engine-1.6.0/feature_engine/_prediction/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_prediction/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9573 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_prediction/base_predictor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6291 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_prediction/target_mean_classifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4043 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/_prediction/target_mean_regressor.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.771604 feature_engine-1.6.0/feature_engine/creation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      374 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/creation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4113 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/creation/base_creation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5933 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/creation/cyclical_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7927 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/creation/math_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9484 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/creation/relative_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9622 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/dataframe_checks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.771604 feature_engine-1.6.0/feature_engine/datasets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       62 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/datasets/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4107 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/datasets/titanic.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.771604 feature_engine-1.6.0/feature_engine/datetime/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      211 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/datetime/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2239 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/datetime/_datetime_constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13574 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/datetime/datetime.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11619 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/datetime/datetime_subtraction.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.771604 feature_engine-1.6.0/feature_engine/discretisation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/discretisation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6521 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/discretisation/arbitrary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2602 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/discretisation/base_discretiser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9481 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/discretisation/decision_tree.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5012 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/discretisation/equal_frequency.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5301 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/discretisation/equal_width.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5369 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/discretisation/geometric_width.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.775604 feature_engine-1.6.0/feature_engine/encoding/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      499 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/_helper_functions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9815 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/base_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6693 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/count_frequency.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11298 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/decision_tree.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8819 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/mean_encoding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11089 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/one_hot.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7202 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/ordinal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9219 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/rare_label.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14120 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/similarity_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7958 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/encoding/woe.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.775604 feature_engine-1.6.0/feature_engine/imputation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      600 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/imputation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4822 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/imputation/arbitrary_number.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2405 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/imputation/base_imputer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9089 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/imputation/categorical.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7456 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/imputation/drop_missing_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6696 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/imputation/end_tail.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3955 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/imputation/mean_median.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5509 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/imputation/missing_indicator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9421 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/imputation/random_sample.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.775604 feature_engine-1.6.0/feature_engine/outliers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/outliers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5764 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/outliers/artbitrary.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9127 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/outliers/base_outlier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4875 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/outliers/trimmer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7249 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/outliers/winsorizer.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.775604 feature_engine-1.6.0/feature_engine/preprocessing/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      265 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/preprocessing/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6401 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/preprocessing/match_categories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8388 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/preprocessing/match_columns.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.779604 feature_engine-1.6.0/feature_engine/selection/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1276 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3249 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/_docstring.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1015 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/_selection_constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6976 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/base_recursive_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5171 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/base_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7514 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/drop_constant_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7576 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/drop_correlated_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5737 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/drop_duplicate_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3753 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/drop_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22717 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/drop_psi_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9245 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/information_value.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10616 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/probe_feature_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6618 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/recursive_feature_addition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6568 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/recursive_feature_elimination.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9754 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/shuffle_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8199 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/single_feature_performance.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13113 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/smart_correlation_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11333 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/selection/target_mean_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1535 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/tags.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.779604 feature_engine-1.6.0/feature_engine/timeseries/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/timeseries/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.779604 feature_engine-1.6.0/feature_engine/timeseries/forecasting/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/timeseries/forecasting/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6784 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/timeseries/forecasting/base_forecast_transformers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7513 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/timeseries/forecasting/expanding_window_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8089 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/timeseries/forecasting/lag_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9142 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/timeseries/forecasting/window_features.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.779604 feature_engine-1.6.0/feature_engine/transformation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/transformation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6861 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/transformation/arcsin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6733 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/transformation/boxcox.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13157 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/transformation/log.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4586 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/transformation/power.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5894 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/transformation/reciprocal.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4394 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/transformation/yeojohnson.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.779604 feature_engine-1.6.0/feature_engine/variable_handling/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/variable_handling/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1094 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/variable_handling/_init_parameter_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1864 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/variable_handling/_variable_type_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14948 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/variable_handling/variable_type_selection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.779604 feature_engine-1.6.0/feature_engine/wrappers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      254 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/wrappers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14558 2023-03-27 17:12:47.000000 feature_engine-1.6.0/feature_engine/wrappers/wrappers.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.767604 feature_engine-1.6.0/feature_engine.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10502 2023-03-27 17:12:58.000000 feature_engine-1.6.0/feature_engine.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10698 2023-03-27 17:12:58.000000 feature_engine-1.6.0/feature_engine.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-27 17:12:58.000000 feature_engine-1.6.0/feature_engine.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-03-27 17:12:58.000000 feature_engine-1.6.0/feature_engine.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2023-03-27 17:12:58.000000 feature_engine-1.6.0/feature_engine.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2023-03-27 17:12:58.000000 feature_engine-1.6.0/feature_engine.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2023-03-27 17:12:47.000000 feature_engine-1.6.0/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-03-27 17:12:58.795604 feature_engine-1.6.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1700 2023-03-27 17:12:47.000000 feature_engine-1.6.0/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2023-03-27 17:12:47.000000 feature_engine-1.6.0/test_requirements.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.763604 feature_engine-1.6.0/tests/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.779604 feature_engine-1.6.0/tests/estimator_checks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/estimator_checks/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1344 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/estimator_checks/dataframe_for_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4320 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/estimator_checks/estimator_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1117 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/estimator_checks/fit_functionality_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2653 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/estimator_checks/get_feature_names_out_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1296 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/estimator_checks/init_params_allowed_values_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6359 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/estimator_checks/init_params_triggered_functionality_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      659 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/estimator_checks/non_fitted_error_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7751 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/estimator_checks/variable_selection_checks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.783604 feature_engine-1.6.0/tests/test_check_input_parameters/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_check_input_parameters/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      569 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_check_input_parameters/test_check_init_input_params.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      566 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_check_input_parameters/test_check_input_dictionary.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.783604 feature_engine-1.6.0/tests/test_creation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_creation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1004 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_creation/test_check_estimator_creation.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5574 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_creation/test_cyclical_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11048 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_creation/test_math_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12174 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_creation/test_relative_features.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.783604 feature_engine-1.6.0/tests/test_datetime/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_datetime/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4134 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_datetime/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_datetime/test_check_estimator_datetime.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17128 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_datetime/test_datetime_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11383 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_datetime/test_datetime_subtraction.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.783604 feature_engine-1.6.0/tests/test_discretisation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_discretisation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3928 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_discretisation/test_arbitrary_discretiser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2623 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_discretisation/test_base_discretizer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1038 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_discretisation/test_check_estimator_discretisers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3771 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_discretisation/test_decision_tree_discretiser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2532 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_discretisation/test_equal_frequency_discretiser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2494 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_discretisation/test_equal_width_discretiser.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3148 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_discretisation/test_geometric_width_discretiser.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.783604 feature_engine-1.6.0/tests/test_encoding/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.787604 feature_engine-1.6.0/tests/test_encoding/test_base_encoders/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_base_encoders/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      628 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1105 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin_na.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5624 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_base_encoders/test_categorical_method_mixin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7775 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_check_estimator_encoders.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14114 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_count_frequency_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6302 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_decision_tree_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_helper_functions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13945 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_mean_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16693 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_onehot_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10606 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_ordinal_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9440 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_rare_label_encoder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10991 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_similarity_encoder.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.787604 feature_engine-1.6.0/tests/test_encoding/test_woe/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_woe/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_woe/test_woe_class.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9656 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_encoding/test_woe/test_woe_encoder.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.787604 feature_engine-1.6.0/tests/test_imputation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_imputation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2891 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_imputation/test_arbitrary_number_imputer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10477 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_imputation/test_categorical_imputer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1143 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_imputation/test_check_estimator_imputers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4123 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_imputation/test_drop_missing_data.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3485 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_imputation/test_end_tail_imputer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2126 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_imputation/test_mean_mdian_imputer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3511 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_imputation/test_missing_indicator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9374 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_imputation/test_random_sample_imputer.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.787604 feature_engine-1.6.0/tests/test_outliers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_outliers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5685 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_outliers/test_arbitrary_capper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      790 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_outliers/test_check_estimator_outliers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3092 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_outliers/test_outlier_trimmer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14498 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_outliers/test_winsorizer.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.787604 feature_engine-1.6.0/tests/test_prediction/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_prediction/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1162 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_prediction/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8815 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_prediction/test_check_estimator_prediction.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7554 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_prediction/test_target_mean_classifier.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4363 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_prediction/test_target_mean_regressor.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.787604 feature_engine-1.6.0/tests/test_preprocessing/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_preprocessing/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1160 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_preprocessing/test_check_estimator_preprocessing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2531 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_preprocessing/test_match_categories.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6058 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_preprocessing/test_match_columns.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.791604 feature_engine-1.6.0/tests/test_selection/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_base_selector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3908 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_check_estimator_selectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5848 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_drop_constant_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4019 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_drop_correlated_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3967 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_drop_duplicate_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3344 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_drop_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    22348 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_drop_high_psi_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5074 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_information_value.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7039 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_probe_feature_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4594 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_recursive_feature_addition.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5260 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_recursive_feature_elimination.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4102 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_recursive_feature_selectors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3761 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_shuffle_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7218 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_single_feature_performance_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6844 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_smart_correlation_selection.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6043 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_selection/test_target_mean_selection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.791604 feature_engine-1.6.0/tests/test_time_series/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_time_series/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.791604 feature_engine-1.6.0/tests/test_time_series/test_forecasting/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_time_series/test_forecasting/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1684 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_time_series/test_forecasting/conftest.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1763 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_time_series/test_forecasting/test_check_estimator_forecasting.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11182 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_time_series/test_forecasting/test_expanding_window_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8001 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_time_series/test_forecasting/test_lag_features.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13490 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_time_series/test_forecasting/test_window_features.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.795604 feature_engine-1.6.0/tests/test_transformation/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_transformation/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2217 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_transformation/test_arcsin_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2320 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_transformation/test_boxcox_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      872 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_transformation/test_check_estimator_transformers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3987 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_transformation/test_log_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8588 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_transformation/test_logcp_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2634 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_transformation/test_power_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2324 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_transformation/test_reciprocal_transformer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2690 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_transformation/test_yeojohnson_transformer.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.795604 feature_engine-1.6.0/tests/test_variable_handling/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_variable_handling/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      828 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_variable_handling/test_init_parameter_checks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13167 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_variable_handling/test_variable_type_selection.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:58.795604 feature_engine-1.6.0/tests/test_wrappers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_wrappers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1531 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_wrappers/test_check_estimator_wrappers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19763 2023-03-27 17:12:47.000000 feature_engine-1.6.0/tests/test_wrappers/test_sklearn_wrapper.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.696991 feature_engine-1.6.1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1541 2023-06-08 06:33:58.000000 feature_engine-1.6.1/LICENSE.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      245 2023-06-08 06:33:58.000000 feature_engine-1.6.1/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10502 2023-06-08 06:34:08.696991 feature_engine-1.6.1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7998 2023-06-08 06:33:58.000000 feature_engine-1.6.1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.672991 feature_engine-1.6.1/feature_engine/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/VERSION
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.672991 feature_engine-1.6.1/feature_engine/_base_transformers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_base_transformers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3765 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_base_transformers/base_numerical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6114 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_base_transformers/mixins.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.672991 feature_engine-1.6.1/feature_engine/_check_input_parameters/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_check_input_parameters/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      493 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_check_input_parameters/check_init_input_params.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      916 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_check_input_parameters/check_input_dictionary.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.672991 feature_engine-1.6.1/feature_engine/_docstrings/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1457 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/fit_attributes.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.672991 feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1245 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/all_trasnformers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      714 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/discretisers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1095 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/encoders.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1464 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/outliers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      605 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1284 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/methods.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.672991 feature_engine-1.6.1/feature_engine/_docstrings/selection/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/selection/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3249 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/selection/_docstring.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      725 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_docstrings/substitute.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.672991 feature_engine-1.6.1/feature_engine/_prediction/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_prediction/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9573 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_prediction/base_predictor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6291 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_prediction/target_mean_classifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4043 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/_prediction/target_mean_regressor.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.672991 feature_engine-1.6.1/feature_engine/creation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      374 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/creation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4136 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/creation/base_creation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5953 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/creation/cyclical_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7947 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/creation/math_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10655 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/creation/relative_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9622 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/dataframe_checks.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.676991 feature_engine-1.6.1/feature_engine/datasets/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       62 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/datasets/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4107 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/datasets/titanic.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.676991 feature_engine-1.6.1/feature_engine/datetime/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      211 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/datetime/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2239 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/datetime/_datetime_constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13574 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/datetime/datetime.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11629 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/datetime/datetime_subtraction.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.676991 feature_engine-1.6.1/feature_engine/discretisation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      526 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/discretisation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6521 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/discretisation/arbitrary.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2622 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/discretisation/base_discretiser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9501 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/discretisation/decision_tree.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5012 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/discretisation/equal_frequency.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5301 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/discretisation/equal_width.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5369 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/discretisation/geometric_width.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.676991 feature_engine-1.6.1/feature_engine/encoding/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      636 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      499 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/_helper_functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9815 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/base_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6693 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/count_frequency.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11298 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/decision_tree.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8819 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/mean_encoding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11089 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/one_hot.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7202 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/ordinal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9375 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/rare_label.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14120 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/similarity_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9644 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/encoding/woe.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.676991 feature_engine-1.6.1/feature_engine/imputation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      600 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/imputation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4822 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/imputation/arbitrary_number.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2405 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/imputation/base_imputer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9089 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/imputation/categorical.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7461 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/imputation/drop_missing_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6696 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/imputation/end_tail.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3955 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/imputation/mean_median.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5509 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/imputation/missing_indicator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9421 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/imputation/random_sample.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.680991 feature_engine-1.6.1/feature_engine/outliers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      261 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/outliers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6212 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/outliers/artbitrary.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9128 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/outliers/base_outlier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4875 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/outliers/trimmer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7251 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/outliers/winsorizer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.680991 feature_engine-1.6.1/feature_engine/preprocessing/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      265 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/preprocessing/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6401 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/preprocessing/match_categories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8388 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/preprocessing/match_columns.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.680991 feature_engine-1.6.1/feature_engine/selection/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1276 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1015 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/_selection_constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6976 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/base_recursive_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5171 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/base_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7526 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/drop_constant_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7588 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/drop_correlated_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5749 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/drop_duplicate_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3753 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/drop_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    30284 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/drop_psi_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9257 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/information_value.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10628 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/probe_feature_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6630 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/recursive_feature_addition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6580 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/recursive_feature_elimination.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10191 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/shuffle_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8211 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/single_feature_performance.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13125 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/smart_correlation_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11345 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/selection/target_mean_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1598 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/tags.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.680991 feature_engine-1.6.1/feature_engine/timeseries/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/timeseries/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.680991 feature_engine-1.6.1/feature_engine/timeseries/forecasting/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/timeseries/forecasting/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6807 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/timeseries/forecasting/base_forecast_transformers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7533 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/timeseries/forecasting/expanding_window_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8109 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/timeseries/forecasting/lag_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9162 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/timeseries/forecasting/window_features.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.684991 feature_engine-1.6.1/feature_engine/transformation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/transformation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6881 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/transformation/arcsin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6773 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/transformation/boxcox.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13237 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/transformation/log.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4626 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/transformation/power.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5873 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/transformation/reciprocal.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4414 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/transformation/yeojohnson.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.684991 feature_engine-1.6.1/feature_engine/variable_handling/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/variable_handling/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1094 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/variable_handling/_init_parameter_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1959 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/variable_handling/_variable_type_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14948 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/variable_handling/variable_type_selection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.684991 feature_engine-1.6.1/feature_engine/wrappers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      254 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/wrappers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14558 2023-06-08 06:33:58.000000 feature_engine-1.6.1/feature_engine/wrappers/wrappers.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.672991 feature_engine-1.6.1/feature_engine.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10502 2023-06-08 06:34:08.000000 feature_engine-1.6.1/feature_engine.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10759 2023-06-08 06:34:08.000000 feature_engine-1.6.1/feature_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-08 06:34:08.000000 feature_engine-1.6.1/feature_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-08 06:34:08.000000 feature_engine-1.6.1/feature_engine.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2023-06-08 06:34:08.000000 feature_engine-1.6.1/feature_engine.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       21 2023-06-08 06:34:08.000000 feature_engine-1.6.1/feature_engine.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       81 2023-06-08 06:33:58.000000 feature_engine-1.6.1/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-08 06:34:08.696991 feature_engine-1.6.1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1700 2023-06-08 06:33:58.000000 feature_engine-1.6.1/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2023-06-08 06:33:58.000000 feature_engine-1.6.1/test_requirements.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.668991 feature_engine-1.6.1/tests/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.684991 feature_engine-1.6.1/tests/estimator_checks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/estimator_checks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1344 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/estimator_checks/dataframe_for_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4351 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/estimator_checks/estimator_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1117 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/estimator_checks/fit_functionality_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2653 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/estimator_checks/get_feature_names_out_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1296 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/estimator_checks/init_params_allowed_values_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6359 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/estimator_checks/init_params_triggered_functionality_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      659 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/estimator_checks/non_fitted_error_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7751 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/estimator_checks/variable_selection_checks.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.684991 feature_engine-1.6.1/tests/test_check_input_parameters/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_check_input_parameters/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      570 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_check_input_parameters/test_check_init_input_params.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      566 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_check_input_parameters/test_check_input_dictionary.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.684991 feature_engine-1.6.1/tests/test_creation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_creation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1694 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_creation/test_check_estimator_creation.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5574 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_creation/test_cyclical_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11048 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_creation/test_math_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13784 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_creation/test_relative_features.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.684991 feature_engine-1.6.1/tests/test_datetime/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_datetime/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4134 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_datetime/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1347 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_datetime/test_check_estimator_datetime.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17530 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_datetime/test_datetime_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11383 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_datetime/test_datetime_subtraction.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.688991 feature_engine-1.6.1/tests/test_discretisation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_discretisation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3928 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_discretisation/test_arbitrary_discretiser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2623 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_discretisation/test_base_discretizer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1668 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_discretisation/test_check_estimator_discretisers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3771 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_discretisation/test_decision_tree_discretiser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2532 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_discretisation/test_equal_frequency_discretiser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2494 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_discretisation/test_equal_width_discretiser.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3148 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_discretisation/test_geometric_width_discretiser.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.688991 feature_engine-1.6.1/tests/test_encoding/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.688991 feature_engine-1.6.1/tests/test_encoding/test_base_encoders/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_base_encoders/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      628 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_base_encoders/test_categorical_init_mixin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1105 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_base_encoders/test_categorical_init_mixin_na.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5624 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_base_encoders/test_categorical_method_mixin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8289 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_check_estimator_encoders.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14113 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_count_frequency_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6302 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_decision_tree_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      815 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_helper_functions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13944 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_mean_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    16693 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_onehot_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10605 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_ordinal_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13706 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_rare_label_encoder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10991 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_similarity_encoder.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.688991 feature_engine-1.6.1/tests/test_encoding/test_woe/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_woe/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2053 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_woe/test_woe_class.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13157 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_encoding/test_woe/test_woe_encoder.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.688991 feature_engine-1.6.1/tests/test_imputation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_imputation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2891 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_imputation/test_arbitrary_number_imputer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10477 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_imputation/test_categorical_imputer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1893 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_imputation/test_check_estimator_imputers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4123 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_imputation/test_drop_missing_data.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3485 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_imputation/test_end_tail_imputer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2126 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_imputation/test_mean_mdian_imputer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3511 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_imputation/test_missing_indicator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9374 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_imputation/test_random_sample_imputer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.692991 feature_engine-1.6.1/tests/test_outliers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_outliers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5685 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_outliers/test_arbitrary_capper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1744 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_outliers/test_check_estimator_outliers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3084 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_outliers/test_outlier_trimmer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14155 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_outliers/test_winsorizer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.692991 feature_engine-1.6.1/tests/test_prediction/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_prediction/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1162 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_prediction/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8815 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_prediction/test_check_estimator_prediction.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7554 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_prediction/test_target_mean_classifier.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4363 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_prediction/test_target_mean_regressor.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.692991 feature_engine-1.6.1/tests/test_preprocessing/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_preprocessing/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1661 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_preprocessing/test_check_estimator_preprocessing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2531 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_preprocessing/test_match_categories.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6058 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_preprocessing/test_match_columns.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.692991 feature_engine-1.6.1/tests/test_selection/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1669 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_base_selector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4739 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_check_estimator_selectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5848 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_drop_constant_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4019 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_drop_correlated_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3967 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_drop_duplicate_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3343 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_drop_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25531 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_drop_high_psi_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5105 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_information_value.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7039 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_probe_feature_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4594 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_recursive_feature_addition.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5260 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_recursive_feature_elimination.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4102 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_recursive_feature_selectors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4259 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_shuffle_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7218 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_single_feature_performance_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6844 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_smart_correlation_selection.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6043 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_selection/test_target_mean_selection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.692991 feature_engine-1.6.1/tests/test_time_series/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_time_series/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.696991 feature_engine-1.6.1/tests/test_time_series/test_forecasting/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_time_series/test_forecasting/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1684 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_time_series/test_forecasting/conftest.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2152 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_time_series/test_forecasting/test_check_estimator_forecasting.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11182 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_time_series/test_forecasting/test_expanding_window_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8001 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_time_series/test_forecasting/test_lag_features.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13658 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_time_series/test_forecasting/test_window_features.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.696991 feature_engine-1.6.1/tests/test_transformation/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_transformation/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2217 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_transformation/test_arcsin_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2320 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_transformation/test_boxcox_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1404 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_transformation/test_check_estimator_transformers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3987 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_transformation/test_log_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8588 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_transformation/test_logcp_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2634 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_transformation/test_power_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2324 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_transformation/test_reciprocal_transformer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2690 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_transformation/test_yeojohnson_transformer.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.696991 feature_engine-1.6.1/tests/test_variable_handling/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_variable_handling/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      828 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_variable_handling/test_init_parameter_checks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    13167 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_variable_handling/test_variable_type_selection.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:34:08.696991 feature_engine-1.6.1/tests/test_wrappers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_wrappers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1531 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_wrappers/test_check_estimator_wrappers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19763 2023-06-08 06:33:58.000000 feature_engine-1.6.1/tests/test_wrappers/test_sklearn_wrapper.py
```

### Comparing `feature_engine-1.6.0/LICENSE.md` & `feature_engine-1.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/PKG-INFO` & `feature_engine-1.6.1/feature_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: feature_engine
-Version: 1.6.0
+Name: feature-engine
+Version: 1.6.1
 Summary: Feature engineering package with Scikit-learn's fit transform functionality
 Home-page: http://github.com/feature-engine/feature_engine
 Author: Soledad Galli
 Author-email: solegalli@protonmail.com
 License: BSD 3 clause
 Description: # Feature Engine
```

### Comparing `feature_engine-1.6.0/README.md` & `feature_engine-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_base_transformers/base_numerical.py` & `feature_engine-1.6.1/feature_engine/_base_transformers/base_numerical.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.feature_names_in_ = X.columns.tolist()
 
         # save train set shape
         self.n_features_in_ = X.shape[1]
 
         return X
 
-    def transform(self, X: pd.DataFrame) -> pd.DataFrame:
+    def _check_transform_input_and_state(self, X: pd.DataFrame) -> pd.DataFrame:
         """
         Checks that the input is a dataframe and of the same size than the one used
         in the fit() method. Checks absence of NA and Inf.
 
         Parameters
         ----------
         X : Pandas DataFrame
```

### Comparing `feature_engine-1.6.0/feature_engine/_base_transformers/mixins.py` & `feature_engine-1.6.1/feature_engine/_base_transformers/mixins.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_check_input_parameters/check_input_dictionary.py` & `feature_engine-1.6.1/feature_engine/_check_input_parameters/check_input_dictionary.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_docstrings/fit_attributes.py` & `feature_engine-1.6.1/feature_engine/_docstrings/fit_attributes.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/all_trasnformers.py` & `feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/all_trasnformers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/discretisers.py` & `feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/discretisers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/encoders.py` & `feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/encoders.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/outliers.py` & `feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/outliers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_docstrings/init_parameters/selection.py` & `feature_engine-1.6.1/feature_engine/_docstrings/init_parameters/selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_docstrings/methods.py` & `feature_engine-1.6.1/feature_engine/_docstrings/methods.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_docstrings/substitute.py` & `feature_engine-1.6.1/feature_engine/_docstrings/substitute.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_prediction/base_predictor.py` & `feature_engine-1.6.1/feature_engine/_prediction/base_predictor.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_prediction/target_mean_classifier.py` & `feature_engine-1.6.1/feature_engine/_prediction/target_mean_classifier.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/_prediction/target_mean_regressor.py` & `feature_engine-1.6.1/feature_engine/_prediction/target_mean_regressor.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/creation/base_creation.py` & `feature_engine-1.6.1/feature_engine/creation/base_creation.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         self.feature_names_in_ = X.columns.tolist()
 
         # save train set shape
         self.n_features_in_ = X.shape[1]
 
         return self
 
-    def transform(self, X: pd.DataFrame) -> pd.DataFrame:
+    def _check_transform_input_and_state(self, X: pd.DataFrame) -> pd.DataFrame:
         """
         Common input and transformer checks.
 
         Parameters
         ----------
         X: pandas dataframe of shape = [n_samples, n_features]
             The data to transform.
```

### Comparing `feature_engine-1.6.0/feature_engine/creation/cyclical_features.py` & `feature_engine-1.6.1/feature_engine/creation/cyclical_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             The data to be transformed.
 
         Returns
         -------
         X_new: Pandas dataframe.
             The original dataframe plus the additional features.
         """
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         for variable in self.variables_:
             max_value = self.max_values_[variable]
             X[f"{variable}_sin"] = np.sin(X[variable] * (2.0 * np.pi / max_value))
             X[f"{variable}_cos"] = np.cos(X[variable] * (2.0 * np.pi / max_value))
 
         if self.drop_original:
```

### Comparing `feature_engine-1.6.0/feature_engine/creation/math_features.py` & `feature_engine-1.6.1/feature_engine/creation/math_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,15 +198,15 @@
             The data to transform.
 
         Returns
         -------
         X_new: Pandas dataframe, shape = [n_samples, n_features + n_operations]
             The input dataframe plus the new variables.
         """
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         new_variable_names = self._get_new_features_name()
 
         if len(new_variable_names) == 1:
             X[new_variable_names[0]] = X[self.variables].agg(self.func, axis=1)
         else:
             X[new_variable_names] = X[self.variables].agg(self.func, axis=1)
```

### Comparing `feature_engine-1.6.0/feature_engine/creation/relative_features.py` & `feature_engine-1.6.1/feature_engine/creation/relative_features.py`

 * *Files 19% similar despite different names*

```diff
@@ -73,14 +73,18 @@
         used as denominator for division and module, or exponent for the exponentiation.
 
     func: list
         The list of functions to be used in the transformation. The list can contain
         one or more of the following strings: 'add', 'mul','sub', 'div', truediv,
         'floordiv', 'mod', 'pow'.
 
+    fill_value: int, float, default=None
+        When dividing by zero, this value is used in place of infinity. If None,
+        then an error will be raised when dividing by zero.
+
     {missing_values}
 
     {drop_original}
 
     Attributes
     ----------
     {variables_}
@@ -124,14 +128,15 @@
     """
 
     def __init__(
         self,
         variables: List[Union[str, int]],
         reference: List[Union[str, int]],
         func: List[str],
+        fill_value: Union[int, float, None] = None,
         missing_values: str = "ignore",
         drop_original: bool = False,
     ) -> None:
 
         if (
             not isinstance(variables, list)
             or not all(isinstance(var, (int, str)) for var in variables)
@@ -159,18 +164,24 @@
         ):
             raise ValueError(
                 "At least one of the entered functions is not supported or you entered "
                 "duplicated functions. "
                 "Supported functions are {}. ".format(", ".join(_PERMITTED_FUNCTIONS))
             )
 
+        if fill_value is not None and not isinstance(fill_value, (float, int)):
+            raise ValueError(
+                "fill_value must be a float, integer or None. "
+                f"Got {fill_value} instead."
+            )
         super().__init__(missing_values, drop_original)
         self.variables = variables
         self.reference = reference
         self.func = func
+        self.fill_value = fill_value
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:
         """
         Add new features.
 
         Parameters
         ----------
@@ -179,15 +190,15 @@
 
         Returns
         -------
         X_new: Pandas dataframe
             The input dataframe plus the new variables.
         """
 
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         methods_dict = {
             "add": self._add,
             "mul": self._mul,
             "sub": self._sub,
             "div": self._div,
             "truediv": self._truediv,
@@ -209,77 +220,100 @@
 
     def _sub(self, X):
         for reference in self.reference:
             varname = [f"{var}_sub_{reference}" for var in self.variables]
             X[varname] = X[self.variables].sub(X[reference], axis=0)
         return X
 
-    def _div(self, X):
-        for reference in self.reference:
-            if (X[reference] == 0).any():
-                raise ValueError(
-                    "Some of the reference variables contain 0 as values. Check and "
-                    "remove those before using this transformer."
-                )
-            varname = [f"{var}_div_{reference}" for var in self.variables]
-            X[varname] = X[self.variables].div(X[reference], axis=0)
-        return X
-
     def _add(self, X):
         for reference in self.reference:
             varname = [f"{var}_add_{reference}" for var in self.variables]
             X[varname] = X[self.variables].add(X[reference], axis=0)
         return X
 
     def _mul(self, X):
         for reference in self.reference:
             varname = [f"{var}_mul_{reference}" for var in self.variables]
             X[varname] = X[self.variables].mul(X[reference], axis=0)
         return X
 
-    def _truediv(self, X):
+    def _div(self, X):
+        for reference in self.reference:
+            zeros_ix, contains_zero = self._find_zeroes_in_reference(X, reference)
 
+            if self.fill_value is None and contains_zero:
+                self._raise_error_when_zero_in_denominator()
+
+            varname = [f"{var}_div_{reference}" for var in self.variables]
+            X[varname] = X[self.variables].div(X[reference], axis=0)
+
+            if contains_zero:
+                X.loc[zeros_ix, varname] = self.fill_value
+        return X
+
+    def _truediv(self, X):
         for reference in self.reference:
-            if (X[reference] == 0).any():
-                raise ValueError(
-                    "Some of the reference variables contain 0 as values. Check and "
-                    "remove those before using this transformer."
-                )
+            zeros_ix, contains_zero = self._find_zeroes_in_reference(X, reference)
+
+            if self.fill_value is None and contains_zero:
+                self._raise_error_when_zero_in_denominator()
+
             varname = [f"{var}_truediv_{reference}" for var in self.variables]
             X[varname] = X[self.variables].truediv(X[reference], axis=0)
+
+            if contains_zero:
+                X.loc[zeros_ix, varname] = self.fill_value
         return X
 
     def _floordiv(self, X):
         for reference in self.reference:
-            if (X[reference] == 0).any():
-                raise ValueError(
-                    "Some of the reference variables contain 0 as values. Check and "
-                    "remove those before using this transformer."
-                )
+            zeros_ix, contains_zero = self._find_zeroes_in_reference(X, reference)
+
+            if self.fill_value is None and contains_zero:
+                self._raise_error_when_zero_in_denominator()
+
             varname = [f"{var}_floordiv_{reference}" for var in self.variables]
             X[varname] = X[self.variables].floordiv(X[reference], axis=0)
+
+            if contains_zero:
+                X.loc[zeros_ix, varname] = self.fill_value
         return X
 
     def _mod(self, X):
         for reference in self.reference:
-            if (X[reference] == 0).any():
-                raise ValueError(
-                    "Some of the reference variables contain 0 as values. Check and "
-                    "remove those before using this transformer."
-                )
+            zeros_ix, contains_zero = self._find_zeroes_in_reference(X, reference)
+
+            if self.fill_value is None and contains_zero:
+                self._raise_error_when_zero_in_denominator()
+
             varname = [f"{var}_mod_{reference}" for var in self.variables]
             X[varname] = X[self.variables].mod(X[reference], axis=0)
+
+            if contains_zero:
+                X.loc[zeros_ix, varname] = self.fill_value
         return X
 
     def _pow(self, X):
         for reference in self.reference:
             varname = [f"{var}_pow_{reference}" for var in self.variables]
             X[varname] = X[self.variables].pow(X[reference], axis=0)
         return X
 
+    def _raise_error_when_zero_in_denominator(self):
+        raise ValueError(
+            "Some of the reference variables contain zeroes. Division by zero "
+            "does not exist. Replace zeros before using this transformer for division "
+            "or set `fill_value` to a number."
+        )
+
+    def _find_zeroes_in_reference(self, X, var):
+        zero_ix = X[var] == 0
+        zero_bool = (zero_ix).any()
+        return zero_ix, zero_bool
+
     def _get_new_features_name(self) -> List:
         """Return names of the created features."""
 
         # Names of new features
         feature_names = [
             f"{var}_{fun}_{reference}"
             for fun in self.func
```

### Comparing `feature_engine-1.6.0/feature_engine/dataframe_checks.py` & `feature_engine-1.6.1/feature_engine/dataframe_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/datasets/titanic.py` & `feature_engine-1.6.1/feature_engine/datasets/titanic.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/datetime/_datetime_constants.py` & `feature_engine-1.6.1/feature_engine/datetime/_datetime_constants.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/datetime/datetime.py` & `feature_engine-1.6.1/feature_engine/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/datetime/datetime_subtraction.py` & `feature_engine-1.6.1/feature_engine/datetime/datetime_subtraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
         """make datetime subtraction"""
         new_df = pd.DataFrame()
         for reference in self.reference_:
             new_varnames = [f"{var}_sub_{reference}" for var in self.variables_]
             new_df[new_varnames] = (
                 dt_df[self.variables_]
                 .sub(dt_df[reference], axis=0)
-                .apply(lambda s: s / np.timedelta64(1, self.output_unit))
+                .div(np.timedelta64(1, self.output_unit).astype("timedelta64[ns]"))
             )
 
         if self.new_variables_names is not None:
             new_df.columns = self.new_variables_names
 
         return new_df
```

### Comparing `feature_engine-1.6.0/feature_engine/discretisation/__init__.py` & `feature_engine-1.6.1/feature_engine/discretisation/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/discretisation/arbitrary.py` & `feature_engine-1.6.1/feature_engine/discretisation/arbitrary.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/discretisation/base_discretiser.py` & `feature_engine-1.6.1/feature_engine/discretisation/base_discretiser.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         Returns
         -------
         X_new: pandas dataframe of shape = [n_samples, n_features]
             The transformed data with the discrete variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # transform variables
         if self.return_boundaries is True:
             for feature in self.variables_:
                 X[feature] = pd.cut(
                     X[feature],
                     self.binner_dict_[feature],
```

### Comparing `feature_engine-1.6.0/feature_engine/discretisation/decision_tree.py` & `feature_engine-1.6.1/feature_engine/discretisation/decision_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
         Returns
         -------
         X_new: pandas dataframe of shape = [n_samples, n_features]
             The dataframe with transformed variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         for feature in self.variables_:
             if self.regression:
                 X[feature] = self.binner_dict_[feature].predict(X[feature].to_frame())
             else:
                 tmp = self.binner_dict_[feature].predict_proba(X[feature].to_frame())
                 X[feature] = tmp[:, 1]
```

### Comparing `feature_engine-1.6.0/feature_engine/discretisation/equal_frequency.py` & `feature_engine-1.6.1/feature_engine/discretisation/equal_frequency.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/discretisation/equal_width.py` & `feature_engine-1.6.1/feature_engine/discretisation/equal_width.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/discretisation/geometric_width.py` & `feature_engine-1.6.1/feature_engine/discretisation/geometric_width.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/encoding/__init__.py` & `feature_engine-1.6.1/feature_engine/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/encoding/base_encoder.py` & `feature_engine-1.6.1/feature_engine/encoding/base_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/encoding/count_frequency.py` & `feature_engine-1.6.1/feature_engine/encoding/count_frequency.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/encoding/decision_tree.py` & `feature_engine-1.6.1/feature_engine/encoding/decision_tree.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/encoding/mean_encoding.py` & `feature_engine-1.6.1/feature_engine/encoding/mean_encoding.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/encoding/one_hot.py` & `feature_engine-1.6.1/feature_engine/encoding/one_hot.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/encoding/ordinal.py` & `feature_engine-1.6.1/feature_engine/encoding/ordinal.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/encoding/rare_label.py` & `feature_engine-1.6.1/feature_engine/encoding/rare_label.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,15 @@
                 # if the total number of categories is smaller than the indicated
                 # the encoder will consider all categories as frequent.
                 warnings.warn(
                     "The number of unique categories for variable {} is less than that "
                     "indicated in n_categories. Thus, all categories will be "
                     "considered frequent".format(var)
                 )
-                self.encoder_dict_[var] = X[var].unique()
+                self.encoder_dict_[var] = list(X[var].unique())
 
         self.variables_ = variables_
         self._get_feature_names_in(X)
         return self
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:
         """
@@ -243,27 +243,27 @@
         X = self._check_transform_input_and_state(X)
 
         # check if dataset contains na
         if self.missing_values == "raise":
             _check_optional_contains_na(X, self.variables_)
 
             for feature in self.variables_:
-                X[feature] = np.where(
-                    X[feature].isin(self.encoder_dict_[feature]),
-                    X[feature],
-                    self.replace_with,
-                )
+                if X[feature].dtype == "category":
+                    X[feature] = X[feature].cat.add_categories(self.replace_with)
+                X.loc[
+                    ~X[feature].isin(self.encoder_dict_[feature]), feature
+                ] = self.replace_with
 
         else:
             for feature in self.variables_:
-                X[feature] = np.where(
-                    X[feature].isin(self.encoder_dict_[feature] + [np.nan]),
-                    X[feature],
-                    self.replace_with,
-                )
+                if X[feature].dtype == "category":
+                    X[feature] = X[feature].cat.add_categories(self.replace_with)
+                X.loc[
+                    ~X[feature].isin(self.encoder_dict_[feature] + [np.nan]), feature
+                ] = self.replace_with
 
         return X
 
     def inverse_transform(self, X: pd.DataFrame):
         """inverse_transform is not implemented for this transformer."""
         raise NotImplementedError(
             "inverse_transform is not implemented for this transformer."
```

### Comparing `feature_engine-1.6.0/feature_engine/encoding/similarity_encoder.py` & `feature_engine-1.6.1/feature_engine/encoding/similarity_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/encoding/woe.py` & `feature_engine-1.6.1/feature_engine/preprocessing/match_columns.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,249 +1,261 @@
-# Authors: Soledad Galli <solegalli@protonmail.com>
-# License: BSD 3 clause
-
 from typing import List, Union
 
 import numpy as np
 import pandas as pd
+from sklearn.base import BaseEstimator, TransformerMixin
+from sklearn.utils.validation import check_is_fitted
 
-from feature_engine._docstrings.fit_attributes import (
-    _feature_names_in_docstring,
-    _n_features_in_docstring,
-    _variables_attribute_docstring,
-)
-from feature_engine._docstrings.init_parameters.all_trasnformers import (
-    _variables_categorical_docstring,
-)
-from feature_engine._docstrings.init_parameters.encoders import (
-    _ignore_format_docstring,
-    _unseen_docstring,
-)
-from feature_engine._docstrings.methods import (
-    _fit_transform_docstring,
-    _inverse_transform_docstring,
-    _transform_encoders_docstring,
-)
-from feature_engine._docstrings.substitute import Substitution
-from feature_engine.dataframe_checks import _check_contains_na, check_X_y
-from feature_engine.encoding._helper_functions import check_parameter_unseen
-from feature_engine.encoding.base_encoder import (
-    CategoricalInitMixin,
-    CategoricalMethodsMixin,
-)
+from feature_engine._base_transformers.mixins import GetFeatureNamesOutMixin
+from feature_engine.dataframe_checks import _check_contains_na, check_X
 from feature_engine.tags import _return_tags
 
 
-class WoE:
-    def _check_fit_input(self, X: pd.DataFrame, y: pd.Series):
-        """
-        Check that X is dataframe, and y a binary series with values 0 and 1.
-        """
-        X, y = check_X_y(X, y)
-
-        # check that y is binary
-        if y.nunique() != 2:
-            raise ValueError(
-                "This encoder is designed for binary classification. The target "
-                "used has more than 2 unique values."
-            )
+class MatchVariables(BaseEstimator, TransformerMixin, GetFeatureNamesOutMixin):
+    """
+    MatchVariables() ensures that the same variables observed in the train set
+    are present in the test set. If the dataset to transform contains variables that
+    were not present in the train set, they are dropped. If the dataset to transform
+    lacks variables that were present in the train set, these variables are added to
+    the dataframe with a value determined by the user (np.nan by default).
 
-        # if target does not have values 0 and 1, we need to remap, to be able to
-        # compute the averages.
-        if y.min() != 0 or y.max() != 1:
-            y = pd.Series(np.where(y == y.min(), 0, 1))
-        return X, y
-
-    def _calculate_woe(self, X: pd.DataFrame, y: pd.Series, variable: Union[str, int]):
-        total_pos = y.sum()
-        inverse_y = y.ne(1).copy()
-        total_neg = inverse_y.sum()
+    .. code-block:: python
 
-        pos = y.groupby(X[variable]).sum() / total_pos
-        neg = inverse_y.groupby(X[variable]).sum() / total_neg
+        train = pd.DataFrame({
+            "Name": ["tom", "nick", "krish", "jack"],
+            "City": ["London", "Manchester", "Liverpool", "Bristol"],
+            "Age": [20, 21, 19, 18],
+            "Marks": [0.9, 0.8, 0.7, 0.6],
+        })
 
-        if not (pos[:] == 0).sum() == 0 or not (neg[:] == 0).sum() == 0:
-            raise ValueError(
-                "The proportion of one of the classes for a category in "
-                "variable {} is zero, and log of zero is not defined".format(variable)
-            )
+        test = pd.DataFrame({
+            "Name": ["tom", "sam", "nick"],
+            "Age": [20, 22, 23],
+            "Marks": [0.9, 0.7, 0.6],
+            "Hobbies": ["tennis", "rugby", "football"]
+        })
 
-        woe = np.log(pos / neg)
-        return pos, neg, woe
+        match_columns = MatchVariables()
 
+        match_columns.fit(train)
 
-@Substitution(
-    ignore_format=_ignore_format_docstring,
-    variables=_variables_categorical_docstring,
-    unseen=_unseen_docstring,
-    variables_=_variables_attribute_docstring,
-    feature_names_in_=_feature_names_in_docstring,
-    n_features_in_=_n_features_in_docstring,
-    fit_transform=_fit_transform_docstring,
-    transform=_transform_encoders_docstring,
-    inverse_transform=_inverse_transform_docstring,
-)
-class WoEEncoder(CategoricalInitMixin, CategoricalMethodsMixin, WoE):
-    """
-    The WoEEncoder() replaces categories by the weight of evidence
-    (WoE). The WoE was used primarily in the financial sector to create credit risk
-    scorecards.
+        df_transformed = match_columns.transform(test)
 
-    The encoder will encode only categorical variables by default
-    (type 'object' or 'categorical'). You can pass a list of variables to encode.
-    Alternatively, the encoder will find and encode all categorical variables
-    (type 'object' or 'categorical').
+    Note that in the returned dataframe, the variable "Hobbies" was removed and the
+    variable "City" was added with np.nan:
 
-    With `ignore_format=True` you have the option to encode numerical variables as well.
-    The procedure is identical, you can either enter the list of variables to encode, or
-    the transformer will automatically select all variables.
+    .. code-block:: python
 
-    The encoder first maps the categories to the weight of evidence for each variable
-    (fit). The encoder then transforms the categories into the mapped numbers
-    (transform).
+        df_transformed
 
-    This categorical encoding is exclusive for binary classification.
+            Name    City  Age  Marks
+        0    tom  np.nan   20    0.9
+        1    sam  np.nan   22    0.7
+        2   nick  np.nan   23    0.6
 
-    **Note**
 
-    The log(0) is not defined and the division by 0 is not defined. Thus, if any of the
-    terms in the WoE equation are 0 for a given category, the encoder will return an
-    error. If this happens, try grouping less frequent categories.
+    The order of the variables in the transformed dataset is also adjusted to match
+    that observed in the train set.
 
-    More details in the :ref:`User Guide <woe_encoder>`.
+    More details in the :ref:`User Guide <match_variables>`.
 
     Parameters
     ----------
-    {variables}
+    fill_value: integer, float or string. Default=np.nan
+        The values for the variables that will be added to the transformed dataset.
 
-    {ignore_format}
-
-    {unseen}
+    missing_values: string, default='ignore'
+        Indicates if missing values should be ignored or raised. If 'raise' the
+        transformer will return an error if the the datasets to `fit` or `transform`
+        contain missing values. If 'ignore', missing data will be ignored when learning
+        parameters or performing the transformation.
+
+    verbose: bool, default=True
+        If True, the transformer will print out the names of the variables that are
+        added and / or removed from the dataset.
 
     Attributes
     ----------
-    encoder_dict_:
-        Dictionary with the WoE per variable.
-
-    {variables_}
-
-    {feature_names_in_}
+    feature_names_in_:
+        The variables present in the train set, in the order observed during fit.
 
-    {n_features_in_}
+    n_features_in_:
+        The number of features in the train set used in fit.
 
     Methods
     -------
     fit:
-        Learn the WoE per category, per variable.
-
-    {transform}
-
-    {fit_transform}
+        Identify the variable names in the train set.
 
-    {inverse_transform}
+    fit_transform:
+        Fit to the data. Then transform it.
 
-    Notes
-    -----
-    For details on the calculation of the weight of evidence visit:
-    https://www.listendata.com/2015/03/weight-of-evidence-woe-and-information.html
+    get_feature_names_out:
+        Get output feature names for transformation.
 
-    NAN are introduced when encoding categories that were not present in the training
-    dataset. If this happens, try grouping infrequent categories using the
-    RareLabelEncoder().
+    get_params:
+        Get parameters for this estimator.
 
-    There is a similar implementation in the the open-source package
-    `Category encoders <https://contrib.scikit-learn.org/category_encoders/>`_
+    set_params:
+        Set the parameters of this estimator.
 
-    See Also
-    --------
-    feature_engine.encoding.RareLabelEncoder
-    feature_engine.discretisation
-    category_encoders.woe.WOEEncoder
+    transform:
+        Add or delete variables to match those observed in the train set.
 
     Examples
     --------
 
     >>> import pandas as pd
-    >>> from feature_engine.encoding import WoEEncoder
-    >>> X = pd.DataFrame(dict(x1 = [1,2,3,4,5], x2 = ["b", "b", "b", "a", "a"]))
-    >>> y = pd.Series([0,1,1,1,0])
-    >>> woe = WoEEncoder()
-    >>> woe.fit(X, y)
-    >>> woe.transform(X)
-       x1        x2
-    0   1  0.287682
-    1   2  0.287682
-    2   3  0.287682
-    3   4 -0.405465
-    4   5 -0.405465
+    >>> from feature_engine.preprocessing import MatchVariables
+    >>> X_train = pd.DataFrame(dict(x1 = ["a","b","c"], x2 = [4,5,6]))
+    >>> X_test = pd.DataFrame(dict(x1 = ["c","b","a","d"],
+    >>>                             x2 = [5,6,4,7],
+    >>>                             x3 = [1,1,1,1]))
+    >>> mv = MatchVariables(missing_values="ignore")
+    >>> mv.fit(X_train)
+    >>> mv.transform(X_train)
+    x1  x2
+    0  a   4
+    1  b   5
+    2  c   6
+    >>> mv.transform(X_test)
+    The following variables are dropped from the DataFrame: ['x3']
+      x1  x2
+    0  c   5
+    1  b   6
+    2  a   4
+    3  d   7
+
+    >>> import pandas as pd
+    >>> from feature_engine.preprocessing import MatchVariables
+    >>> X_train = pd.DataFrame(dict(x1 = ["a","b","c"],
+    >>>                             x2 = [4,5,6], x3 = [1,1,1]))
+    >>> X_test = pd.DataFrame(dict(x1 = ["c","b","a","d"], x2 = [5,6,4,7]))
+    >>> mv = MatchVariables(missing_values="ignore")
+    >>> mv.fit(X_train)
+    >>> mv.transform(X_train)
+      x1  x2  x3
+    0  a   4   1
+    1  b   5   1
+    2  c   6   1
+    >>> mv.transform(X_test)
+    The following variables are added to the DataFrame: ['x3']
+      x1  x2  x3
+    0  c   5 NaN
+    1  b   6 NaN
+    2  a   4 NaN
+    3  d   7 NaN
     """
 
     def __init__(
         self,
-        variables: Union[None, int, str, List[Union[str, int]]] = None,
-        ignore_format: bool = False,
-        unseen: str = "ignore",
-    ) -> None:
-
-        super().__init__(variables, ignore_format)
-        check_parameter_unseen(unseen, ["ignore", "raise"])
-        self.unseen = unseen
+        fill_value: Union[str, int, float] = np.nan,
+        missing_values: str = "raise",
+        verbose: bool = True,
+    ):
 
-    def fit(self, X: pd.DataFrame, y: pd.Series):
-        """
-        Learn the WoE.
+        if missing_values not in ["raise", "ignore"]:
+            raise ValueError(
+                "missing_values takes only values 'raise' or 'ignore'."
+                f"Got '{missing_values} instead."
+            )
+
+        if not isinstance(verbose, bool):
+            raise ValueError(
+                "verbose takes only booleans True and False." f"Got '{verbose} instead."
+            )
+
+        # note: np.nan is an instance of float!!!
+        if not isinstance(fill_value, (str, int, float)):
+            raise ValueError(
+                "fill_value takes integers, floats or strings."
+                f"Got '{fill_value} instead."
+            )
+
+        self.fill_value = fill_value
+        self.missing_values = missing_values
+        self.verbose = verbose
+
+    def fit(self, X: pd.DataFrame, y: pd.Series = None):
+        """Learns and stores the names of the variables in the training dataset.
 
         Parameters
         ----------
+
         X: pandas dataframe of shape = [n_samples, n_features]
-            The training input samples.
-            Can be the entire dataframe, not just the categorical variables.
+            The input dataframe.
 
-        y: pandas series.
-            Target, must be binary.
+        y: None
+            y is not needed for this transformer. You can pass y or None.
         """
-        X, y = self._check_fit_input(X, y)
-        variables_ = self._check_or_select_variables(X)
-        _check_contains_na(X, variables_)
+        X = check_X(X)
 
-        self.encoder_dict_ = {}
+        if self.missing_values == "raise":
+            # check if dataset contains na
+            _check_contains_na(X, X.columns)
 
-        for var in variables_:
-            _, _, woe = self._calculate_woe(X, y, var)
+        # save input features
+        self.feature_names_in_: List[Union[str, int]] = X.columns.tolist()
 
-            self.encoder_dict_[var] = woe.to_dict()
+        self.n_features_in_ = X.shape[1]
 
-        self.variables_ = variables_
-        self._get_feature_names_in(X)
         return self
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:
-        """Replace categories with the learned parameters.
+        """
+        Drops variables that were not seen in the train set and adds variables that
+        were in the train set but not in the data to transform. In other words, it
+        returns a dataframe with matching columns.
 
         Parameters
         ----------
-        X: pandas dataframe of shape = [n_samples, n_features].
-            The dataset to transform.
+        X: pandas dataframe of shape = [n_samples, n_features]
+            The data to transform.
 
         Returns
         -------
-        X_new: pandas dataframe of shape = [n_samples, n_features].
-            The dataframe containing the categories replaced by numbers.
+        X_new: Pandas dataframe, shape = [n_samples, n_features]
+             The dataframe with variables that match those observed in the train set.
         """
+        check_is_fitted(self)
+
+        X = check_X(X)
+
+        if self.missing_values == "raise":
+            # check if dataset contains na
+            _check_contains_na(X, self.feature_names_in_)
+
+        _columns_to_drop = list(set(X.columns) - set(self.feature_names_in_))
+        _columns_to_add = list(set(self.feature_names_in_) - set(X.columns))
+
+        if self.verbose:
+            if len(_columns_to_add) > 0:
+                print(
+                    "The following variables are added to the DataFrame: "
+                    f"{_columns_to_add}"
+                )
+            if len(_columns_to_drop) > 0:
+                print(
+                    "The following variables are dropped from the DataFrame: "
+                    f"{_columns_to_drop}"
+                )
+
+        X = X.drop(_columns_to_drop, axis=1)
+
+        X = X.reindex(columns=self.feature_names_in_, fill_value=self.fill_value)
 
-        X = self._check_transform_input_and_state(X)
-        _check_contains_na(X, self.variables_)
-        X = self._encode(X)
         return X
 
+    # for the check_estimator tests
     def _more_tags(self):
         tags_dict = _return_tags()
-        tags_dict["variables"] = "categorical"
-        tags_dict["requires_y"] = True
-        # in the current format, the tests are performed using continuous np.arrays
-        # this means that when we encode some of the values, the denominator is 0
-        # and this the transformer raises an error, and the test fails.
-        # For this reason, most sklearn transformers will fail. And it has nothing to
-        # do with the class not being compatible, it is just that the inputs passed
-        # are not suitable
-        tags_dict["_skip_test"] = True
+
+        msg = "input shape of dataframes in fit and transform can differ"
+        tags_dict["_xfail_checks"]["check_transformer_general"] = msg
+
+        msg = (
+            "transformer takes categorical variables, and inf cannot be determined"
+            "on these variables. Thus, check is not implemented"
+        )
+        tags_dict["_xfail_checks"]["check_estimators_nan_inf"] = msg
+
         return tags_dict
```

### Comparing `feature_engine-1.6.0/feature_engine/imputation/__init__.py` & `feature_engine-1.6.1/feature_engine/imputation/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/imputation/arbitrary_number.py` & `feature_engine-1.6.1/feature_engine/imputation/arbitrary_number.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/imputation/base_imputer.py` & `feature_engine-1.6.1/feature_engine/imputation/base_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/imputation/categorical.py` & `feature_engine-1.6.1/feature_engine/imputation/categorical.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/imputation/drop_missing_data.py` & `feature_engine-1.6.1/feature_engine/imputation/drop_missing_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 
         X = self._transform(X)
 
         if self.threshold:
             idx = pd.isnull(X[self.variables_]).mean(axis=1) >= self.threshold
             idx = idx[idx]
         else:
-            idx = pd.isnull(X[self.variables_]).any(1)
+            idx = pd.isnull(X[self.variables_]).any(axis=1)
             idx = idx[idx]
 
         return X.loc[idx.index, :]
 
     def _more_tags(self):
         tags_dict = _return_tags()
         tags_dict["allow_nan"] = True
```

### Comparing `feature_engine-1.6.0/feature_engine/imputation/end_tail.py` & `feature_engine-1.6.1/feature_engine/imputation/end_tail.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/imputation/mean_median.py` & `feature_engine-1.6.1/feature_engine/imputation/mean_median.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/imputation/missing_indicator.py` & `feature_engine-1.6.1/feature_engine/imputation/missing_indicator.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/imputation/random_sample.py` & `feature_engine-1.6.1/feature_engine/imputation/random_sample.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/outliers/artbitrary.py` & `feature_engine-1.6.1/feature_engine/outliers/artbitrary.py`

 * *Files 9% similar despite different names*

```diff
@@ -179,14 +179,30 @@
             self.left_tail_caps_ = {}
 
         self.feature_names_in_ = X.columns.to_list()
         self.n_features_in_ = X.shape[1]
 
         return self
 
+    def transform(self, X: pd.DataFrame) -> pd.DataFrame:
+        """
+        Cap the variable values.
+
+        Parameters
+        ----------
+        X: pandas dataframe of shape = [n_samples, n_features]
+            The data to be transformed.
+
+        Returns
+        -------
+        X_new: pandas dataframe of shape = [n_samples, n_features]
+            The dataframe with the capped variables.
+        """
+        return super()._transform(X)
+
     def _more_tags(self):
         tags_dict = _return_tags()
         # add additional test that fails
         tags_dict["_xfail_checks"][
             "check_parameters_default_constructible"
         ] = "transformer has 1 mandatory parameter"
         return tags_dict
```

### Comparing `feature_engine-1.6.0/feature_engine/outliers/base_outlier.py` & `feature_engine-1.6.1/feature_engine/outliers/base_outlier.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             _check_contains_inf(X, self.variables_)
 
         # reorder to match training set
         X = X[self.feature_names_in_]
 
         return X
 
-    def transform(self, X: pd.DataFrame) -> pd.DataFrame:
+    def _transform(self, X: pd.DataFrame) -> pd.DataFrame:
         """
         Cap the variable values.
 
         Parameters
         ----------
         X: pandas dataframe of shape = [n_samples, n_features]
             The data to be transformed.
```

### Comparing `feature_engine-1.6.0/feature_engine/outliers/trimmer.py` & `feature_engine-1.6.1/feature_engine/outliers/trimmer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/outliers/winsorizer.py` & `feature_engine-1.6.1/feature_engine/outliers/winsorizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,19 +173,19 @@
             The dataframe with the capped variables and indicators.
             The number of output variables depends on the values for 'tail' and
             'add_indicators': if passing 'add_indicators=False', will be equal
             to 'n_features', otherwise, will have an additional indicator column
             per processed feature for each tail.
         """
         if not self.add_indicators:
-            X_out = super().transform(X)
+            X_out = super()._transform(X)
 
         else:
             X_orig = check_X(X)
-            X_out = super().transform(X_orig)
+            X_out = super()._transform(X_orig)
             X_orig = X_orig[self.variables_]
             X_out_filtered = X_out[self.variables_]
 
             if self.tail in ["left", "both"]:
                 X_left = X_out_filtered > X_orig
                 X_left.columns = [str(cl) + "_left" for cl in self.variables_]
             if self.tail in ["right", "both"]:
```

### Comparing `feature_engine-1.6.0/feature_engine/preprocessing/match_categories.py` & `feature_engine-1.6.1/feature_engine/preprocessing/match_categories.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/preprocessing/match_columns.py` & `feature_engine-1.6.1/feature_engine/encoding/woe.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,261 +1,291 @@
+# Authors: Soledad Galli <solegalli@protonmail.com>
+# License: BSD 3 clause
+
 from typing import List, Union
 
 import numpy as np
 import pandas as pd
-from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn.utils.validation import check_is_fitted
 
-from feature_engine._base_transformers.mixins import GetFeatureNamesOutMixin
-from feature_engine.dataframe_checks import _check_contains_na, check_X
+from feature_engine._docstrings.fit_attributes import (
+    _feature_names_in_docstring,
+    _n_features_in_docstring,
+    _variables_attribute_docstring,
+)
+from feature_engine._docstrings.init_parameters.all_trasnformers import (
+    _variables_categorical_docstring,
+)
+from feature_engine._docstrings.init_parameters.encoders import (
+    _ignore_format_docstring,
+    _unseen_docstring,
+)
+from feature_engine._docstrings.methods import (
+    _fit_transform_docstring,
+    _inverse_transform_docstring,
+    _transform_encoders_docstring,
+)
+from feature_engine._docstrings.substitute import Substitution
+from feature_engine.dataframe_checks import _check_contains_na, check_X_y
+from feature_engine.encoding._helper_functions import check_parameter_unseen
+from feature_engine.encoding.base_encoder import (
+    CategoricalInitMixin,
+    CategoricalMethodsMixin,
+)
 from feature_engine.tags import _return_tags
 
 
-class MatchVariables(BaseEstimator, TransformerMixin, GetFeatureNamesOutMixin):
-    """
-    MatchVariables() ensures that the same variables observed in the train set
-    are present in the test set. If the dataset to transform contains variables that
-    were not present in the train set, they are dropped. If the dataset to transform
-    lacks variables that were present in the train set, these variables are added to
-    the dataframe with a value determined by the user (np.nan by default).
-
-    .. code-block:: python
-
-        train = pd.DataFrame({
-            "Name": ["tom", "nick", "krish", "jack"],
-            "City": ["London", "Manchester", "Liverpool", "Bristol"],
-            "Age": [20, 21, 19, 18],
-            "Marks": [0.9, 0.8, 0.7, 0.6],
-        })
-
-        test = pd.DataFrame({
-            "Name": ["tom", "sam", "nick"],
-            "Age": [20, 22, 23],
-            "Marks": [0.9, 0.7, 0.6],
-            "Hobbies": ["tennis", "rugby", "football"]
-        })
+class WoE:
+    def _check_fit_input(self, X: pd.DataFrame, y: pd.Series):
+        """
+        Check that X is dataframe, and y a binary series with values 0 and 1.
+        """
+        X, y = check_X_y(X, y)
 
-        match_columns = MatchVariables()
+        # check that y is binary
+        if y.nunique() != 2:
+            raise ValueError(
+                "This encoder is designed for binary classification. The target "
+                "used has more than 2 unique values."
+            )
 
-        match_columns.fit(train)
+        # if target does not have values 0 and 1, we need to remap, to be able to
+        # compute the averages.
+        if y.min() != 0 or y.max() != 1:
+            y = pd.Series(np.where(y == y.min(), 0, 1))
+        return X, y
 
-        df_transformed = match_columns.transform(test)
+    def _calculate_woe(
+        self,
+        X: pd.DataFrame,
+        y: pd.Series,
+        variable: Union[str, int],
+        fill_value: Union[float, None] = None,
+    ):
+        total_pos = y.sum()
+        inverse_y = y.ne(1).copy()
+        total_neg = inverse_y.sum()
+
+        pos = y.groupby(X[variable]).sum() / total_pos
+        neg = inverse_y.groupby(X[variable]).sum() / total_neg
+
+        if not (pos[:] == 0).sum() == 0 or not (neg[:] == 0).sum() == 0:
+            if fill_value is None:
+                raise ValueError(
+                    "The proportion of one of the classes for a category in "
+                    "variable {} is zero, and log of zero is not defined".format(
+                        variable
+                    )
+                )
+            else:
+                pos[pos[:] == 0] = fill_value
+                neg[neg[:] == 0] = fill_value
+
+        woe = np.log(pos / neg)
+        return pos, neg, woe
+
+
+@Substitution(
+    ignore_format=_ignore_format_docstring,
+    variables=_variables_categorical_docstring,
+    unseen=_unseen_docstring,
+    variables_=_variables_attribute_docstring,
+    feature_names_in_=_feature_names_in_docstring,
+    n_features_in_=_n_features_in_docstring,
+    fit_transform=_fit_transform_docstring,
+    transform=_transform_encoders_docstring,
+    inverse_transform=_inverse_transform_docstring,
+)
+class WoEEncoder(CategoricalInitMixin, CategoricalMethodsMixin, WoE):
+    """
+    The WoEEncoder() replaces categories by the weight of evidence
+    (WoE). The WoE was used primarily in the financial sector to create credit risk
+    scorecards.
 
-    Note that in the returned dataframe, the variable "Hobbies" was removed and the
-    variable "City" was added with np.nan:
+    The encoder will encode only categorical variables by default
+    (type 'object' or 'categorical'). You can pass a list of variables to encode.
+    Alternatively, the encoder will find and encode all categorical variables
+    (type 'object' or 'categorical').
 
-    .. code-block:: python
+    With `ignore_format=True` you have the option to encode numerical variables as well.
+    The procedure is identical, you can either enter the list of variables to encode, or
+    the transformer will automatically select all variables.
 
-        df_transformed
+    The encoder first maps the categories to the weight of evidence for each variable
+    (fit). The encoder then transforms the categories into the mapped numbers
+    (transform).
 
-            Name    City  Age  Marks
-        0    tom  np.nan   20    0.9
-        1    sam  np.nan   22    0.7
-        2   nick  np.nan   23    0.6
+    This categorical encoding is exclusive for binary classification.
 
+    **Note**
 
-    The order of the variables in the transformed dataset is also adjusted to match
-    that observed in the train set.
+    The log(0) is not defined and the division by 0 is not defined. Thus, if any of the
+    terms in the WoE equation are 0 for a given category, the encoder will return an
+    error. If this happens, try grouping less frequent categories. Alternatively,
+    you can now add a fill_value (see parameter below).
 
-    More details in the :ref:`User Guide <match_variables>`.
+    More details in the :ref:`User Guide <woe_encoder>`.
 
     Parameters
     ----------
-    fill_value: integer, float or string. Default=np.nan
-        The values for the variables that will be added to the transformed dataset.
+    {variables}
 
-    missing_values: string, default='ignore'
-        Indicates if missing values should be ignored or raised. If 'raise' the
-        transformer will return an error if the the datasets to `fit` or `transform`
-        contain missing values. If 'ignore', missing data will be ignored when learning
-        parameters or performing the transformation.
-
-    verbose: bool, default=True
-        If True, the transformer will print out the names of the variables that are
-        added and / or removed from the dataset.
+    {ignore_format}
+
+    {unseen}
+
+    fill_value: int, float, default=None
+        When the numerator or denominator of the WoE calculation are zero, the WoE
+        calculation is not possible. If `fill_value` is None (recommended), an error
+        will be raised in those cases. Alternatively, fill_value will be used in place
+        of denominators or numerators that equal zero.
 
     Attributes
     ----------
-    feature_names_in_:
-        The variables present in the train set, in the order observed during fit.
+    encoder_dict_:
+        Dictionary with the WoE per variable.
+
+    {variables_}
 
-    n_features_in_:
-        The number of features in the train set used in fit.
+    {feature_names_in_}
+
+    {n_features_in_}
 
     Methods
     -------
     fit:
-        Identify the variable names in the train set.
+        Learn the WoE per category, per variable.
 
-    fit_transform:
-        Fit to the data. Then transform it.
+    {transform}
 
-    get_feature_names_out:
-        Get output feature names for transformation.
+    {fit_transform}
 
-    get_params:
-        Get parameters for this estimator.
+    {inverse_transform}
 
-    set_params:
-        Set the parameters of this estimator.
+    Notes
+    -----
+    For details on the calculation of the weight of evidence visit:
+    https://www.listendata.com/2015/03/weight-of-evidence-woe-and-information.html
 
-    transform:
-        Add or delete variables to match those observed in the train set.
+    NAN are introduced when encoding categories that were not present in the training
+    dataset. If this happens, try grouping infrequent categories using the
+    RareLabelEncoder().
 
-    Examples
+    There is a similar implementation in the the open-source package
+    `Category encoders <https://contrib.scikit-learn.org/category_encoders/>`_
+
+    See Also
     --------
+    feature_engine.encoding.RareLabelEncoder
+    feature_engine.discretisation
+    category_encoders.woe.WOEEncoder
 
-    >>> import pandas as pd
-    >>> from feature_engine.preprocessing import MatchVariables
-    >>> X_train = pd.DataFrame(dict(x1 = ["a","b","c"], x2 = [4,5,6]))
-    >>> X_test = pd.DataFrame(dict(x1 = ["c","b","a","d"],
-    >>>                             x2 = [5,6,4,7],
-    >>>                             x3 = [1,1,1,1]))
-    >>> mv = MatchVariables(missing_values="ignore")
-    >>> mv.fit(X_train)
-    >>> mv.transform(X_train)
-    x1  x2
-    0  a   4
-    1  b   5
-    2  c   6
-    >>> mv.transform(X_test)
-    The following variables are dropped from the DataFrame: ['x3']
-      x1  x2
-    0  c   5
-    1  b   6
-    2  a   4
-    3  d   7
+    Examples
+    --------
 
     >>> import pandas as pd
-    >>> from feature_engine.preprocessing import MatchVariables
-    >>> X_train = pd.DataFrame(dict(x1 = ["a","b","c"],
-    >>>                             x2 = [4,5,6], x3 = [1,1,1]))
-    >>> X_test = pd.DataFrame(dict(x1 = ["c","b","a","d"], x2 = [5,6,4,7]))
-    >>> mv = MatchVariables(missing_values="ignore")
-    >>> mv.fit(X_train)
-    >>> mv.transform(X_train)
-      x1  x2  x3
-    0  a   4   1
-    1  b   5   1
-    2  c   6   1
-    >>> mv.transform(X_test)
-    The following variables are added to the DataFrame: ['x3']
-      x1  x2  x3
-    0  c   5 NaN
-    1  b   6 NaN
-    2  a   4 NaN
-    3  d   7 NaN
+    >>> from feature_engine.encoding import WoEEncoder
+    >>> X = pd.DataFrame(dict(x1 = [1,2,3,4,5], x2 = ["b", "b", "b", "a", "a"]))
+    >>> y = pd.Series([0,1,1,1,0])
+    >>> woe = WoEEncoder()
+    >>> woe.fit(X, y)
+    >>> woe.transform(X)
+       x1        x2
+    0   1  0.287682
+    1   2  0.287682
+    2   3  0.287682
+    3   4 -0.405465
+    4   5 -0.405465
     """
 
     def __init__(
         self,
-        fill_value: Union[str, int, float] = np.nan,
-        missing_values: str = "raise",
-        verbose: bool = True,
-    ):
-
-        if missing_values not in ["raise", "ignore"]:
+        variables: Union[None, int, str, List[Union[str, int]]] = None,
+        ignore_format: bool = False,
+        unseen: str = "ignore",
+        fill_value: Union[int, float, None] = None,
+    ) -> None:
+
+        super().__init__(variables, ignore_format)
+        check_parameter_unseen(unseen, ["ignore", "raise"])
+        if fill_value is not None and not isinstance(fill_value, (int, float)):
             raise ValueError(
-                "missing_values takes only values 'raise' or 'ignore'."
-                f"Got '{missing_values} instead."
+                f"fill_value takes None, integer or float. Got {fill_value} instead."
             )
-
-        if not isinstance(verbose, bool):
-            raise ValueError(
-                "verbose takes only booleans True and False." f"Got '{verbose} instead."
-            )
-
-        # note: np.nan is an instance of float!!!
-        if not isinstance(fill_value, (str, int, float)):
-            raise ValueError(
-                "fill_value takes integers, floats or strings."
-                f"Got '{fill_value} instead."
-            )
-
+        self.unseen = unseen
         self.fill_value = fill_value
-        self.missing_values = missing_values
-        self.verbose = verbose
 
-    def fit(self, X: pd.DataFrame, y: pd.Series = None):
-        """Learns and stores the names of the variables in the training dataset.
+    def fit(self, X: pd.DataFrame, y: pd.Series):
+        """
+        Learn the WoE.
 
         Parameters
         ----------
-
         X: pandas dataframe of shape = [n_samples, n_features]
-            The input dataframe.
+            The training input samples.
+            Can be the entire dataframe, not just the categorical variables.
 
-        y: None
-            y is not needed for this transformer. You can pass y or None.
+        y: pandas series.
+            Target, must be binary.
         """
-        X = check_X(X)
-
-        if self.missing_values == "raise":
-            # check if dataset contains na
-            _check_contains_na(X, X.columns)
-
-        # save input features
-        self.feature_names_in_: List[Union[str, int]] = X.columns.tolist()
+        X, y = self._check_fit_input(X, y)
+        variables_ = self._check_or_select_variables(X)
+        _check_contains_na(X, variables_)
+
+        encoder_dict_ = {}
+        vars_that_fail = []
+
+        for var in variables_:
+            try:
+                _, _, woe = self._calculate_woe(X, y, var, self.fill_value)
+                encoder_dict_[var] = woe.to_dict()
+            except ValueError:
+                vars_that_fail.append(var)
+
+        if len(vars_that_fail) > 0:
+            vars_that_fail_str = (
+                ", ".join(vars_that_fail)
+                if len(vars_that_fail) > 1
+                else vars_that_fail[0]
+            )
 
-        self.n_features_in_ = X.shape[1]
+            raise ValueError(
+                "During the WoE calculation, some of the categories in the "
+                "following features contained 0 in the denominator or numerator, "
+                f"and hence the WoE can't be calculated: {vars_that_fail_str}."
+            )
 
+        self.encoder_dict_ = encoder_dict_
+        self.variables_ = variables_
+        self._get_feature_names_in(X)
         return self
 
     def transform(self, X: pd.DataFrame) -> pd.DataFrame:
-        """
-        Drops variables that were not seen in the train set and adds variables that
-        were in the train set but not in the data to transform. In other words, it
-        returns a dataframe with matching columns.
+        """Replace categories with the learned parameters.
 
         Parameters
         ----------
-        X: pandas dataframe of shape = [n_samples, n_features]
-            The data to transform.
+        X: pandas dataframe of shape = [n_samples, n_features].
+            The dataset to transform.
 
         Returns
         -------
-        X_new: Pandas dataframe, shape = [n_samples, n_features]
-             The dataframe with variables that match those observed in the train set.
+        X_new: pandas dataframe of shape = [n_samples, n_features].
+            The dataframe containing the categories replaced by numbers.
         """
-        check_is_fitted(self)
-
-        X = check_X(X)
-
-        if self.missing_values == "raise":
-            # check if dataset contains na
-            _check_contains_na(X, self.feature_names_in_)
-
-        _columns_to_drop = list(set(X.columns) - set(self.feature_names_in_))
-        _columns_to_add = list(set(self.feature_names_in_) - set(X.columns))
-
-        if self.verbose:
-            if len(_columns_to_add) > 0:
-                print(
-                    "The following variables are added to the DataFrame: "
-                    f"{_columns_to_add}"
-                )
-            if len(_columns_to_drop) > 0:
-                print(
-                    "The following variables are dropped from the DataFrame: "
-                    f"{_columns_to_drop}"
-                )
-
-        X = X.drop(_columns_to_drop, axis=1)
-
-        X = X.reindex(columns=self.feature_names_in_, fill_value=self.fill_value)
 
+        X = self._check_transform_input_and_state(X)
+        _check_contains_na(X, self.variables_)
+        X = self._encode(X)
         return X
 
-    # for the check_estimator tests
     def _more_tags(self):
         tags_dict = _return_tags()
-
-        msg = "input shape of dataframes in fit and transform can differ"
-        tags_dict["_xfail_checks"]["check_transformer_general"] = msg
-
-        msg = (
-            "transformer takes categorical variables, and inf cannot be determined"
-            "on these variables. Thus, check is not implemented"
-        )
-        tags_dict["_xfail_checks"]["check_estimators_nan_inf"] = msg
-
+        tags_dict["variables"] = "categorical"
+        tags_dict["requires_y"] = True
+        # in the current format, the tests are performed using continuous np.arrays
+        # this means that when we encode some of the values, the denominator is 0
+        # and this the transformer raises an error, and the test fails.
+        # For this reason, most sklearn transformers will fail. And it has nothing to
+        # do with the class not being compatible, it is just that the inputs passed
+        # are not suitable
+        tags_dict["_skip_test"] = True
         return tags_dict
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/__init__.py` & `feature_engine-1.6.1/feature_engine/selection/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/selection/_docstring.py` & `feature_engine-1.6.1/feature_engine/_docstrings/selection/_docstring.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/selection/_selection_constants.py` & `feature_engine-1.6.1/feature_engine/selection/_selection_constants.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/selection/base_recursive_selector.py` & `feature_engine-1.6.1/feature_engine/selection/base_recursive_selector.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/selection/base_selector.py` & `feature_engine-1.6.1/feature_engine/selection/base_selector.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/selection/drop_constant_features.py` & `feature_engine-1.6.1/feature_engine/selection/drop_constant_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 )
 from feature_engine._docstrings.init_parameters.selection import (
     _confirm_variables_docstring,
 )
 from feature_engine._docstrings.methods import _fit_transform_docstring
 from feature_engine._docstrings.substitute import Substitution
 from feature_engine.dataframe_checks import _check_contains_na, check_X
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _get_support_docstring,
     _variables_all_docstring,
     _variables_attribute_docstring,
 )
 from feature_engine.selection.base_selector import BaseSelector
 from feature_engine.tags import _return_tags
 from feature_engine.variable_handling._init_parameter_checks import (
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/drop_correlated_features.py` & `feature_engine-1.6.1/feature_engine/selection/drop_correlated_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from feature_engine._docstrings.methods import _fit_transform_docstring
 from feature_engine._docstrings.substitute import Substitution
 from feature_engine.dataframe_checks import (
     _check_contains_inf,
     _check_contains_na,
     check_X,
 )
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _get_support_docstring,
     _missing_values_docstring,
     _variables_attribute_docstring,
     _variables_numerical_docstring,
 )
 from feature_engine.selection.base_selector import BaseSelector
 from feature_engine.variable_handling._init_parameter_checks import (
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/drop_duplicate_features.py` & `feature_engine-1.6.1/feature_engine/selection/drop_duplicate_features.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 from feature_engine._docstrings.init_parameters.selection import (
     _confirm_variables_docstring,
 )
 from feature_engine._docstrings.methods import _fit_transform_docstring
 from feature_engine._docstrings.substitute import Substitution
 from feature_engine.dataframe_checks import _check_contains_na, check_X
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _get_support_docstring,
     _missing_values_docstring,
     _variables_all_docstring,
     _variables_attribute_docstring,
 )
 from feature_engine.selection.base_selector import BaseSelector
 from feature_engine.tags import _return_tags
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/drop_features.py` & `feature_engine-1.6.1/feature_engine/selection/drop_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/selection/drop_psi_features.py` & `feature_engine-1.6.1/feature_engine/selection/drop_psi_features.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,80 +20,112 @@
     _check_contains_na,
     check_X,
 )
 from feature_engine.discretisation import (
     EqualFrequencyDiscretiser,
     EqualWidthDiscretiser,
 )
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _get_support_docstring,
     _variables_attribute_docstring,
-    _variables_numerical_docstring,
 )
 from feature_engine.selection.base_selector import BaseSelector
+from feature_engine.tags import _return_tags
 from feature_engine.variable_handling._init_parameter_checks import (
     _check_init_parameter_variables,
 )
 from feature_engine.variable_handling.variable_type_selection import (
-    find_or_check_numerical_variables,
+    find_categorical_and_numerical_variables,
 )
 
 Variables = Union[None, int, str, List[Union[str, int]]]
 
+PSI = """PSI = sum ( (test_i - basis_i) x ln(test_i/basis_i) )""".rstrip()
+
 
 @Substitution(
     confirm_variables=_confirm_variables_docstring,
-    variables=_variables_numerical_docstring,
     variables_=_variables_attribute_docstring,
     feature_names_in_=_feature_names_in_docstring,
     n_features_in_=_n_features_in_docstring,
     fit_transform=_fit_transform_docstring,
     get_support=_get_support_docstring,
+    psi=PSI,
 )
 class DropHighPSIFeatures(BaseSelector):
     r"""
-    DropHighPSIFeatures drops features which Population Stability Index (PSI) value is
-    above a given threshold. The PSI of a numerical feature is an indication of the
-    shift in its distribution; a feature with high PSI could therefore be considered
+    DropHighPSIFeatures() drops features which Population Stability Index (PSI) is
+    above a given threshold.
+
+    The PSI is used to compare distributions. Higher PSI values mean greater changes in
+    a feature's distribution. Therefore, a feature with high PSI can be considered
     unstable.
 
-    A bigger PSI value indicates a bigger shift in the feature distribution.
+    To compute the PSI, DropHighPSIFeatures() splits the dataset in two: a basis and
+    a test set. Then, it compares the distribution of each feature between those sets.
+
+    To determine the PSI, continuous features are sorted into discrete intervals, and
+    then, the number of observations per interval are compared between the 2
+    distributions.
+
+    The PSI is calculated as:
+
+    {psi}
+
+    where `basis` and `test` are the 2 datasets, `i` refers to each interval, and then,
+    `test_i` and `basis_i` are the number of observations in interval i in each data
+    set.
+
+    The PSI has traditionally been used to assess changes in distributions of
+    continuous variables.
+
+    In version 1.7, we extended the functionality of DropHighPSIFeatures() to
+    calculate the PSI for categorical features as well. In this case, `i` is each
+    unique category, and `test_i` and `basis_i` are the number of observations in
+    category i.
+
+    **Threshold**
 
     Different thresholds can be used to assess the magnitude of the distribution shift
     according to the PSI value. The most commonly used thresholds are:
 
     - Below 10%, the variable has not experienced a significant shift.
     - Above 25%, the variable has experienced a major shift.
     - Between those two values, the shift is intermediate.
 
-    To compute the PSI the DropHighPSIFeatures splits the dataset in two:
+    **Data split**
 
-    First and foremost, the user should enter one variable which will be used to guide
-    the data split. This variable can be of any data type. If the user does not enter a
-    variable name, DropHighPSIFeatures will use the dataframe index.
+    To compute the PSI, DropHighPSIFeatures() splits the dataset in two: a basis and
+    a test set. Then, it compares the distribution of each feature between those sets.
 
-    Second, the user has the option to specify a proportion of observations to put in
-    each data set, or alternatively, provide a cut-off value.
+    There are various options to split a dataset:
 
-    If the user specifies a proportion through the `split_frac` parameter, the data will
+    First, you can indicate which variable should be used to guide the data split. This
+    variable can be of any data type. If you do not enter a variable name,
+    DropHighPSIFeatures() will use the dataframe index.
+
+    Next, you need to specify how that variable (or the index) should be used to split
+    the data. You can specify a proportion of observations to be put in each data set,
+    or alternatively, provide a cut-off value.
+
+    If you specify a proportion through the `split_frac` parameter, the data will
     be sorted to accommodate that proportion. If `split_frac` is 0.5, 50% of the
     observations will go to either basis or test sets. If `split_frac` is 0.6, 60% of
     the samples will go to the basis data set and the remaining 40% to the test set.
 
     If `split_distinct` is True, the data will be sorted considering unique values in
     the selected variables. Check the parameter below for more details.
 
-    If the user defines a numeric cut-off value or a specific date using the `cut_off`
+    If you define a numeric cut-off value or a specific date using the `cut_off`
     parameter, the observations with value <= cut-off will go to the basis data set and
-    the remaining ones to the test set. For categorical values this means they are
-    sorted alphabetically and cut accordingly.
+    the remaining ones to the test set. If the variable used to guide the split is
+    categorical, its values are sorted alphabetically and cut accordingly.
 
-    If the user passes a list of values in the `cut-off`, the observations with the
-    values in the list, will go to the basis set, and the remaining ones to the test
-    set.
+    If you pass a list of values in the `cut-off`, the observations with the values in
+    the list, will go to the basis set, and the remaining ones to the test set.
 
     More details in the :ref:`User Guide <psi_selection>`.
 
     Parameters
     ----------
     split_col: string or int, default=None.
         The variable that will be used to split the dataset into the basis and test
@@ -113,21 +145,22 @@
         on the `cut_off` value.
 
     split_distinct: boolean, default=False.
         If True, `split_frac` is applied to the vector of unique values in `split_col`
         instead of being applied to the whole vector of values. For example, if the
         values in `split_col` are [1, 1, 1, 1, 2, 2, 3, 4] and `split_frac` is
         0.5, we have the following:
-        - `split_distinct=False` splits the vector in two equally sized parts:
-        [1, 1, 1, 1] and [2, 2, 3, 4]. This involves that 2 dataframes with 4
-        observations each are used for the PSI calculations.
-        - `split_distinct=True` computes the vector of unique values in `split_col`
-        ([1, 2, 3, 4]) and splits that vector in two equal parts: [1, 2] and [3, 4].
-        The number of observations in the two dataframes used for the PSI calculations
-        is respectively 6 ([1, 1, 1, 1, 2, 2]) and 2 ([3, 4]).
+
+            - `split_distinct=False` splits the vector in two equally sized parts:
+                [1, 1, 1, 1] and [2, 2, 3, 4]. This involves that 2 dataframes with 4
+                observations each are used for the PSI calculations.
+            - `split_distinct=True` computes the vector of unique values in `split_col`
+                ([1, 2, 3, 4]) and splits that vector in two equal parts: [1, 2] and
+                [3, 4]. The number of observations in the two dataframes used for the
+                PSI calculations is respectively 6 ([1, 1, 1, 1, 2, 2]) and 2 ([3, 4]).
 
     cut_off: int, float, date or list, default=None
         Threshold to split the dataset based on the `split_col` variable. If int, float
         or date, observations where the `split_col` values are <= threshold will
         go to the basis data set and the rest to the test set. If `cut_off` is a list,
         the observations where the `split_col` values are within the list will go to the
         basis data set and the remaining observations to the test set. If `cut_off` is
@@ -139,16 +172,28 @@
         test) will be switched. This is important because the PSI is not symmetric,
         i.e., PSI(a, b) != PSI(b, a)).
 
     threshold: float, str, default = 0.25.
         The threshold to drop a feature. If the PSI for a feature is >= threshold, the
         feature will be dropped. The most common threshold values are 0.25 (large shift)
         and 0.10 (medium shift).
-        If 'auto', the threshold will be calculated based on the size of the base and
-        target dataset and the number of bins.
+        If 'auto', the threshold will be calculated based on the size of the basis and
+        test dataset and the number of bins as:
+
+                threshold = χ2(q, B−1) × (1/N + 1/M)
+
+        where:
+
+            - q = quantile of the distribution (or 1 - p-value),
+            - B = number of bins/categories,
+            - N = size of basis dataset,
+            - M = size of test dataset.
+
+        See formula (5.2) from reference [1].
+
 
     bins: int, default = 10
         Number of bins or intervals. For continuous features with good value spread, 10
         bins is commonly used. For features with lower cardinality or highly skewed
         distributions, lower values may be required.
 
     strategy: string, default='equal_frequency'
@@ -165,15 +210,25 @@
 
     missing_values: str, default='raise'
         Whether to perform the PSI feature selection on a dataframe with missing values.
         Takes values 'raise' or 'ignore'. If 'ignore', missing values will be dropped
         when determining the PSI for that particular feature. If 'raise' the transformer
         will raise an error and features will not be selected.
 
-    {variables}
+    p_value: float, default = 0.001
+        The p-value to test the null hypothesis that there is no feature drift. In that
+        case, the PSI-value approximates a random variable that follows a chi-square
+        distribution. See [1] for details. This parameter is used only if `threshold`
+        is set to 'auto'.
+
+    variables: int, str, list, default = None
+        The list of variables to evaluate. If `None`, the transformer will evaluate all
+        numerical variables in the dataset. If `"all"` the transformer will evaluate all
+        categorical and numerical variables in the dataset. Alternatively, the
+        transformer will evaluate the variables indicated in the list or string.
 
     {confirm_variables}
 
     Attributes
     ----------
     features_to_drop_:
         List with the features that will be dropped.
@@ -215,16 +270,18 @@
        https://scholarworks.wmich.edu/dissertations/3208/
 
     Examples
     --------
 
     >>> import pandas as pd
     >>> from feature_engine.selection import DropHighPSIFeatures
-    >>> X = pd.DataFrame(dict(x1 = [1,1,0,0,0,1,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
-    >>>                 x2 = [32,87,6,32,11,44,8,7,9,0,32,87,6,32,11,44,8,7,9,0]))
+    >>> X = pd.DataFrame(dict(
+    >>>         x1 = [1,1,0,0,0,1,0,0,0,0,0,0,0,0,0,0,0,0,0,0],
+    >>>         x2 = [32,87,6,32,11,44,8,7,9,0,32,87,6,32,11,44,8,7,9,0],
+    >>>         ))
     >>> psi = DropHighPSIFeatures()
     >>> psi.fit_transform(X)
         x2
     0   32
     1   87
     2    6
     3   32
@@ -247,14 +304,15 @@
         threshold: Union[float, int, str] = 0.25,
         bins: int = 10,
         strategy: str = "equal_frequency",
         min_pct_empty_bins: float = 0.0001,
         missing_values: str = "raise",
         variables: Variables = None,
         confirm_variables: bool = False,
+        p_value: float = 0.001,
     ):
 
         if not isinstance(split_col, (str, int, type(None))):
             raise ValueError(
                 f"split_col must be a string an integer or None. Got "
                 f"{split_col} instead."
             )
@@ -315,14 +373,19 @@
             if split_col in variables:
                 raise ValueError(
                     f"{split_col} cannot be used to split the data and be evaluated at "
                     f"the same time. Either remove {split_col} from the variables list "
                     f"or choose another splitting criteria."
                 )
 
+        if not isinstance(p_value, float) or p_value < 0 or p_value > 1:
+            raise ValueError(
+                f"p_value must be a float between 0 and 1. Got {p_value} instead."
+            )
+
         super().__init__(confirm_variables)
 
         # Check the variables before assignment.
         self.variables = _check_init_parameter_variables(variables)
 
         # Set all remaining arguments as attributes.
         self.split_col = split_col
@@ -331,14 +394,15 @@
         self.cut_off = cut_off
         self.switch = switch
         self.threshold = threshold
         self.bins = bins
         self.strategy = strategy
         self.min_pct_empty_bins = min_pct_empty_bins
         self.missing_values = missing_values
+        self.p_value = p_value
 
     def fit(self, X: pd.DataFrame, y: pd.Series = None):
         """
         Find features with high PSI values.
 
         Parameters
         ----------
@@ -347,29 +411,26 @@
 
         y : pandas series. Default = None
             y is not needed in this transformer. You can pass y or None.
         """
         # check input dataframe
         X = check_X(X)
 
-        # If required exclude variables that are not in the input dataframe
-        self._confirm_variables(X)
+        # select variables to evaluate
+        cat_variables_, num_variables_ = self._select_variables(X)
 
-        # find numerical variables or check those entered are present in the dataframe
-        self.variables_ = find_or_check_numerical_variables(X, self.variables_)
-
-        # Remove the split_col from the variables list. It might be added if the
-        # variables are not defined at initialization.
-        if self.split_col in self.variables_:
-            self.variables_.remove(self.split_col)
+        # check that split column is in the dataframe and remove from variable lists
+        cat_variables_, num_variables_ = self._check_split_column(
+            X, cat_variables_, num_variables_
+        )
 
         if self.missing_values == "raise":
             # check if dataset contains na or inf
-            _check_contains_na(X, self.variables_)
-            _check_contains_inf(X, self.variables_)
+            _check_contains_na(X, num_variables_ + cat_variables_)
+            _check_contains_inf(X, num_variables_)
 
         # Split the dataframe into basis and test.
         basis_df, test_df = self._split_dataframe(X)
 
         # Check the shape of the returned dataframes for PSI calculations.
         # The number of observations must be at least equal to the
         # number of bins.
@@ -383,55 +444,169 @@
                 "Please adjust the value of the cut_off or split_frac."
             )
 
         # Switch basis and test dataframes if required.
         if self.switch:
             test_df, basis_df = basis_df, test_df
 
-        if self.threshold == "auto":
-            threshold = self._calculate_auto_threshold(
-                basis_df.shape[0], test_df.shape[0]
-            )
-        else:
-            threshold = self.threshold
+        # Set up parameters for numerical features
+        if len(num_variables_) > 0:
 
-        # set up the discretizer
-        if self.strategy == "equal_width":
-            bucketer = EqualWidthDiscretiser(bins=self.bins)
-        else:
-            bucketer = EqualFrequencyDiscretiser(q=self.bins)
+            # Set up the discretizer for numerical features
+            if self.strategy == "equal_width":
+                bucketer = EqualWidthDiscretiser(bins=self.bins)
+            else:
+                bucketer = EqualFrequencyDiscretiser(q=self.bins)
+
+            # Set up the threshold for numerical features
+            if self.threshold == "auto":
+                threshold_num = self._calculate_auto_threshold(
+                    basis_df.shape[0],
+                    test_df.shape[0],
+                    self.bins,
+                )
+            else:
+                threshold_num = self.threshold
+
+        # Set up the generic threshold for categorical features if used
+        if len(cat_variables_) > 0:
+            if self.threshold != "auto":
+                threshold_cat = self.threshold
 
         # Compute the PSI by looping over the features
         self.psi_values_ = {}
         self.features_to_drop_ = []
 
-        for feature in self.variables_:
-            # Discretize the features.
-
+        # Compute PSI for numerical features
+        for feature in num_variables_:
+            # Discretize feature
             basis_discrete = bucketer.fit_transform(basis_df[[feature]].dropna())
             test_discrete = bucketer.transform(test_df[[feature]].dropna())
 
             # Determine percentage of observations per bin
             basis_distrib, test_distrib = self._observation_frequency_per_bin(
                 basis_discrete, test_discrete
             )
 
             # Calculate the PSI value
             self.psi_values_[feature] = np.sum(
                 (test_distrib - basis_distrib) * np.log(test_distrib / basis_distrib)
             )
+
             # Assess if feature should be dropped
-            if self.psi_values_[feature] > threshold:
+            if self.psi_values_[feature] > threshold_num:
                 self.features_to_drop_.append(feature)
 
+        # Compute the PSI for categorical features
+        for feature in cat_variables_:
+            basis_discrete = basis_df[[feature]]
+            test_discrete = test_df[[feature]]
+
+            # Determine percentage of observations per bin
+            basis_distrib, test_distrib = self._observation_frequency_per_bin(
+                basis_discrete, test_discrete
+            )
+
+            # Calculate the PSI value
+            self.psi_values_[feature] = np.sum(
+                (test_distrib - basis_distrib) * np.log(test_distrib / basis_distrib)
+            )
+
+            # Determine the appropriate threshold for the categorical feature
+            if self.threshold == "auto":
+                n_bins_cat = X[feature].nunique()
+                threshold_cat = self._calculate_auto_threshold(
+                    basis_df.shape[0],
+                    test_df.shape[0],
+                    n_bins_cat,
+                )
+
+            # Assess if feature should be dropped
+            if self.psi_values_[feature] > threshold_cat:
+                self.features_to_drop_.append(feature)
+
+        # store analyzed variables
+        self.variables_ = num_variables_ + cat_variables_
         # save input features
         self._get_feature_names_in(X)
 
         return self
 
+    def _select_variables(self, X: pd.DataFrame):
+        """Based on the user input to the `variables` attribute in init, find or check
+        the variables for which the PSI should be calculated.
+
+        If `None`, select all numerical variables.
+        If `"all", select all numerical and categorical variables.
+        If string or list, check that the variables are numerical or categorical.
+        """
+
+        if self.variables is None:
+            num_variables = list(X.select_dtypes(include="number").columns)
+            if len(num_variables) == 0:
+                raise ValueError(
+                    "No numerical variables found in this dataframe. Please check "
+                    "variable format with pandas dtypes."
+                )
+            cat_variables: List[Union[str, int]] = []
+
+        elif self.variables == "all":
+            (
+                cat_variables,
+                num_variables,
+            ) = find_categorical_and_numerical_variables(X, None)
+
+        else:
+            if not isinstance(self.variables, list):
+                variables = [self.variables]
+            else:
+                variables = self.variables
+
+            if self.confirm_variables is True:
+                variables = [var for var in variables if var in X.columns]
+                # Raise an error if no column is left to work with.
+                if len(variables) == 0:
+                    raise ValueError(
+                        "After confirming variables, no variable remains. At least 1 "
+                        "variable is required for the selection."
+                    )
+
+            (
+                cat_variables,
+                num_variables,
+            ) = find_categorical_and_numerical_variables(X, variables)
+
+        return cat_variables, num_variables
+
+    def _check_split_column(
+        self,
+        X: pd.DataFrame,
+        cat_variables: List[Union[str, int]],
+        num_variables: List[Union[str, int]],
+    ):
+        """Check that split_col is in the dataframe and remove from numerical and
+        categorical variable lists if necessary.
+
+        It will get added if the variables are selected automatically.
+        """
+        if self.split_col is not None:
+            # check that split_col is in the dataframe.
+            if self.split_col not in X.columns:
+                raise ValueError(f"{self.split_col} is not in the dataframe.")
+
+            # Remove the split_col from variables lists. Happens when variables are
+            # selected by transformer.
+            if self.variables is None or self.variables == "all":
+                if self.split_col in num_variables:
+                    num_variables.remove(self.split_col)
+                elif self.split_col in cat_variables:
+                    cat_variables.remove(self.split_col)
+
+        return cat_variables, num_variables
+
     def _observation_frequency_per_bin(self, basis, test):
         """
         Obtain the fraction of observations per interval.
 
         Parameters
         ----------
         basis : pd.DataFrame.
@@ -460,20 +635,21 @@
             .merge(
                 pd.DataFrame(test_distrib),
                 right_index=True,
                 left_index=True,
                 how="outer",
             )
             .fillna(self.min_pct_empty_bins)
+            .replace(to_replace=0, value=self.min_pct_empty_bins)
         )
         distributions.columns = ["basis", "test"]
 
         return distributions.basis, distributions.test
 
-    def _split_dataframe(self, X):
+    def _split_dataframe(self, X: pd.DataFrame):
         """
         Split dataframe according to a cut-off value and return two dataframes: the
         basis dataframe contains all observations <= cut_off and the test dataframe the
         observations > cut_off.
 
         If cut-off is a list, then the basis dataframe will contain all observations
         which values are within the list, and the test dataframe all remaining
@@ -491,21 +667,21 @@
             pandas dataframe with observations which value <= cut_off
 
         test_df: pd.DataFrame
             pandas dataframe with observations which value > cut_off
         """
 
         # Identify the values according to which the split must be done.
-        if not self.split_col:
+        if self.split_col is None:
             reference = pd.Series(X.index)
         else:
             reference = X[self.split_col]
 
         # Raise an error if there are missing values in the reference column.
-        if reference.isna().sum() != 0:
+        if reference.isna().any():
             raise ValueError(
                 f"There are {reference.isna().sum()} missing values in the reference"
                 "variable. Missing data are not allowed in the variable used to "
                 "split the dataframe."
             )
 
         # If cut_off is not pre-defined, compute it.
@@ -543,15 +719,15 @@
             is the closest to the chosen split fraction is used as cut-off.
 
             - The procedure assumes that categorical values are sorted alphabetically
             and cut accordingly.
 
         Parameters
         ----------
-        split_column : pd.Series.
+        split_column: pd.Series.
             Series for which the nth quantile will be computed.
 
         Returns
         -------
         cut_off: (float, int, str, object).
             value for the cut-off.
         """
@@ -573,14 +749,41 @@
             # Get the index (i.e. value) with the quantile that is the closest
             # to the split_frac defined at initialization.
             distance = abs(reference - self.split_frac)
             cut_off = (distance.idxmin()).values[0]
 
         return cut_off
 
-    def _calculate_auto_threshold(self, N, M, q=0.999):
-        # threshold = χ2(q,B−1) × (1/N + 1/M)
-        # where q - quantile (or 1 - p-value) B - number of bins,
-        # N - size of basis dataset, M - size of test dataset
-        # see formula (5.2) from reference
-        # taking q = 0.999 to get higher threshold
-        return stats.chi2.ppf(q, self.bins - 1) * (1.0 / N + 1.0 / M)
+    def _calculate_auto_threshold(self, N, M, bins):
+        """Threshold computation for chi-square test.
+
+        The threshold is given by:
+
+            threshold = χ2(q,B−1) × (1/N + 1/M)
+
+        where:
+
+        q = quantile of the distribution (or 1 - p-value),
+        B = number of bins/categories,
+        N = size of basis dataset,
+        M = size of test dataset.
+        See formula (5.2) from reference [1] in the class docstring.
+
+        Parameters
+        ----------
+        N: float or int
+        M: float or int
+        bins: int
+
+        Returns
+        -------
+        float
+        """
+        return stats.chi2.ppf(1 - self.p_value, bins - 1) * (1.0 / N + 1.0 / M)
+
+    def _more_tags(self):
+        tags_dict = _return_tags()
+        tags_dict["variables"] = "pass"
+        # add additional test that fails
+        tags_dict["_xfail_checks"]["check_estimators_nan_inf"] = "transformer allows NA"
+
+        return tags_dict
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/information_value.py` & `feature_engine-1.6.1/feature_engine/selection/information_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from feature_engine._docstrings.substitute import Substitution
 from feature_engine.dataframe_checks import _check_contains_inf, _check_contains_na
 from feature_engine.discretisation import (
     EqualFrequencyDiscretiser,
     EqualWidthDiscretiser,
 )
 from feature_engine.encoding.woe import WoE
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _features_to_drop_docstring,
     _get_support_docstring,
     _threshold_docstring,
 )
 from feature_engine.selection.base_selector import BaseSelector
 from feature_engine.tags import _return_tags
 from feature_engine.variable_handling._init_parameter_checks import (
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/probe_feature_selection.py` & `feature_engine-1.6.1/feature_engine/selection/probe_feature_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from feature_engine._docstrings.init_parameters.selection import (
     _confirm_variables_docstring,
     _estimator_docstring,
 )
 from feature_engine._docstrings.methods import _fit_transform_docstring
 from feature_engine._docstrings.substitute import Substitution
 from feature_engine.dataframe_checks import check_X_y
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _cv_docstring,
     _features_to_drop_docstring,
     _fit_docstring,
     _get_support_docstring,
     _scoring_docstring,
     _transform_docstring,
     _variables_attribute_docstring,
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/recursive_feature_addition.py` & `feature_engine-1.6.1/feature_engine/selection/recursive_feature_addition.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 from feature_engine._docstrings.init_parameters.selection import (
     _confirm_variables_docstring,
     _estimator_docstring,
 )
 from feature_engine._docstrings.methods import _fit_transform_docstring
 from feature_engine._docstrings.substitute import Substitution
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _cv_docstring,
     _features_to_drop_docstring,
     _fit_docstring,
     _get_support_docstring,
     _initial_model_performance_docstring,
     _scoring_docstring,
     _threshold_docstring,
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/recursive_feature_elimination.py` & `feature_engine-1.6.1/feature_engine/selection/recursive_feature_elimination.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 )
 from feature_engine._docstrings.init_parameters.selection import (
     _confirm_variables_docstring,
     _estimator_docstring,
 )
 from feature_engine._docstrings.methods import _fit_transform_docstring
 from feature_engine._docstrings.substitute import Substitution
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _cv_docstring,
     _features_to_drop_docstring,
     _fit_docstring,
     _get_support_docstring,
     _initial_model_performance_docstring,
     _scoring_docstring,
     _threshold_docstring,
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/shuffle_features.py` & `feature_engine-1.6.1/feature_engine/selection/shuffle_features.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import List, Union
 
 import numpy as np
 import pandas as pd
 from sklearn.base import is_classifier
 from sklearn.metrics import get_scorer
 from sklearn.model_selection import check_cv, cross_validate
-from sklearn.utils.validation import check_random_state
+from sklearn.utils.validation import check_random_state, _check_sample_weight
 
 from feature_engine._docstrings.fit_attributes import (
     _feature_names_in_docstring,
     _n_features_in_docstring,
 )
 from feature_engine._docstrings.init_parameters.selection import (
     _confirm_variables_docstring,
 )
 from feature_engine._docstrings.methods import _fit_transform_docstring
 from feature_engine._docstrings.substitute import Substitution
 from feature_engine.dataframe_checks import check_X_y
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _cv_docstring,
     _estimator_docstring,
     _features_to_drop_docstring,
     _fit_docstring,
     _get_support_docstring,
     _initial_model_performance_docstring,
     _scoring_docstring,
@@ -181,32 +181,44 @@
         self.variables = _check_init_parameter_variables(variables)
         self.estimator = estimator
         self.scoring = scoring
         self.threshold = threshold
         self.cv = cv
         self.random_state = random_state
 
-    def fit(self, X: pd.DataFrame, y: pd.Series):
+    def fit(
+        self,
+        X: pd.DataFrame,
+        y: pd.Series,
+        sample_weight: Union[np.array, pd.Series, List] = None,
+    ):
         """
         Find the important features.
 
         Parameters
         ----------
         X: pandas dataframe of shape = [n_samples, n_features]
            The input dataframe.
+
         y: array-like of shape (n_samples)
            Target variable. Required to train the estimator.
+
+        sample_weight : array-like of shape (n_samples,), default=None
+            Sample weights. If None, then samples are equally weighted.
         """
 
         X, y = check_X_y(X, y)
 
         # reset the index
         X = X.reset_index(drop=True)
         y = y.reset_index(drop=True)
 
+        if sample_weight is not None:
+            sample_weight = _check_sample_weight(sample_weight, X)
+
         # If required exclude variables that are not in the input dataframe
         self._confirm_variables(X)
 
         # find numerical variables or check variables entered by user
         self.variables_ = find_or_check_numerical_variables(X, self.variables_)
 
         # check that there are more than 1 variable to select from
@@ -216,14 +228,15 @@
         model = cross_validate(
             self.estimator,
             X[self.variables_],
             y,
             cv=self.cv,
             return_estimator=True,
             scoring=self.scoring,
+            fit_params={"sample_weight": sample_weight},
         )
 
         # store initial model performance
         self.initial_model_performance_ = model["test_score"].mean()
 
         # extract the validation folds
         cv_ = check_cv(self.cv, y=y, classifier=is_classifier(self.estimator))
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/single_feature_performance.py` & `feature_engine-1.6.1/feature_engine/selection/single_feature_performance.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from feature_engine._docstrings.init_parameters.selection import (
     _confirm_variables_docstring,
 )
 from feature_engine._docstrings.methods import _fit_transform_docstring
 from feature_engine._docstrings.substitute import Substitution
 from feature_engine.dataframe_checks import check_X_y
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _cv_docstring,
     _estimator_docstring,
     _features_to_drop_docstring,
     _fit_docstring,
     _get_support_docstring,
     _initial_model_performance_docstring,
     _scoring_docstring,
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/smart_correlation_selection.py` & `feature_engine-1.6.1/feature_engine/selection/smart_correlation_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from feature_engine._docstrings.methods import _fit_transform_docstring
 from feature_engine._docstrings.substitute import Substitution
 from feature_engine.dataframe_checks import (
     _check_contains_inf,
     _check_contains_na,
     check_X,
 )
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _cv_docstring,
     _estimator_docstring,
     _get_support_docstring,
     _missing_values_docstring,
     _scoring_docstring,
     _variables_attribute_docstring,
     _variables_numerical_docstring,
```

### Comparing `feature_engine-1.6.0/feature_engine/selection/target_mean_selection.py` & `feature_engine-1.6.1/feature_engine/selection/target_mean_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     _confirm_variables_docstring,
 )
 from feature_engine._docstrings.methods import _fit_transform_docstring
 from feature_engine._docstrings.substitute import Substitution
 from feature_engine._prediction.target_mean_classifier import TargetMeanClassifier
 from feature_engine._prediction.target_mean_regressor import TargetMeanRegressor
 from feature_engine.dataframe_checks import check_X_y
-from feature_engine.selection._docstring import (
+from feature_engine._docstrings.selection._docstring import (
     _cv_docstring,
     _features_to_drop_docstring,
     _fit_docstring,
     _get_support_docstring,
     _scoring_docstring,
     _threshold_docstring,
     _transform_docstring,
```

### Comparing `feature_engine-1.6.0/feature_engine/tags.py` & `feature_engine-1.6.1/feature_engine/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
             "check_dtype_object": "Feature-engine transformers use dtypes to select "
             "between numerical and categorical variables. Feature-engine trusts the "
             "user casts the variables appropriately",
             # Test fails because FE does not like the sklearn class _NotAnArray
             # The test aims to check that the check_X_y function from sklearn is
             # working, but we do not use that check, because we work with dfs.
             "check_transformer_data_not_an_array": "Ok to fail",
+            "check_sample_weights_not_an_array": "Ok to fail",
             # TODO: we probably need the test below!!
             "check_methods_sample_order_invariance": "Test does not work on dataframes",
             # TODO: we probably need the test below!!
             # the test below tests that a second fit overrides a first fit.
             # the problem is that the test does not work with pandas df.
             "check_fit_idempotent": "Test does not work on dataframes.",
             "check_fit2d_predict1d": "Test not relevant, Feature-engine transformers "
```

### Comparing `feature_engine-1.6.0/feature_engine/timeseries/forecasting/base_forecast_transformers.py` & `feature_engine-1.6.1/feature_engine/timeseries/forecasting/base_forecast_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,15 @@
         if self.missing_values == "raise":
             self._check_na_and_inf(X)
 
         self._get_feature_names_in(X)
 
         return self
 
-    def transform(self, X: pd.DataFrame) -> pd.DataFrame:
+    def _check_transform_input_and_state(self, X: pd.DataFrame) -> pd.DataFrame:
         """
         Common checks performed before the feature transformation.
 
         Parameters
         ----------
         X: pandas dataframe of shape = [n_samples, n_features]
             The data to transform.
```

### Comparing `feature_engine-1.6.0/feature_engine/timeseries/forecasting/expanding_window_features.py` & `feature_engine-1.6.1/feature_engine/timeseries/forecasting/expanding_window_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
         Returns
         -------
         X_new: Pandas dataframe, shape = [n_samples, n_features + window_features]
             The dataframe with the original plus the new variables.
         """
         # Common dataframe checks and setting up.
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         tmp = (
             X[self.variables_]
             .expanding(min_periods=self.min_periods)
             .agg(self.functions)
             .shift(periods=self.periods, freq=self.freq)
         )
```

### Comparing `feature_engine-1.6.0/feature_engine/timeseries/forecasting/lag_features.py` & `feature_engine-1.6.1/feature_engine/timeseries/forecasting/lag_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
         Returns
         -------
         X_new: Pandas dataframe, shape = [n_samples, n_features + lag_features]
             The dataframe with the original plus the new variables.
         """
         # Common dataframe checks and setting up.
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # if freq is not None, it overrides periods.
         if self.freq is not None:
 
             if isinstance(self.freq, list):
                 df_ls = []
                 for fr in self.freq:
```

### Comparing `feature_engine-1.6.0/feature_engine/timeseries/forecasting/window_features.py` & `feature_engine-1.6.1/feature_engine/timeseries/forecasting/window_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
         Returns
         -------
         X_new: Pandas dataframe, shape = [n_samples, n_features + window_features]
             The dataframe with the original plus the new variables.
         """
         # Common dataframe checks and setting up.
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         if isinstance(self.window, list):
             df_ls = []
             for win in self.window:
                 tmp = (
                     X[self.variables_]
                     .rolling(window=win)
```

### Comparing `feature_engine-1.6.0/feature_engine/transformation/__init__.py` & `feature_engine-1.6.1/feature_engine/transformation/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/transformation/arcsin.py` & `feature_engine-1.6.1/feature_engine/transformation/arcsin.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         Returns
         -------
         X_new: pandas dataframe
             The dataframe with the transformed variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # check if the variables are in the correct range
         if ((X[self.variables_] < 0) | (X[self.variables_] > 1)).any().any():
             raise ValueError(
                 "Some variables contain values outside the possible range 0-1. "
                 "Can't apply the arcsin transformation."
             )
```

### Comparing `feature_engine-1.6.0/feature_engine/transformation/boxcox.py` & `feature_engine-1.6.1/feature_engine/transformation/boxcox.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         Returns
         -------
         X_new: pandas dataframe
             The dataframe with the transformed variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # check contains zero or negative values
         if (X[self.variables_] <= 0).any().any():
             raise ValueError("Data must be positive.")
 
         # transform
         for feature in self.variables_:
@@ -184,15 +184,15 @@
         Returns
         -------
         X_new: pandas dataframe
             The dataframe with the original variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # inverse transform
         for feature in self.variables_:
             X[feature] = inv_boxcox(X[feature], self.lambda_dict_[feature])
 
         return X
```

### Comparing `feature_engine-1.6.0/feature_engine/transformation/log.py` & `feature_engine-1.6.1/feature_engine/transformation/log.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         Returns
         -------
         X_new: pandas dataframe
             The dataframe with the transformed variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # check contains zero or negative values
         if (X[self.variables_] <= 0).any().any():
             raise ValueError(
                 "Some variables contain zero or negative values, can't apply log"
             )
 
@@ -182,15 +182,15 @@
         Returns
         -------
         X_tr: pandas dataframe
             The dataframe with the transformed variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # inverse_transform
         if self.base == "e":
             X.loc[:, self.variables_] = np.exp(X.loc[:, self.variables_])
         elif self.base == "10":
             X.loc[:, self.variables_] = np.array(10 ** X.loc[:, self.variables_])
 
@@ -370,15 +370,15 @@
         Returns
         -------
         X_new: pandas dataframe
             The dataframe with the transformed variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # check variable is positive after adding c
         if (X[self.variables_] + self.C_ <= 0).any().any():
             raise ValueError(
                 "Some variables contain zero or negative values after adding"
                 + "constant C, can't apply log"
             )
@@ -403,15 +403,15 @@
         Returns
         -------
         X_tr: Pandas dataframe
             The dataframe with the transformed variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # inverse transform
         if self.base == "e":
             X.loc[:, self.variables_] = np.exp(X.loc[:, self.variables_]) - self.C_
         elif self.base == "10":
             X.loc[:, self.variables_] = 10 ** X.loc[:, self.variables_] - self.C_
```

### Comparing `feature_engine-1.6.0/feature_engine/transformation/power.py` & `feature_engine-1.6.1/feature_engine/transformation/power.py`

 * *Files 3% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         Returns
         -------
         X_new: pandas Dataframe
             The dataframe with the power transformed variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # transform
         X.loc[:, self.variables_] = np.power(X.loc[:, self.variables_], self.exp)
 
         return X
 
     def inverse_transform(self, X: pd.DataFrame) -> pd.DataFrame:
@@ -160,13 +160,13 @@
         Returns
         -------
         X_tr: pandas Dataframe
             The dataframe with the power transformed variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # inverse_transform
         X.loc[:, self.variables_] = np.power(X.loc[:, self.variables_], 1 / self.exp)
 
         return X
```

### Comparing `feature_engine-1.6.0/feature_engine/transformation/reciprocal.py` & `feature_engine-1.6.1/feature_engine/transformation/reciprocal.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     3  0.110047
     4  0.101726
     """
 
     def __init__(
         self, variables: Union[None, int, str, List[Union[str, int]]] = None
     ) -> None:
-
         self.variables = _check_init_parameter_variables(variables)
 
     def fit(self, X: pd.DataFrame, y: Optional[pd.Series] = None):
         """
         This transformer does not learn parameters.
 
         Parameters
@@ -137,27 +136,28 @@
         Returns
         -------
         X_new: pandas dataframe
             The dataframe with the transformed variables.
         """
 
         # check input dataframe and if class was fitted
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
 
         # check if the variables contain the value 0
         if (X[self.variables_] == 0).any().any():
             raise ValueError(
                 "Some variables contain the value zero, can't apply reciprocal "
                 "transformation."
             )
 
         # transform
         # for some reason reciprocal does not work with integers
-        X.loc[:, self.variables_] = X.loc[:, self.variables_].astype("float")
-        X.loc[:, self.variables_] = np.reciprocal(X.loc[:, self.variables_])
+        X.loc[:, self.variables_] = np.reciprocal(
+            X.loc[:, self.variables_].astype("float")
+        )
 
         return X
 
     def inverse_transform(self, X: pd.DataFrame) -> pd.DataFrame:
         """
         Convert the data back to the original representation.
```

### Comparing `feature_engine-1.6.0/feature_engine/transformation/yeojohnson.py` & `feature_engine-1.6.1/feature_engine/transformation/yeojohnson.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,12 +143,12 @@
         -------
         X: pandas dataframe
             The dataframe with the transformed variables.
         """
 
         # check input dataframe and if class was fitted
 
-        X = super().transform(X)
+        X = self._check_transform_input_and_state(X)
         for feature in self.variables_:
             X[feature] = stats.yeojohnson(X[feature], lmbda=self.lambda_dict_[feature])
 
         return X
```

### Comparing `feature_engine-1.6.0/feature_engine/variable_handling/__init__.py` & `feature_engine-1.6.1/feature_engine/variable_handling/__init__.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/variable_handling/_init_parameter_checks.py` & `feature_engine-1.6.1/feature_engine/variable_handling/_init_parameter_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/variable_handling/_variable_type_checks.py` & `feature_engine-1.6.1/feature_engine/variable_handling/_variable_type_checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+import warnings
+
 import pandas as pd
 from pandas.core.dtypes.common import is_categorical_dtype as is_categorical
 from pandas.core.dtypes.common import is_datetime64_any_dtype as is_datetime
 from pandas.core.dtypes.common import is_numeric_dtype as is_numeric
 from pandas.core.dtypes.common import is_object_dtype as is_object
 
 
 def _is_categorical_and_is_not_datetime(column: pd.Series) -> bool:
-
     # check for datetime only if object cannot be cast as numeric because
     # if it could pd.to_datetime would convert it to datetime regardless
     if is_object(column):
         is_cat = _is_convertible_to_num(column) or not _is_convertible_to_dt(column)
 
     # check for datetime only if the type of the categories is not numeric
     # because pd.to_datetime throws an error when it is an integer
@@ -21,23 +22,24 @@
 
 
 def _is_categories_num(column: pd.Series) -> bool:
     return is_numeric(column.dtype.categories)
 
 
 def _is_convertible_to_dt(column: pd.Series) -> bool:
-    return is_datetime(pd.to_datetime(column, errors="ignore", utc=True))
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        return is_datetime(pd.to_datetime(column, errors="ignore", utc=True))
 
 
 def _is_convertible_to_num(column: pd.Series) -> bool:
     return is_numeric(pd.to_numeric(column, errors="ignore"))
 
 
 def _is_categorical_and_is_datetime(column: pd.Series) -> bool:
-
     # check for datetime only if object cannot be cast as numeric because
     # if it could pd.to_datetime would convert it to datetime regardless
     if is_object(column):
         is_dt = not _is_convertible_to_num(column) and _is_convertible_to_dt(column)
 
     # check for datetime only if the type of the categories is not numeric
     # because pd.to_datetime throws an error when it is an integer
```

### Comparing `feature_engine-1.6.0/feature_engine/variable_handling/variable_type_selection.py` & `feature_engine-1.6.1/feature_engine/variable_handling/variable_type_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine/wrappers/wrappers.py` & `feature_engine-1.6.1/feature_engine/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/feature_engine.egg-info/PKG-INFO` & `feature_engine-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: feature-engine
-Version: 1.6.0
+Name: feature_engine
+Version: 1.6.1
 Summary: Feature engineering package with Scikit-learn's fit transform functionality
 Home-page: http://github.com/feature-engine/feature_engine
 Author: Soledad Galli
 Author-email: solegalli@protonmail.com
 License: BSD 3 clause
 Description: # Feature Engine
```

### Comparing `feature_engine-1.6.0/feature_engine.egg-info/SOURCES.txt` & `feature_engine-1.6.1/feature_engine.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 feature_engine/_docstrings/substitute.py
 feature_engine/_docstrings/init_parameters/__init__.py
 feature_engine/_docstrings/init_parameters/all_trasnformers.py
 feature_engine/_docstrings/init_parameters/discretisers.py
 feature_engine/_docstrings/init_parameters/encoders.py
 feature_engine/_docstrings/init_parameters/outliers.py
 feature_engine/_docstrings/init_parameters/selection.py
+feature_engine/_docstrings/selection/__init__.py
+feature_engine/_docstrings/selection/_docstring.py
 feature_engine/_prediction/__init__.py
 feature_engine/_prediction/base_predictor.py
 feature_engine/_prediction/target_mean_classifier.py
 feature_engine/_prediction/target_mean_regressor.py
 feature_engine/creation/__init__.py
 feature_engine/creation/base_creation.py
 feature_engine/creation/cyclical_features.py
@@ -78,15 +80,14 @@
 feature_engine/outliers/base_outlier.py
 feature_engine/outliers/trimmer.py
 feature_engine/outliers/winsorizer.py
 feature_engine/preprocessing/__init__.py
 feature_engine/preprocessing/match_categories.py
 feature_engine/preprocessing/match_columns.py
 feature_engine/selection/__init__.py
-feature_engine/selection/_docstring.py
 feature_engine/selection/_selection_constants.py
 feature_engine/selection/base_recursive_selector.py
 feature_engine/selection/base_selector.py
 feature_engine/selection/drop_constant_features.py
 feature_engine/selection/drop_correlated_features.py
 feature_engine/selection/drop_duplicate_features.py
 feature_engine/selection/drop_features.py
```

### Comparing `feature_engine-1.6.0/setup.py` & `feature_engine-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/estimator_checks/dataframe_for_checks.py` & `feature_engine-1.6.1/tests/estimator_checks/dataframe_for_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/estimator_checks/estimator_checks.py` & `feature_engine-1.6.1/tests/estimator_checks/estimator_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,16 @@
             check_numerical_variables_assignment(estimator, needs_group=needs_group)
         elif tags["variables"] == "categorical":
             check_categorical_variables_assignment(estimator, needs_group=needs_group)
         elif tags["variables"] == "all":
             check_all_types_variables_assignment(estimator, needs_group=needs_group)
         elif tags["variables"] == "datetime":
             check_datetime_variables_assignment(estimator)
+        else:
+            pass
 
     # Tests based on transformer's init parameters
     if hasattr(estimator, "cv"):
         check_takes_cv_constructor(estimator)
 
     if hasattr(estimator, "missing_values"):
         check_error_param_missing_values(estimator)
```

### Comparing `feature_engine-1.6.0/tests/estimator_checks/fit_functionality_checks.py` & `feature_engine-1.6.1/tests/estimator_checks/fit_functionality_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/estimator_checks/get_feature_names_out_checks.py` & `feature_engine-1.6.1/tests/estimator_checks/get_feature_names_out_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/estimator_checks/init_params_allowed_values_checks.py` & `feature_engine-1.6.1/tests/estimator_checks/init_params_allowed_values_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/estimator_checks/init_params_triggered_functionality_checks.py` & `feature_engine-1.6.1/tests/estimator_checks/init_params_triggered_functionality_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/estimator_checks/non_fitted_error_checks.py` & `feature_engine-1.6.1/tests/estimator_checks/non_fitted_error_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/estimator_checks/variable_selection_checks.py` & `feature_engine-1.6.1/tests/estimator_checks/variable_selection_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_check_input_parameters/test_check_init_input_params.py` & `feature_engine-1.6.1/tests/test_check_input_parameters/test_check_init_input_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pytest
+
 from feature_engine._check_input_parameters.check_init_input_params import (
-    _check_param_missing_values,
     _check_param_drop_original,
+    _check_param_missing_values,
 )
 
 
 @pytest.mark.parametrize("missing_vals", [None, ["Hola"], True, "Hola"])
 def test_check_param_missing_values(missing_vals):
     with pytest.raises(ValueError):
         _check_param_missing_values(missing_vals)
```

### Comparing `feature_engine-1.6.0/tests/test_check_input_parameters/test_check_input_dictionary.py` & `feature_engine-1.6.1/tests/test_check_input_parameters/test_check_input_dictionary.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_creation/test_cyclical_features.py` & `feature_engine-1.6.1/tests/test_creation/test_cyclical_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_creation/test_math_features.py` & `feature_engine-1.6.1/tests/test_creation/test_math_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_creation/test_relative_features.py` & `feature_engine-1.6.1/tests/test_creation/test_relative_features.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,25 @@
         RelativeFeatures(
             variables=["Age", "Name"],
             reference=["Age", "Name"],
             func=_func,
         )
 
 
+@pytest.mark.parametrize("_fill_value", [(2, 3.3), ["test"], "python"])
+def test_error_if_fill_value_not_permitted(_fill_value):
+    with pytest.raises(ValueError):
+        RelativeFeatures(
+            variables=["Age"],
+            reference=["Marks"],
+            func=["sub", "div", "add", "mul"],
+            fill_value=_fill_value,
+        )
+
+
 def test_error_when_drop_original_not_bool():
     for drop_original in ["True", [True]]:
         with pytest.raises(ValueError):
             RelativeFeatures(
                 variables=["Age"],
                 reference=["Marks"],
                 func=["add", "mul"],
@@ -314,28 +325,73 @@
         }
     )
 
     pd.testing.assert_frame_equal(X, ref)
 
 
 @pytest.mark.parametrize("_func", [["div"], ["truediv"], ["floordiv"], ["mod"]])
-def test_error_when_division_by_zero(_func, df_vartypes):
+def test_error_when_division_by_zero_and_fill_value_is_none(_func, df_vartypes):
 
     df_zero = df_vartypes.copy()
     df_zero.loc[1, "Marks"] = 0
 
     transformer = RelativeFeatures(
         variables=["Age"],
         reference=["Marks"],
         func=_func,
     )
     transformer.fit(df_vartypes)
-    with pytest.raises(ValueError):
+
+    with pytest.raises(ValueError) as record:
         transformer.transform(df_zero)
 
+    msg = (
+        "Some of the reference variables contain zeroes. Division by zero "
+        "does not exist. Replace zeros before using this transformer for division "
+        "or set `fill_value` to a number."
+    )
+    # check that the error message matches
+    assert str(record.value) == msg
+
+
+@pytest.mark.parametrize(
+    "_fill_value, _func",
+    [
+        (111.111, ["div"]),
+        (999, ["div"]),
+        (111.111, ["truediv"]),
+        (999, ["truediv"]),
+        (111.111, ["floordiv"]),
+        (999, ["floordiv"]),
+        (111.111, ["mod"]),
+        (999, ["mod"]),
+    ],
+)
+def test_fill_values_when_division_by_zero(_fill_value, _func, df_vartypes):
+    df_zero = df_vartypes.copy()
+    df_zero.loc[2, "Marks"] = 0
+    df_zero.loc[1, "Age"] = np.nan
+    df_zero.loc[3, "Age"] = np.inf
+
+    transformer = RelativeFeatures(
+        variables=["Age"],
+        reference=["Marks"],
+        fill_value=_fill_value,
+        func=_func,
+        missing_values="ignore",
+    )
+
+    X = transformer.fit_transform(df_zero)
+
+    new_var = f"Age_{_func[0]}_Marks"
+
+    assert X.loc[2, new_var] == _fill_value
+    np.testing.assert_equal(X.loc[1, "Age"], np.nan)
+    np.testing.assert_equal(X.loc[3, "Age"], np.inf)
+
 
 @pytest.mark.parametrize("_drop", [True, False])
 def test_get_feature_names_out(_drop, df_vartypes):
     transformer = RelativeFeatures(
         variables=["Age", "Marks"],
         reference=["Age", "Marks"],
         func=["add", "sub"],
```

### Comparing `feature_engine-1.6.0/tests/test_datetime/conftest.py` & `feature_engine-1.6.1/tests/test_datetime/conftest.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_datetime/test_datetime_features.py` & `feature_engine-1.6.1/tests/test_datetime/test_datetime_features.py`

 * *Files 10% similar despite different names*

```diff
@@ -179,14 +179,15 @@
     transformer = DatetimeFeatures()
     X = transformer.fit_transform(df_datetime)
     pd.testing.assert_frame_equal(
         X,
         df_datetime_transformed[
             vars_non_dt + [var + feat for var in vars_dt for feat in feat_names_default]
         ],
+        check_dtype=False,
     )
 
 
 def test_extract_datetime_features_from_specified_variables(
     df_datetime, df_datetime_transformed
 ):
     # single datetime variable
@@ -194,14 +195,15 @@
     pd.testing.assert_frame_equal(
         X,
         df_datetime_transformed[
             vars_non_dt
             + ["datetime_range", "date_obj2", "time_obj"]
             + ["date_obj1" + feat for feat in feat_names_default]
         ],
+        check_dtype=False,
     )
 
     # multiple datetime variables
     X = DatetimeFeatures(variables=["datetime_range", "date_obj2"]).fit_transform(
         df_datetime
     )
     pd.testing.assert_frame_equal(
@@ -211,14 +213,15 @@
             + ["date_obj1", "time_obj"]
             + [
                 var + feat
                 for var in ["datetime_range", "date_obj2"]
                 for feat in feat_names_default
             ]
         ],
+        check_dtype=False,
     )
 
     # multiple datetime variables in different order than they appear in the df
     X = DatetimeFeatures(variables=["date_obj2", "date_obj1"]).fit_transform(
         df_datetime
     )
     pd.testing.assert_frame_equal(
@@ -228,14 +231,15 @@
             + ["datetime_range", "time_obj"]
             + [
                 var + feat
                 for var in ["date_obj2", "date_obj1"]
                 for feat in feat_names_default
             ]
         ],
+        check_dtype=False,
     )
 
     # datetime variable is index
     X = DatetimeFeatures(
         variables="index", features_to_extract=["month", "day_of_month"]
     ).fit_transform(dates_idx_dt)
     pd.testing.assert_frame_equal(
@@ -247,54 +251,61 @@
                     [[2, 27], [2, 28], [3, 1], [3, 2]],
                     index=dates_idx_dt.index,
                     columns=["month", "day_of_month"],
                 ),
             ],
             axis=1,
         ),
+        check_dtype=False,
     )
 
 
 def test_extract_all_datetime_features(df_datetime, df_datetime_transformed):
     X = DatetimeFeatures(features_to_extract="all").fit_transform(df_datetime)
-    pd.testing.assert_frame_equal(X, df_datetime_transformed.drop(vars_dt, axis=1))
+    pd.testing.assert_frame_equal(
+        X, df_datetime_transformed.drop(vars_dt, axis=1), check_dtype=False
+    )
 
 
 def test_extract_specified_datetime_features(df_datetime, df_datetime_transformed):
     X = DatetimeFeatures(features_to_extract=["semester", "week"]).fit_transform(
         df_datetime
     )
     pd.testing.assert_frame_equal(
         X,
         df_datetime_transformed[
             vars_non_dt
             + [var + "_" + feat for var in vars_dt for feat in ["semester", "week"]]
         ],
+        check_dtype=False,
     )
 
     # different order than they appear in the glossary
     X = DatetimeFeatures(features_to_extract=["hour", "day_of_week"]).fit_transform(
         df_datetime
     )
     pd.testing.assert_frame_equal(
         X,
         df_datetime_transformed[
             vars_non_dt
             + [var + "_" + feat for var in vars_dt for feat in ["hour", "day_of_week"]]
         ],
+        check_dtype=False,
     )
 
 
 def test_extract_features_from_categorical_variable(
     df_datetime, df_datetime_transformed
 ):
     cat_date = pd.DataFrame({"date_obj1": df_datetime["date_obj1"].astype("category")})
     X = DatetimeFeatures(variables="date_obj1").fit_transform(cat_date)
     pd.testing.assert_frame_equal(
-        X, df_datetime_transformed[["date_obj1" + feat for feat in feat_names_default]]
+        X,
+        df_datetime_transformed[["date_obj1" + feat for feat in feat_names_default]],
+        check_dtype=False,
     )
 
 
 def test_extract_features_from_different_timezones(
     df_datetime, df_datetime_transformed
 ):
     time_zones = [4, -1, 9, -7]
@@ -307,14 +318,15 @@
     X = transformer.fit_transform(tz_df)
 
     pd.testing.assert_frame_equal(
         X,
         df_datetime_transformed[["time_obj_hour"]].apply(
             lambda x: x.subtract(time_zones)
         ),
+        check_dtype=False,
     )
     exp_err_msg = (
         "ValueError: variable(s) time_obj "
         "could not be converted to datetime. Try setting utc=True"
     )
     with pytest.raises(ValueError) as errinfo:
         assert DatetimeFeatures(
@@ -352,15 +364,15 @@
     # fit attr
     assert transformer.variables_ == ["date_var"]
     assert transformer.features_to_extract_ == ["hour"]
     assert transformer.n_features_in_ == 1
     # transform
     X = transformer.transform(tz_df)
     df_expected = pd.DataFrame({"date_var_hour": [1, 2, 2, 2, 2, 3, 3]})
-    pd.testing.assert_frame_equal(X, df_expected)
+    pd.testing.assert_frame_equal(X, df_expected, check_dtype=False)
 
     # when utc is True
     transformer = DatetimeFeatures(features_to_extract=["hour"], utc=True).fit(tz_df)
 
     # init params
     assert transformer.variables is None
     assert transformer.utc is True
@@ -368,15 +380,15 @@
     # fit attr
     assert transformer.variables_ == ["date_var"]
     assert transformer.features_to_extract_ == ["hour"]
     assert transformer.n_features_in_ == 1
     # transform
     X = transformer.transform(tz_df)
     df_expected = pd.DataFrame({"date_var_hour": [5, 6, 6, 6, 6, 7, 7]})
-    pd.testing.assert_frame_equal(X, df_expected)
+    pd.testing.assert_frame_equal(X, df_expected, check_dtype=False)
 
 
 def test_extract_features_without_dropping_original_variables(
     df_datetime, df_datetime_transformed
 ):
     X = DatetimeFeatures(
         variables=["datetime_range", "date_obj2"],
@@ -395,14 +407,15 @@
                     var + "_" + feat
                     for var in ["datetime_range", "date_obj2"]
                     for feat in ["week", "quarter"]
                 ]
             ],
             axis=1,
         ),
+        check_dtype=False,
     )
 
 
 def test_extract_features_from_variables_containing_nans():
     X = DatetimeFeatures(
         features_to_extract=["year"], missing_values="ignore"
     ).fit_transform(dates_nan)
@@ -431,38 +444,39 @@
 def test_extract_features_with_different_datetime_parsing_options(df_datetime):
     X = DatetimeFeatures(
         features_to_extract=["day_of_month"], dayfirst=True
     ).fit_transform(df_datetime[["date_obj2"]])
     pd.testing.assert_frame_equal(
         X,
         pd.DataFrame({"date_obj2_day_of_month": [10, 31, 30, 17]}),
+        check_dtype=False,
     )
 
     X = DatetimeFeatures(features_to_extract=["year"], yearfirst=True).fit_transform(
         df_datetime[["date_obj2"]]
     )
     pd.testing.assert_frame_equal(
         X,
         pd.DataFrame({"date_obj2_year": [2010, 2009, 1995, 2004]}),
+        check_dtype=False,
     )
 
 
 def test_get_feature_names_out(df_datetime, df_datetime_transformed):
     # default features from all variables
     transformer = DatetimeFeatures()
     X = transformer.fit_transform(df_datetime)
     assert list(X.columns) == transformer.get_feature_names_out()
     assert list(X.columns) == transformer.get_feature_names_out(df_datetime.columns)
 
     with pytest.raises(ValueError):
         transformer.get_feature_names_out(input_features=vars_dt)
 
     with pytest.raises(ValueError):
-        transformer.get_feature_names_out(input_features=["date_obj1"])\
-
+        transformer.get_feature_names_out(input_features=["date_obj1"])
     # default features from 1 variable
     transformer = DatetimeFeatures(variables="date_obj1")
     X = transformer.fit_transform(df_datetime)
     assert list(X.columns) == transformer.get_feature_names_out()
     assert list(X.columns) == transformer.get_feature_names_out(df_datetime.columns)
 
     # all features
```

### Comparing `feature_engine-1.6.0/tests/test_datetime/test_datetime_subtraction.py` & `feature_engine-1.6.1/tests/test_datetime/test_datetime_subtraction.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_discretisation/test_arbitrary_discretiser.py` & `feature_engine-1.6.1/tests/test_discretisation/test_arbitrary_discretiser.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_discretisation/test_base_discretizer.py` & `feature_engine-1.6.1/tests/test_discretisation/test_base_discretizer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_discretisation/test_decision_tree_discretiser.py` & `feature_engine-1.6.1/tests/test_discretisation/test_decision_tree_discretiser.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_discretisation/test_equal_frequency_discretiser.py` & `feature_engine-1.6.1/tests/test_discretisation/test_equal_frequency_discretiser.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_discretisation/test_equal_width_discretiser.py` & `feature_engine-1.6.1/tests/test_discretisation/test_equal_width_discretiser.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_discretisation/test_geometric_width_discretiser.py` & `feature_engine-1.6.1/tests/test_discretisation/test_geometric_width_discretiser.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin.py` & `feature_engine-1.6.1/tests/test_encoding/test_base_encoders/test_categorical_init_mixin.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_base_encoders/test_categorical_init_mixin_na.py` & `feature_engine-1.6.1/tests/test_encoding/test_base_encoders/test_categorical_init_mixin_na.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_base_encoders/test_categorical_method_mixin.py` & `feature_engine-1.6.1/tests/test_encoding/test_base_encoders/test_categorical_method_mixin.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_check_estimator_encoders.py` & `feature_engine-1.6.1/tests/test_encoding/test_check_estimator_encoders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import pytest
-
 from numpy import nan
 from sklearn import clone
 from sklearn.exceptions import NotFittedError
+from sklearn.pipeline import Pipeline
 from sklearn.utils.estimator_checks import check_estimator
 
 from feature_engine.encoding import (
     CountFrequencyEncoder,
     DecisionTreeEncoder,
     MeanEncoder,
     OneHotEncoder,
@@ -46,16 +46,16 @@
 _estimators = [
     CountFrequencyEncoder(),
     DecisionTreeEncoder(regression=False),
     MeanEncoder(),
     OneHotEncoder(),
     OrdinalEncoder(),
     RareLabelEncoder(),
-    WoEEncoder(),
     StringSimilarityEncoder(missing_values="raise"),
+    WoEEncoder(),
 ]
 
 
 @pytest.mark.parametrize("estimator", _estimators)
 def test_check_estimator_from_feature_engine(estimator):
     return check_feature_engine_estimator(estimator)
 
@@ -70,14 +70,29 @@
         transformer.fit(X, y)
 
     # Test when fit is not called prior to transform.
     with pytest.raises(NotFittedError):
         transformer.transform(X)
 
 
+@pytest.mark.parametrize("transformer", _estimators)
+def test_transformers_in_pipeline_with_set_output_pandas(transformer):
+    X = pd.DataFrame(
+        {"feature_1": ["A", "A", "B", "B", "B"], "feature_2": ["A", "A", "B", "B", "B"]}
+    )
+    y = pd.Series([0, 1, 0, 1, 0])
+
+    pipe = Pipeline([("trs", transformer)]).set_output(transform="pandas")
+
+    Xtt = transformer.fit_transform(X, y)
+    Xtp = pipe.fit_transform(X, y)
+
+    pd.testing.assert_frame_equal(Xtt, Xtp)
+
+
 @pytest.mark.parametrize(
     # Key to all: - "non-standard" index that is not the usual
     # contiguous range starting a t 0
     "encoder, df_test, df_expected",
     [
         (
             DecisionTreeEncoder(),
```

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_count_frequency_encoder.py` & `feature_engine-1.6.1/tests/test_encoding/test_count_frequency_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import warnings
 
 import pandas as pd
 import pytest
 from numpy import nan
-
 from sklearn.exceptions import NotFittedError
 
 from feature_engine.encoding import CountFrequencyEncoder
 
 
 # init parameters
 @pytest.mark.parametrize("enc_method", ["arbitrary", False, 1])
```

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_decision_tree_encoder.py` & `feature_engine-1.6.1/tests/test_encoding/test_decision_tree_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_helper_functions.py` & `feature_engine-1.6.1/tests/test_encoding/test_helper_functions.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_mean_encoder.py` & `feature_engine-1.6.1/tests/test_encoding/test_mean_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pandas as pd
 import pytest
-
 from numpy import nan
 from sklearn.exceptions import NotFittedError
 
 from feature_engine.encoding import MeanEncoder
 
 
 # test init params
```

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_onehot_encoder.py` & `feature_engine-1.6.1/tests/test_encoding/test_onehot_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_ordinal_encoder.py` & `feature_engine-1.6.1/tests/test_encoding/test_ordinal_encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pandas as pd
 import pytest
-
 from numpy import nan
 from sklearn.exceptions import NotFittedError
 
 from feature_engine.encoding import OrdinalEncoder
 
 
 def test_ordered_encoding_1_variable(df_enc):
```

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_rare_label_encoder.py` & `feature_engine-1.6.1/tests/test_encoding/test_rare_label_encoder.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,14 +50,42 @@
     assert encoder.variables_ == ["var_A", "var_B", "var_C"]
     assert encoder.n_features_in_ == 3
     assert encoder.encoder_dict_ == frequenc_cat
     # test transform output
     pd.testing.assert_frame_equal(X, df)
 
 
+def test_when_varnames_are_numbers(df_enc_big):
+    input_df = df_enc_big.copy()
+    input_df.columns = [1, 2, 3]
+
+    encoder = RareLabelEncoder(
+        tol=0.06, n_categories=5, variables=None, replace_with="Rare"
+    )
+    X = encoder.fit_transform(input_df)
+
+    # expected output
+    df = {
+        1: ["A"] * 6 + ["B"] * 10 + ["C"] * 4 + ["D"] * 10 + ["Rare"] * 4 + ["G"] * 6,
+        2: ["A"] * 10 + ["B"] * 6 + ["C"] * 4 + ["D"] * 10 + ["Rare"] * 4 + ["G"] * 6,
+        3: ["A"] * 4 + ["B"] * 6 + ["C"] * 10 + ["D"] * 10 + ["Rare"] * 4 + ["G"] * 6,
+    }
+    df = pd.DataFrame(df)
+
+    frequenc_cat = {
+        1: ["B", "D", "A", "G", "C"],
+        2: ["A", "D", "B", "G", "C"],
+        3: ["C", "D", "B", "G", "A"],
+    }
+
+    assert encoder.variables_ == [1, 2, 3]
+    assert encoder.encoder_dict_ == frequenc_cat
+    pd.testing.assert_frame_equal(X, df)
+
+
 def test_correctly_ignores_nan_in_transform(df_enc_big):
     encoder = RareLabelEncoder(
         tol=0.06,
         n_categories=5,
         missing_values="ignore",
     )
     X = encoder.fit_transform(df_enc_big)
@@ -98,15 +126,15 @@
     df.loc[df["var_C"] == "G", "var_C"] = np.nan
 
     encoder = RareLabelEncoder(
         tol=0.06,
         n_categories=3,
         missing_values="ignore",
     )
-    X = encoder.fit_transform(df)
+    encoder.fit(df)
 
     # expected:
     frequenc_cat = {
         "var_A": ["B", "D", "A", "G", "C"],
         "var_B": ["A", "D", "B", "G", "C"],
         "var_C": ["C", "D", "B", "A"],
     }
@@ -130,14 +158,98 @@
         }
     )
 
     X = encoder.transform(t)
     pd.testing.assert_frame_equal(X, tt)
 
 
+def test_correctly_ignores_nan_in_fit_when_var_is_numerical(df_enc_big):
+
+    df = df_enc_big.copy()
+    df["var_C"] = [
+        1,
+        1,
+        1,
+        1,
+        2,
+        2,
+        2,
+        2,
+        2,
+        2,
+        3,
+        3,
+        3,
+        3,
+        3,
+        3,
+        3,
+        3,
+        3,
+        3,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        4,
+        5,
+        5,
+        6,
+        6,
+        np.nan,
+        np.nan,
+        np.nan,
+        np.nan,
+        np.nan,
+        np.nan,
+    ]
+
+    encoder = RareLabelEncoder(
+        tol=0.06,
+        n_categories=3,
+        missing_values="ignore",
+        ignore_format=True,
+    )
+    encoder.fit(df)
+
+    # expected:
+    frequenc_cat = {
+        "var_A": ["B", "D", "A", "G", "C"],
+        "var_B": ["A", "D", "B", "G", "C"],
+        "var_C": [3, 4, 2, 1],
+    }
+    assert encoder.encoder_dict_ == frequenc_cat
+
+    # input
+    t = pd.DataFrame(
+        {
+            "var_A": ["A", np.nan, "J", "G"],
+            "var_B": ["A", np.nan, "J", "G"],
+            "var_C": [3, np.nan, 9, 10],
+        }
+    )
+
+    # expected
+    tt = pd.DataFrame(
+        {
+            "var_A": ["A", np.nan, "Rare", "G"],
+            "var_B": ["A", np.nan, "Rare", "G"],
+            "var_C": [3.0, np.nan, "Rare", "Rare"],
+        }
+    )
+
+    X = encoder.transform(t)
+    pd.testing.assert_frame_equal(X, tt, check_dtype=False)
+
+
 def test_user_provides_grouping_label_name_and_variable_list(df_enc_big):
     # test case 2: user provides alternative grouping value and variable list
     encoder = RareLabelEncoder(
         tol=0.15, n_categories=5, variables=["var_A", "var_B"], replace_with="Other"
     )
     X = encoder.fit_transform(df_enc_big)
 
@@ -312,19 +424,91 @@
         + ["B"] * 6
         + ["C"] * 10
         + ["D"] * 10
         + ["Rare"] * 4
         + ["G"] * 6,
     }
     df = pd.DataFrame(df)
+    df["var_B"] = pd.Categorical(df["var_B"])
 
     # test fit attr
     assert encoder.variables_ == ["var_A", "var_B", "var_C"]
     assert encoder.n_features_in_ == 3
     # test transform output
-    pd.testing.assert_frame_equal(X, df)
+    pd.testing.assert_frame_equal(X, df, check_categorical=False)
+
+
+def test_variables_cast_as_category_with_na_in_transform(df_enc_big):
+    encoder = RareLabelEncoder(
+        tol=0.06,
+        n_categories=5,
+        variables=None,
+        replace_with="Rare",
+        missing_values="ignore",
+    )
+
+    df_enc_big = df_enc_big.copy()
+    df_enc_big["var_B"] = df_enc_big["var_B"].astype("category")
+    encoder.fit(df_enc_big)
+
+    # input
+    t = pd.DataFrame(
+        {
+            "var_A": ["A", np.nan, "J", "G"],
+            "var_B": ["A", np.nan, "J", "G"],
+            "var_C": ["A", np.nan, "J", "G"],
+        }
+    )
+    t["var_B"] = pd.Categorical(t["var_B"])
+
+    # expected
+    tt = pd.DataFrame(
+        {
+            "var_A": ["A", np.nan, "Rare", "G"],
+            "var_B": ["A", np.nan, "Rare", "G"],
+            "var_C": ["A", np.nan, "Rare", "G"],
+        }
+    )
+    tt["var_B"] = pd.Categorical(tt["var_B"])
+    pd.testing.assert_frame_equal(encoder.transform(t), tt, check_categorical=False)
+
+
+def test_variables_cast_as_category_with_na_in_fit(df_enc_big):
+
+    df = df_enc_big.copy()
+    df.loc[df["var_C"] == "G", "var_C"] = np.nan
+    df["var_C"] = df["var_C"].astype("category")
+
+    encoder = RareLabelEncoder(
+        tol=0.06,
+        n_categories=3,
+        missing_values="ignore",
+    )
+    encoder.fit(df)
+
+    # input
+    t = pd.DataFrame(
+        {
+            "var_A": ["A", np.nan, "J", "G"],
+            "var_B": ["A", np.nan, "J", "G"],
+            "var_C": ["C", np.nan, "J", "G"],
+        }
+    )
+    t["var_C"] = pd.Categorical(t["var_C"])
+
+    # expected
+    tt = pd.DataFrame(
+        {
+            "var_A": ["A", np.nan, "Rare", "G"],
+            "var_B": ["A", np.nan, "Rare", "G"],
+            "var_C": ["C", np.nan, "Rare", "Rare"],
+        }
+    )
+    tt["var_C"] = pd.Categorical(tt["var_C"])
+
+    pd.testing.assert_frame_equal(encoder.transform(t), tt, check_categorical=False)
 
 
 def test_inverse_transform_raises_not_implemented_error(df_enc_big):
     enc = RareLabelEncoder().fit(df_enc_big)
     with pytest.raises(NotImplementedError):
         enc.inverse_transform(df_enc_big)
```

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_similarity_encoder.py` & `feature_engine-1.6.1/tests/test_encoding/test_similarity_encoder.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_encoding/test_woe/test_woe_encoder.py` & `feature_engine-1.6.1/tests/test_encoding/test_woe/test_woe_encoder.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import math
+
 import numpy as np
 import pandas as pd
 import pytest
-
 from sklearn.exceptions import NotFittedError
 
 from feature_engine.encoding import WoEEncoder
 
 VAR_A = [
     0.15415067982725836,
     0.15415067982725836,
@@ -172,43 +173,154 @@
             "var_B": ["A"] * 10 + ["B"] * 6 + ["C"] * 4,
             "target": [1, 1, 2, 2, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0],
         }
         df = pd.DataFrame(df)
         encoder.fit(df[["var_A", "var_B"]], df["target"])
 
 
-def test_error_if_denominator_probability_is_zero():
-    # test case 5: when the denominator probability is zero
+def test_error_if_denominator_probability_is_zero_1_var():
+    df = {
+        "var_A": ["A"] * 6 + ["B"] * 10 + ["C"] * 4,
+        "var_B": ["A"] * 10 + ["B"] * 6 + ["C"] * 4,
+        "target": [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0],
+    }
+    df = pd.DataFrame(df)
     encoder = WoEEncoder(variables=None)
-    with pytest.raises(ValueError):
-        df = {
-            "var_A": ["A"] * 6 + ["B"] * 10 + ["C"] * 4,
-            "var_B": ["A"] * 10 + ["B"] * 6 + ["C"] * 4,
-            "target": [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0],
-        }
-        df = pd.DataFrame(df)
+
+    with pytest.raises(ValueError) as record:
         encoder.fit(df[["var_A", "var_B"]], df["target"])
 
-    # # # test case 6: when the numerator probability is zero, woe
-    # # with pytest.raises(ValueError):
-    # #     df = {'var_A': ['A'] * 6 + ['B'] * 10 + ['C'] * 4,
-    # #           'var_B': ['A'] * 10 + ['B'] * 6 + ['C'] * 4,
-    # #           'target': [0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1,
-    # 1, 0, 0]}
-    # #     df = pd.DataFrame(df)
-    # #     encoder.fit(df[['var_A', 'var_B']], df['target'])
-    #
-    # # # test case 7: when the denominator probability is zero, woe
-    # # with pytest.raises(ValueError):
-    # #     df = {'var_A': ['A'] * 6 + ['B'] * 10 + ['C'] * 4,
-    # #           'var_B': ['A'] * 10 + ['B'] * 6 + ['C'] * 4,
-    # #           'target': [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1,
-    # 0, 0]}
-    # #     df = pd.DataFrame(df)
-    # #     encoder.fit(df[['var_A', 'var_B']], df['target'])
+    msg = (
+        "During the WoE calculation, some of the categories in the "
+        "following features contained 0 in the denominator or numerator, "
+        "and hence the WoE can't be calculated: var_A."
+    )
+    assert str(record.value) == msg
+
+    df = {
+        "var_A": ["A"] * 10 + ["B"] * 6 + ["C"] * 4,
+        "var_B": ["A"] * 6 + ["B"] * 10 + ["C"] * 4,
+        "target": [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0],
+    }
+    df = pd.DataFrame(df)
+    encoder = WoEEncoder(variables=None)
+
+    with pytest.raises(ValueError) as record:
+        encoder.fit(df[["var_A", "var_B"]], df["target"])
+
+    msg = (
+        "During the WoE calculation, some of the categories in the "
+        "following features contained 0 in the denominator or numerator, "
+        "and hence the WoE can't be calculated: var_B."
+    )
+    assert str(record.value) == msg
+
+
+def test_error_if_denominator_probability_is_zero_2_vars():
+    df = {
+        "var_A": ["A"] * 6 + ["B"] * 10 + ["C"] * 4,
+        "var_B": ["A"] * 10 + ["B"] * 6 + ["C"] * 4,
+        "var_C": ["A"] * 6 + ["B"] * 10 + ["C"] * 4,
+        "target": [1, 1, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0],
+    }
+    df = pd.DataFrame(df)
+    encoder = WoEEncoder(variables=None)
+
+    with pytest.raises(ValueError) as record:
+        encoder.fit(df, df["target"])
+
+    msg = (
+        "During the WoE calculation, some of the categories in the "
+        "following features contained 0 in the denominator or numerator, "
+        "and hence the WoE can't be calculated: var_A, var_C."
+    )
+    assert str(record.value) == msg
+
+
+def test_error_if_numerator_probability_is_zero():
+    df = {
+        "var_A": ["A"] * 6 + ["B"] * 10 + ["C"] * 4,
+        "var_B": ["A"] * 10 + ["B"] * 6 + ["C"] * 4,
+        "var_C": ["A"] * 6 + ["B"] * 10 + ["C"] * 4,
+        "target": [0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0],
+    }
+    df = pd.DataFrame(df)
+    encoder = WoEEncoder(variables=None)
+
+    with pytest.raises(ValueError) as record:
+        encoder.fit(df, df["target"])
+
+    msg = (
+        "During the WoE calculation, some of the categories in the "
+        "following features contained 0 in the denominator or numerator, "
+        "and hence the WoE can't be calculated: var_A, var_C."
+    )
+    assert str(record.value) == msg
+
+    with pytest.raises(ValueError) as record:
+        encoder.fit(df[["var_A", "var_B"]], df["target"])
+
+    msg = (
+        "During the WoE calculation, some of the categories in the "
+        "following features contained 0 in the denominator or numerator, "
+        "and hence the WoE can't be calculated: var_A."
+    )
+    assert str(record.value) == msg
+
+
+def test_fill_value():
+    df = {
+        "var_A": ["A"] * 9 + ["B"] * 6 + ["C"] * 3 + ["D"] * 2,
+        "var_B": ["A"] * 10 + ["B"] * 6 + ["C"] * 4,
+        "target": [1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 1, 1, 1, 0, 0],
+    }
+    df = pd.DataFrame(df)
+    encoder = WoEEncoder(variables=None, fill_value=1)
+    encoder.fit(df, df["target"])
+    woe_exp_a = {
+        "A": -0.6337237600891445,
+        "B": -0.07410797215372196,
+        "C": -0.8472978603872037,
+        "D": 1.8718021769015913,
+    }
+    woe_exp_b = {
+        "A": -0.7672551527136673,
+        "B": 0.6190392084062234,
+        "C": 0.6190392084062234,
+    }
+    woe_exp = {"var_A": woe_exp_a, "var_B": woe_exp_b}
+
+    for var in ["var_A", "var_B"]:
+        for k, i in woe_exp[var].items():
+            assert math.isclose(encoder.encoder_dict_[var][k], woe_exp[var][k])
+
+    encoder = WoEEncoder(variables=None, fill_value=10)
+    encoder.fit(df, df["target"])
+    woe_exp_a = {
+        "A": -0.6337237600891445,
+        "B": -0.07410797215372196,
+        "C": -3.1498829533812494,
+        "D": 4.174387269895637,
+    }
+    woe_exp = {"var_A": woe_exp_a, "var_B": woe_exp_b}
+    for var in ["var_A", "var_B"]:
+        for k, i in woe_exp[var].items():
+            assert math.isclose(encoder.encoder_dict_[var][k], woe_exp[var][k])
+
+
+@pytest.mark.parametrize("fill_value", ["hola", [10]])
+def test_error_if_fill_value_not_allowed(fill_value):
+    with pytest.raises(ValueError):
+        WoEEncoder(fill_value=fill_value)
+
+
+@pytest.mark.parametrize("fill_value", [0, 1, 10, 0.5, 0.002, None])
+def test_assigns_fill_value_at_init(fill_value):
+    encoder = WoEEncoder(fill_value=fill_value)
+    assert encoder.fill_value == fill_value
 
 
 def test_error_if_contains_na_in_fit(df_enc_na):
     # test case 9: when dataset contains na, fit method
     encoder = WoEEncoder(variables=None)
     with pytest.raises(ValueError) as record:
         encoder.fit(df_enc_na[["var_A", "var_B"]], df_enc_na["target"])
```

### Comparing `feature_engine-1.6.0/tests/test_imputation/test_arbitrary_number_imputer.py` & `feature_engine-1.6.1/tests/test_imputation/test_arbitrary_number_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_imputation/test_categorical_imputer.py` & `feature_engine-1.6.1/tests/test_imputation/test_categorical_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_imputation/test_check_estimator_imputers.py` & `feature_engine-1.6.1/tests/test_outliers/test_check_estimator_outliers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,51 @@
+import pandas as pd
 import pytest
+from sklearn.pipeline import Pipeline
 from sklearn.utils.estimator_checks import check_estimator
 
-from feature_engine.imputation import (
-    AddMissingIndicator,
-    ArbitraryNumberImputer,
-    CategoricalImputer,
-    DropMissingData,
-    EndTailImputer,
-    MeanMedianImputer,
-    RandomSampleImputer,
-)
+from feature_engine.outliers import ArbitraryOutlierCapper, OutlierTrimmer, Winsorizer
 from tests.estimator_checks.estimator_checks import check_feature_engine_estimator
 
 _estimators = [
-    MeanMedianImputer(),
-    ArbitraryNumberImputer(),
-    CategoricalImputer(fill_value=0, ignore_format=True),
-    EndTailImputer(),
-    AddMissingIndicator(),
-    RandomSampleImputer(),
-    DropMissingData(),
+    ArbitraryOutlierCapper(max_capping_dict={"x0": 10}),
+    OutlierTrimmer(),
+    Winsorizer(),
 ]
 
 
 @pytest.mark.parametrize("estimator", _estimators)
 def test_check_estimator_from_sklearn(estimator):
     return check_estimator(estimator)
 
 
 @pytest.mark.parametrize("estimator", _estimators)
 def test_check_estimator_from_feature_engine(estimator):
-    if estimator.__class__.__name__ == "CategoricalImputer":
-        estimator.set_params(ignore_format=False)
-    if estimator.__class__.__name__ in ["DropMissingData", "AddMissingIndicator"]:
-        estimator.set_params(missing_only=False)
+    if estimator.__class__.__name__ == "ArbitraryOutlierCapper":
+        estimator.set_params(max_capping_dict={"var_1": 10})
     return check_feature_engine_estimator(estimator)
+
+
+@pytest.mark.parametrize("transformer", _estimators)
+def test_transformers_in_pipeline_with_set_output_pandas(transformer):
+    if transformer.__class__.__name__ == "ArbitraryOutlierCapper":
+        transformer.set_params(max_capping_dict={"feature_1": 10})
+
+    X = pd.DataFrame({"feature_1": [1, 2, 3, 4, 5], "feature_2": [6, 7, 8, 9, 10]})
+    y = pd.Series([0, 1, 0, 1, 0])
+
+    pipe = Pipeline([("trs", transformer)]).set_output(transform="pandas")
+
+    Xtt = transformer.fit_transform(X)
+    Xtp = pipe.fit_transform(X, y)
+
+    pd.testing.assert_frame_equal(Xtt, Xtp)
+
+    if transformer.__class__.__name__ == "Winsorizer":
+        transformer.set_params(add_indicators=True)
+
+        pipe = Pipeline([("trs", transformer)]).set_output(transform="pandas")
+
+        Xtt = transformer.fit_transform(X)
+        Xtp = pipe.fit_transform(X, y)
+
+        pd.testing.assert_frame_equal(Xtt, Xtp)
```

### Comparing `feature_engine-1.6.0/tests/test_imputation/test_drop_missing_data.py` & `feature_engine-1.6.1/tests/test_imputation/test_drop_missing_data.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_imputation/test_end_tail_imputer.py` & `feature_engine-1.6.1/tests/test_imputation/test_end_tail_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_imputation/test_mean_mdian_imputer.py` & `feature_engine-1.6.1/tests/test_imputation/test_mean_mdian_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_imputation/test_missing_indicator.py` & `feature_engine-1.6.1/tests/test_imputation/test_missing_indicator.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_imputation/test_random_sample_imputer.py` & `feature_engine-1.6.1/tests/test_imputation/test_random_sample_imputer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_outliers/test_arbitrary_capper.py` & `feature_engine-1.6.1/tests/test_outliers/test_arbitrary_capper.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_outliers/test_outlier_trimmer.py` & `feature_engine-1.6.1/tests/test_outliers/test_outlier_trimmer.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,12 @@
 
 def test_quantile_fold_default_value():
     # test case 1: Test quantiles, with fold default = 0.05
     transformer = OutlierTrimmer(capping_method="quantiles")
     assert transformer.fold == 0.05
 
 
-@pytest.mark.parametrize(
-     "strings", ["gaussian", "iqr", "mad"]
- )
+@pytest.mark.parametrize("strings", ["gaussian", "iqr", "mad"])
 def test_other_fold_default_value(strings):
     # test case 2: Test gaussian, iqr, mad, with fold default = 3
     transformer = OutlierTrimmer(capping_method=strings)
     assert transformer.fold == 3
```

### Comparing `feature_engine-1.6.0/tests/test_outliers/test_winsorizer.py` & `feature_engine-1.6.1/tests/test_outliers/test_winsorizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+
 import numpy as np
 import pandas as pd
 import pytest
 
 from feature_engine.outliers import Winsorizer
 
 
@@ -16,18 +17,15 @@
     df_transf["var"] = df_transf["var"].clip(upper=0.1067690260251065)
 
     # test init params
     assert transformer.capping_method == "gaussian"
     assert transformer.tail == "right"
     assert transformer.fold == 1
     # test fit attr
-    assert math.isclose(
-        transformer.right_tail_caps_["var"],
-        0.1067690260251065
-    )
+    assert math.isclose(transformer.right_tail_caps_["var"], 0.1067690260251065)
     assert transformer.left_tail_caps_ == {}
     assert transformer.n_features_in_ == 1
     # test transform outputs
     pd.testing.assert_frame_equal(X, df_transf)
     assert math.isclose(X["var"].max(), 0.10676902602510658)
     assert math.isclose(df_transf["var"].max(), 0.1067690260251065)
 
@@ -35,27 +33,19 @@
 def test_gaussian_capping_both_tails_with_fold_2(df_normal_dist):
     # test case 2: mean and std, both tails, different fold value
     transformer = Winsorizer(capping_method="gaussian", tail="both", fold=2)
     X = transformer.fit_transform(df_normal_dist)
 
     # expected output
     df_transf = df_normal_dist.copy()
-    df_transf["var"] = df_transf["var"].clip(
-        -0.1955956473898675, 0.2075572504967645
-    )
+    df_transf["var"] = df_transf["var"].clip(-0.1955956473898675, 0.2075572504967645)
 
     # test fit params
-    assert math.isclose(
-        transformer.right_tail_caps_["var"],
-        0.2075572504967645
-    )
-    assert math.isclose(
-        transformer.left_tail_caps_["var"],
-        -0.1955956473898675
-    )
+    assert math.isclose(transformer.right_tail_caps_["var"], 0.2075572504967645)
+    assert math.isclose(transformer.left_tail_caps_["var"], -0.1955956473898675)
     # test transform output
     pd.testing.assert_frame_equal(X, df_transf)
     assert math.isclose(X["var"].max(), 0.2075572504967645)
     assert math.isclose(X["var"].min(), -0.1955956473898675)
     assert math.isclose(df_transf["var"].max(), 0.2075572504967645)
     assert math.isclose(df_transf["var"].min(), -0.1955956473898675)
 
@@ -63,27 +53,19 @@
 def test_iqr_capping_both_tails_with_fold_1(df_normal_dist):
     # test case 3: IQR, both tails, fold 1
     transformer = Winsorizer(capping_method="iqr", tail="both", fold=1)
     X = transformer.fit_transform(df_normal_dist)
 
     # expected output
     df_transf = df_normal_dist.copy()
-    df_transf["var"] = df_transf["var"].clip(
-        -0.20247907173293223, 0.21180113880445128
-    )
+    df_transf["var"] = df_transf["var"].clip(-0.20247907173293223, 0.21180113880445128)
 
     # test fit params
-    assert math.isclose(
-        transformer.right_tail_caps_["var"],
-        0.21180113880445128
-    )
-    assert math.isclose(
-        transformer.left_tail_caps_["var"],
-        -0.20247907173293223
-    )
+    assert math.isclose(transformer.right_tail_caps_["var"], 0.21180113880445128)
+    assert math.isclose(transformer.left_tail_caps_["var"], -0.20247907173293223)
     # test transform output
     pd.testing.assert_frame_equal(X, df_transf)
     assert math.isclose(X["var"].max(), 0.21180113880445128)
     assert math.isclose(X["var"].min(), -0.20247907173293223)
     assert math.isclose(df_transf["var"].max(), 0.21180113880445128)
     assert math.isclose(df_transf["var"].min(), -0.20247907173293223)
 
@@ -95,18 +77,15 @@
 
     # expected output
     df_transf = df_normal_dist.copy()
     df_transf["var"] = df_transf["var"].clip(lower=-0.17486039103044)
 
     # test fit params
     assert transformer.right_tail_caps_ == {}
-    assert math.isclose(
-        transformer.left_tail_caps_["var"],
-        -0.17486039103044
-    )
+    assert math.isclose(transformer.left_tail_caps_["var"], -0.17486039103044)
     # test transform output
     pd.testing.assert_frame_equal(X, df_transf)
     assert math.isclose(X["var"].min(), -0.17486039103044)
     assert math.isclose(df_transf["var"].min(), -0.17486039103044)
 
 
 def test_quantile_capping_both_tails_with_fold_10_percent(df_normal_dist):
@@ -115,22 +94,16 @@
     X = transformer.fit_transform(df_normal_dist)
 
     # expected output
     df_transf = df_normal_dist.copy()
     df_transf["var"] = df_transf["var"].clip(-0.12366227743232801, 0.14712481122898166)
 
     # test fit params
-    assert math.isclose(
-        transformer.right_tail_caps_["var"],
-        0.14712481122898166
-    )
-    assert math.isclose(
-        transformer.left_tail_caps_["var"],
-        -0.12366227743232801
-    )
+    assert math.isclose(transformer.right_tail_caps_["var"], 0.14712481122898166)
+    assert math.isclose(transformer.left_tail_caps_["var"], -0.12366227743232801)
     # test transform output
     pd.testing.assert_frame_equal(X, df_transf)
     assert math.isclose(X["var"].max(), 0.14712481122898166)
     assert math.isclose(X["var"].min(), -0.12366227743232801)
     assert math.isclose(df_transf["var"].max(), 0.14712481122898166)
     assert math.isclose(df_transf["var"].min(), -0.12366227743232801)
 
@@ -141,34 +114,29 @@
     X = transformer.fit_transform(df_normal_dist)
 
     # expected output
     df_transf = df_normal_dist.copy()
     df_transf["var"] = df_transf["var"].clip(upper=0.11823196128033647)
 
     # test fit params
-    assert math.isclose(
-        transformer.right_tail_caps_["var"],
-        0.11823196128033647
-    )
+    assert math.isclose(transformer.right_tail_caps_["var"], 0.11823196128033647)
     assert transformer.left_tail_caps_ == {}
     # test transform output
     pd.testing.assert_frame_equal(X, df_transf)
     assert math.isclose(X["var"].max(), 0.11823196128033647)
     assert math.isclose(df_transf["var"].max(), 0.11823196128033647)
 
 
 def test_quantile_fold_default_value():
     # test case 1: Test quantiles, with fold default = 0.05
     transformer = Winsorizer(capping_method="quantiles")
     assert transformer.fold == 0.05
 
 
-@pytest.mark.parametrize(
-     "strings", ["gaussian", "iqr", "mad"]
- )
+@pytest.mark.parametrize("strings", ["gaussian", "iqr", "mad"])
 def test_other_fold_default_value(strings):
     # test case 2: Test gaussian, iqr, mad, with fold default = 3
     transformer = Winsorizer(capping_method=strings)
     assert transformer.fold == 3
 
 
 def test_mad_capping_right_tail_with_fold_1(df_normal_dist):
@@ -181,18 +149,15 @@
     df_transf["var"] = df_transf["var"].clip(upper=0.10995521088494983)
 
     # test init params
     assert transformer.capping_method == "mad"
     assert transformer.tail == "right"
     assert transformer.fold == 1
     # test fit attr
-    assert math.isclose(
-        transformer.right_tail_caps_["var"],
-        0.10995521088494983
-    )
+    assert math.isclose(transformer.right_tail_caps_["var"], 0.10995521088494983)
     assert transformer.left_tail_caps_ == {}
     assert transformer.n_features_in_ == 1
     # test transform outputs
     pd.testing.assert_frame_equal(X, df_transf)
     assert math.isclose(X["var"].max(), 0.10995521088494983)
     assert math.isclose(df_transf["var"].max(), 0.10995521088494983)
 
@@ -203,22 +168,16 @@
     X = transformer.fit_transform(df_normal_dist)
 
     # expected output
     df_transf = df_normal_dist.copy()
     df_transf["var"] = df_transf["var"].clip(-0.1916815859385002, 0.21050080982609987)
 
     # test fit params
-    assert math.isclose(
-        transformer.right_tail_caps_["var"],
-        0.21050080982609987
-    )
-    assert math.isclose(
-        transformer.left_tail_caps_["var"],
-        -0.1916815859385002
-    )
+    assert math.isclose(transformer.right_tail_caps_["var"], 0.21050080982609987)
+    assert math.isclose(transformer.left_tail_caps_["var"], -0.1916815859385002)
     # test transform output
     pd.testing.assert_frame_equal(X, df_transf)
     assert math.isclose(X["var"].max(), 0.21050080982609987)
     assert math.isclose(X["var"].min(), -0.1916815859385002)
     assert math.isclose(df_transf["var"].max(), 0.21050080982609987)
     assert math.isclose(df_transf["var"].min(), -0.1916815859385002)
 
@@ -315,22 +274,16 @@
 
     # expected output
     df_transf = df_na.copy()
     df_transf["Age"] = df_transf["Age"].clip(upper=38.04494616731882)
     df_transf["Marks"] = df_transf["Marks"].clip(upper=0.8784116651786605)
 
     # test fit params
-    assert math.isclose(
-        transformer.right_tail_caps_["Age"],
-        38.04494616731882
-    )
-    assert math.isclose(
-        transformer.right_tail_caps_["Marks"],
-        0.8784116651786605
-    )
+    assert math.isclose(transformer.right_tail_caps_["Age"], 38.04494616731882)
+    assert math.isclose(transformer.right_tail_caps_["Marks"], 0.8784116651786605)
     assert transformer.left_tail_caps_ == {}
     assert transformer.n_features_in_ == 6
     # test transform output
     pd.testing.assert_frame_equal(X, df_transf)
     assert math.isclose(X["Age"].max(), 38.04494616731882)
     assert math.isclose(X["Age"].max(), 38.04494616731882)
     assert math.isclose(X["Marks"].max(), 0.8784116651786605)
```

### Comparing `feature_engine-1.6.0/tests/test_prediction/conftest.py` & `feature_engine-1.6.1/tests/test_prediction/conftest.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_prediction/test_check_estimator_prediction.py` & `feature_engine-1.6.1/tests/test_prediction/test_check_estimator_prediction.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_prediction/test_target_mean_classifier.py` & `feature_engine-1.6.1/tests/test_prediction/test_target_mean_classifier.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_prediction/test_target_mean_regressor.py` & `feature_engine-1.6.1/tests/test_prediction/test_target_mean_regressor.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_preprocessing/test_check_estimator_preprocessing.py` & `feature_engine-1.6.1/tests/test_preprocessing/test_check_estimator_preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import pandas as pd
 import pytest
-
 from numpy import nan
 from sklearn import clone
 from sklearn.exceptions import NotFittedError
+from sklearn.pipeline import Pipeline
 from sklearn.utils.estimator_checks import check_estimator
 
 from feature_engine.preprocessing import MatchCategories, MatchVariables
 from tests.estimator_checks.estimator_checks import (
     check_feature_engine_estimator,
     test_df,
 )
+
 _estimators = [MatchCategories(ignore_format=True), MatchVariables()]
 
 
 @pytest.mark.parametrize("estimator", _estimators)
 def test_check_estimator_from_sklearn(estimator):
     return check_estimator(estimator)
 
@@ -22,16 +24,29 @@
 def test_check_estimator_from_feature_engine(estimator):
     return check_feature_engine_estimator(estimator)
 
 
 @pytest.mark.parametrize("estimator", _estimators)
 def test_raises_non_fitted_error_when_error_during_fit(estimator):
     X, y = test_df(categorical=True)
-    X.loc[len(X)-1] = nan
+    X.loc[len(X) - 1] = nan
     transformer = clone(estimator)
 
     with pytest.raises(ValueError):
         transformer.fit(X, y)
 
     # Test when fit is not called prior to transform.
     with pytest.raises(NotFittedError):
         transformer.transform(X)
+
+
+@pytest.mark.parametrize("transformer", _estimators)
+def test_transformers_in_pipeline_with_set_output_pandas(transformer):
+    X = pd.DataFrame({"feature_1": [1, 2, 3, 4, 5], "feature_2": [6, 7, 8, 9, 10]})
+    y = pd.Series([0, 1, 0, 1, 0])
+
+    pipe = Pipeline([("trs", transformer)]).set_output(transform="pandas")
+
+    Xtt = transformer.fit_transform(X)
+    Xtp = pipe.fit_transform(X, y)
+
+    pd.testing.assert_frame_equal(Xtt, Xtp)
```

### Comparing `feature_engine-1.6.0/tests/test_preprocessing/test_match_categories.py` & `feature_engine-1.6.1/tests/test_preprocessing/test_match_categories.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_preprocessing/test_match_columns.py` & `feature_engine-1.6.1/tests/test_preprocessing/test_match_columns.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/conftest.py` & `feature_engine-1.6.1/tests/test_selection/conftest.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/test_base_selector.py` & `feature_engine-1.6.1/tests/test_selection/test_base_selector.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/test_check_estimator_selectors.py` & `feature_engine-1.6.1/tests/test_selection/test_check_estimator_selectors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import pandas as pd
 import pytest
 from sklearn.linear_model import LogisticRegression
+from sklearn.pipeline import Pipeline
 from sklearn.utils.estimator_checks import check_estimator
 
 from feature_engine.selection import (
     DropConstantFeatures,
     DropCorrelatedFeatures,
     DropDuplicateFeatures,
     DropFeatures,
@@ -101,7 +103,29 @@
 
 @pytest.mark.parametrize("estimator", _model_based_estimators)
 def test_raises_error_when_no_estimator_passed(estimator):
     # these selectors need an estimator as an input param
     # test error otherwise.
     with pytest.raises(TypeError):
         estimator()
+
+
+@pytest.mark.parametrize("transformer", _estimators)
+def test_transformers_in_pipeline_with_set_output_pandas(transformer):
+    if transformer.__class__.__name__ == "DropFeatures":
+        transformer.set_params(features_to_drop=["feature_1"])
+
+    if transformer.__class__.__name__ == "ProbeFeatureSelection":
+        transformer.set_params(cv=2)
+
+    if transformer.__class__.__name__ == "DropHighPSIFeatures":
+        transformer.set_params(bins=2)
+
+    X = pd.DataFrame({"feature_1": [1, 2, 3, 4, 5], "feature_2": [6, 7, 8, 9, 10]})
+    y = pd.Series([0, 1, 0, 1, 0])
+
+    pipe = Pipeline([("trs", transformer)]).set_output(transform="pandas")
+
+    Xtt = transformer.fit_transform(X, y)
+    Xtp = pipe.fit_transform(X, y)
+
+    pd.testing.assert_frame_equal(Xtt, Xtp)
```

### Comparing `feature_engine-1.6.0/tests/test_selection/test_drop_constant_features.py` & `feature_engine-1.6.1/tests/test_selection/test_drop_constant_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/test_drop_correlated_features.py` & `feature_engine-1.6.1/tests/test_selection/test_drop_correlated_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/test_drop_duplicate_features.py` & `feature_engine-1.6.1/tests/test_selection/test_drop_duplicate_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/test_drop_features.py` & `feature_engine-1.6.1/tests/test_selection/test_drop_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     assert X.shape == (4, 4)
     assert type(X) == pd.DataFrame
     pd.testing.assert_frame_equal(X, df)
 
 
 def test_drop_1_variables_str_input(df_vartypes):
     """check that the internal variable features_to_drop has been
-     correctly cast from :str: to list of :str: internally"""
+    correctly cast from :str: to list of :str: internally"""
 
     transformer = DropFeatures(features_to_drop="Marks")
     X = transformer.fit_transform(df_vartypes)
 
     # expected result
     df = pd.DataFrame(
         {
```

### Comparing `feature_engine-1.6.0/tests/test_selection/test_drop_high_psi_features.py` & `feature_engine-1.6.1/tests/test_selection/test_drop_high_psi_features.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from datetime import date
-
 import math
+from datetime import date, datetime
+
 import numpy as np
 import pandas as pd
 import pytest
 from sklearn.datasets import make_classification
 
 from feature_engine.selection import DropHighPSIFeatures
 
@@ -22,150 +22,185 @@
         random_state=1,
     )
 
     # transform array into pandas df
     colnames = ["var_" + str(i) for i in range(6)]
     X = pd.DataFrame(X, columns=colnames)
 
+    # Add a categorical column that does not drift
+    X["cat_1"] = ["A", "B"] * int(X.shape[0] / 2)
+
     # Add drifted features that will be dropped during transformation.
     X["drift_1"] = [number for number in range(X.shape[0])]
     X["drift_2"] = [number / 2 for number in range(X.shape[0])]
+    X["drift_cat_1"] = ["A" for _ in range(int(X.shape[0] / 2))] + [
+        "B" for _ in range(int(X.shape[0] / 2))
+    ]
+    X["drift_cat_1"] = X["drift_cat_1"].astype("category")
 
     return X
 
 
 @pytest.fixture(scope="module")
 def df_mixed_types():
     df = pd.DataFrame(
         {
             "A": [it for it in range(0, 20)],
             "B": [1, 2, 2, 1] * 5,
             "C": ["A", "B", "D", "D"] * 5,
-            "time": [date(2019, 1, it + 1) for it in range(20)],
+            "time": [datetime(2019, 1, it + 1) for it in range(20)],
         }
     )
 
     return df
 
 
+EXPECTED_PSI_NUM = {
+    "var_0": 0.043828484052281,
+    "var_1": 0.040929870747665395,
+    "var_2": 0.04330418495156895,
+    "var_3": 0.03773286532548153,
+    "var_4": 0.05047388515663041,
+    "var_5": 0.014717735595712466,
+    "drift_1": 8.283089355027482,
+    "drift_2": 8.283089355027482,
+}
+
+EXPECTED_PSI_ALL = {
+    "var_0": 0.043828484052281,
+    "var_1": 0.040929870747665395,
+    "var_2": 0.04330418495156895,
+    "var_3": 0.03773286532548153,
+    "var_4": 0.05047388515663041,
+    "var_5": 0.014717735595712466,
+    "drift_1": 8.283089355027482,
+    "drift_2": 8.283089355027482,
+    "cat_1": 0.0,
+    "drift_cat_1": 18.41883867587797,
+}
+
+EXPECTED_PSI_NUM_FEW = {
+    "var_2": 0.04330418495156895,
+    "var_3": 0.03773286532548153,
+    "drift_1": 8.283089355027482,
+    "drift_2": 8.283089355027482,
+}
+
+EXPECTED_PSI_MIXED = {
+    "var_0": 0.043828484052281,
+    "drift_1": 8.283089355027482,
+    "drift_cat_1": 18.41883867587797,
+}
+
+EXPECTED_PSI_CAT_FEW = {
+    "cat_1": 0.0,
+    "drift_cat_1": 18.41883867587797,
+}
+
+EXPECTED_PSI_STRING = {"var_0": 0.043828484052281}
+
+_input_output = [
+    (None, EXPECTED_PSI_NUM),
+    ("all", EXPECTED_PSI_ALL),
+    (["var_2", "var_3", "drift_1", "drift_2"], EXPECTED_PSI_NUM_FEW),
+    (["cat_1", "drift_cat_1"], EXPECTED_PSI_CAT_FEW),
+    (["var_0", "drift_1", "drift_cat_1"], EXPECTED_PSI_MIXED),
+    ("var_0", EXPECTED_PSI_STRING),
+]
+
+
 # ====  test  main functionality of the class ====
-def test_fit_attributes(df):
+@pytest.mark.parametrize("variables, expected_psi", _input_output)
+def test_fit_attributes(variables, expected_psi, df):
     """Check the value of the fit attributes.
-
     The expected PSI values used in the assertion were determined using
     the Probatus package.
     ```
     from probatus.stat_tests import AutoDist
     psi_calculator = AutoDist(statistical_tests=["PSI"],
                     binning_strategies="QuantileBucketer",
                     bin_count=10)
     train_df = data.iloc[0:500,:]
     test_df = data.iloc[500:, :]
     psi = psi_calculator.compute(train_df, test_df)
     ```
     """
-    transformer = DropHighPSIFeatures()
-    transformer.fit_transform(df)
-
-    expected_psi = {
-        "var_0": 0.043828484052281,
-        "var_1": 0.040929870747665395,
-        "var_2": 0.04330418495156895,
-        "var_3": 0.03773286532548153,
-        "var_4": 0.05047388515663041,
-        "var_5": 0.014717735595712466,
-        "drift_1": 8.283089355027482,
-        "drift_2": 8.283089355027482,
-    }
+    transformer = DropHighPSIFeatures(variables=variables)
+    dft = transformer.fit_transform(df)
 
-    assert transformer.variables_ == [
-        "var_0",
-        "var_1",
-        "var_2",
-        "var_3",
-        "var_4",
-        "var_5",
-        "drift_1",
-        "drift_2",
-    ]
+    assert transformer.variables_ == list(expected_psi.keys())
     assert transformer.psi_values_ == pytest.approx(expected_psi, 12)
-    assert transformer.features_to_drop_ == ["drift_1", "drift_2"]
+    assert transformer.features_to_drop_ == [
+        var for var in expected_psi.keys() if "drift" in var
+    ]
+    pd.testing.assert_frame_equal(dft, df.drop(transformer.features_to_drop_, axis=1))
 
 
 def test_auto_threshold_calculation():
-    """Check the results of 'auto' threshold calculation
-    """
-    transformer = DropHighPSIFeatures(threshold='auto', bins=10)
+    """Check the results of 'auto' threshold calculation"""
+    transformer = DropHighPSIFeatures(threshold="auto", p_value=0.001, bins=10)
     assert math.isclose(
-        transformer._calculate_auto_threshold(
-            N=500,
-            M=500,
-            q=0.999
-        ),
-        0.11150865948502628
+        transformer._calculate_auto_threshold(N=500, M=500, bins=10),
+        0.11150865948502628,
     )
-    transformer = DropHighPSIFeatures(threshold='auto', bins=32)
+    transformer = DropHighPSIFeatures(threshold="auto", p_value=0.05, bins=32)
     assert math.isclose(
-        transformer._calculate_auto_threshold(
-            N=1000,
-            M=1500,
-            q=0.95
-        ),
-        0.07497557213394188
+        transformer._calculate_auto_threshold(N=1000, M=1500, bins=32),
+        0.07497557213394188,
     )
-    transformer = DropHighPSIFeatures(threshold='auto', bins=42)
+    transformer = DropHighPSIFeatures(threshold="auto", p_value=0.01, bins=42)
     assert math.isclose(
-        transformer._calculate_auto_threshold(
-            N=777,
-            M=666,
-            q=0.99
-        ),
-        0.18111345503169146
+        transformer._calculate_auto_threshold(N=777, M=666, bins=42),
+        0.18111345503169146,
     )
 
 
-def test_fit_attributes_auto(df):
+@pytest.mark.parametrize("variables, expected_psi", _input_output)
+def test_fit_attributes_with_autothreshold(variables, expected_psi, df):
     """Check the value of the fit attributes.
     The expected PSI values used in the assertion were determined using
     the Probatus package.
     ```
     from probatus.stat_tests import AutoDist
     psi_calculator = AutoDist(statistical_tests=["PSI"],
                     binning_strategies="QuantileBucketer",
                     bin_count=10)
     train_df = data.iloc[0:500,:]
     test_df = data.iloc[500:, :]
     psi = psi_calculator.compute(train_df, test_df)
     ```
     """
-    transformer = DropHighPSIFeatures(threshold='auto', bins=10)
-    transformer.fit_transform(df)
+    transformer = DropHighPSIFeatures(threshold="auto", variables=variables, bins=10)
+    transformer.fit(df)
+
+    assert transformer.psi_values_ == pytest.approx(expected_psi, 12)
+    assert transformer.features_to_drop_ == [
+        var for var in expected_psi.keys() if "drift" in var
+    ]
+
+
+def test_calculation_when_strategy_equal_width(df):
+    transformer = DropHighPSIFeatures(strategy="equal_width")
+    transformer.fit(df)
 
-    expected_psi = {
-        "var_0": 0.043828484052281,
-        "var_1": 0.040929870747665395,
-        "var_2": 0.04330418495156895,
-        "var_3": 0.03773286532548153,
-        "var_4": 0.05047388515663041,
-        "var_5": 0.014717735595712466,
+    expected = {
+        "var_0": 0.014858665472468786,
+        "var_1": 0.04514737836588022,
+        "var_2": 0.03431479397506742,
+        "var_3": 0.04298209189840294,
+        "var_4": 0.02385796430263416,
+        "var_5": 0.046809664317794444,
         "drift_1": 8.283089355027482,
         "drift_2": 8.283089355027482,
     }
-    assert transformer.variables_ == [
-        "var_0",
-        "var_1",
-        "var_2",
-        "var_3",
-        "var_4",
-        "var_5",
-        "drift_1",
-        "drift_2",
+
+    assert transformer.psi_values_ == pytest.approx(expected, 12)
+    assert transformer.features_to_drop_ == [
+        var for var in expected.keys() if "drift" in var
     ]
-    assert transformer.psi_values_ == pytest.approx(expected_psi, 12)
-    assert transformer.features_to_drop_ == ["drift_1", "drift_2"]
 
 
 # ================ test init parameters =================
 
 # Define two dictionaries with arguments: one with default values and
 # one with arbitrary values.
 default_dict = {
@@ -176,28 +211,30 @@
     "switch": False,
     "threshold": 0.25,
     "bins": 10,
     "strategy": "equal_frequency",
     "min_pct_empty_bins": 0.0001,
     "missing_values": "raise",
     "variables": None,
+    "p_value": 0.001,
 }
 
 args_dict = {
     "split_col": "hola",
     "split_frac": 0.6,
     "split_distinct": True,
     "cut_off": ["value_1", "value_2"],
     "switch": True,
     "threshold": 0.10,
     "bins": 5,
     "strategy": "equal_width",
     "min_pct_empty_bins": 0.1,
     "missing_values": "ignore",
     "variables": ["chau", "adios"],
+    "p_value": 0.2,
 }
 
 init_dict = [(None, default_dict), (args_dict, args_dict)]
 
 
 @pytest.mark.parametrize("initialize, attribute_dict", init_dict)
 def test_init_default_parameters(initialize, attribute_dict):
@@ -245,67 +282,145 @@
     with pytest.raises(ValueError):
         DropHighPSIFeatures(min_pct_empty_bins="unknown")
 
     with pytest.raises(ValueError):
         DropHighPSIFeatures(min_pct_empty_bins=-1)
 
 
+@pytest.mark.parametrize("p_value", ["hola", -1, 10])
+def test_p_value_not_allowed(p_value):
+    with pytest.raises(ValueError):
+        DropHighPSIFeatures(p_value=p_value)
+
+
 # ================= test fit() functionality ==================
 
 
 def test_split_col_not_included_in_variables(df):
-    """Check that the split columns is not included among the features
+    """Check that the split column is not included among the features
     to evaluate when these are selected automatically."""
     transformer = DropHighPSIFeatures(split_col="var_3", variables=None)
     transformer.fit(df)
+    assert "var_3" not in transformer.variables_
+    assert "var_3" not in transformer.psi_values_.keys()
 
-    assert transformer.variables is None
+    transformer = DropHighPSIFeatures(split_col="var_3", variables="all")
+    transformer.fit(df)
     assert "var_3" not in transformer.variables_
     assert "var_3" not in transformer.psi_values_.keys()
 
+    transformer = DropHighPSIFeatures(split_col="cat_1", variables="all")
+    transformer.fit(df)
+    assert "cat_1" not in transformer.variables_
+    assert "cat_1" not in transformer.psi_values_.keys()
+
+
+def test_error_split_col_not_in_df(df):
+    transformer = DropHighPSIFeatures(variables=None, split_col="var_0")
+    data = df.copy()
+    data = data.drop(["var_0"], axis=1)
+    msg = "var_0 is not in the dataframe."
+    with pytest.raises(ValueError) as record:
+        transformer.fit(data)
+    assert str(record.value) == msg
+
+
+_input_output = [
+    (["var_2", "var_3", "drift_1", "drift_2"], ["drift_1"], EXPECTED_PSI_NUM_FEW),
+    (["var_0", "drift_1", "drift_cat_1"], ["drift_cat_1"], EXPECTED_PSI_MIXED),
+]
+
+
+@pytest.mark.parametrize("variables, variable, expected_psi", _input_output)
+def test_confirm_variables(variables, variable, expected_psi, df):
+    data = df.copy()
+    data = data.drop(variable, axis=1)
+    del expected_psi[variable[0]]
+
+    transformer = DropHighPSIFeatures(variables=variables, confirm_variables=True)
+    transformer.fit(data)
+
+    assert transformer.variables_ == list(expected_psi.keys())
+    assert transformer.psi_values_ == pytest.approx(expected_psi, 12)
+    assert transformer.features_to_drop_ == [
+        var for var in expected_psi.keys() if "drift" in var
+    ]
+
+
+def test_error_if_variables_is_none_and_no_numerical_in_df(df):
+    transformer = DropHighPSIFeatures(variables=None)
+    msg = (
+        "No numerical variables found in this dataframe. Please check "
+        "variable format with pandas dtypes."
+    )
+    with pytest.raises(ValueError) as record:
+        transformer.fit(df[["cat_1", "drift_cat_1"]])
+
+    assert str(record.value) == msg
+
+
+def test_error_if_confirm_variables_returns_empty_list(df):
+    transformer = DropHighPSIFeatures(
+        variables=["cat_1", "drift_cat_1"], confirm_variables=True
+    )
+    data = df.copy()
+    data = data.drop(["cat_1", "drift_cat_1"], axis=1)
+    msg = (
+        "After confirming variables, no variable remains. At least 1 "
+        "variable is required for the selection."
+    )
+    with pytest.raises(ValueError) as record:
+        transformer.fit(data)
+
+    assert str(record.value) == msg
+
 
 def test_error_if_na_in_split_col(df):
     """Test an error is raised if the split column contains missing values."""
     data = df.copy()
-    data.iloc[15, data.columns.get_loc("var_3")] = np.nan
+    data.loc[15, "var_3"] = np.nan
 
     transformer = DropHighPSIFeatures(split_col="var_3")
 
     with pytest.raises(ValueError):
-        transformer.fit_transform(data)
+        transformer.fit(data)
 
 
 def test_raise_error_if_na_in_df(df):
     """Test an error is raised when missing values is set to raise."""
     data = df.copy()
-    data.iloc[15, data.columns.get_loc("var_3")] = np.nan
+    data.loc[15, "var_3"] = np.nan
 
     transformer = DropHighPSIFeatures(missing_values="raise")
 
     with pytest.raises(ValueError):
         transformer.fit(data)
 
 
 def test_missing_value_ignored(df):
     """Test if PSI are computed when missing values are present in the dataframe."""
     data = df.copy()
-    data.iloc[15, data.columns.get_loc("var_3")] = np.nan
-
-    var_col = [col for col in data if "var" in col]
+    data.loc[15, "var_3"] = np.nan
 
     transformer = DropHighPSIFeatures(missing_values="ignore")
     transformed = transformer.fit_transform(data)
 
-    pd.testing.assert_frame_equal(transformed, data[var_col])
+    assert transformer.psi_values_ == pytest.approx(EXPECTED_PSI_NUM, 12)
+    assert transformer.features_to_drop_ == [
+        var for var in EXPECTED_PSI_NUM if "drift" in var
+    ]
+    pd.testing.assert_frame_equal(
+        transformed, data.drop(transformer.features_to_drop_, axis=1)
+    )
 
 
 def test_raise_error_if_inf_in_df(df):
     """Test an error is raised for inf when missing values is set to raise."""
     data = df.copy()
-    data.iloc[15, data.columns.get_loc("var_3")] = np.nan
+    data.loc[15, "var_3"] = np.inf
 
     transformer = DropHighPSIFeatures(missing_values="raise")
 
     with pytest.raises(ValueError):
         transformer.fit(data)
 
 
@@ -409,43 +524,54 @@
 
 
 def test_calculation_df_split_with_different_variable_types(df_mixed_types):
     """Test the split of the dataframe using different type of variables."""
     results = {}
     cut_offs = {}
     for split_col in df_mixed_types.columns:
-        test = DropHighPSIFeatures(split_frac=0.5, split_col=split_col)
+        test = DropHighPSIFeatures(split_frac=0.5, split_col=split_col, variables="all")
         test.fit_transform(df_mixed_types)
         results[split_col] = test.psi_values_
         cut_offs[split_col] = test.cut_off_
 
-    assert results["A"] == pytest.approx({"B": 0.0}, 12)
-    assert results["B"] == pytest.approx({"A": 3.0375978817052403}, 12)
+    assert results["A"] == pytest.approx({"B": 0.0, "C": 0.1621860432432657}, 12)
+    assert results["B"] == pytest.approx(
+        {"A": 3.0375978817052403, "C": 8.515489752777954}, 12
+    )
     assert results["C"] == pytest.approx({"A": 2.27819841127893, "B": 0.0}, 12)
-    assert results["time"] == pytest.approx({"A": 8.283089355027482, "B": 0.0}, 12)
+    assert results["time"] == pytest.approx(
+        {"A": 8.283089355027482, "B": 0.0, "C": 0.1621860432432657}, 12
+    )
 
-    expected_cut_offs = {"A": 9.5, "B": 1.5, "C": "B", "time": date(2019, 1, 10)}
+    expected_cut_offs = {
+        "A": 9.5,
+        "B": 1.5,
+        "C": "B",
+        "time": np.datetime64(datetime(2019, 1, 10)),
+    }
 
     assert cut_offs == expected_cut_offs
 
-    # Test when no data frame with mixed data types when no split_col is provided.
-    test = DropHighPSIFeatures(split_frac=0.5)
+    # Test when no dataframe with mixed data types when no split_col is provided.
+    test = DropHighPSIFeatures(split_frac=0.5, variables="all")
     test.fit_transform(df_mixed_types)
-    assert test.psi_values_ == pytest.approx({"A": 8.283089355027482, "B": 0.0}, 12)
+    assert test.psi_values_ == pytest.approx(
+        {"A": 8.283089355027482, "B": 0.0, "C": 0.1621860432432657}, 12
+    )
 
 
 # =========== tests for user entered cut_off values ===========
 
 
 type_test = [
     ("A", 14, [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14]),
     ("B", 1, [0, 3, 4, 7, 8, 11, 12, 15, 16, 19]),
     ("C", ["B"], [1, 5, 9, 13, 17]),
     ("C", "B", [0, 1, 4, 5, 8, 9, 12, 13, 16, 17]),
-    ("time", date(2019, 1, 4), [0, 1, 2, 3]),
+    ("time", datetime(2019, 1, 4), [0, 1, 2, 3]),
 ]
 
 
 @pytest.mark.parametrize("col, cut_off, expected", type_test)
 def test_split_using_cut_off(col, cut_off, expected, df_mixed_types):
     """Test the cut off for different data types."""
     test = DropHighPSIFeatures(split_col=col, cut_off=cut_off)
@@ -490,15 +616,14 @@
     ),
 ]
 
 
 @pytest.mark.parametrize("col, expected_index", split_distinct_test)
 def test_split_distinct(col, expected_index):
     """Test the cut off for different data types.
-
     For columns B, C and time we have 6 distinct values, 5 appearing 20 times and
     1 appearing 100 times. A 50% split based on the number of values will result
     in 2 groups of 3. One has 60 appearances (in total) and the other has 140.
     """
     data = pd.DataFrame(
         {
             "A": [it for it in range(0, 200)],
@@ -636,69 +761,26 @@
         a_bins.reset_index(drop=True), expected_a_bins, check_names=False
     )
     pd.testing.assert_series_equal(
         b_bins.reset_index(drop=True), expected_b_bins, check_names=False
     )
 
 
-def test_param_variable_definition(df):
-    """Test defining the subset of features through the variable argument.
-
-    Due to the small split_frac value, all variables will fail the PSI test, that is,
-    the variables in the list will show a high PSI value and this will be removed.
-
-    The aim of the test is to show that only those variables defined in the variable
-    argument are examined.
-    """
-    #
-    select = DropHighPSIFeatures(variables=["var_1", "var_3", "var_5"], split_frac=0.01)
-    transformed_df = select.fit_transform(df)
-
-    assert select.variables == ["var_1", "var_3", "var_5"]
-    assert select.variables_ == ["var_1", "var_3", "var_5"]
-    assert list(select.psi_values_.keys()) == ["var_1", "var_3", "var_5"]
-    assert select.features_to_drop_ == ["var_1", "var_3", "var_5"]
-
-    assert transformed_df.columns.to_list() == [
-        "var_0",
-        "var_2",
-        "var_4",
-        "drift_1",
-        "drift_2",
-    ]
-
-
-def test_transform_standard(df):
-    """Test the transform method in a standard approach."""
-    test = DropHighPSIFeatures()
-    test.fit(df)
-    transformed = test.transform(df)
-
-    # Check the features to drop
-    assert test.features_to_drop_ == ["drift_1", "drift_2"]
-
-    # Check the transformed dataframe
-    pd.testing.assert_frame_equal(
-        transformed, df[[col for col in df if "drift" not in col]]
-    )
-
-
 def test_transform_feature_to_drop_not_present(df):
     """Test transform when the feature to drop in not in the dataframe."""
     test = DropHighPSIFeatures()
     test.fit(df)
 
     # Define new dataframe with additional column
     data = df.copy()
     data["A"] = [1] * 1000
     # Remove one of the feature to drop
     data = data.drop("drift_1", axis=1)
 
     with pytest.raises(KeyError):
-        # Transform
         test.transform(data)
 
 
 def test_transform_different_number_of_columns(df):
     """Test transform on df with different number of features to train set."""
     test = DropHighPSIFeatures()
     test.fit(df)
```

### Comparing `feature_engine-1.6.0/tests/test_selection/test_information_value.py` & `feature_engine-1.6.1/tests/test_selection/test_information_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+
 import numpy as np
 import pandas as pd
 import pytest
 
 from feature_engine.selection import SelectByInformationValue
 
 
@@ -138,23 +139,25 @@
     for key in exp_dict.keys():
         assert math.isclose(exp_dict[key], sel.information_values_[key])
     assert sel.features_to_drop_ == features_to_drop
     assert X_tr.equals(exp_df)
 
 
 def test_transformer_with_equal_frequency_discretization(df_enc):
-    df = pd.DataFrame({
-        "var_C": np.linspace(0, 20, num=20),
-        "var_D": np.linspace(0, 20, num=20),
-        "target": [1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0],
-    })
+    df = pd.DataFrame(
+        {
+            "var_C": np.linspace(0, 20, num=20),
+            "var_D": np.linspace(0, 20, num=20),
+            "target": [1, 1, 0, 0, 0, 0, 0, 0, 0, 0, 1, 1, 0, 0, 0, 0, 1, 1, 0, 0],
+        }
+    )
     X = df.drop("target", axis=1).copy()
     y = df["target"].copy()
 
     sel = SelectByInformationValue(bins=3, strategy="equal_frequency")
     sel.fit(df.drop("target", axis=1), df["target"])
     sel.fit(X, y)
 
-    exp_dict = {'var_C': 0.010625883395914762, 'var_D': 0.010625883395914762}
+    exp_dict = {"var_C": 0.010625883395914762, "var_D": 0.010625883395914762}
 
     for key in exp_dict.keys():
         assert math.isclose(exp_dict[key], sel.information_values_[key])
```

### Comparing `feature_engine-1.6.0/tests/test_selection/test_probe_feature_selection.py` & `feature_engine-1.6.1/tests/test_selection/test_probe_feature_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/test_recursive_feature_addition.py` & `feature_engine-1.6.1/tests/test_selection/test_recursive_feature_addition.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/test_recursive_feature_elimination.py` & `feature_engine-1.6.1/tests/test_selection/test_recursive_feature_elimination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import pytest
 from sklearn.ensemble import RandomForestClassifier
-from sklearn.linear_model import Lasso, LogisticRegression, LinearRegression
+from sklearn.linear_model import Lasso, LinearRegression, LogisticRegression
 from sklearn.tree import DecisionTreeRegressor
 
 from feature_engine.selection import RecursiveFeatureElimination
 
 # tests for classification
 _model_and_expectations = [
     (
```

### Comparing `feature_engine-1.6.0/tests/test_selection/test_recursive_feature_selectors.py` & `feature_engine-1.6.1/tests/test_selection/test_recursive_feature_selectors.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/test_shuffle_features.py` & `feature_engine-1.6.1/tests/test_selection/test_shuffle_features.py`

 * *Files 14% similar despite different names*

```diff
@@ -130,7 +130,25 @@
         "var_8",
         "var_9",
         "var_10",
         "var_11",
     ]
     # test transform output
     pd.testing.assert_frame_equal(sel.transform(X), Xtransformed)
+
+
+def test_sample_weights():
+    X = pd.DataFrame(
+        dict(
+            x1=[1000, 2000, 1000, 1000, 2000, 3000],
+            x2=[1000, 2000, 1000, 1000, 2000, 3000],
+        )
+    )
+    y = pd.Series([1, 0, 0, 1, 1, 0])
+
+    sbs = SelectByShuffling(
+        RandomForestClassifier(random_state=42), cv=2, random_state=42
+    )
+
+    sample_weight = [1000, 2000, 1000, 1000, 2000, 3000]
+    sbs.fit_transform(X, y, sample_weight=sample_weight)
+    assert sbs.initial_model_performance_ == 0.125
```

### Comparing `feature_engine-1.6.0/tests/test_selection/test_single_feature_performance_selection.py` & `feature_engine-1.6.1/tests/test_selection/test_single_feature_performance_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/test_smart_correlation_selection.py` & `feature_engine-1.6.1/tests/test_selection/test_smart_correlation_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_selection/test_target_mean_selection.py` & `feature_engine-1.6.1/tests/test_selection/test_target_mean_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_time_series/test_forecasting/conftest.py` & `feature_engine-1.6.1/tests/test_time_series/test_forecasting/conftest.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_time_series/test_forecasting/test_check_estimator_forecasting.py` & `feature_engine-1.6.1/tests/test_time_series/test_forecasting/test_check_estimator_forecasting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pandas as pd
 import pytest
 from sklearn.base import clone
+from sklearn.pipeline import Pipeline
 from sklearn.utils.estimator_checks import check_estimator
 
 from feature_engine.timeseries.forecasting import (
     ExpandingWindowFeatures,
     LagFeatures,
     WindowFeatures,
 )
@@ -60,7 +61,19 @@
 
     with pytest.raises(NotImplementedError):
         transformer.fit(Xd)
 
     transformer.fit(X)
     with pytest.raises(NotImplementedError):
         transformer.transform(Xd)
+
+
+@pytest.mark.parametrize("transformer", _estimators)
+def test_transformers_in_pipeline_with_set_output_pandas(df_time, transformer):
+    X = df_time.copy()
+
+    pipe = Pipeline([("trs", transformer)]).set_output(transform="pandas")
+
+    Xtt = transformer.fit_transform(X)
+    Xtp = pipe.fit_transform(X)
+
+    pd.testing.assert_frame_equal(Xtt, Xtp)
```

### Comparing `feature_engine-1.6.0/tests/test_time_series/test_forecasting/test_expanding_window_features.py` & `feature_engine-1.6.1/tests/test_time_series/test_forecasting/test_expanding_window_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_time_series/test_forecasting/test_lag_features.py` & `feature_engine-1.6.1/tests/test_time_series/test_forecasting/test_lag_features.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_time_series/test_forecasting/test_window_features.py` & `feature_engine-1.6.1/tests/test_time_series/test_forecasting/test_window_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,16 +376,18 @@
     )
     df_time_tr = transformer.fit_transform(df_time)
 
     # Expected
     X = df_time.copy()
     num_vars = ["ambient_temp", "module_temp", "irradiation"]
     tmp = X[num_vars].rolling(2).agg(["sum", "mean"]).shift(periods=15, freq="min")
+    tmp.columns = tmp.columns.droplevel()
     X_tr = X.merge(tmp, left_index=True, right_index=True, how="left")
     tmp = X[num_vars].rolling(3).agg(["sum", "mean"]).shift(periods=15, freq="min")
+    tmp.columns = tmp.columns.droplevel()
     X_tr = X_tr.merge(tmp, left_index=True, right_index=True, how="left")
     X_tr.columns = transformer.get_feature_names_out()
 
     assert df_time_tr.equals(X_tr)
 
     # Case 2: user indicates multiple variables
     transformer = WindowFeatures(
@@ -400,21 +402,23 @@
     X = df_time.copy()
     tmp = (
         X[["ambient_temp", "irradiation"]]
         .rolling(2)
         .agg(["sum", "mean"])
         .shift(freq="30min")
     )
+    tmp.columns = tmp.columns.droplevel()
     X_tr = X.merge(tmp, left_index=True, right_index=True, how="left")
     tmp = (
         X[["ambient_temp", "irradiation"]]
         .rolling(3)
         .agg(["sum", "mean"])
         .shift(freq="30min")
     )
+    tmp.columns = tmp.columns.droplevel()
     X_tr = X_tr.merge(tmp, left_index=True, right_index=True, how="left")
     X_tr.columns = transformer.get_feature_names_out()
 
     assert df_time_tr.equals(X_tr)
 
     # Case 4: user indicates 1 variable
     transformer = WindowFeatures(
```

### Comparing `feature_engine-1.6.0/tests/test_transformation/test_arcsin_transformer.py` & `feature_engine-1.6.1/tests/test_transformation/test_arcsin_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_transformation/test_boxcox_transformer.py` & `feature_engine-1.6.1/tests/test_transformation/test_boxcox_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_transformation/test_check_estimator_transformers.py` & `feature_engine-1.6.1/tests/test_transformation/test_check_estimator_transformers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import pandas as pd
 import pytest
+from sklearn.pipeline import Pipeline
 from sklearn.utils.estimator_checks import check_estimator
 
 from feature_engine.transformation import (
     ArcsinTransformer,
     BoxCoxTransformer,
     LogCpTransformer,
     LogTransformer,
@@ -27,7 +29,22 @@
 def test_check_estimator_from_sklearn(estimator):
     return check_estimator(estimator)
 
 
 @pytest.mark.parametrize("estimator", _estimators[4:])
 def test_check_estimator_from_feature_engine(estimator):
     return check_feature_engine_estimator(estimator)
+
+
+@pytest.mark.parametrize("transformer", _estimators)
+def test_transformers_in_pipeline_with_set_output_pandas(transformer):
+    X = pd.DataFrame(
+        {"feature_1": [0.1, 0.2, 0.3, 0.4, 0.5], "feature_2": [0.6, 0.7, 0.8, 0.9, 0.1]}
+    )
+    y = pd.Series([0, 1, 0, 1, 0])
+
+    pipe = Pipeline([("trs", transformer)]).set_output(transform="pandas")
+
+    Xtt = transformer.fit_transform(X)
+    Xtp = pipe.fit_transform(X, y)
+
+    pd.testing.assert_frame_equal(Xtt, Xtp)
```

### Comparing `feature_engine-1.6.0/tests/test_transformation/test_log_transformer.py` & `feature_engine-1.6.1/tests/test_transformation/test_log_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_transformation/test_logcp_transformer.py` & `feature_engine-1.6.1/tests/test_transformation/test_logcp_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_transformation/test_power_transformer.py` & `feature_engine-1.6.1/tests/test_transformation/test_power_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_transformation/test_reciprocal_transformer.py` & `feature_engine-1.6.1/tests/test_transformation/test_reciprocal_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_transformation/test_yeojohnson_transformer.py` & `feature_engine-1.6.1/tests/test_transformation/test_yeojohnson_transformer.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_variable_handling/test_init_parameter_checks.py` & `feature_engine-1.6.1/tests/test_variable_handling/test_init_parameter_checks.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_variable_handling/test_variable_type_selection.py` & `feature_engine-1.6.1/tests/test_variable_handling/test_variable_type_selection.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_wrappers/test_check_estimator_wrappers.py` & `feature_engine-1.6.1/tests/test_wrappers/test_check_estimator_wrappers.py`

 * *Files identical despite different names*

### Comparing `feature_engine-1.6.0/tests/test_wrappers/test_sklearn_wrapper.py` & `feature_engine-1.6.1/tests/test_wrappers/test_sklearn_wrapper.py`

 * *Files identical despite different names*

