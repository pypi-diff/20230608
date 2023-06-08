# Comparing `tmp/evalml-0.76.0.tar.gz` & `tmp/evalml-0.77.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/github/workspace/dist/.tmp-khmpqtc9/evalml-0.76.0.tar", last modified: Wed May 10 14:56:56 2023, max compression
+gzip compressed data, was "/github/workspace/dist/.tmp-b8ja8cfa/evalml-0.77.0.tar", last modified: Thu Jun  8 13:55:18 2023, max compression
```

## Comparing `evalml-0.76.0.tar` & `evalml-0.77.0.tar`

### file list

```diff
@@ -1,444 +1,444 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/
--rw-r--r--   0 root         (0) root         (0)     1513 2023-05-10 14:56:39.000000 evalml-0.76.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8233 2023-05-10 14:56:56.000000 evalml-0.76.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4824 2023-05-10 14:56:39.000000 evalml-0.76.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/
--rw-r--r--   0 root         (0) root         (0)      763 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      355 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/automl/
--rw-r--r--   0 root         (0) root         (0)      412 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/automl/automl_algorithm/
--rw-r--r--   0 root         (0) root         (0)      318 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/automl_algorithm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11921 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/automl_algorithm/automl_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    29145 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/automl_algorithm/default_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    21384 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/automl_algorithm/iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    86362 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/automl_search.py
--rw-r--r--   0 root         (0) root         (0)     2494 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/callbacks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/automl/engine/
--rw-r--r--   0 root         (0) root         (0)      409 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6902 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/engine/cf_engine.py
--rw-r--r--   0 root         (0) root         (0)     6907 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/engine/dask_engine.py
--rw-r--r--   0 root         (0) root         (0)    15405 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/engine/engine_base.py
--rw-r--r--   0 root         (0) root         (0)     5060 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/engine/sequential_engine.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/pipeline_search_plots.py
--rw-r--r--   0 root         (0) root         (0)     6401 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/progress.py
--rw-r--r--   0 root         (0) root         (0)    12122 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/automl/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/data_checks/
--rw-r--r--   0 root         (0) root         (0)     1847 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11989 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/class_imbalance_data_check.py
--rw-r--r--   0 root         (0) root         (0)      916 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check.py
--rw-r--r--   0 root         (0) root         (0)     3060 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_action.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_action_code.py
--rw-r--r--   0 root         (0) root         (0)    11405 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_action_option.py
--rw-r--r--   0 root         (0) root         (0)     3156 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_message.py
--rw-r--r--   0 root         (0) root         (0)     6580 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_message_code.py
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_check_message_type.py
--rw-r--r--   0 root         (0) root         (0)     4716 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/data_checks.py
--rw-r--r--   0 root         (0) root         (0)    25088 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/datetime_format_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4873 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/default_data_checks.py
--rw-r--r--   0 root         (0) root         (0)    11488 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/id_columns_data_check.py
--rw-r--r--   0 root         (0) root         (0)    20762 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/invalid_target_data_check.py
--rw-r--r--   0 root         (0) root         (0)     2905 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/multicollinearity_data_check.py
--rw-r--r--   0 root         (0) root         (0)    11843 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/no_variance_data_check.py
--rw-r--r--   0 root         (0) root         (0)    17159 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/null_data_check.py
--rw-r--r--   0 root         (0) root         (0)     9500 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/outliers_data_check.py
--rw-r--r--   0 root         (0) root         (0)     6213 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/sparsity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     7242 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/target_distribution_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8124 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/target_leakage_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4569 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/ts_parameters_data_check.py
--rw-r--r--   0 root         (0) root         (0)     5099 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/ts_splitting_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8205 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/uniqueness_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/data_checks/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/demos/
--rw-r--r--   0 root         (0) root         (0)      297 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/__init__.py
--rw-r--r--   0 root         (0) root         (0)      605 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/breast_cancer.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/churn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/demos/data/
--rw-r--r--   0 root         (0) root         (0)   977501 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/data/churn.csv
--rw-r--r--   0 root         (0) root         (0)    67921 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/data/daily-min-temperatures.csv
--rw-r--r--   0 root         (0) root         (0)  2661094 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/data/fraud_transactions.csv.gz
--rw-r--r--   0 root         (0) root         (0)     1103 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/diabetes.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/fraud.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/weather.py
--rw-r--r--   0 root         (0) root         (0)      573 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/demos/wine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/exceptions/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5886 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/exceptions/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/model_family/
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_family/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2627 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_family/model_family.py
--rw-r--r--   0 root         (0) root         (0)      910 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_family/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/model_understanding/
--rw-r--r--   0 root         (0) root         (0)     1273 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4365 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py
--rw-r--r--   0 root         (0) root         (0)    18388 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/_partial_dependence_utils.py
--rw-r--r--   0 root         (0) root         (0)     8990 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/decision_boundary.py
--rw-r--r--   0 root         (0) root         (0)     8042 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/feature_explanations.py
--rw-r--r--   0 root         (0) root         (0)     5020 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/force_plots.py
--rw-r--r--   0 root         (0) root         (0)    15125 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/metrics.py
--rw-r--r--   0 root         (0) root         (0)    27420 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/partial_dependence_functions.py
--rw-r--r--   0 root         (0) root         (0)    13556 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/permutation_importance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/
--rw-r--r--   0 root         (0) root         (0)      175 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13317 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/_algorithms.py
--rw-r--r--   0 root         (0) root         (0)     4687 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py
--rw-r--r--   0 root         (0) root         (0)    36936 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/_user_interface.py
--rw-r--r--   0 root         (0) root         (0)    15630 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/prediction_explanations/explainers.py
--rw-r--r--   0 root         (0) root         (0)    22293 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/model_understanding/visualizations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/objectives/
--rw-r--r--   0 root         (0) root         (0)     1663 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/binary_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/cost_benefit_matrix.py
--rw-r--r--   0 root         (0) root         (0)     3392 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/fraud_cost.py
--rw-r--r--   0 root         (0) root         (0)     1780 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/lead_scoring.py
--rw-r--r--   0 root         (0) root         (0)      450 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/multiclass_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     7652 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/objective_base.py
--rw-r--r--   0 root         (0) root         (0)      406 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/regression_objective.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/sensitivity_low_alert.py
--rw-r--r--   0 root         (0) root         (0)    33866 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/standard_metrics.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/time_series_regression_objective.py
--rw-r--r--   0 root         (0) root         (0)    15394 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/objectives/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/
--rw-r--r--   0 root         (0) root         (0)     1928 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4893 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/binary_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/binary_classification_pipeline_mixin.py
--rw-r--r--   0 root         (0) root         (0)     7845 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    40232 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/component_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/
--rw-r--r--   0 root         (0) root         (0)     1935 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10149 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/component_base.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/component_base_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/ensemble/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/ensemble/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2226 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2617 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/estimators/
--rw-r--r--   0 root         (0) root         (0)      964 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/
--rw-r--r--   0 root         (0) root         (0)     1445 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4960 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py
--rw-r--r--   0 root         (0) root         (0)     6296 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3656 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4626 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3661 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4076 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py
--rw-r--r--   0 root         (0) root         (0)     8797 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     3736 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1940 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     4811 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py
--rw-r--r--   0 root         (0) root         (0)     5042 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     8530 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/estimator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/
--rw-r--r--   0 root         (0) root         (0)     1685 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13466 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4996 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4021 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2148 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5051 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/et_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7329 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py
--rw-r--r--   0 root         (0) root         (0)     7295 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1793 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py
--rw-r--r--   0 root         (0) root         (0)     9356 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3355 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     4503 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py
--rw-r--r--   0 root         (0) root         (0)     2371 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py
--rw-r--r--   0 root         (0) root         (0)     5128 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/
--rw-r--r--   0 root         (0) root         (0)     1478 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6235 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/column_selectors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/
--rw-r--r--   0 root         (0) root         (0)      273 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/
--rw-r--r--   0 root         (0) root         (0)      439 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/label_encoder.py
--rw-r--r--   0 root         (0) root         (0)    13779 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py
--rw-r--r--   0 root         (0) root         (0)    12206 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/encoders/target_encoder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/
--rw-r--r--   0 root         (0) root         (0)      599 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4136 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py
--rw-r--r--   0 root         (0) root         (0)     5285 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py
--rw-r--r--   0 root         (0) root         (0)     3116 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8253 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/imputer.py
--rw-r--r--   0 root         (0) root         (0)     4640 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py
--rw-r--r--   0 root         (0) root         (0)     3881 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py
--rw-r--r--   0 root         (0) root         (0)     6187 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py
--rw-r--r--   0 root         (0) root         (0)     5357 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/target_imputer.py
--rw-r--r--   0 root         (0) root         (0)    11389 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5899 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    15805 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py
--rw-r--r--   0 root         (0) root         (0)     1667 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2509 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py
--rw-r--r--   0 root         (0) root         (0)     3213 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     8673 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/lsa.py
--rw-r--r--   0 root         (0) root         (0)     6461 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py
--rw-r--r--   0 root         (0) root         (0)    17526 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py
--rw-r--r--   0 root         (0) root         (0)      946 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py
--rw-r--r--   0 root         (0) root         (0)    12599 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    13192 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py
--rw-r--r--   0 root         (0) root         (0)     4985 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/samplers/
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/samplers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5354 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/samplers/base_sampler.py
--rw-r--r--   0 root         (0) root         (0)     7283 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/samplers/oversampler.py
--rw-r--r--   0 root         (0) root         (0)     8265 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/samplers/undersampler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/pipelines/components/transformers/scalers/
--rw-r--r--   0 root         (0) root         (0)      141 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/scalers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2962 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/transformers/transformer.py
--rw-r--r--   0 root         (0) root         (0)    18498 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/components/utils.py
--rw-r--r--   0 root         (0) root         (0)     2765 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/multiclass_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    33202 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/pipeline_meta.py
--rw-r--r--   0 root         (0) root         (0)     4636 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/regression_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    17176 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/time_series_classification_pipelines.py
--rw-r--r--   0 root         (0) root         (0)    15747 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/time_series_pipeline_base.py
--rw-r--r--   0 root         (0) root         (0)    12880 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/time_series_regression_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    53306 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/pipelines/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/preprocessing/
--rw-r--r--   0 root         (0) root         (0)      269 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/
--rw-r--r--   0 root         (0) root         (0)      367 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/no_split.py
--rw-r--r--   0 root         (0) root         (0)      777 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/sk_splitters.py
--rw-r--r--   0 root         (0) root         (0)     5599 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/time_series_split.py
--rw-r--r--   0 root         (0) root         (0)     3669 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/data_splitters/training_validation_split.py
--rw-r--r--   0 root         (0) root         (0)     6589 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/preprocessing/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/problem_types/
--rw-r--r--   0 root         (0) root         (0)      306 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/problem_types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/problem_types/problem_types.py
--rw-r--r--   0 root         (0) root         (0)     6085 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/problem_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/automl_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5757 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/dask_test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9622 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py
--rw-r--r--   0 root         (0) root         (0)    17604 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py
--rw-r--r--   0 root         (0) root         (0)    14529 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py
--rw-r--r--   0 root         (0) root         (0)   185850 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl.py
--rw-r--r--   0 root         (0) root         (0)     4307 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    38707 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)    38820 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_classification.py
--rw-r--r--   0 root         (0) root         (0)    15745 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py
--rw-r--r--   0 root         (0) root         (0)     8716 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_regression.py
--rw-r--r--   0 root         (0) root         (0)     7055 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py
--rw-r--r--   0 root         (0) root         (0)    12934 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_automl_utils.py
--rw-r--r--   0 root         (0) root         (0)    32956 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_default_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7793 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_engine_base.py
--rw-r--r--   0 root         (0) root         (0)    36749 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_iterative_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     2109 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_pipeline_search_plots.py
--rw-r--r--   0 root         (0) root         (0)     4330 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_progress.py
--rw-r--r--   0 root         (0) root         (0)     5068 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_search.py
--rw-r--r--   0 root         (0) root         (0)     4126 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_search_iterative.py
--rw-r--r--   0 root         (0) root         (0)     3431 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/automl_tests/test_time_series_split.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/component_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27084 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py
--rw-r--r--   0 root         (0) root         (0)    11644 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py
--rw-r--r--   0 root         (0) root         (0)    15261 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_arima_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6678 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_baseline_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1495 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_baseline_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_catboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_catboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)     8548 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_column_selector_transformers.py
--rw-r--r--   0 root         (0) root         (0)    64838 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_components.py
--rw-r--r--   0 root         (0) root         (0)    14114 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_datetime_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_decision_tree_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1370 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_decision_tree_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     7573 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py
--rw-r--r--   0 root         (0) root         (0)     4797 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_drop_rows_transformer.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_en_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_en_regressor.py
--rw-r--r--   0 root         (0) root         (0)    15118 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_estimators.py
--rw-r--r--   0 root         (0) root         (0)     2076 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_et_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_et_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6226 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py
--rw-r--r--   0 root         (0) root         (0)     6206 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_feature_selectors.py
--rw-r--r--   0 root         (0) root         (0)    14950 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_featuretools.py
--rw-r--r--   0 root         (0) root         (0)     9627 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py
--rw-r--r--   0 root         (0) root         (0)    25736 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_imputer.py
--rw-r--r--   0 root         (0) root         (0)     1770 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_knn_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2979 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_knn_imputer.py
--rw-r--r--   0 root         (0) root         (0)     8017 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_label_encoder.py
--rw-r--r--   0 root         (0) root         (0)     5079 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_lda.py
--rw-r--r--   0 root         (0) root         (0)    13414 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_lgbm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     9754 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_lgbm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_log_transformer.py
--rw-r--r--   0 root         (0) root         (0)     8111 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_lsa.py
--rw-r--r--   0 root         (0) root         (0)    20457 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_natural_language_featurizer.py
--rw-r--r--   0 root         (0) root         (0)     9988 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_nullable_types_replacer.py
--rw-r--r--   0 root         (0) root         (0)    26816 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_one_hot_encoder.py
--rw-r--r--   0 root         (0) root         (0)    25966 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_ordinal_encoder.py
--rw-r--r--   0 root         (0) root         (0)    19941 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_oversampler.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_pca.py
--rw-r--r--   0 root         (0) root         (0)    12025 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_per_column_imputer.py
--rw-r--r--   0 root         (0) root         (0)     5021 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_prophet_regressor.py
--rw-r--r--   0 root         (0) root         (0)    23430 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_simple_imputer.py
--rw-r--r--   0 root         (0) root         (0)    18269 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py
--rw-r--r--   0 root         (0) root         (0)    10542 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py
--rw-r--r--   0 root         (0) root         (0)     2733 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_standard_scaler.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_svm_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_svm_regressor.py
--rw-r--r--   0 root         (0) root         (0)     8928 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_target_encoder.py
--rw-r--r--   0 root         (0) root         (0)     9398 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_target_imputer.py
--rw-r--r--   0 root         (0) root         (0)    30311 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_time_series_featurizer.py
--rw-r--r--   0 root         (0) root         (0)    24722 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_time_series_imputer.py
--rw-r--r--   0 root         (0) root         (0)     9937 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_time_series_regularizer.py
--rw-r--r--   0 root         (0) root         (0)     6246 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_undersampler.py
--rw-r--r--   0 root         (0) root         (0)     9766 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2150 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py
--rw-r--r--   0 root         (0) root         (0)     3980 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_xgboost_classifier.py
--rw-r--r--   0 root         (0) root         (0)     2792 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/component_tests/test_xgboost_regressor.py
--rw-r--r--   0 root         (0) root         (0)    80078 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/data/
--rw-r--r--   0 root         (0) root         (0)   977501 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data/churn.csv
--rw-r--r--   0 root         (0) root         (0)    67921 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data/daily-min-temperatures.csv
--rw-r--r--   0 root         (0) root         (0)  2661094 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data/fraud_transactions.csv.gz
--rw-r--r--   0 root         (0) root         (0)     9729 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data/tips.csv
--rw-r--r--   0 root         (0) root         (0)    61194 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data/titanic.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/data_checks_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24199 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_action.py
--rw-r--r--   0 root         (0) root         (0)    20667 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_action_option.py
--rw-r--r--   0 root         (0) root         (0)     7842 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_message.py
--rw-r--r--   0 root         (0) root         (0)    29212 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_data_checks.py
--rw-r--r--   0 root         (0) root         (0)    19715 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py
--rw-r--r--   0 root         (0) root         (0)    12185 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py
--rw-r--r--   0 root         (0) root         (0)    30182 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py
--rw-r--r--   0 root         (0) root         (0)     3958 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py
--rw-r--r--   0 root         (0) root         (0)    26417 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_null_data_check.py
--rw-r--r--   0 root         (0) root         (0)     8238 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_outliers_data_check.py
--rw-r--r--   0 root         (0) root         (0)     5609 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py
--rw-r--r--   0 root         (0) root         (0)    18212 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1938 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py
--rw-r--r--   0 root         (0) root         (0)     4898 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py
--rw-r--r--   0 root         (0) root         (0)     1225 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/data_checks_tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/demo_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/demo_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2441 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/demo_tests/test_datasets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/dependency_update_check/
--rw-r--r--   0 root         (0) root         (0)      658 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt
--rw-r--r--   0 root         (0) root         (0)      642 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/dependency_update_check/minimum_requirements.txt
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/integration_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10709 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py
--rw-r--r--   0 root         (0) root         (0)     5184 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/integration_tests/test_nullable_types.py
--rw-r--r--   0 root         (0) root         (0)     7110 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/integration_tests/test_time_series_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/model_family_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_family_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2249 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_family_tests/test_model_family.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14158 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py
--rw-r--r--   0 root         (0) root         (0)    67430 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py
--rw-r--r--   0 root         (0) root         (0)     9790 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py
--rw-r--r--   0 root         (0) root         (0)    19357 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py
--rw-r--r--   0 root         (0) root         (0)    15261 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_decision_boundary.py
--rw-r--r--   0 root         (0) root         (0)    14744 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_feature_explanations.py
--rw-r--r--   0 root         (0) root         (0)    26774 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)    98520 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_partial_dependence.py
--rw-r--r--   0 root         (0) root         (0)    29313 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_permutation_importance.py
--rw-r--r--   0 root         (0) root         (0)    26181 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/model_understanding_tests/test_visualizations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/objective_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4728 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_binary_classification_objective.py
--rw-r--r--   0 root         (0) root         (0)     5863 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py
--rw-r--r--   0 root         (0) root         (0)     6236 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_fraud_detection.py
--rw-r--r--   0 root         (0) root         (0)     3865 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_lead_scoring.py
--rw-r--r--   0 root         (0) root         (0)    13953 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_objectives.py
--rw-r--r--   0 root         (0) root         (0)     2418 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_sla.py
--rw-r--r--   0 root         (0) root         (0)    27155 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/objective_tests/test_standard_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6706 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py
--rw-r--r--   0 root         (0) root         (0)     4688 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py
--rw-r--r--   0 root         (0) root         (0)     2080 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/pipeline_tests/regression_pipeline_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/regression_pipeline_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3652 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py
--rw-r--r--   0 root         (0) root         (0)    94308 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_component_graph.py
--rw-r--r--   0 root         (0) root         (0)     8969 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_graphs.py
--rw-r--r--   0 root         (0) root         (0)    49985 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_pipeline_utils.py
--rw-r--r--   0 root         (0) root         (0)   101489 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     5622 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py
--rw-r--r--   0 root         (0) root         (0)    70356 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/test_no_split.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/test_sk_splitters.py
--rw-r--r--   0 root         (0) root         (0)     3849 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/test_split_data.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/preprocessing_tests/test_training_validation_split.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/problem_type_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/problem_type_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6537 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/problem_type_tests/test_problem_types.py
--rw-r--r--   0 root         (0) root         (0)      516 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/test_all_test_dirs_included.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/tuner_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/tuner_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2941 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/tuner_tests/test_grid_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     3959 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/tuner_tests/test_random_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     9170 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/tuner_tests/test_skopt_tuner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tests/utils_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3993 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/test_cli_utils.py
--rw-r--r--   0 root         (0) root         (0)    30486 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/test_gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/test_logger.py
--rw-r--r--   0 root         (0) root         (0)     6714 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/test_nullable_type_utils.py
--rw-r--r--   0 root         (0) root         (0)    12628 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tests/utils_tests/test_woodwork_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/tuners/
--rw-r--r--   0 root         (0) root         (0)      316 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/grid_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     4675 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/random_search_tuner.py
--rw-r--r--   0 root         (0) root         (0)     3809 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/skopt_tuner.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/tuner.py
--rw-r--r--   0 root         (0) root         (0)      319 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/tuners/tuner_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml/utils/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1598 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/base_meta.py
--rw-r--r--   0 root         (0) root         (0)     6540 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/cli_utils.py
--rw-r--r--   0 root         (0) root         (0)    26270 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/gen_utils.py
--rw-r--r--   0 root         (0) root         (0)     2159 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/logger.py
--rw-r--r--   0 root         (0) root         (0)     7066 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/nullable_type_utils.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/update_checker.py
--rw-r--r--   0 root         (0) root         (0)     6346 2023-05-10 14:56:39.000000 evalml-0.76.0/evalml/utils/woodwork_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8233 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20684 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1292 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-10 14:56:56.000000 evalml-0.76.0/evalml.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5088 2023-05-10 14:56:39.000000 evalml-0.76.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 14:56:56.000000 evalml-0.76.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-06-08 13:55:04.000000 evalml-0.77.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-06-08 13:55:18.000000 evalml-0.77.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-06-08 13:55:04.000000 evalml-0.77.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/
+-rw-r--r--   0 root         (0) root         (0)      763 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/automl/
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/automl/automl_algorithm/
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/automl_algorithm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12705 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/automl_algorithm/automl_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    30444 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/automl_algorithm/default_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    21703 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/automl_algorithm/iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    88380 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/automl_search.py
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/callbacks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/automl/engine/
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6902 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/engine/cf_engine.py
+-rw-r--r--   0 root         (0) root         (0)     6907 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/engine/dask_engine.py
+-rw-r--r--   0 root         (0) root         (0)    15405 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/engine/engine_base.py
+-rw-r--r--   0 root         (0) root         (0)     5060 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/engine/sequential_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/pipeline_search_plots.py
+-rw-r--r--   0 root         (0) root         (0)     6401 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/progress.py
+-rw-r--r--   0 root         (0) root         (0)    12122 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/automl/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/data_checks/
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11989 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/class_imbalance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check.py
+-rw-r--r--   0 root         (0) root         (0)     3060 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_action.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_action_code.py
+-rw-r--r--   0 root         (0) root         (0)    11405 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_action_option.py
+-rw-r--r--   0 root         (0) root         (0)     3156 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_message.py
+-rw-r--r--   0 root         (0) root         (0)     6580 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_message_code.py
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_check_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     4716 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    25088 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/datetime_format_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4873 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/default_data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11818 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/id_columns_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    20762 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/invalid_target_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/multicollinearity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    11843 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/no_variance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    17159 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/null_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     9500 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/outliers_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     6213 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/sparsity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     7242 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/target_distribution_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8124 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/target_leakage_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4569 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/ts_parameters_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     5099 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/ts_splitting_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8205 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/uniqueness_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/data_checks/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/demos/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      605 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/breast_cancer.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/churn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/demos/data/
+-rw-r--r--   0 root         (0) root         (0)   977501 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/data/churn.csv
+-rw-r--r--   0 root         (0) root         (0)    67921 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/data/daily-min-temperatures.csv
+-rw-r--r--   0 root         (0) root         (0)  2661094 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/data/fraud_transactions.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/diabetes.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/fraud.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/weather.py
+-rw-r--r--   0 root         (0) root         (0)      573 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/demos/wine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/exceptions/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5886 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/exceptions/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/model_family/
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_family/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_family/model_family.py
+-rw-r--r--   0 root         (0) root         (0)      910 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_family/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/model_understanding/
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py
+-rw-r--r--   0 root         (0) root         (0)    18388 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/_partial_dependence_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8990 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/decision_boundary.py
+-rw-r--r--   0 root         (0) root         (0)     8042 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/feature_explanations.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/force_plots.py
+-rw-r--r--   0 root         (0) root         (0)    16822 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    27420 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/partial_dependence_functions.py
+-rw-r--r--   0 root         (0) root         (0)    13556 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/permutation_importance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13317 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py
+-rw-r--r--   0 root         (0) root         (0)    36936 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/_user_interface.py
+-rw-r--r--   0 root         (0) root         (0)    15630 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/prediction_explanations/explainers.py
+-rw-r--r--   0 root         (0) root         (0)    22293 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/model_understanding/visualizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/objectives/
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/binary_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/cost_benefit_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/fraud_cost.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/lead_scoring.py
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/multiclass_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     7652 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/objective_base.py
+-rw-r--r--   0 root         (0) root         (0)      406 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/regression_objective.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/sensitivity_low_alert.py
+-rw-r--r--   0 root         (0) root         (0)    33866 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/standard_metrics.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/time_series_regression_objective.py
+-rw-r--r--   0 root         (0) root         (0)    15394 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/objectives/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     1928 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4893 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/binary_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/binary_classification_pipeline_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     7845 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    40232 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/component_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10149 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/component_base.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/component_base_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/ensemble/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/ensemble/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2226 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py
+-rw-r--r--   0 root         (0) root         (0)     2942 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2617 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/estimators/
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4960 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3661 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4076 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     8797 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     3736 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1940 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     4811 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     8530 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/estimator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13678 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4996 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4021 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     5051 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/et_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     7329 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     9356 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3355 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     4503 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     5128 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6235 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/column_selectors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/label_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    13779 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    12206 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/encoders/target_encoder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/
+-rw-r--r--   0 root         (0) root         (0)      599 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py
+-rw-r--r--   0 root         (0) root         (0)     5285 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3116 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8253 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/imputer.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     3881 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     5357 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/target_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    11389 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)     1854 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5899 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    15805 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2509 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     8673 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/lsa.py
+-rw-r--r--   0 root         (0) root         (0)     6461 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py
+-rw-r--r--   0 root         (0) root         (0)    17526 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)      946 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/samplers/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/samplers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5354 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/samplers/base_sampler.py
+-rw-r--r--   0 root         (0) root         (0)     7283 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/samplers/oversampler.py
+-rw-r--r--   0 root         (0) root         (0)     8265 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/samplers/undersampler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/pipelines/components/transformers/scalers/
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/scalers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/transformers/transformer.py
+-rw-r--r--   0 root         (0) root         (0)    19130 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/components/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2765 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/multiclass_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    33202 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/pipeline_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/regression_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    17176 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/time_series_classification_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)    15747 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/time_series_pipeline_base.py
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/time_series_regression_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    53306 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/pipelines/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/preprocessing/
+-rw-r--r--   0 root         (0) root         (0)      269 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/no_split.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/sk_splitters.py
+-rw-r--r--   0 root         (0) root         (0)     5599 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/time_series_split.py
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/data_splitters/training_validation_split.py
+-rw-r--r--   0 root         (0) root         (0)     6589 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/preprocessing/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/problem_types/
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/problem_types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/problem_types/problem_types.py
+-rw-r--r--   0 root         (0) root         (0)     6085 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/problem_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/automl_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5757 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/dask_test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9622 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py
+-rw-r--r--   0 root         (0) root         (0)    17604 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py
+-rw-r--r--   0 root         (0) root         (0)    14529 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py
+-rw-r--r--   0 root         (0) root         (0)   189671 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl.py
+-rw-r--r--   0 root         (0) root         (0)     4307 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    39282 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)    38820 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_classification.py
+-rw-r--r--   0 root         (0) root         (0)    15745 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_regression.py
+-rw-r--r--   0 root         (0) root         (0)     7055 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py
+-rw-r--r--   0 root         (0) root         (0)    12934 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_automl_utils.py
+-rw-r--r--   0 root         (0) root         (0)    33493 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_default_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7793 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_engine_base.py
+-rw-r--r--   0 root         (0) root         (0)    37654 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_iterative_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     2109 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_pipeline_search_plots.py
+-rw-r--r--   0 root         (0) root         (0)     4330 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_progress.py
+-rw-r--r--   0 root         (0) root         (0)     5068 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_search.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_search_iterative.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/automl_tests/test_time_series_split.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/component_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27084 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)    11644 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py
+-rw-r--r--   0 root         (0) root         (0)    16112 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_arima_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6678 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_baseline_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_baseline_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_catboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_catboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     8548 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_column_selector_transformers.py
+-rw-r--r--   0 root         (0) root         (0)    64838 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_components.py
+-rw-r--r--   0 root         (0) root         (0)    14114 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_datetime_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_decision_tree_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_decision_tree_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     7573 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     4797 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_drop_rows_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_en_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_en_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    15118 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_estimators.py
+-rw-r--r--   0 root         (0) root         (0)     2076 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_et_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_et_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_feature_selectors.py
+-rw-r--r--   0 root         (0) root         (0)    14950 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_featuretools.py
+-rw-r--r--   0 root         (0) root         (0)     9627 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py
+-rw-r--r--   0 root         (0) root         (0)    25736 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     1770 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_knn_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_knn_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     8017 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_label_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     5079 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_lda.py
+-rw-r--r--   0 root         (0) root         (0)    13414 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_lgbm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     9754 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_lgbm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_log_transformer.py
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_lsa.py
+-rw-r--r--   0 root         (0) root         (0)    20457 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_natural_language_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)     9988 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_nullable_types_replacer.py
+-rw-r--r--   0 root         (0) root         (0)    26816 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_one_hot_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    25966 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_ordinal_encoder.py
+-rw-r--r--   0 root         (0) root         (0)    19941 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_oversampler.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_pca.py
+-rw-r--r--   0 root         (0) root         (0)    12025 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_per_column_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     5021 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_prophet_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    23430 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_simple_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    18269 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py
+-rw-r--r--   0 root         (0) root         (0)    10542 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_standard_scaler.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_svm_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_svm_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     8928 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_target_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     9398 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_target_imputer.py
+-rw-r--r--   0 root         (0) root         (0)    30311 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_time_series_featurizer.py
+-rw-r--r--   0 root         (0) root         (0)    24722 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_time_series_imputer.py
+-rw-r--r--   0 root         (0) root         (0)     9937 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_time_series_regularizer.py
+-rw-r--r--   0 root         (0) root         (0)     6246 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_undersampler.py
+-rw-r--r--   0 root         (0) root         (0)     9766 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py
+-rw-r--r--   0 root         (0) root         (0)     3980 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_xgboost_classifier.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/component_tests/test_xgboost_regressor.py
+-rw-r--r--   0 root         (0) root         (0)    80162 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/data/
+-rw-r--r--   0 root         (0) root         (0)   977501 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data/churn.csv
+-rw-r--r--   0 root         (0) root         (0)    67921 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data/daily-min-temperatures.csv
+-rw-r--r--   0 root         (0) root         (0)  2661094 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data/fraud_transactions.csv.gz
+-rw-r--r--   0 root         (0) root         (0)     9729 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data/tips.csv
+-rw-r--r--   0 root         (0) root         (0)    61194 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data/titanic.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/data_checks_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24199 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_action.py
+-rw-r--r--   0 root         (0) root         (0)    20667 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_action_option.py
+-rw-r--r--   0 root         (0) root         (0)     7842 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_message.py
+-rw-r--r--   0 root         (0) root         (0)    29212 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_data_checks.py
+-rw-r--r--   0 root         (0) root         (0)    19715 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    13086 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    30182 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     3958 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    26417 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_null_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     8238 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_outliers_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py
+-rw-r--r--   0 root         (0) root         (0)    18212 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     4898 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/data_checks_tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/demo_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/demo_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/demo_tests/test_datasets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/dependency_update_check/
+-rw-r--r--   0 root         (0) root         (0)      659 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt
+-rw-r--r--   0 root         (0) root         (0)      642 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/dependency_update_check/minimum_requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      778 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/integration_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/integration_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10709 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py
+-rw-r--r--   0 root         (0) root         (0)     5184 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/integration_tests/test_nullable_types.py
+-rw-r--r--   0 root         (0) root         (0)     7110 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/integration_tests/test_time_series_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/model_family_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_family_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2249 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_family_tests/test_model_family.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14158 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py
+-rw-r--r--   0 root         (0) root         (0)    67430 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py
+-rw-r--r--   0 root         (0) root         (0)     9790 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py
+-rw-r--r--   0 root         (0) root         (0)    19357 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py
+-rw-r--r--   0 root         (0) root         (0)    15261 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_decision_boundary.py
+-rw-r--r--   0 root         (0) root         (0)    14744 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_feature_explanations.py
+-rw-r--r--   0 root         (0) root         (0)    27456 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)    98520 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_partial_dependence.py
+-rw-r--r--   0 root         (0) root         (0)    29313 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_permutation_importance.py
+-rw-r--r--   0 root         (0) root         (0)    26181 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/model_understanding_tests/test_visualizations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/objective_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4728 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_binary_classification_objective.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py
+-rw-r--r--   0 root         (0) root         (0)     6236 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_fraud_detection.py
+-rw-r--r--   0 root         (0) root         (0)     3865 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_lead_scoring.py
+-rw-r--r--   0 root         (0) root         (0)    13953 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_objectives.py
+-rw-r--r--   0 root         (0) root         (0)     2418 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_sla.py
+-rw-r--r--   0 root         (0) root         (0)    27155 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/objective_tests/test_standard_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6706 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py
+-rw-r--r--   0 root         (0) root         (0)     4688 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py
+-rw-r--r--   0 root         (0) root         (0)     2080 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/pipeline_tests/regression_pipeline_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/regression_pipeline_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py
+-rw-r--r--   0 root         (0) root         (0)    94308 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_component_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8969 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_graphs.py
+-rw-r--r--   0 root         (0) root         (0)    50312 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_pipeline_utils.py
+-rw-r--r--   0 root         (0) root         (0)   101489 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     5621 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    70356 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/test_no_split.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/test_sk_splitters.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/test_split_data.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/preprocessing_tests/test_training_validation_split.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/problem_type_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/problem_type_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/problem_type_tests/test_problem_types.py
+-rw-r--r--   0 root         (0) root         (0)      516 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/test_all_test_dirs_included.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/tuner_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/tuner_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/tuner_tests/test_grid_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     3959 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/tuner_tests/test_random_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     9170 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/tuner_tests/test_skopt_tuner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tests/utils_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3993 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/test_cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)    30486 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/test_gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/test_logger.py
+-rw-r--r--   0 root         (0) root         (0)     6714 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/test_nullable_type_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12628 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tests/utils_tests/test_woodwork_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/tuners/
+-rw-r--r--   0 root         (0) root         (0)      316 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/grid_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     4675 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/random_search_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/skopt_tuner.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/tuner.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/tuners/tuner_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml/utils/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/base_meta.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/cli_utils.py
+-rw-r--r--   0 root         (0) root         (0)    26270 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/gen_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/logger.py
+-rw-r--r--   0 root         (0) root         (0)     7066 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/nullable_type_utils.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/update_checker.py
+-rw-r--r--   0 root         (0) root         (0)     6346 2023-06-08 13:55:04.000000 evalml-0.77.0/evalml/utils/woodwork_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8233 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20684 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-08 13:55:18.000000 evalml-0.77.0/evalml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-06-08 13:55:04.000000 evalml-0.77.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 13:55:18.000000 evalml-0.77.0/setup.cfg
```

### Comparing `evalml-0.76.0/LICENSE` & `evalml-0.77.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/PKG-INFO` & `evalml-0.77.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalml
-Version: 0.76.0
+Version: 0.77.0
 Summary: an AutoML library that builds, optimizes, and evaluates machine learning pipelines using domain-specific objective functions
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Alteryx, Inc.
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalml Version: 0.76.0 Summary: an AutoML library
+Metadata-Version: 2.1 Name: evalml Version: 0.77.0 Summary: an AutoML library
 that builds, optimizes, and evaluates machine learning pipelines using domain-
 specific objective functions Author-email: "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-Clause License Copyright (c) 2019, Alteryx, Inc.
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
```

### Comparing `evalml-0.76.0/README.md` & `evalml-0.77.0/README.md`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/__init__.py` & `evalml-0.77.0/evalml/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 with warnings.catch_warnings():
     warnings.simplefilter("ignore", FutureWarning)
     warnings.simplefilter("ignore", DeprecationWarning)
     import skopt
 warnings.filterwarnings("ignore", category=FutureWarning)
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
-__version__ = "0.76.0"
+__version__ = "0.77.0"
```

### Comparing `evalml-0.76.0/evalml/automl/automl_algorithm/automl_algorithm.py` & `evalml-0.77.0/evalml/automl/automl_algorithm/automl_algorithm.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,17 @@
         text_in_ensembling (boolean): If True and ensembling is True, then n_jobs will be set to 1 to avoid downstream sklearn stacking issues related to nltk. Defaults to None.
         random_seed (int): Seed for the random number generator. Defaults to 0.
     """
 
     def __init__(
         self,
         allowed_pipelines=None,
+        allowed_model_families=None,
+        excluded_model_families=None,
+        allowed_component_graphs=None,
         search_parameters=None,
         tuner_class=None,
         text_in_ensembling=False,
         random_seed=0,
         n_jobs=-1,
     ):
         self.random_seed = random_seed
@@ -53,14 +56,29 @@
         self.allowed_pipelines = []
         if allowed_pipelines is not None:
             self._set_allowed_pipelines(allowed_pipelines)
         self._pipeline_number = 0
         self._batch_number = 0
         self._default_max_batches = 1
 
+        if allowed_component_graphs is not None:
+            if excluded_model_families is not None:
+                raise ValueError(
+                    "Both `excluded_model_families` and `allowed_component_graphs` cannot be set.",
+                )
+        self.allowed_component_graphs = allowed_component_graphs
+
+        if allowed_model_families is not None and excluded_model_families is not None:
+            raise ValueError(
+                "Both `allowed_model_families` and `excluded_model_families` cannot be set.",
+            )
+
+        self.allowed_model_families = allowed_model_families
+        self.excluded_model_families = excluded_model_families
+
     @abstractmethod
     def next_batch(self):
         """Get the next batch of pipelines to evaluate.
 
         Returns:
             list[PipelineBase]: A list of instances of PipelineBase subclasses, ready to be trained and evaluated.
         """
```

### Comparing `evalml-0.76.0/evalml/automl/automl_algorithm/default_algorithm.py` & `evalml-0.77.0/evalml/automl/automl_algorithm/default_algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,22 +71,28 @@
         num_long_pipelines_per_batch (int): number of pipelines per batch for each top n pipeline through long mode.
         allow_long_running_models (bool): Whether or not to allow longer-running models for large multiclass problems. If False and no pipelines, component graphs, or model families are provided,
             AutoMLSearch will not use Elastic Net or XGBoost when there are more than 75 multiclass targets and will not use CatBoost when there are more than 150 multiclass targets. Defaults to False.
         features (list)[FeatureBase]: List of features to run DFS on in AutoML pipelines. Defaults to None. Features will only be computed if the columns used by the feature exist in the input and if the feature has not been computed yet.
         verbose (boolean): Whether or not to display logging information regarding pipeline building. Defaults to False.
         exclude_featurizers (list[str]): A list of featurizer components to exclude from the pipelines built by DefaultAlgorithm.
             Valid options are "DatetimeFeaturizer", "EmailFeaturizer", "URLFeaturizer", "NaturalLanguageFeaturizer", "TimeSeriesFeaturizer"
+        allowed_model_families (list(str, ModelFamily)): The model families to search. The default of None searches over all
+            model families. Run evalml.pipelines.components.utils.allowed_model_families("binary") to see options. Change `binary`
+            to `multiclass` or `regression` depending on the problem type.
+        excluded_model_families (list[ModelFamily]): A list of model families to exclude from the estimators used when building pipelines. For default algorithm, this only excludes estimators in the non-naive batches.
     """
 
     def __init__(
         self,
         X,
         y,
         problem_type,
         sampler_name,
+        allowed_model_families=None,
+        excluded_model_families=None,
         tuner_class=None,
         random_seed=0,
         search_parameters=None,
         n_jobs=1,
         text_in_ensembling=False,
         top_n=3,
         ensembling=False,
@@ -95,14 +101,17 @@
         allow_long_running_models=False,
         features=None,
         verbose=False,
         exclude_featurizers=None,
     ):
         super().__init__(
             allowed_pipelines=[],
+            allowed_model_families=allowed_model_families,
+            excluded_model_families=excluded_model_families,
+            allowed_component_graphs=None,
             search_parameters=search_parameters,
             tuner_class=None,
             random_seed=random_seed,
         )
         self.X = infer_feature_types(X)
         self.y = infer_feature_types(y)
         self.problem_type = problem_type
@@ -122,14 +131,22 @@
         self.allow_long_running_models = allow_long_running_models
         self._X_with_cat_cols = None
         self._X_without_cat_cols = None
         self.features = features
         self.ensembling = ensembling
         self.exclude_featurizers = exclude_featurizers or []
 
+        if allowed_model_families is not None and excluded_model_families is not None:
+            raise ValueError(
+                "Both `allowed_model_families` and `excluded_model_families` cannot be set.",
+            )
+
+        self.allowed_model_families = allowed_model_families
+        self.excluded_model_families = excluded_model_families
+
         # TODO remove on resolution of 3186
         if is_time_series(self.problem_type) and self.ensembling:
             raise ValueError(
                 "Ensembling is not available for time series problems in DefaultAlgorithm.",
             )
 
         if verbose:
@@ -190,15 +207,19 @@
             handle_component_class(estimator) for estimator in naive_estimators
         ]
         return estimators
 
     def _non_naive_estimators(self):
         return [
             est
-            for est in get_estimators(self.problem_type)
+            for est in get_estimators(
+                self.problem_type,
+                model_families=self.allowed_model_families,
+                excluded_model_families=self.excluded_model_families,
+            )
             if est not in self._naive_estimators()
         ]
 
     def _init_pipelines_with_starter_params(self, pipelines):
         next_batch = []
         for pipeline in pipelines:
             self._create_tuner(pipeline)
```

### Comparing `evalml-0.76.0/evalml/automl/automl_algorithm/iterative_algorithm.py` & `evalml-0.77.0/evalml/automl/automl_algorithm/iterative_algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,15 @@
         y (pd.Series): Target data.
         problem_type (ProblemType): Problem type associated with training data.
         sampler_name (BaseSampler): Sampler to use for preprocessing. Defaults to None.
         allowed_model_families (list(str, ModelFamily)): The model families to search. The default of None searches over all
             model families. Run evalml.pipelines.components.utils.allowed_model_families("binary") to see options. Change `binary`
             to `multiclass` or `regression` depending on the problem type. Note that if allowed_pipelines is provided,
             this parameter will be ignored.
+        excluded_model_families (list[ModelFamily]): A list of model families to exclude from the estimators used when building pipelines.
         allowed_component_graphs (dict): A dictionary of lists or ComponentGraphs indicating the component graphs allowed in the search.
             The format should follow { "Name_0": [list_of_components], "Name_1": [ComponentGraph(...)] }
 
             The default of None indicates all pipeline component graphs for this problem type are allowed. Setting this field will cause
             allowed_model_families to be ignored.
 
             e.g. allowed_component_graphs = { "My_Graph": ["Imputer", "One Hot Encoder", "Random Forest Classifier"] }
@@ -73,14 +74,15 @@
     def __init__(
         self,
         X,
         y,
         problem_type,
         sampler_name=None,
         allowed_model_families=None,
+        excluded_model_families=None,
         allowed_component_graphs=None,
         max_batches=None,
         max_iterations=None,
         tuner_class=None,
         random_seed=0,
         pipelines_per_batch=5,
         n_jobs=-1,  # TODO remove
@@ -95,15 +97,14 @@
         exclude_featurizers=None,
     ):
         self.X = infer_feature_types(X)
         self.y = infer_feature_types(y)
         self.problem_type = problem_type
         self.random_seed = random_seed
         self.sampler_name = sampler_name
-        self.allowed_model_families = allowed_model_families
         self.pipelines_per_batch = pipelines_per_batch
         self.n_jobs = n_jobs
         self.number_features = number_features
         self._first_batch_results = []
         self._best_pipeline_info = {}
         self.ensembling = ensembling
         self.search_parameters = search_parameters or {}
@@ -122,20 +123,22 @@
         if search_parameters and not isinstance(search_parameters, dict):
             raise ValueError(
                 f"If search_parameters provided, must be of type dict. Received {type(search_parameters)}",
             )
         self.allowed_pipelines = []
 
         self.features = features
-        self.allowed_component_graphs = allowed_component_graphs
         self._set_additional_pipeline_params()
         self.exclude_featurizers = exclude_featurizers
 
         super().__init__(
             allowed_pipelines=self.allowed_pipelines,
+            allowed_model_families=allowed_model_families,
+            excluded_model_families=excluded_model_families,
+            allowed_component_graphs=allowed_component_graphs,
             search_parameters=self.search_parameters,
             tuner_class=tuner_class,
             text_in_ensembling=self.text_in_ensembling,
             random_seed=random_seed,
             n_jobs=self.n_jobs,
         )
         self._separate_hyperparameters_from_parameters()
@@ -147,15 +150,16 @@
         pipelines_to_sort = []
         pipelines_end = []
         self.allowed_pipelines = []
         if self.allowed_component_graphs is None:
             self.logger.info("Generating pipelines to search over...")
             allowed_estimators = get_estimators(
                 self.problem_type,
-                self.allowed_model_families,
+                model_families=self.allowed_model_families,
+                excluded_model_families=self.excluded_model_families,
             )
             allowed_estimators = self._filter_estimators(
                 allowed_estimators,
                 self.problem_type,
                 self.allow_long_running_models,
                 self.allowed_model_families,
                 self.y.nunique(),
```

### Comparing `evalml-0.76.0/evalml/automl/automl_search.py` & `evalml-0.77.0/evalml/automl/automl_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -433,14 +433,16 @@
 
         verbose (boolean): Whether or not to display semi-real-time updates to stdout while search is running. Defaults to False.
 
         timing (boolean): Whether or not to write pipeline search times to the logger. Defaults to False.
         exclude_featurizers (list[str]): A list of featurizer components to exclude from the pipelines built by search.
             Valid options are "DatetimeFeaturizer", "EmailFeaturizer", "URLFeaturizer", "NaturalLanguageFeaturizer", "TimeSeriesFeaturizer"
 
+        excluded_model_families (list[ModelFamily]): A list of model families to exclude from the estimators used when building pipelines. For default algorithm, this only excludes estimators in the non-naive batches.
+
         holdout_set_size (float): The size of the holdout set that AutoML search will take for datasets larger than 500 rows. If set to 0, holdout set will not be taken regardless of number of rows. Must be between 0 and 1, exclusive. Defaults to 0.1.
 
         use_recommendation (bool): Whether or not to use a recommendation score to rank pipelines instead of optimization objective. Defaults to False.
 
         include_recommendation (list[str]): A list of objectives to include beyond the defaults in the recommendation score. Defaults to None.
 
         exclude_recommendation (list[str]): A list of objectives to exclude from the defaults in the recommendation score. Defaults to None.
@@ -462,14 +464,15 @@
         max_iterations=None,
         max_time=None,
         patience=None,
         tolerance=None,
         data_splitter=None,
         allowed_component_graphs=None,
         allowed_model_families=None,
+        excluded_model_families=None,
         features=None,
         start_iteration_callback=None,
         add_result_callback=None,
         error_callback=None,
         additional_objectives=None,
         alternate_thresholding_objective="F1",
         random_seed=0,
@@ -602,14 +605,15 @@
                     "Parameter allowed_component_graphs must be either None or a dictionary!",
                 )
             for graph_name, graph in allowed_component_graphs.items():
                 if not isinstance(graph, (list, dict, ComponentGraph)):
                     raise ValueError(
                         "Every component graph passed must be of type list, dictionary, or ComponentGraph!",
                     )
+
         self.allowed_component_graphs = allowed_component_graphs
         self.allowed_model_families = allowed_model_families
         self.allow_long_running_models = allow_long_running_models
         self._start = 0.0
         self._baseline_cv_scores = {}
         self.show_batch_output = False
 
@@ -837,14 +841,26 @@
                 and "DatetimeFeaturizer" not in exclude_featurizers
             ):
                 raise ValueError(
                     "For time series problems, if TimeSeriesFeaturizer is excluded, must also exclude DatetimeFeaturizer",
                 )
         self.exclude_featurizers = exclude_featurizers or []
 
+        if excluded_model_families:
+            if not isinstance(excluded_model_families, list):
+                raise ValueError(
+                    "`excluded_model_families` must be passed in the form of a list.",
+                )
+            if not all(isinstance(x, ModelFamily) for x in excluded_model_families):
+                raise ValueError(
+                    "All values in `excluded_model_families` must be of type `ModelFamily`.",
+                )
+
+        self.excluded_model_families = excluded_model_families
+
         if is_classification(self.problem_type):
             self._sampler_name = self.sampler_method
             if self.sampler_method == "auto":
                 self._sampler_name = get_best_sampler_for_data(
                     self.X_train,
                     self.y_train,
                     self.sampler_method,
@@ -894,14 +910,15 @@
             self.automl_algorithm = IterativeAlgorithm(
                 X=self.X_train,
                 y=self.y_train,
                 problem_type=self.problem_type,
                 sampler_name=self._sampler_name,
                 allowed_component_graphs=self.allowed_component_graphs,
                 allowed_model_families=self.allowed_model_families,
+                excluded_model_families=self.excluded_model_families,
                 max_iterations=self.max_iterations,
                 max_batches=self.max_batches,
                 tuner_class=self.tuner_class,
                 random_seed=self.random_seed,
                 n_jobs=self.n_jobs,
                 number_features=self.X_train.shape[1],
                 pipelines_per_batch=self._pipelines_per_batch,
@@ -915,14 +932,16 @@
             )
         elif automl_algorithm == "default":
             self.automl_algorithm = DefaultAlgorithm(
                 X=self.X_train,
                 y=self.y_train,
                 problem_type=self.problem_type,
                 sampler_name=self._sampler_name,
+                allowed_model_families=self.allowed_model_families,
+                excluded_model_families=self.excluded_model_families,
                 tuner_class=self.tuner_class,
                 random_seed=self.random_seed,
                 search_parameters=internal_search_parameters,
                 text_in_ensembling=text_in_ensembling,
                 allow_long_running_models=allow_long_running_models,
                 features=features,
                 ensembling=self.ensembling,
@@ -1710,14 +1729,38 @@
                 pd.Series(recommendation_scores.values()),
             )
 
         rankings_df.sort_values(ranking_column, ascending=ascending, inplace=True)
         rankings_df.reset_index(drop=True, inplace=True)
         return rankings_df
 
+    def get_recommendation_score_breakdown(self, pipeline_id):
+        """Reports the scores for the objectives used in the given pipeline's recommendation score calculation.
+
+        Note that these scores are reported in their raw form, not scaled to be between 0 and 1.
+
+        Args:
+            pipeline_id (int): The id of the pipeline to get the recommendation score breakdown for.
+
+        Returns:
+            dict: A dictionary of the scores for each objective used in the recommendation score calculation.
+        """
+        if len(self.recommendation_objectives) == 0:
+            self.recommendation_objectives = get_default_recommendation_objectives(
+                self.problem_type,
+            )
+        all_objectives = self._results["pipeline_results"][pipeline_id][
+            "ranking_additional_objectives"
+        ]
+        rec_objectives = {
+            objective: all_objectives[objective]
+            for objective in self.recommendation_objectives
+        }
+        return rec_objectives
+
     def get_recommendation_scores(
         self,
         priority=None,
         custom_weights=None,
         use_pipeline_names=False,
     ):
         """Calculates recommendation scores for all pipelines in the search results.
```

### Comparing `evalml-0.76.0/evalml/automl/callbacks.py` & `evalml-0.77.0/evalml/automl/callbacks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/automl/engine/cf_engine.py` & `evalml-0.77.0/evalml/automl/engine/cf_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/automl/engine/dask_engine.py` & `evalml-0.77.0/evalml/automl/engine/dask_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/automl/engine/engine_base.py` & `evalml-0.77.0/evalml/automl/engine/engine_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/automl/engine/sequential_engine.py` & `evalml-0.77.0/evalml/automl/engine/sequential_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/automl/pipeline_search_plots.py` & `evalml-0.77.0/evalml/automl/pipeline_search_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/automl/progress.py` & `evalml-0.77.0/evalml/automl/progress.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/automl/utils.py` & `evalml-0.77.0/evalml/automl/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/__init__.py` & `evalml-0.77.0/evalml/data_checks/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/class_imbalance_data_check.py` & `evalml-0.77.0/evalml/data_checks/class_imbalance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/data_check.py` & `evalml-0.77.0/evalml/data_checks/data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/data_check_action.py` & `evalml-0.77.0/evalml/data_checks/data_check_action.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/data_check_action_code.py` & `evalml-0.77.0/evalml/data_checks/data_check_action_code.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/data_check_action_option.py` & `evalml-0.77.0/evalml/data_checks/data_check_action_option.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/data_check_message.py` & `evalml-0.77.0/evalml/data_checks/data_check_message.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/data_check_message_code.py` & `evalml-0.77.0/evalml/data_checks/data_check_message_code.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/data_checks.py` & `evalml-0.77.0/evalml/data_checks/data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/datetime_format_data_check.py` & `evalml-0.77.0/evalml/data_checks/datetime_format_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/default_data_checks.py` & `evalml-0.77.0/evalml/data_checks/default_data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/id_columns_data_check.py` & `evalml-0.77.0/evalml/data_checks/id_columns_data_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,23 @@
 
 
 class IDColumnsDataCheck(DataCheck):
     """Check if any of the features are likely to be ID columns.
 
     Args:
         id_threshold (float): The probability threshold to be considered an ID column. Defaults to 1.0.
+        exclude_time_index (bool): If True, the column set as the time index will not be
+            included in the data check. Default is True.
     """
 
-    def __init__(self, id_threshold=1.0):
+    def __init__(self, id_threshold=1.0, exclude_time_index=True):
         if id_threshold < 0 or id_threshold > 1:
             raise ValueError("id_threshold must be a float between 0 and 1, inclusive.")
         self.id_threshold = id_threshold
+        self.exclude_time_index = exclude_time_index
 
     def validate(self, X, y=None):
         """Check if any of the features are likely to be ID columns. Currently performs a number of simple checks.
 
         Checks performed are:
 
             - column name is "id"
@@ -164,14 +167,16 @@
             ...             }
             ...         ]
             ...    }
             ... ]
         """
         messages = []
         X = infer_feature_types(X)
+        if X.ww.time_index and self.exclude_time_index:
+            X = X.ww.select(exclude="time_index")
 
         col_names = [col for col in X.columns]
         cols_named_id = [
             col for col in col_names if (str(col).lower() == "id")
         ]  # columns whose name is "id"
         id_cols = {col: 0.95 for col in cols_named_id}
```

### Comparing `evalml-0.76.0/evalml/data_checks/invalid_target_data_check.py` & `evalml-0.77.0/evalml/data_checks/invalid_target_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/multicollinearity_data_check.py` & `evalml-0.77.0/evalml/data_checks/multicollinearity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/no_variance_data_check.py` & `evalml-0.77.0/evalml/data_checks/no_variance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/null_data_check.py` & `evalml-0.77.0/evalml/data_checks/null_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/outliers_data_check.py` & `evalml-0.77.0/evalml/data_checks/outliers_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/sparsity_data_check.py` & `evalml-0.77.0/evalml/data_checks/sparsity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/target_distribution_data_check.py` & `evalml-0.77.0/evalml/data_checks/target_distribution_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/target_leakage_data_check.py` & `evalml-0.77.0/evalml/data_checks/target_leakage_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/ts_parameters_data_check.py` & `evalml-0.77.0/evalml/data_checks/ts_parameters_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/ts_splitting_data_check.py` & `evalml-0.77.0/evalml/data_checks/ts_splitting_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/uniqueness_data_check.py` & `evalml-0.77.0/evalml/data_checks/uniqueness_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/data_checks/utils.py` & `evalml-0.77.0/evalml/data_checks/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/demos/breast_cancer.py` & `evalml-0.77.0/evalml/demos/breast_cancer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/demos/churn.py` & `evalml-0.77.0/evalml/demos/churn.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/demos/data/churn.csv` & `evalml-0.77.0/evalml/demos/data/churn.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/demos/data/daily-min-temperatures.csv` & `evalml-0.77.0/evalml/demos/data/daily-min-temperatures.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/demos/data/fraud_transactions.csv.gz` & `evalml-0.77.0/evalml/demos/data/fraud_transactions.csv.gz`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/demos/diabetes.py` & `evalml-0.77.0/evalml/demos/diabetes.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/demos/fraud.py` & `evalml-0.77.0/evalml/demos/fraud.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/demos/weather.py` & `evalml-0.77.0/evalml/demos/weather.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/demos/wine.py` & `evalml-0.77.0/evalml/demos/wine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/exceptions/__init__.py` & `evalml-0.77.0/evalml/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/exceptions/exceptions.py` & `evalml-0.77.0/evalml/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_family/model_family.py` & `evalml-0.77.0/evalml/model_family/model_family.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_family/utils.py` & `evalml-0.77.0/evalml/model_family/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/__init__.py` & `evalml-0.77.0/evalml/model_understanding/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py` & `evalml-0.77.0/evalml/model_understanding/_partial_dependence_fast_mode_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/_partial_dependence_utils.py` & `evalml-0.77.0/evalml/model_understanding/_partial_dependence_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/decision_boundary.py` & `evalml-0.77.0/evalml/model_understanding/decision_boundary.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/feature_explanations.py` & `evalml-0.77.0/evalml/model_understanding/feature_explanations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/force_plots.py` & `evalml-0.77.0/evalml/model_understanding/force_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/metrics.py` & `evalml-0.77.0/evalml/model_understanding/metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Standard metrics used for model understanding."""
 import warnings
 
 import numpy as np
 import pandas as pd
+from scipy.stats import chisquare, kstest, wilcoxon
 from sklearn.metrics import auc as sklearn_auc
 from sklearn.metrics import confusion_matrix as sklearn_confusion_matrix
 from sklearn.metrics import precision_recall_curve as sklearn_precision_recall_curve
 from sklearn.metrics import roc_curve as sklearn_roc_curve
 from sklearn.preprocessing import LabelBinarizer
 from sklearn.utils.multiclass import unique_labels
 
 from evalml.exceptions import NoPositiveLabelException
+from evalml.problem_types import is_classification, is_regression, is_time_series
 from evalml.utils import import_or_raise, infer_feature_types, jupyter_check
 
 
 def confusion_matrix(y_true, y_predicted, normalize_method="true"):
     """Confusion matrix for binary and multiclass classification.
 
     Args:
@@ -356,7 +358,38 @@
             x=[0, 1],
             y=[0, 1],
             name="Trivial Model (AUC 0.5)",
             line=dict(dash="dash"),
         ),
     )
     return _go.Figure(layout=layout, data=graph_data)
+
+
+def check_distribution(y_true, y_pred, problem_type, threshold=0.1):
+    """Determines if the distribution of the predicted data is likely to match that of the ground truth data.
+
+    Will use a different statistical test based on the given problem type:
+    - Classification (Binary or Multiclass) - chi squared test
+    - Regression - Kolmogorov-Smirnov test
+    - Time Series Regression  - Wilcoxon signed-rank test
+    Args:
+        y_true (pd.Series): The ground truth data.
+        y_pred (pd.Series): Predictions from a pipeline.
+        problem_type (str or ProblemType): The pipeline's problem type, used to determine the method.
+        threshold (float): The threshold for the p value where we choose to accept or reject the null hypothesis.
+            Should be between 0 and 1, non-inclusive. Defaults to 0.1.
+
+    Returns:
+        int: 0 if the distribution of predicted values is not likely to match the true distribution, 1 if it is.
+    """
+    if is_classification(problem_type):
+        true_value_counts = y_true.value_counts()
+        pred_value_counts = y_pred.value_counts()
+        # Prevents an error in the baseline case where only one class is predicted
+        if len(true_value_counts) != len(pred_value_counts):
+            return 0
+        p_value = chisquare(pred_value_counts, f_exp=true_value_counts).pvalue
+    elif is_time_series(problem_type):
+        p_value = wilcoxon(y_true, y_pred).pvalue
+    elif is_regression(problem_type):
+        p_value = kstest(y_true, y_pred).pvalue
+    return 0 if p_value < threshold else 1
```

### Comparing `evalml-0.76.0/evalml/model_understanding/partial_dependence_functions.py` & `evalml-0.77.0/evalml/model_understanding/partial_dependence_functions.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/permutation_importance.py` & `evalml-0.77.0/evalml/model_understanding/permutation_importance.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/prediction_explanations/_algorithms.py` & `evalml-0.77.0/evalml/model_understanding/prediction_explanations/_algorithms.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py` & `evalml-0.77.0/evalml/model_understanding/prediction_explanations/_report_creator_factory.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/prediction_explanations/_user_interface.py` & `evalml-0.77.0/evalml/model_understanding/prediction_explanations/_user_interface.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/prediction_explanations/explainers.py` & `evalml-0.77.0/evalml/model_understanding/prediction_explanations/explainers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/model_understanding/visualizations.py` & `evalml-0.77.0/evalml/model_understanding/visualizations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/objectives/__init__.py` & `evalml-0.77.0/evalml/objectives/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/objectives/binary_classification_objective.py` & `evalml-0.77.0/evalml/objectives/binary_classification_objective.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/objectives/cost_benefit_matrix.py` & `evalml-0.77.0/evalml/objectives/cost_benefit_matrix.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/objectives/fraud_cost.py` & `evalml-0.77.0/evalml/objectives/fraud_cost.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/objectives/lead_scoring.py` & `evalml-0.77.0/evalml/objectives/lead_scoring.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/objectives/objective_base.py` & `evalml-0.77.0/evalml/objectives/objective_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/objectives/sensitivity_low_alert.py` & `evalml-0.77.0/evalml/objectives/sensitivity_low_alert.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/objectives/standard_metrics.py` & `evalml-0.77.0/evalml/objectives/standard_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/objectives/utils.py` & `evalml-0.77.0/evalml/objectives/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/__init__.py` & `evalml-0.77.0/evalml/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/binary_classification_pipeline.py` & `evalml-0.77.0/evalml/pipelines/binary_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/binary_classification_pipeline_mixin.py` & `evalml-0.77.0/evalml/pipelines/binary_classification_pipeline_mixin.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/classification_pipeline.py` & `evalml-0.77.0/evalml/pipelines/classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/component_graph.py` & `evalml-0.77.0/evalml/pipelines/component_graph.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/__init__.py` & `evalml-0.77.0/evalml/pipelines/components/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/component_base.py` & `evalml-0.77.0/evalml/pipelines/components/component_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/component_base_meta.py` & `evalml-0.77.0/evalml/pipelines/components/component_base_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py` & `evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/ensemble/stacked_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/__init__.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/__init__.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/elasticnet_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/et_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/kneighbors_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/lightgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/rf_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/svm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/vowpal_wabbit_classifiers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/classifiers/xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/estimator.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/estimator.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/__init__.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/arima_regressor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Autoregressive Integrated Moving Average Model. The three parameters (p, d, q) are the AR order, the degree of differencing, and the MA order. More information here: https://www.statsmodels.org/devel/generated/statsmodels.tsa.arima.model.ARIMA.html."""
 from typing import Dict, Hashable, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
+from pandas.api.types import is_integer_dtype
 from skopt.space import Integer
 
 from evalml.model_family import ModelFamily
 from evalml.pipelines.components.estimators import Estimator
 from evalml.problem_types import ProblemTypes
 from evalml.utils import (
     import_or_raise,
@@ -150,32 +151,33 @@
                 y.index = X.index
         return X, y
 
     def _set_forecast(self, X: pd.DataFrame):
         from sktime.forecasting.base import ForecastingHorizon
 
         # we can only calculate the difference if the indices are of the same type
-        if isinstance(X.index[0], type(self.last_X_index)):
-            units_diff = X.index[0] - self.last_X_index
-            if isinstance(X.index, pd.DatetimeIndex):
-                dates_diff = pd.date_range(
-                    start=self.last_X_index,
-                    end=X.index[0],
-                    freq=X.index.freq,
-                )
-                units_diff = len(dates_diff) - 1
-            fh_ = ForecastingHorizon(
-                [units_diff + i for i in range(len(X))],
-                is_relative=True,
-            )
-        else:
-            fh_ = ForecastingHorizon(
-                [i + 1 for i in range(len(X))],
-                is_relative=True,
+        units_diff = 1
+        if isinstance(X.index[0], type(self.last_X_index)) and isinstance(
+            X.index,
+            pd.DatetimeIndex,
+        ):
+            dates_diff = pd.date_range(
+                start=self.last_X_index,
+                end=X.index[0],
+                freq=X.index.freq,
             )
+            units_diff = len(dates_diff) - 1
+        elif is_integer_dtype(type(X.index[0])) and is_integer_dtype(
+            type(self.last_X_index),
+        ):
+            units_diff = X.index[0] - self.last_X_index
+        fh_ = ForecastingHorizon(
+            [units_diff + i for i in range(len(X))],
+            is_relative=True,
+        )
         return fh_
 
     def _get_sp(self, X: pd.DataFrame) -> int:
         if X is None:
             return 1
         freq_mappings = {
             "D": 7,
@@ -209,15 +211,15 @@
         if X is not None:
             X = X.ww.fillna(X.mean())
         if y is None:
             raise ValueError("ARIMA Regressor requires y as input.")
 
         sp = self._get_sp(X)
         self._component_obj.sp = sp
-        self.last_X_index = X.index[-1] if X is not None else y.index
+        self.last_X_index = X.index[-1] if X is not None else y.index[-1]
 
         X = self._remove_datetime(X, features=True)
 
         if X is not None:
             X.ww.set_types(
                 {
                     col: "Double"
@@ -275,15 +277,20 @@
             if fh_[0] != 1:
                 # pmdarima (which sktime uses under the hood) only forecasts off the training data
                 # but sktime circumvents this by predicting everything from the end of training data to the date / periods requested
                 # and only returning the values for dates / periods given to sktime. Because of this,
                 # pmdarima requires the number of covariate rows to equal the length of the total number of periods (X.shape[0] == fh_[-1]) if covariates are used.
                 # We circument this by adding arbitrary rows to the start of X since sktime discards these values when predicting.
                 num_rows_diff = fh_[-1] - X.shape[0]
-                X_ = pd.concat([X.head(num_rows_diff), X], ignore_index=True)
+                filler = pd.DataFrame(
+                    columns=X.columns,
+                    index=range(num_rows_diff),
+                ).fillna(0)
+                X_ = pd.concat([filler, X], ignore_index=True)
+                X_.ww.init(schema=X.ww.schema)
             else:
                 X_ = X
             y_pred_intervals = self._component_obj.predict_interval(
                 fh=fh_,
                 X=X_,
                 coverage=[0.95],
             )
```

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/baseline_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/catboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/elasticnet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/et_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/et_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/exponential_smoothing_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/lightgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/linear_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/prophet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/rf_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/svm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/time_series_baseline_estimator.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/vowpal_wabbit_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py` & `evalml-0.77.0/evalml/pipelines/components/estimators/regressors/xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/__init__.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/column_selectors.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/column_selectors.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/lda.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/dimensionality_reduction/pca.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/encoders/label_encoder.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/encoders/label_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/encoders/onehot_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/encoders/ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/encoders/target_encoder.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/encoders/target_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/__init__.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/recursive_feature_elimination_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/rf_classifier_feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/feature_selection/rf_regressor_feature_selector.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/__init__.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/imputer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/knn_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/simple_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/target_imputer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/target_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/imputers/time_series_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/__init__.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/datetime_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_nan_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_null_columns.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/drop_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/featuretools.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/log_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/lsa.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/lsa.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/natural_language_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/polynomial_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/replace_nullable_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/stl_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/text_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/time_series_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/time_series_regularizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/preprocessing/transform_primitive_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/samplers/base_sampler.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/samplers/base_sampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/samplers/oversampler.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/samplers/oversampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/samplers/undersampler.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/samplers/undersampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/scalers/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/transformers/transformer.py` & `evalml-0.77.0/evalml/pipelines/components/transformers/transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/components/utils.py` & `evalml-0.77.0/evalml/pipelines/components/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,39 +52,49 @@
             for problem in estimator.supported_problem_types
         ):
             estimators.append(estimator)
 
     return list(set([e.model_family for e in estimators]))
 
 
-def get_estimators(problem_type, model_families=None):
+def get_estimators(problem_type, model_families=None, excluded_model_families=None):
     """Returns the estimators allowed for a particular problem type.
 
     Can also optionally filter by a list of model types.
 
     Args:
         problem_type (ProblemTypes or str): Problem type to filter for.
         model_families (list[ModelFamily] or list[str]): Model families to filter for.
+        excluded_model_families (list[ModelFamily]): A list of model families to exclude from the results.
 
     Returns:
         list[class]: A list of estimator subclasses.
 
     Raises:
         TypeError: If the model_families parameter is not a list.
         RuntimeError: If a model family is not valid for the problem type.
     """
+    if model_families not in (None, []) and excluded_model_families not in (None, []):
+        raise ValueError(
+            "Both `model_families` and `excluded_model_families` cannot be set.",
+        )
     if model_families is not None and not isinstance(model_families, list):
         raise TypeError("model_families parameter is not a list.")
     problem_type = handle_problem_types(problem_type)
     if model_families is None:
         model_families = allowed_model_families(problem_type)
+    if excluded_model_families is None:
+        excluded_model_families = []
 
     model_families = [
         handle_model_family(model_family) for model_family in model_families
     ]
+    excluded_model_families = [
+        handle_model_family(model_family) for model_family in excluded_model_families
+    ]
     all_model_families = allowed_model_families(problem_type)
     for model_family in model_families:
         if model_family not in all_model_families:
             raise RuntimeError(
                 "Unrecognized model type for problem type %s: %s"
                 % (problem_type, model_family),
             )
@@ -92,14 +102,16 @@
     estimator_classes = []
     for estimator_class in _all_estimators_used_in_search():
         if problem_type not in [
             handle_problem_types(supported_pt)
             for supported_pt in estimator_class.supported_problem_types
         ]:
             continue
+        if estimator_class.model_family in excluded_model_families:
+            continue
         if estimator_class.model_family not in model_families:
             continue
         estimator_classes.append(estimator_class)
     return estimator_classes
 
 
 def estimator_unable_to_handle_nans(estimator_class):
```

### Comparing `evalml-0.76.0/evalml/pipelines/multiclass_classification_pipeline.py` & `evalml-0.77.0/evalml/pipelines/multiclass_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/pipeline_base.py` & `evalml-0.77.0/evalml/pipelines/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/pipeline_meta.py` & `evalml-0.77.0/evalml/pipelines/pipeline_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/regression_pipeline.py` & `evalml-0.77.0/evalml/pipelines/regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/time_series_classification_pipelines.py` & `evalml-0.77.0/evalml/pipelines/time_series_classification_pipelines.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/time_series_pipeline_base.py` & `evalml-0.77.0/evalml/pipelines/time_series_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/pipelines/time_series_regression_pipeline.py` & `evalml-0.77.0/evalml/pipelines/time_series_regression_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,46 +110,45 @@
         Args:
             X (pd.DataFrame, np.ndarray): Data the pipeline was trained on of shape [n_samples_train, n_feautures].
 
         Raises:
             ValueError: If pipeline is not trained.
 
         Returns:
-            pd.Series: Datetime periods out to `forecast_horizon + gap`.
+            pd.Series: Datetime periods from `gap` to `forecast_horizon + gap`.
 
         Example:
             >>> X = pd.DataFrame({'date': pd.date_range(start='1-1-2022', periods=10, freq='D'), 'feature': range(10, 20)})
             >>> y = pd.Series(range(0, 10), name='target')
             >>> gap = 1
             >>> forecast_horizon = 2
             >>> pipeline = TimeSeriesRegressionPipeline(component_graph=["Linear Regressor"],
             ...                                         parameters={"Simple Imputer": {"impute_strategy": "mean"},
             ...                                                     "pipeline": {"gap": gap, "max_delay": 1, "forecast_horizon": forecast_horizon, "time_index": "date"}},
             ...                                        )
             >>> pipeline.fit(X, y)
             pipeline = TimeSeriesRegressionPipeline(component_graph={'Linear Regressor': ['Linear Regressor', 'X', 'y']}, parameters={'Linear Regressor':{'fit_intercept': True, 'n_jobs': -1}, 'pipeline':{'gap': 1, 'max_delay': 1, 'forecast_horizon': 2, 'time_index': 'date'}}, random_seed=0)
             >>> dates = pipeline.get_forecast_period(X)
-            >>> expected = pd.Series(pd.date_range(start='2022-01-11', periods=(gap + forecast_horizon), freq='D'), name='date', index=[10, 11, 12])
+            >>> expected = pd.Series(pd.date_range(start='2022-01-11', periods=forecast_horizon, freq='D').shift(gap), name='date', index=[10, 11])
             >>> assert dates.equals(expected)
         """
         if not self._is_fitted:
             raise ValueError("Pipeline must be fitted before getting forecast.")
 
         X = infer_feature_types(X)
 
         # Generate prediction periods
         first_date = X.iloc[-1][self.time_index]
         predicted_date_range = pd.Series(
             pd.date_range(
                 start=first_date,
                 periods=self.forecast_horizon
-                + self.gap
                 + 1,  # Add additional period to account for dropping first date row
                 freq=self.frequency,
-            ),
+            ).shift(self.gap),
         )
 
         # Generate numerical index
         first_idx = len(X) - 1 if not isinstance(X.index.dtype, int) else X.index[-1]
         num_idx = pd.Series(range(first_idx, first_idx + predicted_date_range.size))
         predicted_date_range.index = num_idx
 
@@ -161,15 +160,15 @@
         """Generates all possible forecasting predictions based on last period of X.
 
         Args:
             X (pd.DataFrame, np.ndarray): Data the pipeline was trained on of shape [n_samples_train, n_feautures].
             y (pd.Series, np.ndarray): Targets used to train the pipeline of shape [n_samples_train].
 
         Returns:
-            Predictions out to `forecast_horizon + gap` periods.
+            Predictions from `gap` periods out to `forecast_horizon + gap` periods.
         """
         X, y = self._convert_to_woodwork(X, y)
         pred_dates = pd.DataFrame(self.get_forecast_period(X))
         preds = self.predict(pred_dates, objective=None, X_train=X, y_train=y)
         return preds
 
     def get_prediction_intervals(
```

### Comparing `evalml-0.76.0/evalml/pipelines/utils.py` & `evalml-0.77.0/evalml/pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/preprocessing/data_splitters/no_split.py` & `evalml-0.77.0/evalml/preprocessing/data_splitters/no_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/preprocessing/data_splitters/sk_splitters.py` & `evalml-0.77.0/evalml/preprocessing/data_splitters/sk_splitters.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/preprocessing/data_splitters/time_series_split.py` & `evalml-0.77.0/evalml/preprocessing/data_splitters/time_series_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/preprocessing/data_splitters/training_validation_split.py` & `evalml-0.77.0/evalml/preprocessing/data_splitters/training_validation_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/preprocessing/utils.py` & `evalml-0.77.0/evalml/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/problem_types/problem_types.py` & `evalml-0.77.0/evalml/problem_types/problem_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/problem_types/utils.py` & `evalml-0.77.0/evalml/problem_types/utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/dask_test_utils.py` & `evalml-0.77.0/evalml/tests/automl_tests/dask_test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py` & `evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_automl_dask.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py` & `evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_cf_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py` & `evalml-0.77.0/evalml/tests/automl_tests/parallel_tests/test_dask_engine.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_automl.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_automl.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 )
 from evalml.objectives.utils import (
     get_all_objective_names,
     get_core_objectives,
     get_default_recommendation_objectives,
     get_non_core_objectives,
     get_objective,
+    get_optimization_objectives,
 )
 from evalml.pipelines import (
     BinaryClassificationPipeline,
     ComponentGraph,
     MulticlassClassificationPipeline,
     PipelineBase,
     RegressionPipeline,
@@ -66,14 +67,16 @@
 )
 from evalml.pipelines.components import (
     ARIMARegressor,
     DateTimeFeaturizer,
     DecisionTreeClassifier,
     EmailFeaturizer,
     NaturalLanguageFeaturizer,
+    RandomForestClassifier,
+    SelectColumns,
     TimeSeriesFeaturizer,
     URLFeaturizer,
 )
 from evalml.pipelines.utils import (
     _get_pipeline_base_class,
     _make_stacked_ensemble_pipeline,
 )
@@ -5228,14 +5231,82 @@
             problem_configuration=problem_configuration,
             exclude_featurizers=[
                 "TimeSeriesFeaturizer",
             ],
         )
 
 
+@pytest.mark.parametrize("automl_algorithm", ["default", "iterative"])
+def test_excluded_model_families(
+    automl_algorithm,
+    X_y_binary,
+    AutoMLTestEnv,
+):
+    X, y = X_y_binary
+
+    automl = AutoMLSearch(
+        X_train=X,
+        y_train=y,
+        problem_type=ProblemTypes.BINARY,
+        automl_algorithm=automl_algorithm,
+        excluded_model_families=[ModelFamily.RANDOM_FOREST],
+    )
+
+    env = AutoMLTestEnv(ProblemTypes.BINARY)
+    with env.test_context(score_return_value={automl.objective.name: 1.0}):
+        automl.search()
+
+    pipelines = [
+        automl.get_pipeline(i) for i in range(len(automl.results["pipeline_results"]))
+    ]
+
+    for pl in pipelines:
+        # Accounts for case in default algorithm where we only exclude Random Forest for third batch
+        # (e.g. only after feature selection occurs).
+        if (
+            automl_algorithm == "default"
+            and RandomForestClassifier.name in pl.component_graph.compute_order
+        ):
+            assert SelectColumns.name not in pl.component_graph.compute_order
+        else:
+            assert RandomForestClassifier.name not in pl.component_graph.compute_order
+
+
+def test_excluded_model_families_error(
+    X_y_binary,
+):
+    X, y = X_y_binary
+
+    match_text = "`excluded_model_families` must be passed in the form of a list."
+    with pytest.raises(
+        ValueError,
+        match=match_text,
+    ):
+        AutoMLSearch(
+            X_train=X,
+            y_train=y,
+            problem_type=ProblemTypes.BINARY,
+            excluded_model_families=ModelFamily.RANDOM_FOREST,
+        )
+
+    match_text = (
+        "All values in `excluded_model_families` must be of type `ModelFamily`."
+    )
+    with pytest.raises(
+        ValueError,
+        match=match_text,
+    ):
+        AutoMLSearch(
+            X_train=X,
+            y_train=y,
+            problem_type=ProblemTypes.BINARY,
+            excluded_model_families=[ModelFamily.RANDOM_FOREST, "XGBoost"],
+        )
+
+
 def test_init_holdout_set(X_y_binary, caplog):
     X, y = X_y_binary
     X_train, X_holdout, y_train, y_holdout = split_data(X, y, "binary")
 
     match_text = "Must specify training data target values as a 1d vector using the y_holdout argument"
     with pytest.raises(
         ValueError,
@@ -5488,14 +5559,47 @@
     assert_series_equal(
         automl.rankings["holdout_score"],
         automl.rankings["ranking_score"],
         check_names=False,
     )
 
 
+@pytest.mark.parametrize("problem_type", ["binary", "multiclass", "regression"])
+def test_get_recommendation_score_breakdown(problem_type, X_y_binary, AutoMLTestEnv):
+    X, y = X_y_binary
+
+    automl = AutoMLSearch(
+        X_train=X,
+        y_train=y,
+        problem_type=problem_type,
+    )
+
+    objectives = get_default_recommendation_objectives(problem_type)
+    all_objectives = get_optimization_objectives(problem_type)
+
+    env = AutoMLTestEnv(problem_type)
+    with env.test_context(
+        score_return_value={objective.name: 0.75 for objective in all_objectives},
+    ):
+        automl.search()
+
+    breakdown = automl.get_recommendation_score_breakdown(3)
+    assert isinstance(breakdown, dict)
+    # Should not have all objectives, just the recommendation ones
+    assert (
+        breakdown.keys()
+        != automl.results["pipeline_results"][3]["ranking_additional_objectives"]
+    )
+    assert breakdown.keys() == objectives
+
+    # check that the output scores are not normalized, even though the recommendation scores are
+    for score in breakdown.values():
+        assert score == 0.75
+
+
 def test_get_recommendation_scores(X_y_binary):
     X, y = X_y_binary
 
     # Test that we can still get recommendation scores without setting use_recommendation
     automl = AutoMLSearch(
         X_train=X,
         y_train=y,
@@ -5686,7 +5790,28 @@
     objectives = objectives - {"F1", "AUC"}
     with env.test_context(
         score_return_value={objective: 0.75 for objective in objectives},
     ):
         automl.search()
     custom_rankings = automl.rankings["recommendation_score"]
     assert all(default_rankings != custom_rankings)
+
+
+@pytest.mark.parametrize("automl_algorithm", ["iterative", "default"])
+def test_automl_allowed_graphs_and_families_both_set_error(
+    automl_algorithm,
+    X_y_binary,
+):
+    X, y = X_y_binary
+
+    error_text = (
+        "Both `allowed_model_families` and `excluded_model_families` cannot be set."
+    )
+    with pytest.raises(ValueError, match=error_text):
+        AutoMLSearch(
+            X_train=X,
+            y_train=y,
+            problem_type="binary",
+            allowed_model_families=[ModelFamily.RANDOM_FOREST],
+            excluded_model_families=[ModelFamily.XGBOOST],
+            automl_algorithm=automl_algorithm,
+        )
```

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_automl_algorithm.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_automl_algorithm.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_automl_iterative_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1139,7 +1139,25 @@
     error_text = "Pipeline ID 12 is not a valid ensemble pipeline"
     with pytest.raises(ValueError, match=error_text):
         automl.get_ensembler_input_pipelines(12)
 
     error_text = "Pipeline ID 500 is not a valid ensemble pipeline"
     with pytest.raises(ValueError, match=error_text):
         automl.get_ensembler_input_pipelines(500)
+
+
+def test_automl_allowed_graphs_and_families_both_set_error_iterative(
+    X_y_binary,
+):
+    X, y = X_y_binary
+    error_text = (
+        "Both `excluded_model_families` and `allowed_component_graphs` cannot be set."
+    )
+    with pytest.raises(ValueError, match=error_text):
+        AutoMLSearch(
+            X_train=X,
+            y_train=y,
+            problem_type="binary",
+            allowed_component_graphs={"Name_0": ["Imputer", "Linear Regressor"]},
+            excluded_model_families=[ModelFamily.XGBOOST],
+            automl_algorithm="iterative",
+        )
```

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_classification.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_classification_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_regression.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_regression.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_automl_search_regression_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_automl_utils.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_automl_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_default_algorithm.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_default_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1039,7 +1039,25 @@
     )
     assert not any(
         [
             TimeSeriesFeaturizer.name in pl.component_graph.compute_order
             for pl in pipelines
         ],
     )
+
+
+def test_default_algorithm_allowed_graphs_and_families_both_set_error(
+    X_y_binary,
+):
+    X, y = X_y_binary
+    error_text = (
+        "Both `allowed_model_families` and `excluded_model_families` cannot be set."
+    )
+    with pytest.raises(ValueError, match=error_text):
+        DefaultAlgorithm(
+            X=X,
+            y=y,
+            problem_type="binary",
+            allowed_model_families=[ModelFamily.RANDOM_FOREST],
+            excluded_model_families=[ModelFamily.XGBOOST],
+            sampler_name=None,
+        )
```

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_engine_base.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_engine_base.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_iterative_algorithm.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_iterative_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1134,7 +1134,36 @@
     )
     assert not any(
         [
             TimeSeriesFeaturizer.name in pl.component_graph.compute_order
             for pl in pipelines
         ],
     )
+
+
+def test_iterative_algorithm_allowed_graphs_and_families_both_set_error(
+    X_y_binary,
+):
+    X, y = X_y_binary
+    error_text = (
+        "Both `excluded_model_families` and `allowed_component_graphs` cannot be set."
+    )
+    with pytest.raises(ValueError, match=error_text):
+        IterativeAlgorithm(
+            X=X,
+            y=y,
+            problem_type="binary",
+            allowed_component_graphs={"Imputer": ["X", "y"]},
+            excluded_model_families=[ModelFamily.XGBOOST],
+        )
+
+    error_text = (
+        "Both `allowed_model_families` and `excluded_model_families` cannot be set."
+    )
+    with pytest.raises(ValueError, match=error_text):
+        IterativeAlgorithm(
+            X=X,
+            y=y,
+            problem_type="binary",
+            allowed_model_families=[ModelFamily.RANDOM_FOREST],
+            excluded_model_families=[ModelFamily.XGBOOST],
+        )
```

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_pipeline_search_plots.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_pipeline_search_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_progress.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_search.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_search_iterative.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_search_iterative.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/automl_tests/test_time_series_split.py` & `evalml-0.77.0/evalml/tests/automl_tests/test_time_series_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py` & `evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py` & `evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_polynomial_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py` & `evalml-0.77.0/evalml/tests/component_tests/decomposer_tests/test_stl_decomposer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_arima_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_arima_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,15 @@
     X_train, _, y_train = ts_data(
         train_features_index_dt=False,
         train_target_index_dt=False,
         train_none=False,
         datetime_feature=False,
         no_features=False,
         test_features_index_dt=False,
+        match_indices=False,
     )
 
     assert not X_train.index.equals(y_train.index)
 
     clf = ARIMARegressor()
     X_, y_ = clf._match_indices(X_train, y_train)
     assert X_.index.equals(y_.index)
@@ -267,14 +268,15 @@
     X_train, X_test, y_train = ts_data(
         train_features_index_dt,
         train_target_index_dt,
         train_none,
         datetime_feature,
         no_features,
         test_features_index_dt,
+        match_indices=False,
     )
 
     a_clf = AutoARIMA(maxiter=10)
     with pytest.raises(Exception):
         a_clf.fit(X=X_train, y=y_train)
 
     m_clf = ARIMARegressor(d=None)
@@ -471,14 +473,46 @@
     arima.fit(X_train, y_train)
 
     assert (
         arima.predict(X_test).tail(5).tolist() == arima.predict(X_test_last_5).tolist()
     )
 
 
+@pytest.mark.parametrize("use_covariates", [True, False])
+def test_arima_regressor_can_forecast_arbitrary_dates_past_holdout(
+    use_covariates,
+    ts_data,
+):
+    X, _, y = ts_data(
+        train_features_index_dt=False,
+        train_target_index_dt=False,
+    )
+
+    # Create a training and testing set that are not continuous
+    X_train, X_test, y_train, _ = split_data(
+        X,
+        y,
+        problem_type="time series regression",
+        test_size=0.1,
+        random_seed=0,
+    )
+    X_train, _, y_train, _ = split_data(
+        X_train,
+        y_train,
+        problem_type="time series regression",
+        test_size=0.4,
+        random_seed=0,
+    )
+
+    arima = ARIMARegressor(use_covariates=use_covariates)
+    arima.fit(X_train, y_train)
+
+    arima.predict(X_test)
+
+
 @pytest.mark.parametrize(
     "nullable_ltype",
     ["IntegerNullable", "AgeNullable"],
 )
 def test_arima_regressor_with_nullable_types(nullable_ltype):
     X = pd.DataFrame()
     X["nums"] = pd.Series([i for i in range(100)], dtype="Int64")
```

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_baseline_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_baseline_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_baseline_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_baseline_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_catboost_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_catboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_catboost_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_catboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_column_selector_transformers.py` & `evalml-0.77.0/evalml/tests/component_tests/test_column_selector_transformers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_components.py` & `evalml-0.77.0/evalml/tests/component_tests/test_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_datetime_featurizer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_datetime_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_decision_tree_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_decision_tree_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_decision_tree_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_drop_nan_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_drop_null_columns_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_drop_rows_transformer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_drop_rows_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_en_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_en_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_en_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_en_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_estimators.py` & `evalml-0.77.0/evalml/tests/component_tests/test_estimators.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_et_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_et_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_et_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_et_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_exponential_smoothing_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_feature_selectors.py` & `evalml-0.77.0/evalml/tests/component_tests/test_feature_selectors.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_featuretools.py` & `evalml-0.77.0/evalml/tests/component_tests/test_featuretools.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py` & `evalml-0.77.0/evalml/tests/component_tests/test_ft_transform_primitive_components.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_imputer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_knn_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_knn_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_knn_imputer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_knn_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_label_encoder.py` & `evalml-0.77.0/evalml/tests/component_tests/test_label_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_lda.py` & `evalml-0.77.0/evalml/tests/component_tests/test_lda.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_lgbm_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_lgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_lgbm_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_lgbm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_log_transformer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_log_transformer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_lsa.py` & `evalml-0.77.0/evalml/tests/component_tests/test_lsa.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_natural_language_featurizer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_natural_language_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_nullable_types_replacer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_nullable_types_replacer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_one_hot_encoder.py` & `evalml-0.77.0/evalml/tests/component_tests/test_one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_ordinal_encoder.py` & `evalml-0.77.0/evalml/tests/component_tests/test_ordinal_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_oversampler.py` & `evalml-0.77.0/evalml/tests/component_tests/test_oversampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_pca.py` & `evalml-0.77.0/evalml/tests/component_tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_per_column_imputer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_per_column_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_prophet_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_prophet_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_simple_imputer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_simple_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_stacked_ensemble_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_stacked_ensemble_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_standard_scaler.py` & `evalml-0.77.0/evalml/tests/component_tests/test_standard_scaler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_svm_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_svm_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_svm_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_svm_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_target_encoder.py` & `evalml-0.77.0/evalml/tests/component_tests/test_target_encoder.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_target_imputer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_target_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_time_series_featurizer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_time_series_featurizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_time_series_imputer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_time_series_imputer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_time_series_regularizer.py` & `evalml-0.77.0/evalml/tests/component_tests/test_time_series_regularizer.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_undersampler.py` & `evalml-0.77.0/evalml/tests/component_tests/test_undersampler.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_utils.py` & `evalml-0.77.0/evalml/tests/component_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_multiclass_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_vowpal_wabbit_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_xgboost_classifier.py` & `evalml-0.77.0/evalml/tests/component_tests/test_xgboost_classifier.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/component_tests/test_xgboost_regressor.py` & `evalml-0.77.0/evalml/tests/component_tests/test_xgboost_regressor.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/conftest.py` & `evalml-0.77.0/evalml/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,19 +313,22 @@
         train_target_index_dt=True,
         train_none=False,
         datetime_feature=True,
         no_features=False,
         test_features_index_dt=True,
         freq="D",
         problem_type="time series regression",
+        match_indices=True,
     ):
         X = pd.DataFrame(index=[i + 1 for i in range(50)])
         dates = pd.date_range("1/1/21", periods=50, freq=freq)
         feature = pd.Series([1, 4, 2] * 10 + [3, 1] * 10, index=X.index)
         y = pd.Series([1, 2, 3, 4, 5, 6, 5, 4, 3, 2] * 5)
+        if match_indices:
+            y.index = X.index
 
         X_train = X.iloc[:40]
         X_test = X.iloc[40:]
         y_train = y.iloc[:40]
         logical_types = {}
 
         if train_features_index_dt:
```

### Comparing `evalml-0.76.0/evalml/tests/data/churn.csv` & `evalml-0.77.0/evalml/tests/data/churn.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data/daily-min-temperatures.csv` & `evalml-0.77.0/evalml/tests/data/daily-min-temperatures.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data/fraud_transactions.csv.gz` & `evalml-0.77.0/evalml/tests/data/fraud_transactions.csv.gz`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data/tips.csv` & `evalml-0.77.0/evalml/tests/data/tips.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data/titanic.csv` & `evalml-0.77.0/evalml/tests/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_class_imbalance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_action.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_action.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_action_option.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_action_option.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_data_check_message.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_data_check_message.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_data_checks.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_data_checks.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_datetime_format_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_id_columns_data_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,25 +93,27 @@
             "234567890123456",
             "3456789012345678",
             "45678901234567",
         ],
         "Id": ["z", "y", "x", "a"],
         "col_5": ["0", "0", "1", "2"],
         "col_6": [0.1, 0.2, 0.3, 0.4],
+        "col_7_id": ["2023-01-01", "2023-01-02", "2023-01-03", "2023-01-04"],
     }
     X = pd.DataFrame.from_dict(X_dict)
     X.ww.init(
         logical_types={
             "col_1": "categorical",
             "col_2": "categorical",
             "Id": "categorical",
             "col_5": "categorical",
         },
+        time_index="col_7_id",
     )
-    id_cols_check = IDColumnsDataCheck(id_threshold=0.95)
+    id_cols_check = IDColumnsDataCheck(id_threshold=0.95, exclude_time_index=True)
     assert id_cols_check.validate(X) == [
         DataCheckWarning(
             message="Columns 'Id', 'col_2', 'col_3_id' are 95.0% or more likely to be an ID column",
             data_check_name=id_data_check_name,
             message_code=DataCheckMessageCode.HAS_ID_COLUMN,
             details={"columns": ["Id", "col_2", "col_3_id"]},
             action_options=[
@@ -120,14 +122,31 @@
                     data_check_name=id_data_check_name,
                     metadata={"columns": ["Id", "col_2", "col_3_id"]},
                 ),
             ],
         ).to_dict(),
     ]
 
+    id_cols_check = IDColumnsDataCheck(id_threshold=0.95, exclude_time_index=False)
+    assert id_cols_check.validate(X) == [
+        DataCheckWarning(
+            message="Columns 'Id', 'col_2', 'col_3_id', 'col_7_id' are 95.0% or more likely to be an ID column",
+            data_check_name=id_data_check_name,
+            message_code=DataCheckMessageCode.HAS_ID_COLUMN,
+            details={"columns": ["Id", "col_2", "col_3_id", "col_7_id"]},
+            action_options=[
+                DataCheckActionOption(
+                    DataCheckActionCode.DROP_COL,
+                    data_check_name=id_data_check_name,
+                    metadata={"columns": ["Id", "col_2", "col_3_id", "col_7_id"]},
+                ),
+            ],
+        ).to_dict(),
+    ]
+
     id_cols_check = IDColumnsDataCheck(id_threshold=1.0)
     assert id_cols_check.validate(X) == [
         DataCheckWarning(
             message="Columns 'Id', 'col_3_id' are 100.0% or more likely to be an ID column",
             data_check_name=id_data_check_name,
             message_code=DataCheckMessageCode.HAS_ID_COLUMN,
             details={"columns": ["Id", "col_3_id"]},
```

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_invalid_target_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_multicollinearity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_no_variance_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_null_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_null_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_outliers_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_outliers_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_sparsity_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_target_distribution_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_target_leakage_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_ts_parameters_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_ts_splitting_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_uniqueness_data_check.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/data_checks_tests/test_utils.py` & `evalml-0.77.0/evalml/tests/data_checks_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/demo_tests/test_datasets.py` & `evalml-0.77.0/evalml/tests/demo_tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt` & `evalml-0.77.0/evalml/tests/dependency_update_check/latest_dependency_versions.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 networkx==3.1
 nlp-primitives==2.11.0
 numpy==1.23.5
 packaging==23.1
 pandas==1.5.3
 plotly==5.14.1
 pmdarima==2.0.3
-pyzmq==25.0.2
+pyzmq==25.1.0
 scikit-learn==1.2.2
 scikit-optimize==0.9.0
-scipy==1.9.1
+scipy==1.10.1
 seaborn==0.12.2
 shap==0.41.0
 sktime==0.17.0
 statsmodels==0.14.0
 texttable==1.6.7
 tomli==2.0.1
 vowpalwabbit==9.8.0
-woodwork==0.23.0
+woodwork==0.24.0
 xgboost==1.7.5
```

### Comparing `evalml-0.76.0/evalml/tests/dependency_update_check/minimum_requirements.txt` & `evalml-0.77.0/evalml/tests/dependency_update_check/minimum_requirements.txt`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt` & `evalml-0.77.0/evalml/tests/dependency_update_check/minimum_test_requirements.txt`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py` & `evalml-0.77.0/evalml/tests/integration_tests/test_data_checks_and_actions_integration.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/integration_tests/test_nullable_types.py` & `evalml-0.77.0/evalml/tests/integration_tests/test_nullable_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/integration_tests/test_time_series_integration.py` & `evalml-0.77.0/evalml/tests/integration_tests/test_time_series_integration.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/model_family_tests/test_model_family.py` & `evalml-0.77.0/evalml/tests/model_family_tests/test_model_family.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py` & `evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_algorithms.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py` & `evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_explainers.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py` & `evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_force_plots.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py` & `evalml-0.77.0/evalml/tests/model_understanding_tests/prediction_explanations_tests/test_user_interface.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/model_understanding_tests/test_decision_boundary.py` & `evalml-0.77.0/evalml/tests/model_understanding_tests/test_decision_boundary.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/model_understanding_tests/test_feature_explanations.py` & `evalml-0.77.0/evalml/tests/model_understanding_tests/test_feature_explanations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/model_understanding_tests/test_metrics.py` & `evalml-0.77.0/evalml/tests/model_understanding_tests/test_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pandas as pd
 import pytest
 from sklearn.exceptions import UndefinedMetricWarning
 from sklearn.preprocessing import label_binarize
 
 from evalml.exceptions import NoPositiveLabelException
 from evalml.model_understanding.metrics import (
+    check_distribution,
     confusion_matrix,
     graph_confusion_matrix,
     graph_precision_recall_curve,
     graph_roc_curve,
     normalize_confusion_matrix,
     precision_recall_curve,
     roc_curve,
@@ -627,7 +628,27 @@
         import_check.assert_called_with("ipywidgets", warning=True)
     with pytest.warns(None) as graph_valid:
         rs = get_random_state(42)
         y_pred_proba = y * rs.random(y.shape)
         graph_roc_curve(y, y_pred_proba)
         assert len(graph_valid) == 0
         import_check.assert_called_with("ipywidgets", warning=True)
+
+
+@pytest.mark.parametrize(
+    "problem_type",
+    ["binary", "multiclass", "regression", "time series regression"],
+)
+@pytest.mark.parametrize("expected_distribution", ["matching", "not matching"])
+def test_check_distribution(problem_type, expected_distribution):
+    np.random.seed(0)
+    y_true = pd.Series(np.random.normal(size=500))
+    if expected_distribution == "matching":
+        y_pred = pd.Series(np.random.normal(size=500))
+    else:
+        y_pred = pd.Series([-2] * 500)
+
+    result = check_distribution(y_true, y_pred, problem_type)
+    if expected_distribution == "matching":
+        assert result == 1
+    else:
+        assert result == 0
```

### Comparing `evalml-0.76.0/evalml/tests/model_understanding_tests/test_partial_dependence.py` & `evalml-0.77.0/evalml/tests/model_understanding_tests/test_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/model_understanding_tests/test_permutation_importance.py` & `evalml-0.77.0/evalml/tests/model_understanding_tests/test_permutation_importance.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/model_understanding_tests/test_visualizations.py` & `evalml-0.77.0/evalml/tests/model_understanding_tests/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/objective_tests/test_binary_classification_objective.py` & `evalml-0.77.0/evalml/tests/objective_tests/test_binary_classification_objective.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py` & `evalml-0.77.0/evalml/tests/objective_tests/test_cost_benefit_matrix.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/objective_tests/test_fraud_detection.py` & `evalml-0.77.0/evalml/tests/objective_tests/test_fraud_detection.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/objective_tests/test_lead_scoring.py` & `evalml-0.77.0/evalml/tests/objective_tests/test_lead_scoring.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/objective_tests/test_objectives.py` & `evalml-0.77.0/evalml/tests/objective_tests/test_objectives.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/objective_tests/test_sla.py` & `evalml-0.77.0/evalml/tests/objective_tests/test_sla.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/objective_tests/test_standard_metrics.py` & `evalml-0.77.0/evalml/tests/objective_tests/test_standard_metrics.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py` & `evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_binary_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py` & `evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py` & `evalml-0.77.0/evalml/tests/pipeline_tests/classification_pipeline_tests/test_multiclass_classification.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py` & `evalml-0.77.0/evalml/tests/pipeline_tests/regression_pipeline_tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/pipeline_tests/test_component_graph.py` & `evalml-0.77.0/evalml/tests/pipeline_tests/test_component_graph.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/pipeline_tests/test_graphs.py` & `evalml-0.77.0/evalml/tests/pipeline_tests/test_graphs.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/pipeline_tests/test_pipeline_utils.py` & `evalml-0.77.0/evalml/tests/pipeline_tests/test_pipeline_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -627,14 +627,22 @@
         get_estimators(
             problem_type=ProblemTypes.REGRESSION,
             model_families="random_forest",
         )
     with pytest.raises(KeyError):
         get_estimators(problem_type="Not A Valid Problem Type")
 
+    match_text = "Both `model_families` and `excluded_model_families` cannot be set."
+    with pytest.raises(ValueError, match=match_text):
+        get_estimators(
+            ProblemTypes.REGRESSION,
+            model_families=[ModelFamily.RANDOM_FOREST],
+            excluded_model_families=[ModelFamily.XGBOOST],
+        )
+
 
 def test_generate_code_pipeline_errors():
     with pytest.raises(ValueError, match="Element must be a pipeline instance"):
         generate_pipeline_code(BinaryClassificationPipeline)
 
     with pytest.raises(ValueError, match="Element must be a pipeline instance"):
         generate_pipeline_code(RegressionPipeline)
```

### Comparing `evalml-0.76.0/evalml/tests/pipeline_tests/test_pipelines.py` & `evalml-0.77.0/evalml/tests/pipeline_tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py` & `evalml-0.77.0/evalml/tests/pipeline_tests/test_time_series_baseline_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,27 +103,27 @@
         match="Pipeline must be fitted before getting forecast.",
     ):
         clf.get_forecast_period(X)
 
     clf.fit(X, y)
     result = clf.get_forecast_period(X)
 
-    assert result.size == forecast_horizon + gap
-    assert all(result.index == range(len(X), len(X) + forecast_horizon + gap))
-    assert result.iloc[0] == X.iloc[-1]["date"] + np.timedelta64(1, clf.frequency)
+    assert result.size == forecast_horizon
+    assert all(result.index == range(len(X), len(X) + forecast_horizon))
+    assert result.iloc[0] == X.iloc[-1]["date"] + np.timedelta64(1 + gap, clf.frequency)
     assert np.issubdtype(result.dtype, np.datetime64)
     assert result.name == "date"
 
 
 @pytest.mark.parametrize("forecast_horizon,gap", [[3, 0], [10, 2], [2, 5]])
 def test_time_series_get_forecast_predictions(forecast_horizon, gap, ts_data):
     X, _, y = ts_data(problem_type=ProblemTypes.TIME_SERIES_REGRESSION)
 
     X_train, y_train = X.iloc[:15], y.iloc[:15]
-    X_validation = X.iloc[15 : (15 + gap + forecast_horizon)]
+    X_validation = X.iloc[15 + gap : (15 + gap + forecast_horizon)]
 
     clf = TimeSeriesRegressionPipeline(
         component_graph={
             "Time Series Featurizer": [
                 "Time Series Featurizer",
                 "X",
                 "y",
@@ -162,9 +162,8 @@
             },
         },
     )
 
     clf.fit(X_train, y_train)
     forecast_preds = clf.get_forecast_predictions(X=X_train, y=y_train)
     X_val_preds = clf.predict(X_validation, X_train=X_train, y_train=y_train)
-
     assert_series_equal(forecast_preds, X_val_preds)
```

### Comparing `evalml-0.76.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py` & `evalml-0.77.0/evalml/tests/pipeline_tests/test_time_series_pipeline.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/preprocessing_tests/test_no_split.py` & `evalml-0.77.0/evalml/tests/preprocessing_tests/test_no_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/preprocessing_tests/test_sk_splitters.py` & `evalml-0.77.0/evalml/tests/preprocessing_tests/test_sk_splitters.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/preprocessing_tests/test_split_data.py` & `evalml-0.77.0/evalml/tests/preprocessing_tests/test_split_data.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/preprocessing_tests/test_training_validation_split.py` & `evalml-0.77.0/evalml/tests/preprocessing_tests/test_training_validation_split.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/problem_type_tests/test_problem_types.py` & `evalml-0.77.0/evalml/tests/problem_type_tests/test_problem_types.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/test_all_test_dirs_included.py` & `evalml-0.77.0/evalml/tests/test_all_test_dirs_included.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/tuner_tests/test_grid_search_tuner.py` & `evalml-0.77.0/evalml/tests/tuner_tests/test_grid_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/tuner_tests/test_random_search_tuner.py` & `evalml-0.77.0/evalml/tests/tuner_tests/test_random_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/tuner_tests/test_skopt_tuner.py` & `evalml-0.77.0/evalml/tests/tuner_tests/test_skopt_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/utils_tests/test_cli_utils.py` & `evalml-0.77.0/evalml/tests/utils_tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/utils_tests/test_gen_utils.py` & `evalml-0.77.0/evalml/tests/utils_tests/test_gen_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/utils_tests/test_logger.py` & `evalml-0.77.0/evalml/tests/utils_tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/utils_tests/test_nullable_type_utils.py` & `evalml-0.77.0/evalml/tests/utils_tests/test_nullable_type_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tests/utils_tests/test_woodwork_utils.py` & `evalml-0.77.0/evalml/tests/utils_tests/test_woodwork_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tuners/grid_search_tuner.py` & `evalml-0.77.0/evalml/tuners/grid_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tuners/random_search_tuner.py` & `evalml-0.77.0/evalml/tuners/random_search_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tuners/skopt_tuner.py` & `evalml-0.77.0/evalml/tuners/skopt_tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/tuners/tuner.py` & `evalml-0.77.0/evalml/tuners/tuner.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/utils/__init__.py` & `evalml-0.77.0/evalml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/utils/base_meta.py` & `evalml-0.77.0/evalml/utils/base_meta.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/utils/cli_utils.py` & `evalml-0.77.0/evalml/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/utils/gen_utils.py` & `evalml-0.77.0/evalml/utils/gen_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/utils/logger.py` & `evalml-0.77.0/evalml/utils/logger.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/utils/nullable_type_utils.py` & `evalml-0.77.0/evalml/utils/nullable_type_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml/utils/woodwork_utils.py` & `evalml-0.77.0/evalml/utils/woodwork_utils.py`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml.egg-info/PKG-INFO` & `evalml-0.77.0/evalml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evalml
-Version: 0.76.0
+Version: 0.77.0
 Summary: an AutoML library that builds, optimizes, and evaluates machine learning pipelines using domain-specific objective functions
 Author-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 Maintainer-email: "Alteryx, Inc." <open_source_support@alteryx.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2019, Alteryx, Inc.
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evalml Version: 0.76.0 Summary: an AutoML library
+Metadata-Version: 2.1 Name: evalml Version: 0.77.0 Summary: an AutoML library
 that builds, optimizes, and evaluates machine learning pipelines using domain-
 specific objective functions Author-email: "Alteryx, Inc."
 alteryx.com> Maintainer-email: "Alteryx, Inc."
 alteryx.com> License: BSD 3-Clause License Copyright (c) 2019, Alteryx, Inc.
 All rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: * Redistributions of source code must retain the above copyright notice,
```

### Comparing `evalml-0.76.0/evalml.egg-info/SOURCES.txt` & `evalml-0.77.0/evalml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/evalml.egg-info/requires.txt` & `evalml-0.77.0/evalml.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `evalml-0.76.0/pyproject.toml` & `evalml-0.77.0/pyproject.toml`

 * *Files identical despite different names*

