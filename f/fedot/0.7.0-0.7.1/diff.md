# Comparing `tmp/fedot-0.7.0.tar.gz` & `tmp/fedot-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedot-0.7.0.tar", last modified: Thu Feb 23 08:41:30 2023, max compression
+gzip compressed data, was "fedot-0.7.1.tar", last modified: Thu Jun  8 08:47:24 2023, max compression
```

## Comparing `fedot-0.7.0.tar` & `fedot-0.7.1.tar`

### file list

```diff
@@ -1,337 +1,340 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.775071 fedot-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-02-23 08:41:24.000000 fedot-0.7.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-23 08:41:24.000000 fedot-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15989 2023-02-23 08:41:30.775071 fedot-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20480 2023-02-23 08:41:24.000000 fedot-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.735071 fedot-0.7.0/cases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-02-23 08:41:24.000000 fedot-0.7.0/cases/dataset_preparation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-02-23 08:41:24.000000 fedot-0.7.0/cases/kc2_sourcecode_defects_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-02-23 08:41:24.000000 fedot-0.7.0/cases/metocean_forecasting_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-02-23 08:41:24.000000 fedot-0.7.0/cases/multi_target_levels_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-02-23 08:41:24.000000 fedot-0.7.0/cases/multi_ts_level_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-02-23 08:41:24.000000 fedot-0.7.0/cases/multivariate_ts_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-02-23 08:41:24.000000 fedot-0.7.0/cases/spam_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-02-23 08:41:24.000000 fedot-0.7.0/cases/time_series_gapfilling_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.735071 fedot-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.739071 fedot-0.7.0/examples/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/additional_learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.739071 fedot-0.7.0/examples/advanced/automl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/automl/h2o_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/automl/pipeline_from_automl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/automl/tpot_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/automl/tpot_vs_fedot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.739071 fedot-0.7.0/examples/advanced/decompose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/decompose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/decompose/classification_refinement_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/decompose/refinement_forecast_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/decompose/regression_refinement_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.739071 fedot-0.7.0/examples/advanced/fedot_based_solutions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/fedot_based_solutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/fedot_based_solutions/external_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/gpu_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/multi_modal_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/multimodal_text_num_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/multiobj_optimisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/multitask_classification_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/parallelization_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/pipeline_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/profiler_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.739071 fedot-0.7.0/examples/advanced/remote_execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/remote_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/remote_execution/remote_fit_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/remote_execution/ts_composer_with_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.743071 fedot-0.7.0/examples/advanced/sensitivity_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/sensitivity_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/sensitivity_analysis/case_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/sensitivity_analysis/complex_analysis_with_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/sensitivity_analysis/dataset_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/sensitivity_analysis/mta_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/sensitivity_analysis/pipeline_export_with_sa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/sensitivity_analysis/pipelines_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/sensitivity_analysis/run_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.743071 fedot-0.7.0/examples/advanced/time_series_forecasting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/time_series_forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/time_series_forecasting/composing_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/time_series_forecasting/custom_model_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/time_series_forecasting/exogenous.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/time_series_forecasting/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/time_series_forecasting/nemo.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/time_series_forecasting/nemo_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/project_import_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.743071 fedot-0.7.0/examples/simple/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.743071 fedot-0.7.0/examples/simple/classification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/classification/api_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/classification/classification_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/classification/classification_with_tuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/classification/image_classification_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/classification/multiclass_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/classification/resample_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.743071 fedot-0.7.0/examples/simple/cli_application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/cli_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/cli_application/cli_call_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.747071 fedot-0.7.0/examples/simple/interpretable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/interpretable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/interpretable/api_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/interpretable/pipeline_explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/multitask_classification_regression_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/pipeline_and_history_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/pipeline_import_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/pipeline_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/pipeline_tune.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/pipeline_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.747071 fedot-0.7.0/examples/simple/regression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/regression/api_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/regression/regression_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/regression/regression_with_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.747071 fedot-0.7.0/examples/simple/time_series_forecasting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/time_series_forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/time_series_forecasting/api_forecasting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/time_series_forecasting/cgru.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/time_series_forecasting/fitted_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/time_series_forecasting/gapfilling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/time_series_forecasting/ts_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-02-23 08:41:24.000000 fedot-0.7.0/examples/simple/time_series_forecasting/tuning_pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.747071 fedot-0.7.0/fedot/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.747071 fedot-0.7.0/fedot/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.751071 fedot-0.7.0/fedot/api/api_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20841 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/api_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/api_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/api_data_analyser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.751071 fedot-0.7.0/fedot/api/api_utils/assumptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/assumptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/assumptions/assumptions_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/assumptions/assumptions_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/assumptions/operations_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/assumptions/preprocessing_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/assumptions/task_assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/data_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/predefined_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/api_utils/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/fedot_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    29145 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/api/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.751071 fedot-0.7.0/fedot/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.751071 fedot-0.7.0/fedot/core/caching/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/caching/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/caching/base_cache_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/caching/pipelines_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/caching/pipelines_cache_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/caching/preprocessing_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/caching/preprocessing_cache_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.755071 fedot-0.7.0/fedot/core/composer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/composer/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/composer/composer_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.755071 fedot-0.7.0/fedot/core/composer/gp_composer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/composer/gp_composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/composer/gp_composer/gp_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/composer/gp_composer/specific_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10445 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/composer/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/composer/random_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.755071 fedot-0.7.0/fedot/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/array_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    27483 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/data_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/data_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/data_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/load_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.755071 fedot-0.7.0/fedot/core/data/merge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/merge/data_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/merge/supplementary_data_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/multi_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/supplementary_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/data/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.759071 fedot-0.7.0/fedot/core/operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/atomized_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/atomized_template.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/data_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.759071 fedot-0.7.0/fedot/core/operations/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10264 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/common_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/evaluation_interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.759071 fedot-0.7.0/fedot/core/operations/evaluation/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/gpu/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/gpu/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/gpu/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/gpu/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.759071 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.763071 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)    35225 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.763071 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/svc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.763071 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py
--rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)    13077 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/evaluation/time_series.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/hyperparameters_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/operation_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/operations/operation_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.763071 fedot-0.7.0/fedot/core/optimisers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/optimisers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.763071 fedot-0.7.0/fedot/core/optimisers/objective/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/optimisers/objective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/optimisers/objective/data_objective_advisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/optimisers/objective/data_objective_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/optimisers/objective/data_source_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/optimisers/objective/metrics_objective.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/optimisers/objective/objective_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.767071 fedot-0.7.0/fedot/core/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/automl_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    17783 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/pipeline_advisor.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/pipeline_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/pipeline_composer_requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/pipeline_graph_generation_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/pipeline_node_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/random_pipeline_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    18702 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/ts_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.767071 fedot-0.7.0/fedot/core/pipelines/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/tuning/hyperparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    13284 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/tuning/search_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/tuning/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/tuning/tuner_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    15161 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/pipelines/verification_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.771071 fedot-0.7.0/fedot/core/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.771071 fedot-0.7.0/fedot/core/repository/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/data/automl_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/data/data_operation_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/data/default_operation_params.json
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/data/gpu_models_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/data/model_repository.json
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/dataset_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/default_params_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/graph_operation_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/json_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/operation_types_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/pipeline_operation_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/quality_metrics_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/repository/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.771071 fedot-0.7.0/fedot/core/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/validation/split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.771071 fedot-0.7.0/fedot/core/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/core/visualisation/pipeline_specific_visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.771071 fedot-0.7.0/fedot/explainability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/explainability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/explainability/explainer_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/explainability/explainers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/explainability/surrogate_explainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.771071 fedot-0.7.0/fedot/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/preprocessing/base_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/preprocessing/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/preprocessing/data_type_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    29084 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/preprocessing/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/preprocessing/dummy_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23460 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/preprocessing/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/preprocessing/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.771071 fedot-0.7.0/fedot/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.771071 fedot-0.7.0/fedot/remote/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/remote/infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.775071 fedot-0.7.0/fedot/remote/infrastructure/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/remote/infrastructure/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/remote/infrastructure/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/remote/infrastructure/clients/datamall_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/remote/infrastructure/clients/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/remote/pipeline_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/remote/remote_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/remote/run_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.775071 fedot-0.7.0/fedot/sensitivity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.775071 fedot-0.7.0/fedot/sensitivity/deletion_methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/deletion_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/deletion_methods/multi_times_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/node_sa_approaches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/nodes_sensitivity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.775071 fedot-0.7.0/fedot/sensitivity/operations_hp_sensitivity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/operations_hp_sensitivity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/operations_hp_sensitivity/multi_operations_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/operations_hp_sensitivity/one_operation_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/operations_hp_sensitivity/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/operations_hp_sensitivity/sa_and_sample_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/pipeline_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/pipeline_sensitivity_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/sensitivity/sa_requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.775071 fedot-0.7.0/fedot/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/utilities/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/utilities/define_metric_by_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/utilities/golem_imports_transition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/utilities/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/utilities/pattern_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/utilities/project_import_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/utilities/synth_dataset_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-02-23 08:41:24.000000 fedot-0.7.0/fedot/utilities/ts_gapfilling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.747071 fedot-0.7.0/fedot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15989 2023-02-23 08:41:30.000000 fedot-0.7.0/fedot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-02-23 08:41:30.000000 fedot-0.7.0/fedot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 08:41:30.000000 fedot-0.7.0/fedot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-02-23 08:41:30.000000 fedot-0.7.0/fedot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-23 08:41:30.000000 fedot-0.7.0/fedot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 08:41:30.775071 fedot-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-02-23 08:41:24.000000 fedot-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:41:30.775071 fedot-0.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-02-23 08:41:24.000000 fedot-0.7.0/test/test_gpu_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-08 08:47:17.000000 fedot-0.7.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 08:47:17.000000 fedot-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-06-08 08:47:24.587392 fedot-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21646 2023-06-08 08:47:17.000000 fedot-0.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.547392 fedot-0.7.1/cases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/dataset_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/kc2_sourcecode_defects_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/metocean_forecasting_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/multi_target_levels_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/multi_ts_level_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/multivariate_ts_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/spam_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-08 08:47:17.000000 fedot-0.7.1/cases/time_series_gapfilling_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.551392 fedot-0.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.551392 fedot-0.7.1/examples/advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/additional_learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.551392 fedot-0.7.1/examples/advanced/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/automl/h2o_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/automl/pipeline_from_automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/automl/tpot_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/automl/tpot_vs_fedot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.555392 fedot-0.7.1/examples/advanced/decompose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/decompose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/decompose/classification_refinement_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/decompose/refinement_forecast_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/decompose/regression_refinement_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.555392 fedot-0.7.1/examples/advanced/fedot_based_solutions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/fedot_based_solutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/fedot_based_solutions/external_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/gpu_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/multi_modal_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/multimodal_text_num_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/multiobj_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/multitask_classification_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/parallelization_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/pipeline_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/profiler_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.555392 fedot-0.7.1/examples/advanced/remote_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/remote_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/remote_execution/remote_fit_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/remote_execution/ts_composer_with_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.555392 fedot-0.7.1/examples/advanced/sensitivity_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/case_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/complex_analysis_with_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/dataset_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/mta_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/pipeline_export_with_sa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/pipelines_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/sensitivity_analysis/run_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/surrogate_optimization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.555392 fedot-0.7.1/examples/advanced/time_series_forecasting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/composing_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/custom_model_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/exogenous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/nemo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/nemo_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/project_import_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.559392 fedot-0.7.1/examples/simple/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/examples/simple/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/api_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/classification_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/classification_with_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/image_classification_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/multiclass_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/classification/resample_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/examples/simple/cli_application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/cli_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/cli_application/cli_call_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/examples/simple/interpretable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/interpretable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/interpretable/api_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/interpretable/pipeline_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/multitask_classification_regression_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/pipeline_and_history_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/pipeline_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/pipeline_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/pipeline_tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/pipeline_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/examples/simple/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/regression/api_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/regression/regression_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/regression/regression_with_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/examples/simple/time_series_forecasting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/api_forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/cgru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/fitted_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/gapfilling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/ts_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-08 08:47:17.000000 fedot-0.7.1/examples/simple/time_series_forecasting/tuning_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.563392 fedot-0.7.1/fedot/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.567392 fedot-0.7.1/fedot/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.567392 fedot-0.7.1/fedot/api/api_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9084 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/api_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/api_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/api_params_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.567392 fedot-0.7.1/fedot/api/api_utils/assumptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/assumptions_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/assumptions_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/operations_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/preprocessing_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/assumptions/task_assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/data_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/input_analyser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/predefined_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/api_utils/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/fedot_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31298 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/api/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.567392 fedot-0.7.1/fedot/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.571392 fedot-0.7.1/fedot/core/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/base_cache_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/pipelines_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/pipelines_cache_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/preprocessing_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/caching/preprocessing_cache_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.571392 fedot-0.7.1/fedot/core/composer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/composer_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.571392 fedot-0.7.1/fedot/core/composer/gp_composer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/gp_composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/gp_composer/gp_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/gp_composer/specific_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/meta_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/composer/random_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.571392 fedot-0.7.1/fedot/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/array_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28271 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/data_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/data_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/data_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.571392 fedot-0.7.1/fedot/core/data/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/merge/data_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/merge/supplementary_data_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/multi_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/supplementary_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/data/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.575392 fedot-0.7.1/fedot/core/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/atomized_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/atomized_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/data_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.575392 fedot-0.7.1/fedot/core/operations/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/common_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/evaluation_interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.575392 fedot-0.7.1/fedot/core/operations/evaluation/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/gpu/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/gpu/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/gpu/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/gpu/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.575392 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.575392 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9072 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35322 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.579392 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/svc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.579392 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8611 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13174 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/evaluation/time_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/hyperparameters_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/operation_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/operations/operation_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.579392 fedot-0.7.1/fedot/core/optimisers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.579392 fedot-0.7.1/fedot/core/optimisers/objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/data_objective_advisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/data_objective_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/data_source_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/metrics_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/optimisers/objective/objective_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.579392 fedot-0.7.1/fedot/core/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/automl_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14837 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17807 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline_advisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline_composer_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline_graph_generation_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/pipeline_node_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/random_pipeline_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18702 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/ts_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/core/pipelines/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/tuning/hyperparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/tuning/search_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/tuning/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/tuning/tuner_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16905 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/pipelines/verification_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/core/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/core/repository/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/data/automl_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11567 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/data/data_operation_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/data/default_operation_params.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/data/gpu_models_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/data/model_repository.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/dataset_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/default_params_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/graph_operation_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/json_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/operation_types_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/pipeline_operation_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/quality_metrics_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/repository/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/core/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/validation/split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/core/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/core/visualisation/pipeline_specific_visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/explainability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/explainability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/explainability/explainer_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/explainability/explainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/explainability/surrogate_explainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.583392 fedot-0.7.1/fedot/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/base_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/data_type_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29084 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/dummy_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23886 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/preprocessing/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/remote/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/remote/infrastructure/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/infrastructure/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/infrastructure/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/infrastructure/clients/datamall_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/infrastructure/clients/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/pipeline_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/remote_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/remote/run_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/sensitivity/deletion_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/deletion_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/deletion_methods/multi_times_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14594 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/node_sa_approaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/nodes_sensitivity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/multi_operations_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/one_operation_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/sa_and_sample_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/pipeline_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/pipeline_sensitivity_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/sensitivity/sa_requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/fedot/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/define_metric_by_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/golem_imports_transition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/pattern_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/project_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/synth_dataset_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-06-08 08:47:17.000000 fedot-0.7.1/fedot/utilities/ts_gapfilling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.567392 fedot-0.7.1/fedot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-06-08 08:47:24.000000 fedot-0.7.1/fedot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13351 2023-06-08 08:47:24.000000 fedot-0.7.1/fedot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:47:24.000000 fedot-0.7.1/fedot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-08 08:47:24.000000 fedot-0.7.1/fedot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 08:47:24.000000 fedot-0.7.1/fedot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:47:24.587392 fedot-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-08 08:47:17.000000 fedot-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:47:24.587392 fedot-0.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-08 08:47:17.000000 fedot-0.7.1/test/test_gpu_strategy.py
```

### Comparing `fedot-0.7.0/LICENSE.md` & `fedot-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/PKG-INFO` & `fedot-0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedot
-Version: 0.7.0
+Version: 0.7.1
 Summary: Automated machine learning framework for composite pipelines
 Home-page: https://github.com/aimclub/FEDOT
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -30,62 +30,59 @@
 .. start-badges
 .. list-table::
    :stub-columns: 1
 
    * - package
      - | |pypi| |python|
    * - tests
-     - | |build| |coverage|
+     - | |build| |integration| |coverage|
    * - docs
      - |docs|
    * - license
      - | |license|
    * - stats
      - | |downloads_stats|
    * - support
      - | |tg|
    * - languages
      - | |eng| |rus|
+   * - mirror
+     - | |gitlab|
+   * - funding
+     - | |ITMO| |NCCR|
 .. end-badges
 
 **FEDOT** is an open-source framework for automated modeling and machine learning (AutoML) problems. This framework is distributed under the 3-Clause BSD license.
 
 It provides automatic generative design of machine learning pipelines for various real-world problems. The core of FEDOT is based on an evolutionary approach and supports classification (binary and multiclass), regression, clustering, and time series prediction problems.
 
-.. image:: /docs/pipeline_small.png
-   :alt: The structure of the modeling pipeline that can be optimised by FEDOT
+.. image:: /docs/fedot-workflow.png
+   :alt: The structure of the AutoML workflow in FEDOT
 
 The key feature of the framework is the complex management of interactions between various blocks of pipelines. It is represented as a graph that defines connections between data preprocessing and model blocks.
 
 The project is maintained by the research team of the Natural Systems Simulation Lab, which is a part of the `National Center for Cognitive Research of ITMO University <https://actcognitive.org/>`__.
 
 More details about FEDOT are available in the next video:
 
 
 .. image:: https://res.cloudinary.com/marcomontalbano/image/upload/v1606396758/video_to_markdown/images/youtube--RjbuV6i6de4-c05b58ac6eb4c4700831b2b3070cd403.jpg
    :target: http://www.youtube.com/watch?v=RjbuV6i6de4
    :alt: Introducing Fedot
 
-FEDOT Features
+FEDOT concepts
 ==============
 
-The main features of the framework are as follows:
-
-- **Flexibility.** FEDOT is highly flexible: it can be used to automate the construction of solutions for various problems, data types, and models;
-- **Integration with ML libraries.** FEDOT supports widely used ML libraries (Scikit-Learn, Catboost, Xgboost, etc.) and allows you to integrate custom ones;
-- **Extensibility for new domains.** Pipeline optimization algorithms are data- and task-independent, yet you can use special templates for a specific task class or data type (time series forecasting, NLP, tabular data, etc.) to increase the efficiency;
-- **No limits.** The framework is versatile and is not limited to specific modeling tasks, for example, it can be used in ODE or PDE;
-- **Support of hyper-parameter tuning.** Hyper-parameter tuning methods are supported. Custom methods can also be integrated in FEDOT;
-- **Reproducibility.** You can export the resulting pipelines in JSON format for experiment reproducibility.
-
-Compared to other frameworks:
-
-- There are no limits to specific modeling tasks, therefore FEDOT claims versatility and expandability;
-- Allows managing the complexity of models and thereby achieving better results.
-- Allows building pipelines using different types of input data (texts, images, tables, etc.) and consisting of various models.
+- **Flexibility.** FEDOT can be used to automate the construction of solutions for various `problems <https://fedot.readthedocs.io/en/master/introduction/fedot_features/main_features.html#involved-tasks>`_, `data types <https://fedot.readthedocs.io/en/master/introduction/fedot_features/automation_features.html#data-nature>`_ (texts, images, tables), and `models <https://fedot.readthedocs.io/en/master/advanced/automated_pipelines_design.html>`_;
+- **Extensibility.** Pipeline optimization algorithms are data- and task-independent, yet you can use `special strategies <https://fedot.readthedocs.io/en/master/api/strategies.html>`_ for specific tasks or data types (time-series forecasting, NLP, tabular data, etc.) to increase the efficiency;
+- **Integrability.** FEDOT supports widely used ML libraries (Scikit-learn, CatBoost, XGBoost, etc.) and allows you to integrate `custom ones <https://fedot.readthedocs.io/en/master/api/strategies.html#module-fedot.core.operations.evaluation.custom>`_;
+- **Tuningability.** Various `hyper-parameters tuning methods <https://fedot.readthedocs.io/en/master/advanced/hyperparameters_tuning.html>`_ are supported including models' custom evaluation metrics and search spaces;
+- **Versatility.** FEDOT is `not limited to specific modeling tasks <https://fedot.readthedocs.io/en/master/advanced/architecture.html>`_, for example, it can be used in ODE or PDE;
+- **Reproducibility.** Resulting pipelines can be `exported separately as JSON <https://fedot.readthedocs.io/en/master/advanced/pipeline_import_export.html>`_ or `together with your input data as ZIP archive <https://fedot.readthedocs.io/en/master/advanced/project_import_export.html>`_ for experiments reproducibility;
+- **Customizability.** FEDOT allows `managing models complexity <https://fedot.readthedocs.io/en/master/introduction/fedot_features/automation_features.html#models-used>`_ and thereby achieving desired quality.
 
 Installation
 ============
 
 The simplest way to install FEDOT is using ``pip``:
 
 .. code-block::
@@ -213,16 +210,14 @@
 Also, we are doing several research tasks related to AutoML time-series benchmarking and multi-modal modeling.
 
 Any contribution is welcome. Our R&D team is open for cooperation with other scientific teams as well as with industrial partners.
 
 Documentation
 =============
 
-The general description is available in the `FEDOT.Docs <https://itmo-nss-team.github.io/FEDOT.Miscellaneous>`__ repository.
-
 Also, a detailed FEDOT API description is available in `Read the Docs <https://fedot.readthedocs.io/en/latest/>`__.
 
 Contribution Guide
 ==================
 
 - The contribution guide is available in this `repository <https://github.com/aimclub/FEDOT/blob/master/docs/source/contribution.rst>`__.
 
@@ -273,15 +268,19 @@
 
 .. |docs| image:: https://readthedocs.org/projects/ebonite/badge/?style=flat
    :target: https://fedot.readthedocs.io/en/latest/
    :alt: Documentation Status
 
 .. |build| image:: https://github.com/aimclub/FEDOT/workflows/Build/badge.svg?branch=master
    :alt: Build Status
-   :target: https://github.com/aimclub/FEDOT/actions
+   :target: https://github.com/aimclub/FEDOT/actions/workflows/unit-build.yml
+
+.. |integration| image:: https://github.com/aimclub/FEDOT/workflows/Integration/badge.svg?branch=master
+   :alt: Integration Build Status
+   :target: https://github.com/aimclub/FEDOT/actions/workflows/integration-build.yml
 
 .. |coverage| image:: https://codecov.io/gh/aimclub/FEDOT/branch/master/graph/badge.svg
    :alt: Coverage Status
    :target: https://codecov.io/gh/aimclub/FEDOT
 
 .. |pypi| image:: https://badge.fury.io/py/fedot.svg
    :alt: Supported Python Versions
@@ -297,7 +296,19 @@
 
 .. |downloads_stats| image:: https://static.pepy.tech/personalized-badge/fedot?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads
    :target: https://pepy.tech/project/fedot
 
 .. |tg| image:: https://img.shields.io/badge/Telegram-Group-blue.svg
           :target: https://t.me/FEDOT_helpdesk
           :alt: Telegram Chat
+
+.. |ITMO| image:: https://github.com/ITMO-NSS-team/open-source-ops/blob/add_badge/badges/ITMO_badge_rus.svg
+   :alt: Acknowledgement to ITMO
+   :target: https://itmo.ru
+
+.. |NCCR| image:: https://github.com/ITMO-NSS-team/open-source-ops/blob/add_badge/badges/NCCR_badge.svg
+   :alt: Acknowledgement to NCCR
+   :target: https://actcognitive.org/
+
+.. |gitlab| image:: https://camo.githubusercontent.com/9bd7b8c5b418f1364e72110a83629772729b29e8f3393b6c86bff237a6b784f6/68747470733a2f2f62616467656e2e6e65742f62616467652f6769746c61622f6d6972726f722f6f72616e67653f69636f6e3d6769746c6162
+   :alt: GitLab mirror for this repository
+   :target: https://gitlab.actcognitive.org/itmo-nss-team/FEDOT
```

### Comparing `fedot-0.7.0/README.rst` & `fedot-0.7.1/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -10,62 +10,59 @@
 .. start-badges
 .. list-table::
    :stub-columns: 1
 
    * - package
      - | |pypi| |python|
    * - tests
-     - | |build| |coverage|
+     - | |build| |integration| |coverage|
    * - docs
      - |docs|
    * - license
      - | |license|
    * - stats
      - | |downloads_stats|
    * - support
      - | |tg|
    * - languages
      - | |eng| |rus|
+   * - mirror
+     - | |gitlab|
+   * - funding
+     - | |ITMO| |NCCR|
 .. end-badges
 
 **FEDOT** - это open-source фреймворк для решения задач из области автоматизированного моделирования и машинного обучения (AutoML). Фреймворк распространяется под лицензией 3-Clause BSD.
 
 FEDOT предоставляет возможность использовать генеративный дизайн для проектирования пайплайнов машинного обучения для различных реальных задач. Ядро фреймворка основано на эволюционном подходе и поддерживает классификацию (бинарную и мультиклассовую), регрессию, кластеризацию и задачи прогнозирования временных рядов.
 
-.. image:: docs/pipeline_small.png
-   :alt: Структура пайплайна для моделирования, который может быть оптимизирован с помощью FEDOT
+.. image:: docs/fedot-workflow.png
+   :alt: Реализация процесса автоматического машинного обучения в FEDOT
 
 Ключевой особенностью фреймворка является управление сложными взаимодействиями между различными частями пайплайнов. Они представлены в виде графика, который определяет связи между предварительной обработкой данных и блоками модели.
 
 Проект поддерживается исследовательской группой Natural Systems Simulation Lab, которая является частью `Национального центра когнитивных разработок Университета ИТМО <https://actcognitive.org/>`__.
 
 Более подробная информация о FEDOT доступна в следующем видео:
 
 
 .. image:: https://res.cloudinary.com/marcomontalbano/image/upload/v1606396758/video_to_markdown/images/youtube--RjbuV6i6de4-c05b58ac6eb4c4700831b2b3070cd403.jpg
    :target: http://www.youtube.com/watch?v=RjbuV6i6de4
    :alt: Introducing Fedot
 
-Особенности фреймворка
-=====================
-
-Основные особенности фреймворка:
+Концепции FEDOT'а
+=================
 
-- **Гибкость.** FEDOT очень гибкий: его можно использовать для автоматизации поиска решений для различных классов задач, типов данных и моделей;
-- **Интеграция с другими библиотеками МО.** FEDOT поддерживает широко используемые библиотеки МО (Scikit-Learn, Can boost, Xgboost и т.д.) и позволяет интегрировать пользовательские библиотеки;
-- **Расширяемость для новых видов задач.** Алгоритмы для оптимизации пайплайнов не зависят от вида данных и задач, однако можно использовать специальные шаблоны для определенных классов задач или типов данных (прогнозирование временных рядов, NLP, табличные данные и т.д.) для повышения эффективности;
-- **Отсутствие ограничений.** Фреймворк универсальный и не ограничивается конкретными задачами моделирования, например, его можно использовать в ODE или PDE;
-- **Поддержка настройки гиперпараметров.** Поддерживаются методы настройки гиперпараметров. Пользовательские методы также могут быть интегрированы в FEDOT;
-- **Воспроизводимость.** Можно экспортировать получившиеся паплайны в формате JSON для воспроизводимости эксперимента.
-
-По сравнению с другими фреймворками, FEDOT:
-
-- можно считать универсальным и расширяемым, т.к. у него нет ограничений для видов задач моделирования;
-- позволяет управлять сложностью моделей и тем самым достигать лучших результатов;
-- позволяет строить пайплайны состоящие из различных моделей, используя различные типы входных данных (тексты, изображения, таблицы и т.д.).
+- **Гибкость.** FEDOT может быть использован для автоматизации поиска решений для различных `классов задач <https://fedot.readthedocs.io/en/master/introduction/fedot_features/main_features.html#involved-tasks>`_, `типов данных <https://fedot.readthedocs.io/en/master/introduction/fedot_features/automation_features.html#data-nature>`_ (тексты, изображения, таблицы), и `моделей <https://fedot.readthedocs.io/en/master/advanced/automated_pipelines_design.html>`_;
+- **Расширяемость.** Алгоритмы для оптимизации пайплайнов не зависят от вида данных и задач, однако можно использовать `специальные стратегии <https://fedot.readthedocs.io/en/master/api/strategies.html>`_ для определенных классов задач или типов данных (прогнозирование временных рядов, NLP, табличные данные и т.д.) для повышения эффективности;
+- **Интегрируемость.** FEDOT поддерживает широко используемые библиотеки МО (Scikit-learn, CatBoost, XGBoost и т.д.) и позволяет интегрировать `пользовательские библиотеки <https://fedot.readthedocs.io/en/master/api/strategies.html#module-fedot.core.operations.evaluation.custom>`_;
+- **Тюнингуемость.** Поддерживаются различные методы `настройки гиперпараметров <https://fedot.readthedocs.io/en/master/advanced/hyperparameters_tuning.html>`_, включая пользовательские метрики оценивания и пространства параметров моделей;
+- **Универсальность.** FEDOT `не ограничивается конкретными задачами моделирования <https://fedot.readthedocs.io/en/master/advanced/architecture.html>`_, например, его можно использовать в ODE или PDE;
+- **Воспроизводимость.** Получаемые паплайны можно `экспортировать в формате JSON отдельно <https://fedot.readthedocs.io/en/master/advanced/pipeline_import_export.html>`_ или `вместе с входными данными в формате архива ZIP <https://fedot.readthedocs.io/en/master/advanced/project_import_export.html>`_, для воспроизведения экспериментов;
+- **Кастомизируемость.** FEDOT позволяет `настраивать сложность моделей <https://fedot.readthedocs.io/en/master/introduction/fedot_features/automation_features.html#models-used>`_, тем самым, получать необходимое качество.
 
 Установка
 =========
 
 Самый простой способ установить FEDOT - это использовать ``pip``:
 
 .. code-block::
@@ -192,16 +189,14 @@
 Кроме того, мы работаем над рядом исследовательских задач, связанных с бенчмаркингом прогнозирования временных рядов с помощью AutoML и мультимодального моделирования.
 
 Наша научно-исследовательская команда открыта для сотрудничества с другими научными коллективами, а также с партнерами из индустрии.
 
 Документация
 ============
 
-Общее описание доступно в репозитории `FEDOT.Docs <https://itmo-nss-team.github.io/FEDOT.Miscellaneous>`__.
-
 Подробное описание FEDOT API доступно в разделе `Read the Docs <https://fedot.readthedocs.io/en/latest/>`__.
 
 Как участвовать
 ===============
 
 - Инструкция для добавления изменений находится в `репозитории <https://github.com/aimclub/FEDOT/blob/master/docs/source/contribution.rst>`__.
 
@@ -254,14 +249,18 @@
    :target: https://fedot.readthedocs.io/en/latest/
    :alt: Documentation Status
 
 .. |build| image:: https://github.com/aimclub/FEDOT/workflows/Build/badge.svg?branch=master
    :alt: Build Status
    :target: https://github.com/aimclub/FEDOT/actions
 
+.. |integration| image:: https://github.com/aimclub/FEDOT/workflows/Integration/badge.svg?branch=master
+   :alt: Integration Build Status
+   :target: https://github.com/aimclub/FEDOT/actions/workflows/integration-build.yml
+
 .. |coverage| image:: https://codecov.io/gh/aimclub/FEDOT/branch/master/graph/badge.svg
    :alt: Coverage Status
    :target: https://codecov.io/gh/aimclub/FEDOT
 
 .. |pypi| image:: https://badge.fury.io/py/fedot.svg
    :alt: Supported Python Versions
    :target: https://badge.fury.io/py/fedot
@@ -276,7 +275,19 @@
 
 .. |downloads_stats| image:: https://static.pepy.tech/personalized-badge/fedot?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads
    :target: https://pepy.tech/project/fedot
 
 .. |tg| image:: https://img.shields.io/badge/Telegram-Group-blue.svg
           :target: https://t.me/FEDOT_helpdesk
           :alt: Telegram Chat
+
+.. |ITMO| image:: https://github.com/ITMO-NSS-team/open-source-ops/blob/add_badge/badges/ITMO_badge_rus.svg
+   :alt: Acknowledgement to ITMO
+   :target: https://itmo.ru
+
+.. |NCCR| image:: https://github.com/ITMO-NSS-team/open-source-ops/blob/add_badge/badges/NCCR_badge.svg
+   :alt: Acknowledgement to NCCR
+   :target: https://actcognitive.org/
+
+.. |gitlab| image:: https://camo.githubusercontent.com/9bd7b8c5b418f1364e72110a83629772729b29e8f3393b6c86bff237a6b784f6/68747470733a2f2f62616467656e2e6e65742f62616467652f6769746c61622f6d6972726f722f6f72616e67653f69636f6e3d6769746c6162
+   :alt: GitLab mirror for this repository
+   :target: https://gitlab.actcognitive.org/itmo-nss-team/FEDOT
```

### Comparing `fedot-0.7.0/cases/dataset_preparation.py` & `fedot-0.7.1/cases/dataset_preparation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/cases/kc2_sourcecode_defects_classification.py` & `fedot-0.7.1/cases/kc2_sourcecode_defects_classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/cases/metocean_forecasting_problem.py` & `fedot-0.7.1/cases/metocean_forecasting_problem.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/cases/multi_target_levels_forecasting.py` & `fedot-0.7.1/cases/multi_target_levels_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/cases/multi_ts_level_forecasting.py` & `fedot-0.7.1/cases/multi_ts_level_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/cases/multivariate_ts_forecasting.py` & `fedot-0.7.1/cases/multivariate_ts_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/cases/spam_detection.py` & `fedot-0.7.1/cases/spam_detection.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/cases/time_series_gapfilling_case.py` & `fedot-0.7.1/cases/time_series_gapfilling_case.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/additional_learning.py` & `fedot-0.7.1/examples/advanced/additional_learning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/automl/h2o_example.py` & `fedot-0.7.1/examples/advanced/automl/h2o_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/automl/pipeline_from_automl.py` & `fedot-0.7.1/examples/advanced/automl/pipeline_from_automl.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/automl/tpot_example.py` & `fedot-0.7.1/examples/advanced/automl/tpot_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/automl/tpot_vs_fedot.py` & `fedot-0.7.1/examples/advanced/automl/tpot_vs_fedot.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/decompose/classification_refinement_example.py` & `fedot-0.7.1/examples/advanced/decompose/classification_refinement_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/decompose/refinement_forecast_example.py` & `fedot-0.7.1/examples/advanced/decompose/refinement_forecast_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/decompose/regression_refinement_example.py` & `fedot-0.7.1/examples/advanced/decompose/regression_refinement_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/fedot_based_solutions/external_optimizer.py` & `fedot-0.7.1/examples/advanced/fedot_based_solutions/external_optimizer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/gpu_example.py` & `fedot-0.7.1/examples/advanced/gpu_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/multi_modal_pipeline.py` & `fedot-0.7.1/examples/advanced/multi_modal_pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/multimodal_text_num_example.py` & `fedot-0.7.1/examples/advanced/multimodal_text_num_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     data = MultiModalData.from_csv(file_path=path, task=task, target_columns='variety', index_col=None)
     fit_data, predict_data = train_test_data_setup(data, shuffle_flag=True, split_ratio=0.7)
 
     automl_model = Fedot(problem=task, timeout=10, with_tuning=with_tuning)
     automl_model.fit(features=fit_data,
                      target=fit_data.target)
 
-    prediction = automl_model.predict(predict_data)
-    metrics = automl_model.get_metrics()
+    _ = automl_model.predict(predict_data)
+    metrics = automl_model.get_metrics(metric_names='f1')
 
     if visualization:
         automl_model.current_pipeline.show()
 
     print(f'F1 for validation sample is {round(metrics["f1"], 3)}')
 
     return metrics["f1"]
```

### Comparing `fedot-0.7.0/examples/advanced/multiobj_optimisation.py` & `fedot-0.7.1/examples/advanced/multiobj_optimisation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/multitask_classification_regression.py` & `fedot-0.7.1/examples/advanced/multitask_classification_regression.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import os
 from datetime import timedelta
+from typing import Tuple
 
 import numpy as np
 import pandas as pd
 from golem.core.tuning.simultaneous import SimultaneousTuner
 
 from fedot.core.data.data import InputData
 from fedot.core.data.multi_modal import MultiModalData
 from fedot.core.data.supplementary_data import SupplementaryData
 from fedot.core.pipelines.node import PipelineNode
 from fedot.core.pipelines.pipeline import Pipeline
 from fedot.core.pipelines.tuning.tuner_builder import TunerBuilder
 from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.core.repository.quality_metrics_repository import RegressionMetricsEnum
 from fedot.core.repository.tasks import TaskTypesEnum, Task
-from test.unit.api.test_api_cli_params import project_root_path
+from fedot.core.utils import fedot_project_root
 
 
 def get_multitask_pipeline():
     logit_node = PipelineNode('logit')
     data_source_node = PipelineNode('data_source_table/regression')
     final_node = PipelineNode('dtreg', nodes_from=[logit_node, data_source_node])
     return Pipeline(final_node)
 
 
-def prepare_multitask_data() -> (MultiModalData, MultiModalData):
+def prepare_multitask_data() -> Tuple[MultiModalData, MultiModalData]:
     """ Load data for multitask regression / classification pipeline """
-    ex_data = os.path.join(project_root_path, 'examples/data')
-    train_df = pd.read_csv(os.path.join(ex_data, 'train_synthetic_regression_classification.csv'))
-    test_df = pd.read_csv(os.path.join(ex_data, 'test_synthetic_regression_classification.csv'))
+    ex_data = fedot_project_root().joinpath('examples/data')
+    train_df = pd.read_csv(ex_data.joinpath('train_synthetic_regression_classification.csv'))
+    test_df = pd.read_csv(ex_data.joinpath('test_synthetic_regression_classification.csv'))
 
     # Data for classification
     class_task = Task(TaskTypesEnum.classification)
     class_train = InputData(idx=np.arange(0, len(train_df)), features=np.array(train_df[['feature_1', 'feature_2']]),
                             target=np.array(train_df['class']), task=class_task, data_type=DataTypesEnum.table,
                             supplementary_data=SupplementaryData(is_main_target=False))
     class_test = InputData(idx=np.arange(0, len(test_df)), features=np.array(test_df[['feature_1', 'feature_2']]),
@@ -62,20 +62,22 @@
 
     :param with_tuning: is tuning required or not
     """
     train_input, test_input = prepare_multitask_data()
     multitask_pipeline = get_multitask_pipeline()
 
     if with_tuning:
-        tuner = TunerBuilder(train_input.task)\
-            .with_tuner(SimultaneousTuner)\
-            .with_metric(RegressionMetricsEnum.MAE)\
-            .with_iterations(100)\
-            .with_timeout(timedelta(minutes=2))\
+        tuner = (
+            TunerBuilder(train_input.task)
+            .with_tuner(SimultaneousTuner)
+            .with_metric(RegressionMetricsEnum.MAE)
+            .with_iterations(100)
+            .with_timeout(timedelta(minutes=2))
             .build(train_input)
+        )
         multitask_pipeline = tuner.tune(multitask_pipeline)
 
     multitask_pipeline.fit(train_input)
     side_pipeline = multitask_pipeline.pipeline_for_side_task(task_type=TaskTypesEnum.classification)
 
     # Replace the name of main "data source" in preprocessor
     side_pipeline.preprocessor.main_target_source_name = 'logit'
```

### Comparing `fedot-0.7.0/examples/advanced/parallelization_comparison.py` & `fedot-0.7.1/examples/advanced/parallelization_comparison.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/pipeline_sensitivity.py` & `fedot-0.7.1/examples/advanced/pipeline_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/profiler_example.py` & `fedot-0.7.1/examples/advanced/profiler_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/remote_execution/remote_fit_example.py` & `fedot-0.7.1/examples/advanced/remote_execution/remote_fit_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/remote_execution/ts_composer_with_integration.py` & `fedot-0.7.1/examples/advanced/remote_execution/ts_composer_with_integration.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/sensitivity_analysis/case_analysis.py` & `fedot-0.7.1/examples/advanced/sensitivity_analysis/case_analysis.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/sensitivity_analysis/complex_analysis_with_requirements.py` & `fedot-0.7.1/examples/advanced/sensitivity_analysis/complex_analysis_with_requirements.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/sensitivity_analysis/dataset_access.py` & `fedot-0.7.1/examples/advanced/sensitivity_analysis/dataset_access.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/sensitivity_analysis/mta_example.py` & `fedot-0.7.1/examples/advanced/sensitivity_analysis/mta_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/sensitivity_analysis/pipeline_export_with_sa.py` & `fedot-0.7.1/examples/advanced/sensitivity_analysis/pipeline_export_with_sa.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/sensitivity_analysis/pipelines_access.py` & `fedot-0.7.1/examples/advanced/sensitivity_analysis/pipelines_access.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/sensitivity_analysis/run_cases.py` & `fedot-0.7.1/examples/advanced/sensitivity_analysis/run_cases.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/time_series_forecasting/composing_pipelines.py` & `fedot-0.7.1/examples/advanced/time_series_forecasting/composing_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/time_series_forecasting/custom_model_tuning.py` & `fedot-0.7.1/examples/advanced/time_series_forecasting/custom_model_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/time_series_forecasting/exogenous.py` & `fedot-0.7.1/examples/advanced/time_series_forecasting/exogenous.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py` & `fedot-0.7.1/examples/advanced/time_series_forecasting/multi_ts_arctic_forecasting.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/time_series_forecasting/multistep.py` & `fedot-0.7.1/examples/advanced/time_series_forecasting/multistep.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/time_series_forecasting/nemo.py` & `fedot-0.7.1/examples/advanced/time_series_forecasting/nemo.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/advanced/time_series_forecasting/nemo_multiple.py` & `fedot-0.7.1/examples/advanced/time_series_forecasting/nemo_multiple.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,24 +150,25 @@
     errors_df = {}
 
     train_input, predict_input, train_input_exog, predict_input_exog, test_data = \
         prepare_data(time_series=time_series,
                      exog_variable=exog_variable,
                      len_forecast=len_forecast)
 
-    pipelines = {'ARIMA': {
-        'tr_nodes_data': {"arima": train_input},
-        'pr_nodes_data': {"arima": predict_input},
-        'model': get_arima_pipeline()
-    },
-        'STL_ARIMA': {
-            'tr_nodes_data': {"stl_arima": train_input},
-            'pr_nodes_data': {"stl_arima": predict_input},
-            'model': get_stlarima_pipeline()
-        },
+    pipelines = {
+        'ARIMA':
+            {'tr_nodes_data': {"arima": train_input},
+             'pr_nodes_data': {"arima": predict_input},
+             'model': get_arima_pipeline()
+             },
+        'STL_ARIMA':
+            {'tr_nodes_data': {"stl_arima": train_input},
+             'pr_nodes_data': {"stl_arima": predict_input},
+             'model': get_stlarima_pipeline()
+             },
         'RIDGE':
             {'tr_nodes_data': {"lagged/1": train_input, "lagged/2": train_input},
              'pr_nodes_data': {"lagged/1": predict_input, "lagged/2": predict_input},
              'model': get_ridge_pipeline()
              },
         'ARIMA_NEMO':
             {'tr_nodes_data': {"arima": train_input, "exog_ts": train_input_exog},
@@ -265,22 +266,24 @@
     df = pd.DataFrame(columns=['POINT', 'RIDGE', 'RIDGE_NEMO',
                                'ARIMA', 'ARIMA_NEMO',
                                'STL_ARIMA', 'STL_ARIMA_NEMO'])
     return df
 
 
 def add_data_to_errors_df(df, error_name, point, errors):
-    df = df.append({'POINT': point,
-                    'RIDGE': errors['RIDGE_' + error_name],
-                    'RIDGE_NEMO': errors['RIDGE_NEMO_' + error_name],
-                    'ARIMA': errors['ARIMA_' + error_name],
-                    'ARIMA_NEMO': errors['ARIMA_NEMO_' + error_name],
-                    'STL_ARIMA': errors['STL_ARIMA_' + error_name],
-                    'STL_ARIMA_NEMO': errors['STL_ARIMA_NEMO_' + error_name],
-                    }, ignore_index=True)
+    more_data = pd.DataFrame({
+        'POINT': point,
+        'RIDGE': errors['RIDGE_' + error_name],
+        'RIDGE_NEMO': errors['RIDGE_NEMO_' + error_name],
+        'ARIMA': errors['ARIMA_' + error_name],
+        'ARIMA_NEMO': errors['ARIMA_NEMO_' + error_name],
+        'STL_ARIMA': errors['STL_ARIMA_' + error_name],
+        'STL_ARIMA_NEMO': errors['STL_ARIMA_NEMO_' + error_name],
+    }, index=[0])
+    df = pd.concat([df, more_data], ignore_index=True)
     return df
 
 
 def run_multiple_example(path_to_file, path_to_exog_file, out_path=None, visualization=False, len_forecast=40):
     mse_errors_df = create_errors_df()
     mae_errors_df = create_errors_df()
     mape_errors_df = create_errors_df()
```

### Comparing `fedot-0.7.0/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py` & `fedot-0.7.1/examples/advanced/time_series_forecasting/sparse_lagged_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/project_import_export.py` & `fedot-0.7.1/examples/project_import_export.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/classification/api_classification.py` & `fedot-0.7.1/examples/simple/classification/api_classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/classification/classification_pipelines.py` & `fedot-0.7.1/examples/simple/classification/classification_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/classification/classification_with_tuning.py` & `fedot-0.7.1/examples/simple/classification/classification_with_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/classification/image_classification_problem.py` & `fedot-0.7.1/examples/simple/classification/image_classification_problem.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/classification/multiclass_prediction.py` & `fedot-0.7.1/examples/simple/classification/multiclass_prediction.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/classification/resample_example.py` & `fedot-0.7.1/examples/simple/classification/resample_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/cli_application/cli_call_example.py` & `fedot-0.7.1/examples/simple/cli_application/cli_call_example.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/interpretable/api_explain.py` & `fedot-0.7.1/examples/simple/interpretable/api_explain.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/interpretable/pipeline_explain.py` & `fedot-0.7.1/examples/simple/interpretable/pipeline_explain.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/multitask_classification_regression_api.py` & `fedot-0.7.1/examples/simple/multitask_classification_regression_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
+from typing import Tuple
 
 import numpy as np
 import pandas as pd
 
 from fedot.api.main import Fedot
-from test.unit.api.test_api_cli_params import project_root_path
+from fedot.core.utils import fedot_project_root
 
 
-def load_train_test_dataframes() -> (pd.DataFrame, pd.DataFrame):
+def load_train_test_dataframes() -> Tuple[dict, dict, dict]:
     """ Load data for multitask regression / classification problem """
-    data_path = os.path.join(project_root_path, 'examples/data')
+    data_path = fedot_project_root().joinpath('examples/data')
     train_df = pd.read_csv(os.path.join(data_path, 'train_synthetic_regression_classification.csv'))
     test_df = pd.read_csv(os.path.join(data_path, 'test_synthetic_regression_classification.csv'))
 
     # Prepare numpy arrays into dictionaries
     # For regression and classification features are the same
     mm_train_features = {'regression': np.array(train_df[['feature_1', 'feature_2']]),
                          'classification': np.array(train_df[['feature_1', 'feature_2']])}
```

### Comparing `fedot-0.7.0/examples/simple/pipeline_and_history_visualization.py` & `fedot-0.7.1/examples/simple/pipeline_and_history_visualization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/pipeline_import_export.py` & `fedot-0.7.1/examples/simple/pipeline_import_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 
 from examples.simple.regression.regression_with_tuning import get_regression_dataset
 from examples.simple.regression.regression_pipelines import regression_ransac_pipeline
 from fedot.core.data.data import InputData
 from fedot.core.pipelines.pipeline import Pipeline
 from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.core.repository.tasks import Task, TaskTypesEnum
+from fedot.core.utils import fedot_project_root
 
 
 def create_correct_path(path: str, dirname_flag: bool = False):
     """
     Create path with time which was created during the testing process.
     """
+    # TODO: this function is used in many places, but now is not really needed
     last_el = None
     for dirname in next(os.walk(os.path.curdir))[1]:
         if dirname.endswith(path):
             if dirname_flag:
                 last_el = dirname
             else:
                 file = os.path.join(dirname, path + '.json')
@@ -54,19 +56,19 @@
     pipeline.fit_from_scratch(train_input)
 
     predicted_output = pipeline.predict(predict_input)
     prediction_before_export = np.array(predicted_output.predict)
     print(f'Before export {prediction_before_export[:4]}')
 
     # Export it
-    pipeline.save(path=pipeline_path)
+    path_to_save_and_load = f'{fedot_project_root()}/examples/simple/{pipeline_path}'
+    pipeline.save(path=path_to_save_and_load, create_subdir=False, is_datetime_in_path=False)
 
     # Import pipeline
-    json_path_load = create_correct_path(pipeline_path)
-    new_pipeline = Pipeline.from_serialized(json_path_load)
+    new_pipeline = Pipeline().load(path_to_save_and_load)
 
     predicted_output_after_export = new_pipeline.predict(predict_input)
     prediction_after_export = np.array(predicted_output_after_export.predict)
 
     print(f'After import {prediction_after_export[:4]}')
 
     dict_pipeline, dict_fitted_operations = pipeline.save()
```

### Comparing `fedot-0.7.0/examples/simple/pipeline_log.py` & `fedot-0.7.1/examples/simple/pipeline_log.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/pipeline_tune.py` & `fedot-0.7.1/examples/simple/pipeline_tune.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/pipeline_visualization.py` & `fedot-0.7.1/examples/simple/pipeline_visualization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/regression/api_regression.py` & `fedot-0.7.1/examples/simple/regression/api_regression.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     data_path = f'{fedot_project_root()}/cases/data/cholesterol/cholesterol.csv'
 
     data = InputData.from_csv(data_path,
                               task=Task(TaskTypesEnum.regression))
     train, test = train_test_data_setup(data)
     problem = 'regression'
 
-    composer_params = {'history_folder': 'custom_history_folder', 'preset': 'auto'}
+    composer_params = {'history_dir': 'custom_history_dir', 'preset': 'auto'}
     auto_model = Fedot(problem=problem, seed=42, timeout=2, logging_level=logging.INFO,
                        with_tuning=with_tuning, **composer_params)
 
     auto_model.fit(features=train, target='target')
     prediction = auto_model.predict(features=test)
     if visualise:
         auto_model.history.save('saved_regression_history.json')
```

### Comparing `fedot-0.7.0/examples/simple/regression/regression_pipelines.py` & `fedot-0.7.1/examples/simple/regression/regression_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/regression/regression_with_tuning.py` & `fedot-0.7.1/examples/simple/regression/regression_with_tuning.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/time_series_forecasting/api_forecasting.py` & `fedot-0.7.1/examples/simple/time_series_forecasting/api_forecasting.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from typing import Optional
 
 import pandas as pd
 
 from fedot.api.main import Fedot
 from fedot.core.data.data import InputData
 from fedot.core.data.data_split import train_test_data_setup
 from fedot.core.repository.dataset_types import DataTypesEnum
@@ -15,16 +14,17 @@
 datasets = {
     'australia': f'{fedot_project_root()}/examples/data/ts/australia.csv',
     'beer': f'{fedot_project_root()}/examples/data/ts/beer.csv',
     'salaries': f'{fedot_project_root()}/examples/data/ts/salaries.csv',
     'stackoverflow': f'{fedot_project_root()}/examples/data/ts/stackoverflow.csv'}
 
 
-def get_ts_data(dataset: str = 'beer', horizon: int = 10, validation_blocks: Optional[int] = None):
+def get_ts_data(dataset='australia', horizon: int = 30, validation_blocks=None):
     time_series = pd.read_csv(datasets[dataset])
+
     task = Task(TaskTypesEnum.ts_forecasting,
                 TsForecastingParams(forecast_length=horizon))
     if dataset not in ['australia']:
         idx = pd.to_datetime(time_series['idx'].values)
     else:
         # non datetime indexes
         idx = time_series['idx'].values
@@ -36,15 +36,15 @@
                             data_type=DataTypesEnum.ts)
     train_data, test_data = train_test_data_setup(train_input, validation_blocks=validation_blocks)
     return train_data, test_data
 
 
 def run_ts_forecasting_example(dataset='australia', horizon: int = 30, validation_blocks=2, timeout: float = None,
                                visualization=False, with_tuning=True):
-    train_data, test_data = get_ts_data(dataset, horizon, 2)
+    train_data, test_data = get_ts_data(dataset, horizon, validation_blocks)
     # init model for the time series forecasting
     model = Fedot(problem='ts_forecasting',
                   task_params=Task(TaskTypesEnum.ts_forecasting,
                 TsForecastingParams(forecast_length=horizon)).task_params,
                   timeout=timeout,
                   n_jobs=1,
                   with_tuning=with_tuning,
```

### Comparing `fedot-0.7.0/examples/simple/time_series_forecasting/cgru.py` & `fedot-0.7.1/examples/simple/time_series_forecasting/cgru.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/time_series_forecasting/fitted_values.py` & `fedot-0.7.1/examples/simple/time_series_forecasting/fitted_values.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/time_series_forecasting/gapfilling.py` & `fedot-0.7.1/examples/simple/time_series_forecasting/gapfilling.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/time_series_forecasting/ts_pipelines.py` & `fedot-0.7.1/examples/simple/time_series_forecasting/ts_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/examples/simple/time_series_forecasting/tuning_pipelines.py` & `fedot-0.7.1/examples/simple/time_series_forecasting/tuning_pipelines.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/api/api_utils/api_data.py` & `fedot-0.7.1/fedot/api/api_utils/api_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                                           target=target,
                                           task=self.task,
                                           is_predict=is_predict)
             if isinstance(data, dict) and idx is not None:
                 for key in data:
                     data[key].idx = idx
         except Exception as ex:
-            raise ValueError('Please specify the "features" as path to as path to csv file/'
+            raise ValueError('Please specify the "features" as path to csv file/'
                              'Numpy array/Pandas DataFrame/FEDOT InputData/dict for multimodal data, '
                              f'Exception: {ex}')
 
         # Perform obligatory steps of data preprocessing
         if is_predict:
             data = self.preprocessor.obligatory_prepare_for_predict(data)
         else:
```

### Comparing `fedot-0.7.0/fedot/api/api_utils/assumptions/assumptions_builder.py` & `fedot-0.7.1/fedot/api/api_utils/assumptions/assumptions_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/api/api_utils/assumptions/assumptions_handler.py` & `fedot-0.7.1/fedot/api/api_utils/assumptions/assumptions_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 
 
 class AssumptionsHandler:
     def __init__(self, data: InputData):
         """
         Class for handling operations related with assumptions
 
-        :param data: data for pipelines
+        Args:
+            data: data for pipelines.
         """
         self.log = default_log(self)
         self.data = data
 
     def propose_assumptions(self,
                             initial_assumption: Union[List[Pipeline], Pipeline, None],
                             available_operations: List,
```

### Comparing `fedot-0.7.0/fedot/api/api_utils/assumptions/operations_filter.py` & `fedot-0.7.1/fedot/api/api_utils/assumptions/operations_filter.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/api/api_utils/assumptions/preprocessing_builder.py` & `fedot-0.7.1/fedot/api/api_utils/assumptions/preprocessing_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/api/api_utils/assumptions/task_assumptions.py` & `fedot-0.7.1/fedot/api/api_utils/assumptions/task_assumptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,28 +44,25 @@
     """ Simple static dictionary-based assumptions for time series forecasting task. """
 
     @property
     def builders(self):
         return {
             'glm_ridge':
                 PipelineBuilder()
-                    .add_branch('glm', 'lagged')
-                    .add_node('ridge', branch_idx=1)
-                    .join_branches('ridge'),
+                .add_branch('glm', 'lagged')
+                .add_node('ridge', branch_idx=1)
+                .join_branches('ridge'),
             'lagged_ridge':
                 PipelineBuilder()
-                    .add_sequence('lagged', 'ridge'),
+                .add_sequence('lagged', 'ridge'),
             'polyfit_ridge':
                 PipelineBuilder()
-                    .add_branch('polyfit', 'lagged')
-                    .grow_branches(None, 'ridge')
-                    .join_branches('ridge'),
-            'smoothing_ar':
-                PipelineBuilder()
-                    .add_sequence('smoothing', 'ar'),
+                .add_branch('polyfit', 'lagged')
+                .grow_branches(None, 'ridge')
+                .join_branches('ridge')
         }
 
     def ensemble_operation(self) -> str:
         return 'ridge'
 
     def processing_builders(self) -> List[PipelineBuilder]:
         return list(self.builders.values())
@@ -104,15 +101,15 @@
     """ Simple static dictionary-based assumptions for classification task. """
 
     @property
     def builders(self):
         return {
             'rf': PipelineBuilder().add_node('rf'),
             'logit': PipelineBuilder().add_node('logit'),
-            'cnn': PipelineBuilder().add_node('cnn'),
+            'catboost': PipelineBuilder().add_node('catboost'),
         }
 
     def ensemble_operation(self) -> str:
         return 'rf'
 
     def processing_builders(self) -> List[PipelineBuilder]:
         return list(self.builders.values())
```

### Comparing `fedot-0.7.0/fedot/api/api_utils/data_definition.py` & `fedot-0.7.1/fedot/api/api_utils/data_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                     target: str = None,
                     is_predict: bool = False) -> InputData:
         if target is None:
             target = np.array([])
 
         if isinstance(target, str) and target in features.columns:
             target_array = features[target]
-            features = features.drop(columns=[target])
+            features = features.drop(columns=target)
         else:
             target_array = target
 
         data = array_to_input_data(features_array=np.asarray(features),
                                    target_array=np.asarray(target_array),
                                    task=task)
         return data
@@ -117,27 +117,26 @@
 class CsvStrategy(StrategyDefineData):
     def define_data(self, features: Union[str, PathLike],
                     task: Task,
                     target: str = None,
                     is_predict: bool = False) -> InputData:
         # CSV files as input data, by default - table data
 
-        data_type = DataTypesEnum.table
         if task.task_type == TaskTypesEnum.ts_forecasting:
             # For time series forecasting format - time series
             data = InputData.from_csv_time_series(task=task,
                                                   file_path=features,
                                                   target_column=target,
                                                   is_predict=is_predict)
         else:
             # Make default features table
             # CSV files as input data
             data = InputData.from_csv(features, task=task,
                                       target_columns=target,
-                                      data_type=data_type)
+                                      data_type=DataTypesEnum.table)
         return data
 
 
 class MultimodalStrategy(StrategyDefineData):
     """
     Gets dict of NumPy arrays or InputData sources as input data
     and returns MultiModalData object with source names defined by data type
@@ -151,17 +150,17 @@
     def define_data(self, features: dict,
                     task: Task,
                     target: str = None,
                     is_predict: bool = False,
                     idx=None) -> MultiModalData:
 
         # change data type to InputData
-        for source in features:
-            if not isinstance(features[source], InputData):
-                features[source] = array_to_input_data(features_array=features[source], target_array=target,
+        for source, inner_data in features.items():
+            if not isinstance(inner_data, InputData):
+                features[source] = array_to_input_data(features_array=inner_data, target_array=target,
                                                        task=task, idx=idx)
         # create labels for data sources
         sources = dict((f'{self.source_name_by_type.get(features[data_part_key].data_type.name)}/{data_part_key}',
                         data_part)
                        for (data_part_key, data_part) in features.items())
         data = MultiModalData(sources)
         return data
```

### Comparing `fedot-0.7.0/fedot/api/api_utils/metrics.py` & `fedot-0.7.1/fedot/api/api_utils/metrics.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-from typing import Callable, Union, Sequence
+from typing import Callable, Union, Sequence, Optional
+
+from golem.core.utilities.data_structures import ensure_wrapped_in_sequence
 
 from fedot.core.composer.metrics import Metric
 from fedot.core.repository.quality_metrics_repository import (ClassificationMetricsEnum, ClusteringMetricsEnum,
-                                                              ComplexityMetricsEnum, RegressionMetricsEnum)
+                                                              ComplexityMetricsEnum, RegressionMetricsEnum, MetricType,
+                                                              MetricsEnum)
+from fedot.core.repository.tasks import Task
+from fedot.utilities.define_metric_by_task import MetricByTask
 
 
 class ApiMetrics:
     """
     Class for metrics matching. Handling both "metric name" - "metric instance"
     both for composer and tuner
     """
 
-    _task_dict = {
-        'regression': ['rmse', 'mae'],
-        'classification': ['roc_auc', 'f1'],
-        'multiclassification': 'f1',
-        'clustering': 'silhouette',
-        'ts_forecasting': ['rmse', 'mae']
-    }
-
     _metrics_dict = {
         'acc': ClassificationMetricsEnum.accuracy,
         'roc_auc': ClassificationMetricsEnum.ROCAUC,
         'f1': ClassificationMetricsEnum.f1,
         'logloss': ClassificationMetricsEnum.logloss,
         'mae': RegressionMetricsEnum.MAE,
         'mse': RegressionMetricsEnum.MSE,
@@ -32,24 +29,43 @@
         'r2': RegressionMetricsEnum.R2,
         'rmse': RegressionMetricsEnum.RMSE,
         'rmse_pen': RegressionMetricsEnum.RMSE_penalty,
         'silhouette': ClusteringMetricsEnum.silhouette,
         'node_num': ComplexityMetricsEnum.node_num
     }
 
-    def __init__(self, problem: str):
-        if '/' in problem:
-            # Solve multitask problem
-            self.main_problem, self.side_problem = problem.split('/')
-        else:
-            self.main_problem = problem
-            self.side_problem = None
+    def __init__(self, task: Task, metrics: Optional[Union[str, MetricsEnum, Callable, Sequence]]):
+        self.task: Task = task
+        self.metric_functions: Sequence[MetricType] = self.obtain_metrics(metrics)
+
+    @property
+    def metric_names(self):
+        return ApiMetrics.get_metric_names(self.metric_functions)
 
-    def get_problem_metrics(self) -> Union[str, Sequence[str]]:
-        return ApiMetrics._task_dict[self.main_problem]
+    @staticmethod
+    def get_metric_names(metrics: Union[MetricType, Sequence[MetricType]]) -> Sequence[str]:
+        return [str(metric) for metric in ensure_wrapped_in_sequence(metrics)]
 
     @staticmethod
     def get_metrics_mapping(metric_name: Union[str, Callable]) -> Union[Metric, Callable]:
         if isinstance(metric_name, Callable):
             # for custom metric
             return metric_name
         return ApiMetrics._metrics_dict[metric_name]
+
+    def obtain_metrics(self, metrics: Optional[Union[str, MetricsEnum, Callable, Sequence]]) -> Sequence[MetricType]:
+        """Chooses metric to use for quality assessment of pipeline during composition"""
+        if metrics is None:
+            metrics = MetricByTask.get_default_quality_metrics(self.task.task_type)
+
+        metric_ids = []
+        for specific_metric in ensure_wrapped_in_sequence(metrics):
+            metric = None
+            if isinstance(specific_metric, (str, Callable)):
+                # metric was defined by name (str) or metric is a custom function
+                metric = ApiMetrics.get_metrics_mapping(metric_name=specific_metric)
+            elif isinstance(specific_metric, MetricsEnum):
+                metric = specific_metric
+            if metric is None:
+                raise ValueError(f'Incorrect metric {specific_metric}')
+            metric_ids.append(metric)
+        return metric_ids
```

### Comparing `fedot-0.7.0/fedot/api/api_utils/params.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,187 +1,260 @@
-import random
-from typing import Any, Dict, List, Optional, Union
+from copy import copy
+from typing import Optional
 
 import numpy as np
-from golem.core.log import Log, LoggerAdapter, default_log
-from golem.core.utilities.random import RandomStateHandler
-
-from fedot.api.api_utils.presets import OperationsPreset
-from fedot.core.constants import AUTO_PRESET_NAME, DEFAULT_FORECAST_LENGTH
-from fedot.core.data.data import InputData
-from fedot.core.data.multi_modal import MultiModalData
+from scipy import stats
+from scipy.special import boxcox, inv_boxcox
+from statsmodels.tsa.api import STLForecast
+from statsmodels.tsa.arima.model import ARIMA
+
+from fedot.core.data.data import InputData, OutputData
+from fedot.core.operations.evaluation.operation_implementations.data_operations.ts_transformations import ts_to_table
+from fedot.core.operations.evaluation.operation_implementations.implementation_interfaces import ModelImplementation
+from fedot.core.operations.operation_parameters import OperationParameters
 from fedot.core.repository.dataset_types import DataTypesEnum
-from fedot.core.repository.tasks import Task, TaskParams, TaskTypesEnum, TsForecastingParams
+from fedot.utilities.ts_gapfilling import SimpleGapFiller
+
+
+class ARIMAImplementation(ModelImplementation):
 
+    def __init__(self, params: Optional[OperationParameters] = None):
+        super().__init__(params)
+        self.arima = None
+        self.lambda_value = None
+        self.scope = None
+        self.actual_ts_len = None
 
-class ApiParams:
+    def fit(self, input_data):
+        """ Class fit arima model on data
 
-    def __init__(self):
-        self.api_params: dict = None
-        self.log: LoggerAdapter = None
-        self.task: Task = None
-        self.task_params: TaskParams = None
-        self.metric_name: Union[str, List[str]] = None
+        :param input_data: data with features, target and ids to process
+        """
+        source_ts = np.array(input_data.features)
+        # Save actual time series length
+        self.actual_ts_len = len(source_ts)
+
+        # Apply box-cox transformation for positive values
+        transformed_ts = self._apply_boxcox(source_ts)
 
-    def initialize_params(self, input_params: Dict[str, Any]):
-        """ Merge input_params dictionary with several parameters for AutoML algorithm """
-        self.get_initial_params(input_params)
+        # Set parameters
+        p = int(self.params.get('p'))
+        d = int(self.params.get('d'))
+        q = int(self.params.get('q'))
+        params = {'order': (p, d, q)}
 
-        # Final check for correctness for timeout and generations
-        self.api_params = check_timeout_vs_generations(self.api_params)
+        self.arima = ARIMA(transformed_ts, **params).fit()
 
-    def update_available_operations_by_preset(self, data: InputData):
-        preset_operations = OperationsPreset(task=self.task, preset_name=self.api_params['preset'])
-        self.api_params = preset_operations.composer_params_based_on_preset(self.api_params, data.data_type)
+        return self.arima
 
-    def get_initial_params(self, input_params: Dict[str, Any]):
-        self._parse_input_params(input_params)
+    def predict(self, input_data: InputData):
+        """ Method for time series prediction on forecast length
 
-        param_dict = {
-            'task': self.task,
-            'logger': self.log
-        }
-        self.api_params = {**self.api_params, **param_dict}
+        :param input_data: data with features, target and ids to process
 
-    def accept_and_apply_recommendations(self, input_data: Union[InputData, MultiModalData], recommendations: Dict):
+        :return output_data: output data with smoothed time series
         """
-        Accepts recommendations for api params from DataAnalyser
+        input_data = copy(input_data)
+        forecast_length = input_data.task.task_params.forecast_length
+        self.handle_new_data(input_data)
+
+        start_id = self.actual_ts_len
+        end_id = start_id + forecast_length - 1
+
+        predicted = self.arima.predict(start=start_id,
+                                       end=end_id)
+        predicted = self._inverse_boxcox(predicted=predicted,
+                                         lambda_param=self.lambda_value)
+        predict = self._inverse_shift(predicted)
+
+        predict = np.array(predict).reshape(1, -1)
+        output_data = self._convert_to_output(input_data,
+                                              predict=predict,
+                                              data_type=DataTypesEnum.table)
+
+        return output_data
+
+    def predict_for_fit(self, input_data: InputData):
+        input_data = copy(input_data)
+        forecast_length = input_data.task.task_params.forecast_length
+        fitted_values = self.arima.fittedvalues
+
+        fitted_values = self._inverse_boxcox(predicted=fitted_values,
+                                             lambda_param=self.lambda_value)
+        fitted_values = self._inverse_shift(fitted_values)
+
+        diff = int(self.actual_ts_len - len(fitted_values))
+        # If first elements skipped
+        if diff != 0:
+            # Fill nans with first values
+            first_element = fitted_values[0]
+            first_elements = [first_element] * diff
+            first_elements.extend(list(fitted_values))
+
+            fitted_values = np.array(first_elements)
+
+        _, predict = ts_to_table(idx=input_data.idx,
+                                 time_series=fitted_values,
+                                 window_size=forecast_length)
+
+        new_idx, target_columns = ts_to_table(idx=input_data.idx,
+                                              time_series=input_data.target,
+                                              window_size=forecast_length)
+        input_data.idx = new_idx
+        input_data.target = target_columns
+
+        output_data = self._convert_to_output(input_data,
+                                              predict=predict,
+                                              data_type=DataTypesEnum.table)
+
+        return output_data
 
-        :param input_data - data for preprocessing
-        :param recommendations - dict with recommendations
+    def handle_new_data(self, input_data: InputData):
         """
-        # TODO fix multimodality
-        if isinstance(input_data, MultiModalData):
-            self.api_params['cv_folds'] = None  # there are no support for multimodal data now
-            for data_source_name, values in input_data.items():
-                self.accept_and_apply_recommendations(input_data[data_source_name],
-                                                      recommendations[data_source_name])
+        Method to update x samples inside a model (used when we want to use old model to a new data)
+
+        :param input_data: new input_data
+        """
+        if input_data.idx[0] > self.actual_ts_len:
+            self.arima = self.fit(input_data)
+            self.log.info("Arima refitted for handling a new data")
+
+    def _apply_boxcox(self, source_ts):
+        min_value = np.min(source_ts)
+        if min_value > 0:
+            pass
         else:
-            if 'label_encoded' in recommendations:
-                self.log.info("Change preset due to label encoding")
-                self.change_preset_for_label_encoded_data(input_data.task, input_data.data_type)
-
-    def change_preset_for_label_encoded_data(self, task: Task, data_type: DataTypesEnum):
-        """ Change preset on tree like preset, if data had been label encoded """
-        if 'preset' in self.api_params:
-            preset_name = ''.join((self.api_params['preset'], '*tree'))
+            # Making a shift to positive values
+            self.scope = abs(min_value) + 1
+            source_ts = source_ts + self.scope
+
+        _, self.lambda_value = stats.boxcox(source_ts)
+        transformed_ts = boxcox(source_ts, self.lambda_value)
+
+        return transformed_ts
+
+    def _inverse_boxcox(self, predicted, lambda_param):
+        """ Method apply inverse Box-Cox transformation """
+        if lambda_param == 0:
+            return np.exp(predicted)
         else:
-            preset_name = '*tree'
-        preset_operations = OperationsPreset(task=task, preset_name=preset_name)
-
-        if self.api_params.get('available_operations') is not None:
-            del self.api_params['available_operations']
-        self.api_params = preset_operations.composer_params_based_on_preset(self.api_params, data_type)
-        param_dict = {
-            'task': self.task,
-            'logger': self.log
-        }
-        self.api_params = {**self.api_params, **param_dict}
-
-    def _parse_input_params(self, input_params: Dict[str, Any]):
-        """ Parses input params into different class fields """
-
-        # reset logging level for Singleton
-        Log().reset_logging_level(input_params['logging_level'])
-        self.log = default_log(prefix='FEDOT logger')
-
-        simple_keys = ['problem', 'n_jobs', 'parallelization_mode', 'timeout']
-        self.api_params = {k: input_params[k] for k in simple_keys}
-
-        default_evo_params = self.get_default_evo_params(self.api_params['problem'])
-        if input_params['composer_tuner_params'] is None:
-            evo_params = default_evo_params
+            res = inv_boxcox(predicted, lambda_param)
+            res = self._filling_gaps(res)
+            return res
+
+    def _inverse_shift(self, values):
+        """ Method apply inverse shift operation """
+        if self.scope is None:
+            pass
         else:
-            evo_params = {**default_evo_params, **input_params['composer_tuner_params']}
-        self.api_params.update(evo_params)
-        if 'preset' not in input_params['composer_tuner_params']:
-            self.api_params['preset'] = 'auto'
-
-        # If early_stopping_generations is not specified,
-        # than estimate it as in time-based manner as: 0.33 * composing_timeout.
-        # The minimal number of generations is 5.
-        if 'early_stopping_iterations' not in input_params['composer_tuner_params']:
-            if input_params['timeout']:
-                depending_on_timeout = int(input_params['timeout'] / 3)
-                self.api_params['early_stopping_iterations'] = \
-                    depending_on_timeout if depending_on_timeout > 5 else 5
-
-        specified_seed = input_params['seed']
-        if specified_seed is not None:
-            np.random.seed(specified_seed)
-            random.seed(specified_seed)
-            RandomStateHandler.MODEL_FITTING_SEED = specified_seed
-
-        self.task_params = input_params['task_params']
-        if self.api_params['problem'] == 'ts_forecasting' and self.task_params is None:
-            self.log.warning(f'The value of the forecast depth was set to {DEFAULT_FORECAST_LENGTH}.')
-            self.task_params = TsForecastingParams(forecast_length=DEFAULT_FORECAST_LENGTH)
-
-        if self.api_params['problem'] == 'clustering':
-            raise ValueError('This type of task is not supported in API now')
-
-        self.task = ApiParams.get_task(self.api_params['problem'], self.task_params)
-        self.metric_name = self.get_default_metric(self.api_params['problem'])
-        self.api_params.pop('problem')
+            values = values - self.scope
 
-    @staticmethod
-    def get_default_evo_params(problem: str):
-        """ Dictionary with default parameters for composer """
-        params = {'max_depth': 6,
-                  'max_arity': 3,
-                  'pop_size': 20,
-                  'num_of_generations': None,
-                  'keep_n_best': 1,
-                  'with_tuning': True,
-                  'preset': AUTO_PRESET_NAME,
-                  'genetic_scheme': None,
-                  'early_stopping_iterations': 30,
-                  'early_stopping_timeout': 10,
-                  'use_input_preprocessing': True,
-                  'use_pipelines_cache': True,
-                  'use_preprocessing_cache': True,
-                  'cache_folder': None}
-
-        if problem in ['classification', 'regression']:
-            params['cv_folds'] = 5
-        elif problem == 'ts_forecasting':
-            params['cv_folds'] = 3
-            params['validation_blocks'] = 2
-        return params
+        return values
 
     @staticmethod
-    def get_default_metric(problem: str) -> Union[str, List[str]]:
-        default_test_metric_dict = {
-            'regression': ['rmse', 'mae'],
-            'classification': ['roc_auc', 'f1'],
-            'multiclassification': 'f1',
-            'clustering': 'silhouette',
-            'ts_forecasting': ['rmse', 'mae']
-        }
-        return default_test_metric_dict[problem]
+    def _filling_gaps(res):
+        nan_ind = np.argwhere(np.isnan(res))
+        res[nan_ind] = -100.0
+
+        # Gaps in first and last elements fills with mean value
+        if 0 in nan_ind:
+            res[0] = np.mean(res)
+        if int(len(res) - 1) in nan_ind:
+            res[int(len(res) - 1)] = np.mean(res)
+
+        # Gaps in center of timeseries fills with linear interpolation
+        if len(np.ravel(np.argwhere(np.isnan(res)))) != 0:
+            gf = SimpleGapFiller()
+            res = gf.linear_interpolation(res)
+
+        return res
+
+
+class STLForecastARIMAImplementation(ModelImplementation):
+    def __init__(self, params: Optional[OperationParameters] = None):
+        super().__init__(params)
+        self.model = None
+        self.lambda_param = None
+        self.scope = None
+        self.actual_ts_len = None
 
-    @staticmethod
-    def get_task(problem: str, task_params: Optional[TaskParams] = None):
-        """ Return task by the given ML problem name and the parameters """
-        task_dict = {'regression': Task(TaskTypesEnum.regression, task_params=task_params),
-                     'classification': Task(TaskTypesEnum.classification, task_params=task_params),
-                     'clustering': Task(TaskTypesEnum.clustering, task_params=task_params),
-                     'ts_forecasting': Task(TaskTypesEnum.ts_forecasting, task_params=task_params)}
-        try:
-            return task_dict[problem]
-        except ValueError as exc:
-            ValueError('Wrong type name of the given task')
-
-
-def check_timeout_vs_generations(api_params):
-    timeout = api_params['timeout']
-    num_of_generations = api_params['num_of_generations']
-    if timeout in [-1, None]:
-        api_params['timeout'] = None
-        if num_of_generations is None:
-            raise ValueError('"num_of_generations" should be specified if infinite "timeout" is given')
-    elif timeout > 0:
-        if num_of_generations is None:
-            api_params['num_of_generations'] = 10000
-    else:
-        raise ValueError(f'invalid "timeout" value: timeout={timeout}')
-    return api_params
+    def fit(self, input_data):
+        """ Class fit STLForecast arima model on data
+
+        :param input_data: data with features, target and ids to process
+        """
+
+        source_ts = np.array(input_data.features)
+        # Save actual time series length
+        self.actual_ts_len = len(source_ts)
+
+        p = int(self.params.setdefault('p', 2))
+        d = int(self.params.setdefault('d', 0))
+        q = int(self.params.setdefault('q', 2))
+        period = int(self.params.setdefault('period', 365))
+        params = {'period': period, 'model_kwargs': {'order': (p, d, q)}}
+        self.model = STLForecast(source_ts, ARIMA, **params).fit()
+
+        return self.model
+
+    def predict(self, input_data: InputData) -> OutputData:
+        """ Method for time series prediction on forecast length
+
+        :param input_data: data with features, target and ids to process
+
+        :return output_data: output data with smoothed time series
+        """
+        parameters = input_data.task.task_params
+        forecast_length = parameters.forecast_length
+
+        # in case in(out) sample forecasting
+        self.handle_new_data(input_data)
+        start_id = self.actual_ts_len
+        end_id = start_id + forecast_length - 1
+        predicted = self.model.get_prediction(start=start_id, end=end_id).predicted_mean
+
+        predict = np.array(predicted).reshape(1, -1)
+        new_idx = np.arange(start_id, end_id + 1)
+
+        input_data.idx = new_idx
+
+        output_data = self._convert_to_output(input_data,
+                                              predict=predict,
+                                              data_type=DataTypesEnum.table)
+        return output_data
+
+    def predict_for_fit(self, input_data: InputData) -> OutputData:
+        parameters = input_data.task.task_params
+        forecast_length = parameters.forecast_length
+        idx = input_data.idx
+        target = input_data.target
+        fitted_values = self.model.get_prediction(start=idx[0], end=idx[-1]).predicted_mean
+        diff = int(self.actual_ts_len) - len(fitted_values)
+        # If first elements skipped
+        if diff != 0:
+            # Fill nans with first values
+            first_element = fitted_values[0]
+            first_elements = [first_element] * diff
+            first_elements.extend(list(fitted_values))
+
+            fitted_values = np.array(first_elements)
+
+        _, predict = ts_to_table(idx=idx,
+                                 time_series=fitted_values,
+                                 window_size=forecast_length)
+
+        new_idx, target_columns = ts_to_table(idx=idx,
+                                              time_series=target,
+                                              window_size=forecast_length)
+
+        input_data.idx = new_idx
+        input_data.target = target_columns
+        output_data = self._convert_to_output(input_data,
+                                              predict=predict,
+                                              data_type=DataTypesEnum.table)
+        return output_data
+
+    def handle_new_data(self, input_data: InputData):
+        """ Refit model if use new test data"""
+        if input_data.idx[0] > self.actual_ts_len:
+            self.model = self.fit(input_data)
+            self.log.info("STL Arima refitted for handling a new data")
```

### Comparing `fedot-0.7.0/fedot/api/api_utils/predefined_model.py` & `fedot-0.7.1/fedot/api/api_utils/predefined_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import traceback
 from typing import Union
 
-from golem.core.log import Log
+from golem.core.log import LoggerAdapter
 
 from fedot.api.api_utils.assumptions.assumptions_builder import AssumptionsBuilder
 from fedot.core.data.data import InputData
 from fedot.core.pipelines.node import PipelineNode
 from fedot.core.pipelines.pipeline import Pipeline
 from fedot.core.pipelines.verification import verify_pipeline
 
 
 class PredefinedModel:
-    def __init__(self, predefined_model: Union[str, Pipeline], data: InputData, log: Log,
+    def __init__(self, predefined_model: Union[str, Pipeline], data: InputData, log: LoggerAdapter,
                  use_input_preprocessing: bool = True):
         self.predefined_model = predefined_model
         self.data = data
         self.log = log
         self.pipeline = self._get_pipeline(use_input_preprocessing)
 
     def _get_pipeline(self, use_input_preprocessing: bool = True) -> Pipeline:
```

### Comparing `fedot-0.7.0/fedot/api/api_utils/presets.py` & `fedot-0.7.1/fedot/api/api_utils/presets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from copy import copy
 from typing import Optional
 
 from fedot.api.time import ApiTime
 from fedot.core.constants import BEST_QUALITY_PRESET_NAME, \
-    FAST_TRAIN_PRESET_NAME
+    FAST_TRAIN_PRESET_NAME, AUTO_PRESET_NAME
 from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.core.repository.operation_types_repository import OperationTypesRepository, get_operations_for_task
 from fedot.core.repository.tasks import Task
 
 
 class OperationsPreset:
     """ Class for presets processing. Preset is a set of operations (data operations
@@ -26,26 +26,26 @@
         based on defined preset
         """
         updated_params = copy(api_params)
 
         if self.preset_name is None and 'preset' in updated_params:
             self.preset_name = updated_params['preset']
 
-        if self.preset_name is not None and 'available_operations' not in api_params:
+        if self.preset_name is not None and api_params.get('available_operations') is None:
             available_operations = self.filter_operations_by_preset(data_type)
             updated_params['available_operations'] = available_operations
 
         return updated_params
 
     def filter_operations_by_preset(self, data_type: Optional[DataTypesEnum] = None):
         """ Filter operations by preset, remove "heavy" operations and save
         appropriate ones
         """
         preset_name = self.preset_name
-        if 'auto' in preset_name:
+        if AUTO_PRESET_NAME in preset_name:
             available_operations = get_operations_for_task(self.task, data_type, mode='all')
             return available_operations
 
         # TODO remove workaround
         # Use best_quality preset but exclude several operations
         if 'stable' in self.preset_name:
             # Use best_quality preset but exclude several operations
```

### Comparing `fedot-0.7.0/fedot/api/fedot_cli.py` & `fedot-0.7.1/fedot/api/fedot_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
               'arity': 'max_arity',
               'popsize': 'pop_size',
               'gen_num': 'num_of_generations',
               'opers': 'available_operations',
               'tuning': 'with_tuning',
               'cv_folds': 'cv_folds',
               'val_bl': 'validation_blocks',
-              'hist_path': 'history_folder',
+              'hist_path': 'history_dir',
               'for_len': 'forecast_length'
               }
 
 
 def run_cli():
     parser = create_parser(arguments_dicts)
     parameters = parser.parse_args()
```

### Comparing `fedot-0.7.0/fedot/api/help.py` & `fedot-0.7.1/fedot/api/help.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,42 +11,49 @@
 
     task = _get_task_by_name(task_name)
 
     repository = OperationTypesRepository(operation_type='model')
 
     # Filter operations
     repository_operations_list = _filter_operations_by_type(repository, task)
+    search_space = PipelineSearchSpace()
     for model in repository_operations_list:
         if model.id != 'custom':
-            hyperparameters = PipelineSearchSpace().get_operation_parameter_range(str(model.id))
+            hyperparameters = search_space.get_operation_parameter_range(str(model.id))
             implementation_info = model.current_strategy(task)(model.id).implementation_info
-            print(f"Model name - '{model.id}'")
-            print(f"Available hyperparameters to optimize with tuner - {hyperparameters}")
-            print(f"Strategy implementation - {model.current_strategy(task)}")
-            print(f"Model implementation - {implementation_info}\n")
+            info_lst = [
+                f"Model name - '{model.id}'",
+                f"Available hyperparameters to optimize with tuner - {hyperparameters}",
+                f"Strategy implementation - {model.current_strategy(task)}",
+                f"Model implementation - {implementation_info}\n"
+            ]
+            print('\n'.join(info_lst))
 
 
 def print_data_operations_info(task_name):
     """ Function display data operations and information about it for considered task
 
     :param task_name: name of available task type
     """
 
     task = _get_task_by_name(task_name)
 
     repository = OperationTypesRepository(operation_type='data_operation')
-    # Filter operations
     repository_operations_list = _filter_operations_by_type(repository, task)
+    search_space = PipelineSearchSpace()
     for operation in repository_operations_list:
-        hyperparameters = PipelineSearchSpace().get_operation_parameter_range(str(operation.id))
+        hyperparameters = search_space.get_operation_parameter_range(str(operation.id))
         implementation_info = operation.current_strategy(task)(operation.id).implementation_info
-        print(f"Data operation name - '{operation.id}'")
-        print(f"Available hyperparameters to optimize with tuner - {hyperparameters}")
-        print(f"Strategy implementation - {operation.current_strategy(task)}")
-        print(f"Operation implementation - {implementation_info}\n")
+        info_lst = [
+            f"Data operation name - '{operation.id}'",
+            f"Available hyperparameters to optimize with tuner - {hyperparameters}",
+            f"Strategy implementation - {operation.current_strategy(task)}",
+            f"Operation implementation - {implementation_info}\n"
+        ]
+        print('\n'.join(info_lst))
 
 
 def _filter_operations_by_type(repository, task):
     """ Function filter operations in repository by task
 
     :param repository: repository with operations to filter
     :param task: task type, if None, return all models
```

### Comparing `fedot-0.7.0/fedot/api/main.py` & `fedot-0.7.1/fedot/api/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,150 +1,196 @@
 import logging
 from copy import deepcopy
-from typing import Any, List, Optional, Sequence, Tuple, Union
+from typing import Any, List, Optional, Sequence, Tuple, Union, Callable
 
 import numpy as np
 import pandas as pd
 from golem.core.dag.graph_utils import graph_structure
+from golem.core.log import default_log, Log
 from golem.core.optimisers.opt_history_objects.opt_history import OptHistory
 from golem.core.tuning.simultaneous import SimultaneousTuner
-from golem.core.utilities.data_structures import ensure_wrapped_in_sequence
 from golem.visualisation.opt_viz_extra import visualise_pareto
 
 from fedot.api.api_utils.api_composer import ApiComposer
 from fedot.api.api_utils.api_data import ApiDataProcessor
-from fedot.api.api_utils.api_data_analyser import DataAnalyser
 from fedot.api.api_utils.data_definition import FeaturesType, TargetType
+from fedot.api.api_utils.input_analyser import InputAnalyser
 from fedot.api.api_utils.metrics import ApiMetrics
 from fedot.api.api_utils.params import ApiParams
 from fedot.api.api_utils.predefined_model import PredefinedModel
 from fedot.core.constants import DEFAULT_API_TIMEOUT_MINUTES, DEFAULT_TUNING_ITERATIONS_NUMBER
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.data.multi_modal import MultiModalData
 from fedot.core.data.visualisation import plot_biplot, plot_forecast, plot_roc_auc
+from fedot.core.optimisers.objective import PipelineObjectiveEvaluate
+from fedot.core.optimisers.objective.metrics_objective import MetricsObjective
 from fedot.core.pipelines.pipeline import Pipeline
 from fedot.core.pipelines.ts_wrappers import convert_forecast_to_output, out_of_sample_ts_forecast
 from fedot.core.pipelines.tuning.tuner_builder import TunerBuilder
-from fedot.core.repository.quality_metrics_repository import MetricsRepository
 from fedot.core.repository.tasks import TaskParams, TaskTypesEnum
+from fedot.core.utils import set_random_seed
 from fedot.explainability.explainer_template import Explainer
 from fedot.explainability.explainers import explain_pipeline
 from fedot.preprocessing.base_preprocessing import BasePreprocessor
 from fedot.remote.remote_evaluator import RemoteEvaluator
 from fedot.utilities.memory import MemoryAnalytics
 from fedot.utilities.project_import_export import export_project_to_zip, import_project_from_zip
 
 NOT_FITTED_ERR_MSG = 'Model not fitted yet'
 
 
 class Fedot:
     """Main class for FEDOT API.
 
-    Facade for ApiDataProcessor, ApiComposer, ApiMetrics, ApiInitialAssumptions.
+    Facade for
+    :class:`ApiParams`, :class:`ApiDataProcessor`, :class:`ApiComposer`, :class:`ApiMetrics`,
+    :class:`~fedot.api.api_utils.assumptions.assumptions_handler.AssumptionsHandler`.
 
     Args:
-        problem: the name of modelling problem to solve
-
-            .. details:: possible ``problem`` options:
+        problem: name of the modelling problem to solve.
+            .. details:: Possible options:
 
                 - ``classification`` -> for classification task
                 - ``regression`` -> for regression task
-                - ``ts_forecasting`` -> for time serires forecasting task
+                - ``ts_forecasting`` -> for time series forecasting task
 
-        timeout: time for model design (in minutes): ``None`` or ``-1`` means infinite time
-        task_params: additional parameters of the task
-        seed: value for fixed random seed
-        logging_level: logging levels are the same as in 'logging'
-
-            .. details:: possible ``logging_level`` options:
-
-                    - ``50`` -> critical
-                    - ``40`` -> error
-                    - ``30`` -> warning
-                    - ``20`` -> info
-                    - ``10`` -> debug
-                    - ``0`` -> nonset
+        timeout: time for model design (in minutes): ``None`` or ``-1`` means infinite time.
+        task_params: additional parameters of the task.
+        seed: value for a fixed random seed.
+        logging_level: logging levels are the same as in `logging <https://docs.python.org/3/library/logging.html>`_.
+
+            .. details:: Possible options:
+
+                - ``50`` -> critical
+                - ``40`` -> error
+                - ``30`` -> warning
+                - ``20`` -> info
+                - ``10`` -> debug
+                - ``0`` -> nonset
 
         safe_mode: if set ``True`` it will cut large datasets to prevent memory overflow and use label encoder
-            instead of oneHot encoder if summary cardinality of categorical features is high.
-        n_jobs: num of ``n_jobs`` for parallelization (``-1`` for use all cpu's)
-        parallelization_mode: type of evaluation for candidate solution groups (populational or sequential)
-        max_depth: max depth of the pipeline
-        max_arity: max arity of the pipeline nodes
-        pop_size: population size for composer
-        num_of_generations: number of generations for composer
-        keep_n_best: Number of the best individuals of previous generation to keep in next generation.
-        available_operations: list of model names to use
-        early_stopping_iterations: composer will stop after ``n`` generation without improving
-        early_stopping_timeout: stagnation timeout in minutes: composer will stop after ``n`` minutes without improving
-        with_tuning: allow hyperparameters tuning for the model
-        cv_folds: number of folds for cross-validation
-        validation_blocks: number of validation blocks for time series forecasting
-        max_pipeline_fit_time: time constraint for operation fitting (in minutes)
-        initial_assumption: initial assumption for composer
-        genetic_scheme: name of the genetic scheme
-        history_folder: name of the folder for composing history
-        metric:  metric for quality calculation during composing, also is used for tuning if ``with_tuning=True``
-        collect_intermediate_metric: save metrics for intermediate (non-root) nodes in pipeline
-        preset: name of preset for model building (e.g. 'best_quality', 'fast_train', 'gpu'):
+            instead of OneHot encoder if summary cardinality of categorical features is high.
+            Default value is ``False``.
+
+        n_jobs: num of ``n_jobs`` for parallelization (set to ``-1`` to use all cpu's). Defaults to ``-1``.
+        parallelization_mode (str): type of evaluation for groups of individuals (``'populational'`` or
+            ``'sequential'``). Default value is ``'populational'``.
+
+        initial_assumption (Union[Pipeline, List[Pipeline]]): initial assumption(s) for composer.
+            Can be either a single :class:`Pipeline` or sequence of ones. Default values are task-specific and
+            selected by the method :meth:`~fedot.api.api_utils.assumptions.task_assumptions.TaskAssumptions.for_task`.
+
+        available_operations (List[str])): list of model names to use. Pick the names according to the `repositories \
+            <https://github.com/aimclub/FEDOT/tree/master/fedot/core/repository/data>`_.
+
+        metric (Union[str, Callable, fedot.core.repository.quality_metrics_repository.MetricsEnum, List[str, \
+            Callable, fedot.core.repository.quality_metrics_repository.MetricsEnum]):
+            metric for quality calculation during composing, also is used for tuning if ``with_tuning=True``.
+
+            .. details:: Default value depends on a given task:
+
+                - ``roc_auc`` -> for classification
+                - ``rmse`` -> for regression & time series forecasting
+
+            .. details:: Available metrics are listed in the following enumerations:
+
+                - classification -> \
+                    :class:`~fedot.core.repository.quality_metrics_repository.ClassificationMetricsEnum`
+                - regression & time series forcasting -> \
+                    :class:`~fedot.core.repository.quality_metrics_repository.RegressionMetricsEnum`
+                - pipeline complexity (task-independent)-> \
+                    :class:`~fedot.core.repository.quality_metrics_repository.ComplexityMetricsEnum`
+
+        collect_intermediate_metric (bool): save metrics for intermediate (non-root) nodes in composed
+            :class:`Pipeline`.
 
-            .. details:: possible ``preset`` options:
+        cv_folds (int): number of folds for cross-validation.
 
-                - ``best_quality`` -> All models that are available for this data type and task are used
-                - ``fast_train`` -> Models that learn quickly. This includes preprocessing operations
+            .. details:: Default value depends on the given ``problem``:
+
+                - ``5`` -> for classification and regression tasks
+                - ``3`` -> for time series forecasting task
+
+        validation_blocks (int): number of validation blocks for time series forecasting. Default value is ``2``.
+
+        show_progress (bool): indicates whether to show progress using tqdm/tuner or not. Defaults to ``True``.
+
+        num_of_generations (int): number of evolutionary generations for composer. Defaults to ``None`` - no limit.
+        early_stopping_iterations (int): composer will stop after `n` generation without improving.
+        early_stopping_timeout (int): stagnation timeout in minutes: composer will stop after `n` minutes
+            without improving. Defaults to ``10``.
+        max_pipeline_fit_time (int): time constraint for operation fitting (in minutes).
+            Defaults to ``None`` - no limit. Once the limit is reached, the candidate pipeline will be dropped.
+
+        max_depth (int): max depth of the pipeline. Defaults to ``6``.
+        max_arity (int): max arity of the pipeline nodes. Defaults to ``3``.
+        pop_size (int): size of population (generation) during composing. Defaults to ``20``.
+        keep_n_best (int): number of the best individuals in generation that survive during the evolution.
+             Defaults to ``1``.
+        genetic_scheme (str): name of the genetic scheme. Defaults to ``steady_state``.
+
+        with_tuning (bool): flag for tuning hyperparameters of the final evolved :class:`Pipeline`.
+            Defaults to ``True``.
+
+        preset (str): name of the preset for model building (e.g. ``'best_quality'``, ``'fast_train'``, ``'gpu'``).
+            Default value is ``'auto'``.
+
+            .. details:: Possible options:
+
+                - ``'best_quality'`` -> All models that are available for this data type and task are used
+                - ``'fast_train'`` -> Models that learn quickly. This includes preprocessing operations
                   (data operations) that only reduce the dimensionality of the data, but cannot increase it.
                   For example, there are no polynomial features and one-hot encoding operations
-                - ``stable`` -> The most reliable preset in which the most stable operations are included.
-                - ``auto`` -> Automatically determine which preset should be used.
-                - ``gpu`` -> Models that use GPU resources for computation.
-                - ``ts`` -> A special preset with models for time series forecasting task.
-                - ``automl`` -> A special preset with only AutoML libraries such as TPOT and H2O as operations.
-
-        use_input_preprocessing: bool indicating whether to do preprocessing of further given data, enabled by default.
-        use_pipelines_cache: bool indicating whether to use pipeline structures caching, enabled by default.
-        use_preprocessing_cache: bool indicating whether to use optional preprocessors caching, enabled by default.
-        cache_folder: path to the place where cache files should be stored (if any cache is enabled).
-        show_progress: bool indicating whether to show progress using tqdm/tuner or not
+                - ``'stable'`` -> The most reliable preset in which the most stable operations are included
+                - ``'auto'`` -> Automatically determine which preset should be used
+                - ``'gpu'`` -> Models that use GPU resources for computation
+                - ``'ts'`` -> A special preset with models for time series forecasting task
+                - ``'automl'`` -> A special preset with only AutoML libraries such as TPOT and H2O as operations
+
+        use_input_preprocessing (bool): indicates whether to do preprocessing of further given data.
+            Defaults to ``True``.
+        use_meta_rules (bool): indicates whether to change set params according to FEDOT meta rules.
+        use_pipelines_cache (bool): indicates whether to use pipeline structures caching. Defaults to ``True``.
+        use_preprocessing_cache (bool): bool indicating whether to use optional preprocessors caching.
+            Defaults to ``True``.
+        cache_dir (str): path to the directory containing cache files (if any cache is enabled).
+            By default, creates a folder named "FEDOT" in temporary system files of the OS.
+        history_dir (str): relative or absolute path of the folder for composing history. Has the same default value
+            as ``cache_dir``. A relative path is relative to the default value.
+
+        optimizer (Type[golem.core.optimisers.optimizer.GraphOptimizer]): inherit from
+            :class:`~golem.core.optimisers.optimizer.GraphOptimizer` to specify a custom optimizer.
+            Default optimizer is :class:`~golem.core.optimisers.genetic.gp_optimizer.EvoGraphOptimizer`.
+            See the `example \
+<https://github.com/aimclub/FEDOT/blob/master/examples/advanced/fedot_based_solutions/external_optimizer.py>`_
     """
 
     def __init__(self,
                  problem: str,
                  timeout: Optional[float] = DEFAULT_API_TIMEOUT_MINUTES,
                  task_params: TaskParams = None,
-                 seed=None, logging_level: int = logging.ERROR,
-                 safe_mode=False,
+                 seed: Optional[int] = None, logging_level: int = logging.ERROR,
+                 safe_mode: bool = False,
                  n_jobs: int = -1,
-                 parallelization_mode: str = 'populational',
                  **composer_tuner_params
                  ):
 
+        set_random_seed(seed)
+        self.log = self._init_logger(logging_level)
+
         # Classes for dealing with metrics, data sources and hyperparameters
-        self.metrics = ApiMetrics(problem)
-        self.api_composer = ApiComposer(problem)
-        self.params = ApiParams()
-
-        # Define parameters, that were set via init in init
-        input_params = {'problem': self.metrics.main_problem, 'timeout': timeout,
-                        'composer_tuner_params': composer_tuner_params, 'task_params': task_params,
-                        'seed': seed, 'logging_level': logging_level,
-                        'n_jobs': n_jobs, 'parallelization_mode': parallelization_mode}
-        self.params.initialize_params(input_params)
-
-        # Initialize ApiComposer's cache parameters via ApiParams
-        self.api_composer.init_cache(use_pipelines_cache=self.params.api_params['use_pipelines_cache'],
-                                     use_input_preprocessing=self.params.api_params['use_input_preprocessing'],
-                                     use_preprocessing_cache=self.params.api_params['use_preprocessing_cache'],
-                                     cache_folder=self.params.api_params['cache_folder'])
-        self.tuner_requirements = None
+        self.params = ApiParams(composer_tuner_params, problem, task_params, n_jobs, timeout)
+        self.metrics = ApiMetrics(self.params.task, self.params.get('metric'))
+
+        self.api_composer = ApiComposer(self.params, self.metrics)
 
         # Initialize data processors for data preprocessing and preliminary data analysis
-        self.data_processor = ApiDataProcessor(task=self.params.api_params['task'],
-                                               use_input_preprocessing=self.params.api_params[
-                                                   'use_input_preprocessing'])
-        self.data_analyser = DataAnalyser(safe_mode=safe_mode)
+        self.data_processor = ApiDataProcessor(task=self.params.task,
+                                               use_input_preprocessing=self.params.get('use_input_preprocessing'))
+        self.data_analyser = InputAnalyser(safe_mode=safe_mode)
 
         self.target: Optional[TargetType] = None
         self.prediction: Optional[OutputData] = None
         self._is_in_sample_prediction = True
         self.train_data: Optional[InputData] = None
         self.test_data: Optional[InputData] = None
 
@@ -173,107 +219,103 @@
         """
 
         MemoryAnalytics.start()
 
         self.target = target
 
         self.train_data = self.data_processor.define_data(features=features, target=target, is_predict=False)
-        if self.params.api_params['use_input_preprocessing']:
+        self.params.update_available_operations_by_preset(self.train_data)
+
+        if self.params.get('use_input_preprocessing'):
             # Launch data analyser - it gives recommendations for data preprocessing
-            recommendations = self.data_analyser.give_recommendation(self.train_data)
-            self.data_processor.accept_and_apply_recommendations(self.train_data, recommendations)
-            self.params.accept_and_apply_recommendations(self.train_data, recommendations)
+            recommendations_for_data, recommendations_for_params = \
+                self.data_analyser.give_recommendations(input_data=self.train_data,
+                                                        input_params=self.params)
+            self.data_processor.accept_and_apply_recommendations(input_data=self.train_data,
+                                                                 recommendations=recommendations_for_data)
+            self.params.accept_and_apply_recommendations(input_data=self.train_data,
+                                                         recommendations=recommendations_for_params)
         else:
-            recommendations = None
+            recommendations_for_data = None
 
         self._init_remote_if_necessary()
 
-        if self.params.api_params['preset'] != 'auto':
-            self.params.update_available_operations_by_preset(self.train_data)
-
-        self.params.api_params['train_data'] = self.train_data
-
         if predefined_model is not None:
-            self.api_composer.set_tuner_requirements(**self.params.api_params)
-
             # Fit predefined model and return it without composing
-            self.current_pipeline = PredefinedModel(predefined_model,
-                                                    self.train_data,
-                                                    self.params.api_params['logger'],
-                                                    use_input_preprocessing=self.params.api_params[
-                                                        'use_input_preprocessing']).fit()
+            self.current_pipeline = PredefinedModel(predefined_model, self.train_data, self.log,
+                                                    use_input_preprocessing=self.params.get(
+                                                        'use_input_preprocessing')).fit()
         else:
-            self.current_pipeline, self.best_models, self.history = \
-                self.api_composer.obtain_model(**self.params.api_params)
+            self.current_pipeline, self.best_models, self.history = self.api_composer.obtain_model(self.train_data)
 
             if self.current_pipeline is None:
                 raise ValueError('No models were found')
 
             full_train_not_preprocessed = deepcopy(self.train_data)
             # Final fit for obtained pipeline on full dataset
             if self.history and not self.history.is_empty() or not self.current_pipeline.is_fitted:
-                self._train_pipeline_on_full_dataset(recommendations, full_train_not_preprocessed)
-                self.params.api_params['logger'].message('Final pipeline was fitted')
+                self._train_pipeline_on_full_dataset(recommendations_for_data, full_train_not_preprocessed)
+                self.log.message('Final pipeline was fitted')
             else:
-                self.params.api_params['logger'].message('Already fitted initial pipeline is used')
+                self.log.message('Already fitted initial pipeline is used')
 
         # Store data encoder in the pipeline if it is required
         self.current_pipeline.preprocessor = BasePreprocessor.merge_preprocessors(
             self.data_processor.preprocessor, self.current_pipeline.preprocessor)
 
-        self.params.api_params['logger'].message(f'Final pipeline: {graph_structure(self.current_pipeline)}')
+        self.log.message(f'Final pipeline: {graph_structure(self.current_pipeline)}')
 
         MemoryAnalytics.finish()
 
         return self.current_pipeline
 
     def tune(self,
-             input_data: InputData = None,
-             metric_name: str = None,
+             input_data: Optional[InputData] = None,
+             metric_name: Optional[Union[str, Callable]] = None,
              iterations: int = DEFAULT_TUNING_ITERATIONS_NUMBER,
              timeout: Optional[float] = None,
-             cv_folds: int = None,
-             n_jobs: int = None,
+             cv_folds: Optional[int] = None,
+             validation_blocks: Optional[int] = None,
+             n_jobs: Optional[int] = None,
              show_progress: bool = False) -> Pipeline:
         """Method for hyperparameters tuning of current pipeline
 
         Args:
-            input_data: data for tuning pipeline
-            metric_name: name of metric for quality tuning
-            iterations: numbers of tuning iterations
-            timeout: time for tuning (in minutes). If ``None`` or ``-1`` means tuning until max iteration reach
+            input_data: data for tuning pipeline.
+            metric_name: name of metric for quality tuning.
+            iterations: numbers of tuning iterations.
+            timeout: time for tuning (in minutes). If ``None`` or ``-1`` means tuning until max iteration reach.
             cv_folds: number of folds on data for cross-validation.
-            n_jobs: num of ``n_jobs`` for parallelization (``-1`` for use all cpu's)
-            show_progress: shows progress of tuning if true
+            validation_blocks: number of validation blocks (used for time-series forecasting problem).
+            n_jobs: num of ``n_jobs`` for parallelization (``-1`` for use all cpu's).
+            show_progress: shows progress of tuning if ``True``.
 
         Returns:
-            Pipeline object
+            :class:`Pipeline` object.
 
         """
         if self.current_pipeline is None:
             raise ValueError(NOT_FITTED_ERR_MSG)
 
         input_data = input_data or self.train_data
-
-        if metric_name is None:
-            metric_name = self.metrics.get_problem_metrics()[0]
-
-        if cv_folds is not None:
-            self.api_composer.tuner_requirements.cv_folds = cv_folds
-
-        if n_jobs is not None:
-            self.api_composer.tuner_requirements.n_jobs = n_jobs
-
-        pipeline_tuner = TunerBuilder(self.params.task) \
-            .with_tuner(SimultaneousTuner) \
-            .with_requirements(self.api_composer.tuner_requirements) \
-            .with_metric(self.metrics.get_metrics_mapping(metric_name)) \
-            .with_iterations(iterations) \
-            .with_timeout(timeout) \
-            .build(input_data)
+        cv_folds = cv_folds or self.params.get('cv_folds')
+        validation_blocks = validation_blocks or self.params.get('validation_blocks')
+        n_jobs = n_jobs or self.params.n_jobs
+
+        metric = self.metrics.obtain_metrics(metric_name)[0] if metric_name else self.metrics.metric_functions[0]
+
+        pipeline_tuner = (TunerBuilder(self.params.task)
+                          .with_tuner(SimultaneousTuner)
+                          .with_cv_folds(cv_folds)
+                          .with_validation_blocks(validation_blocks)
+                          .with_n_jobs(n_jobs)
+                          .with_metric(metric)
+                          .with_iterations(iterations)
+                          .with_timeout(timeout)
+                          .build(input_data))
 
         self.current_pipeline = pipeline_tuner.tune(self.current_pipeline, show_progress)
         self.api_composer.was_tuned = pipeline_tuner.was_tuned
 
         # Tuner returns a not fitted pipeline, and it is required to fit on train dataset
         self.current_pipeline.fit(self.train_data)
         return self.current_pipeline
@@ -285,32 +327,32 @@
                 validation_blocks: Optional[int] = None) -> np.ndarray:
         """Predicts new target using already fitted model.
 
         For time-series performs forecast with depth ``forecast_length`` if ``in_sample=False``.
         If ``in_sample=True`` performs in-sample forecast using features as sample.
 
         Args:
-            features: the array with features of test data
-            save_predictions: if ``True`` - save predictions as csv-file in working directory
+            features: the array with features of test data.
+            save_predictions: if ``True`` - save predictions as csv-file in working directory.
             in_sample: used while time-series prediction. If ``in_sample=True`` performs in-sample forecast using
                 features with number if iterations specified in ``validation_blocks``.
             validation_blocks: number of validation blocks for in-sample forecast.
                 If ``validation_blocks = None`` uses number of validation blocks set during model initialization
-                (default is 2).
+                (default is ``2``).
 
 
         Returns:
-            the array with prediction values
+            The array with prediction values.
         """
         if self.current_pipeline is None:
             raise ValueError(NOT_FITTED_ERR_MSG)
 
         self.test_data = self.data_processor.define_data(target=self.target, features=features, is_predict=True)
         self._is_in_sample_prediction = in_sample
-        validation_blocks = validation_blocks or self.params.api_params.get('validation_blocks')
+        validation_blocks = validation_blocks or self.params.get('validation_blocks')
 
         self.prediction = self.data_processor.define_predictions(current_pipeline=self.current_pipeline,
                                                                  test_data=self.test_data,
                                                                  in_sample=self._is_in_sample_prediction,
                                                                  validation_blocks=validation_blocks)
 
         if save_predictions:
@@ -321,26 +363,26 @@
     def predict_proba(self,
                       features: FeaturesType,
                       save_predictions: bool = False,
                       probs_for_all_classes: bool = False) -> np.ndarray:
         """Predicts the probability of new target using already fitted classification model
 
         Args:
-            features: the array with features of test data
-            save_predictions: if ``True`` - save predictions as csv-file in working directory
-            probs_for_all_classes: if ``True`` - return probability for each class even for binary case
+            features: the array with features of test data.
+            save_predictions: if ``True`` - save predictions as ``.csv`` file in working directory.
+            probs_for_all_classes: if ``True`` - return probability for each class even for binary classification.
 
         Returns:
-            the array with prediction values
+            The array with prediction values.
         """
 
         if self.current_pipeline is None:
             raise ValueError(NOT_FITTED_ERR_MSG)
 
-        if self.params.api_params['task'].task_type == TaskTypesEnum.classification:
+        if self.params.task.task_type == TaskTypesEnum.classification:
             self.test_data = self.data_processor.define_data(target=self.target,
                                                              features=features, is_predict=True)
 
             mode = 'full_probs' if probs_for_all_classes else 'probs'
 
             self.prediction = self.current_pipeline.predict(self.test_data, output_mode=mode)
 
@@ -355,20 +397,20 @@
                  pre_history: Optional[Union[str, Tuple[np.ndarray, np.ndarray], InputData, dict]] = None,
                  horizon: Optional[int] = None,
                  save_predictions: bool = False) -> np.ndarray:
         """Forecasts the new values of time series. If horizon is bigger than forecast length of fitted model -
         out-of-sample forecast is applied (not supported for multi-modal data).
 
         Args:
-            pre_history: the array with features for pre-history of the forecast
-            horizon: num of steps to forecast
-            save_predictions: if ``True`` save predictions as csv-file in working directory
+            pre_history: the array with features for pre-history of the forecast.
+            horizon: amount of steps to forecast.
+            save_predictions: if ``True`` save predictions as csv-file in working directory.
 
         Returns:
-            the array with prediction values
+            The array with prediction values.
         """
         self._check_forecast_applicable()
 
         forecast_length = self.train_data.task.task_params.forecast_length
         horizon = horizon or forecast_length
         if pre_history is None:
             pre_history = self.train_data
@@ -383,135 +425,126 @@
             self.save_predict(self.prediction)
         return self.prediction.predict
 
     def _check_forecast_applicable(self):
         if self.current_pipeline is None:
             raise ValueError(NOT_FITTED_ERR_MSG)
 
-        if self.params.api_params['task'].task_type != TaskTypesEnum.ts_forecasting:
+        if self.params.task.task_type != TaskTypesEnum.ts_forecasting:
             raise ValueError('Forecasting can be used only for the time series')
 
     def load(self, path):
         """Loads saved graph from disk
 
         Args:
-            path: path to ``json`` file with model
+            path: path to ``json`` file with model.
         """
-        self.current_pipeline = Pipeline(use_input_preprocessing=self.params.api_params['use_input_preprocessing'])
+        self.current_pipeline = Pipeline(use_input_preprocessing=self.params.get('use_input_preprocessing'))
         self.current_pipeline.load(path)
         self.data_processor.preprocessor = self.current_pipeline.preprocessor
 
     def plot_pareto(self):
-        metric_names = self.api_composer.metric_names
+        metric_names = self.metrics.metric_names
         # archive_history stores archives of the best models.
         # Each archive is sorted from the best to the worst model,
         # so the best_candidates is sorted too.
         best_candidates = self.history.archive_history[-1]
         visualise_pareto(front=best_candidates,
                          objectives_names=metric_names,
                          show=True)
 
     def plot_prediction(self, in_sample: Optional[bool] = None, target: Optional[Any] = None):
         """Plots the prediction obtained from graph
 
         Args:
-            in_sample: if current prediction is in_sample (for time-series forecasting).
-            Plots predictions as future values
-            target: user-specified name of target variable for :obj:`MultiModalData`
+            in_sample: if current prediction is in_sample (for time-series forecasting), plots predictions as future
+                values.
+            target: user-specified name of target variable for :class:`MultiModalData`.
 
         """
+        task = self.params.task
+
         if self.prediction is not None:
-            if self.params.api_params['task'].task_type == TaskTypesEnum.ts_forecasting:
+            if task.task_type == TaskTypesEnum.ts_forecasting:
                 in_sample = in_sample or self._is_in_sample_prediction
                 plot_forecast(self.test_data, self.prediction, in_sample, target)
-            elif self.params.api_params['task'].task_type == TaskTypesEnum.regression:
+            elif task.task_type == TaskTypesEnum.regression:
                 plot_biplot(self.prediction)
-            elif self.params.api_params['task'].task_type == TaskTypesEnum.classification:
+            elif task.task_type == TaskTypesEnum.classification:
                 self.predict_proba(self.test_data)
                 plot_roc_auc(self.test_data, self.prediction)
             else:
-                self.params.api_params['logger'].error('Not supported yet')
-                raise NotImplementedError(f"For task {self.params.api_params['task']} plot prediction is not supported")
+                self.log.error('Not supported yet')
+                raise NotImplementedError(f"For task {task} plot prediction is not supported")
         else:
-            self.params.api_params['logger'].error('No prediction to visualize')
+            self.log.error('No prediction to visualize')
             raise ValueError('Prediction from model is empty')
 
     def get_metrics(self,
                     target: Union[np.ndarray, pd.Series] = None,
                     metric_names: Union[str, List[str]] = None,
                     in_sample: Optional[bool] = None,
                     validation_blocks: Optional[int] = None) -> dict:
         """Gets quality metrics for the fitted graph
 
         Args:
-            target: the array with target values of test data. If None, target specified for fit is used
+            target: the array with target values of test data. If ``None``, target specified for fit is used.
             metric_names: the names of required metrics.
-            in_sample: used for time-series forecasting.
+            in_sample: used for time series forecasting.
                 If True prediction will be obtained as ``.predict(..., in_sample=True)``.
-            validation_blocks: number of validation blocks for in-sample forecast.
-                If None uses number of validation blocks set during model initialisation
-                (default is 2).
+            validation_blocks: number of validation blocks for time series in-sample forecast.
+                If ``None``, uses number of validation blocks set during model initialization (default is ``2``).
 
         Returns:
-            the values of quality metrics
+            The values of quality metrics.
         """
-        if metric_names is None:
-            metric_names = self.params.metric_name
+        if self.current_pipeline is None:
+            raise ValueError(NOT_FITTED_ERR_MSG)
 
         if target is not None:
             if self.test_data is None:
                 self.test_data = InputData(idx=range(len(self.prediction.predict)),
                                            features=None,
                                            target=target[:len(self.prediction.predict)],
                                            task=self.train_data.task,
                                            data_type=self.train_data.data_type)
             else:
                 self.test_data.target = target[:len(self.prediction.predict)]
 
-        metric_names = ensure_wrapped_in_sequence(metric_names)
+        metrics = self.metrics.obtain_metrics(metric_names) if metric_names else self.metrics.metric_functions
+        metric_names = self.metrics.get_metric_names(metrics)
 
-        calculated_metrics = dict()
-        for metric_name in metric_names:
-            if self.metrics.get_metrics_mapping(metric_name) is NotImplemented:
-                self.params.api_params['logger'].warning(f'{metric_name} is not available as metric')
-            else:
-                composer_metric = self.metrics.get_metrics_mapping(metric_name)
-                metric_cls = MetricsRepository().metric_class_by_id(composer_metric)
-                prediction = deepcopy(self.prediction)
-                if metric_name == "roc_auc":  # for roc-auc we need probabilities
-                    prediction.predict = self.predict_proba(self.test_data)
-                else:
-                    if in_sample is not None:
-                        self._is_in_sample_prediction = in_sample
-                    prediction.predict = self.predict(self.test_data, in_sample=self._is_in_sample_prediction,
-                                                      validation_blocks=validation_blocks)
-                real = deepcopy(self.test_data)
-
-                # Work inplace - correct predictions
-                self.data_processor.correct_predictions(real=real,
-                                                        prediction=prediction)
-
-                real.target = np.ravel(real.target)
-
-                metric_value = abs(metric_cls.metric(reference=real,
-                                                     predicted=prediction))
-                calculated_metrics[metric_name] = round(metric_value, 3)
+        in_sample = in_sample if in_sample is not None else self._is_in_sample_prediction
 
-        return calculated_metrics
+        if in_sample:
+            validation_blocks = validation_blocks or self.params.get('validation_blocks')
+        else:
+            validation_blocks = None
+
+        objective = MetricsObjective(metrics)
+        obj_eval = PipelineObjectiveEvaluate(objective=objective,
+                                             data_producer=lambda: (yield self.train_data, self.test_data),
+                                             validation_blocks=validation_blocks, eval_n_jobs=self.params.n_jobs,
+                                             do_unfit=False)
+
+        metrics = obj_eval.evaluate(self.current_pipeline).values
+        metrics = {metric_name: round(abs(metric), 3) for (metric_name, metric) in zip(metric_names, metrics)}
+
+        return metrics
 
     def save_predict(self, predicted_data: OutputData):
         # TODO unify with OutputData.save_to_csv()
         """ Saves pipeline forecasts in csv file """
         if len(predicted_data.predict.shape) >= 2:
             prediction = predicted_data.predict.tolist()
         else:
             prediction = predicted_data.predict
         pd.DataFrame({'Index': predicted_data.idx,
                       'Prediction': prediction}).to_csv(r'./predictions.csv', index=False)
-        self.params.api_params['logger'].message('Predictions was saved in current directory.')
+        self.log.message('Predictions was saved in current directory.')
 
     def export_as_project(self, project_path='fedot_project.zip'):
         export_project_to_zip(zip_name=project_path, opt_history=self.history,
                               pipeline=self.current_pipeline,
                               train_data=self.train_data, test_data=self.test_data)
 
     def import_as_project(self, project_path='fedot_project.zip'):
@@ -528,35 +561,40 @@
             An :obj:`Explainer` instance will return.
 
         Args:
             features: samples to be explained. If ``None``, ``train_data`` from last fit will be used.
             method: explanation method, defaults to ``surrogate_dt``
             visualization: print and plot the explanation simultaneously, defaults to ``True``.
         Notes:
-            The explanation can be retrieved later by executing :obj:`explainer.visualize()`
+            The explanation can be retrieved later by executing :obj:`explainer.visualize()`.
         """
         pipeline = self.current_pipeline
         if features is None:
             data = self.train_data
         else:
             data = self.data_processor.define_data(features=features,
                                                    is_predict=False)
         explainer = explain_pipeline(pipeline=pipeline, data=data, method=method,
                                      visualization=visualization, **kwargs)
 
         return explainer
 
+    @staticmethod
+    def _init_logger(logging_level: int):
+        # reset logging level for Singleton
+        Log().reset_logging_level(logging_level)
+        return default_log(prefix='FEDOT logger')
+
     def _init_remote_if_necessary(self):
         remote = RemoteEvaluator()
         if remote.is_enabled and remote.remote_task_params is not None:
-            task = self.params.api_params['task']
+            task = self.params.task
             if task.task_type is TaskTypesEnum.ts_forecasting:
-                task_str = \
-                    f'Task(TaskTypesEnum.ts_forecasting, ' \
-                    f'TsForecastingParams(forecast_length={task.task_params.forecast_length}))'
+                task_str = (f'Task(TaskTypesEnum.ts_forecasting, '
+                            f'TsForecastingParams(forecast_length={task.task_params.forecast_length}))')
             else:
                 task_str = f'Task({str(task.task_type)})'
             remote.remote_task_params.task_type = task_str
             remote.remote_task_params.is_multi_modal = isinstance(self.train_data, MultiModalData)
 
             if isinstance(self.target, str) and remote.remote_task_params.target is None:
                 remote.remote_task_params.target = self.target
@@ -569,9 +607,9 @@
         if recommendations is not None:
             # if data was cut we need to refit pipeline on full data
             self.data_processor.accept_and_apply_recommendations(full_train_not_preprocessed,
                                                                  {k: v for k, v in recommendations.items()
                                                                   if k != 'cut'})
         self.current_pipeline.fit(
             full_train_not_preprocessed,
-            n_jobs=self.params.api_params['n_jobs']
+            n_jobs=self.params.n_jobs
         )
```

### Comparing `fedot-0.7.0/fedot/api/time.py` & `fedot-0.7.1/fedot/api/time.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/caching/base_cache.py` & `fedot-0.7.1/fedot/core/caching/base_cache.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/caching/base_cache_db.py` & `fedot-0.7.1/fedot/core/caching/base_cache_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 
 class BaseCacheDB:
     """
     Base class for caching in database.
     Includes low-level idea of caching data using relational database.
 
     :param main_table: table to store into or load from
-    :param cache_folder: path to the place where cache files should be stored.
+    :param cache_dir: path to the place where cache files should be stored.
     :param use_stats: bool indicating if it is needed to use cache performance dict
     :param stats_keys: sequence of keys for supporting cache effectiveness
     """
 
-    def __init__(self, main_table: str = 'default', cache_folder: Optional[str] = None, use_stats: bool = False,
+    def __init__(self, main_table: str = 'default', cache_dir: Optional[str] = None, use_stats: bool = False,
                  stats_keys: Sequence = ('default_hit', 'default_total')):
         self._main_table = main_table
         self._db_suffix = f'.{main_table}_db'
-        if cache_folder is None:
+        if cache_dir is None or Path(cache_dir).samefile(default_fedot_data_dir()):
             self.db_path = Path(default_fedot_data_dir())
             self._del_prev_temps()
         else:
-            self.db_path = Path(cache_folder)
+            self.db_path = Path(cache_dir)
         self.db_path = self.db_path.joinpath(f'cache_{os.getpid()}').with_suffix(self._db_suffix)
 
         self._eff_table = 'effectiveness'
         self.use_stats = use_stats
         self._effectiveness_keys = stats_keys
         self._init_eff()
```

### Comparing `fedot-0.7.0/fedot/core/caching/pipelines_cache.py` & `fedot-0.7.1/fedot/core/caching/pipelines_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+import sqlite3
 from typing import List, Optional, TYPE_CHECKING, Union
 
 from golem.core.utilities.data_structures import ensure_wrapped_in_sequence
 
 from fedot.core.caching.base_cache import BaseCache
 from fedot.core.caching.pipelines_cache_db import OperationsCacheDB
 from fedot.core.pipelines.node import PipelineNode
-from fedot.utilities.debug import is_test_session
 
 if TYPE_CHECKING:
     from fedot.core.pipelines.pipeline import Pipeline
 
 
 class OperationsCache(BaseCache):
     """
     Stores/loads nodes `fitted_operation` field to increase performance of calculations.
 
-    :param cache_folder: path to the place where cache files should be stored.
+    :param cache_dir: path to the place where cache files should be stored.
     """
 
-    def __init__(self, cache_folder: Optional[str] = None):
-        super().__init__(OperationsCacheDB(cache_folder))
+    def __init__(self, cache_dir: Optional[str] = None):
+        super().__init__(OperationsCacheDB(cache_dir))
 
     def save_nodes(self, nodes: Union[PipelineNode, List[PipelineNode]], fold_id: Optional[int] = None):
         """
         :param nodes: node/nodes to be cached
         :param fold_id: optional part of cache item UID
                             (can be used to specify the number of CV fold)
         """
@@ -31,15 +31,16 @@
             mapped = [
                 (_get_structural_id(node, fold_id), node.fitted_operation)
                 for node in ensure_wrapped_in_sequence(nodes)
                 if node.fitted_operation is not None
             ]
             self._db.add_operations(mapped)
         except Exception as ex:
-            self.log.warning(f'Nodes can not be saved: {ex}. Continue', raise_if_test=True)
+            unexpected_exc = not (isinstance(ex, sqlite3.DatabaseError) and 'disk is full' in str(ex))
+            self.log.warning(f'Nodes can not be saved: {ex}. Continue', exc=ex, raise_if_test=unexpected_exc)
 
     def save_pipeline(self, pipeline: 'Pipeline', fold_id: Optional[int] = None):
         """
         :param pipeline: pipeline to be cached
         :param fold_id: optional part of cache item UID
                             (can be used to specify the number of CV fold)
         """
@@ -57,15 +58,15 @@
             cached_ops = self._db.get_operations(structural_ids)
             for idx, cached_op in enumerate(cached_ops):
                 if cached_op is not None:
                     nodes_lst[idx].fitted_operation = cached_op
                 else:
                     nodes_lst[idx].fitted_operation = None
         except Exception as ex:
-            self.log.warning(f'Cache can not be loaded: {ex}. Continue.', raise_if_test=True)
+            self.log.warning(f'Cache can not be loaded: {ex}. Continue.', exc=ex, raise_if_test=True)
 
     def try_load_into_pipeline(self, pipeline: 'Pipeline', fold_id: Optional[int] = None):
         """
         :param pipeline: pipeline for loading into from cache
         :param fold_id: optional part of cache item UID (number of the CV fold)
         """
         self.try_load_nodes(pipeline.nodes, fold_id)
```

### Comparing `fedot-0.7.0/fedot/core/caching/pipelines_cache_db.py` & `fedot-0.7.1/fedot/core/caching/pipelines_cache_db.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 
 class OperationsCacheDB(BaseCacheDB):
     """
     Database for `OperationsCache` class.
     Includes low-level idea of caching pipeline nodes using relational database.
 
-    :param cache_folder: path to the place where cache files should be stored.
+    :param cache_dir: path to the place where cache files should be stored.
     """
 
-    def __init__(self, cache_folder: Optional[str] = None):
-        super().__init__('operations', cache_folder, False, ['pipelines_hit', 'pipelines_total', 'nodes_hit', 'nodes_total'])
+    def __init__(self, cache_dir: Optional[str] = None):
+        super().__init__('operations', cache_dir, False, ['pipelines_hit', 'pipelines_total', 'nodes_hit', 'nodes_total'])
         self._init_db()
 
     @staticmethod
     def _create_temp_for_ordered_select(cur: sqlite3.Cursor, uids: List[str]) -> str:
         """
         Creates temp table to keep order of uids while doing select operation in operations getter.
```

### Comparing `fedot-0.7.0/fedot/core/caching/preprocessing_cache.py` & `fedot-0.7.1/fedot/core/caching/preprocessing_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 
 class PreprocessingCache(BaseCache):
     """
     Usage of that class makes sense only if you have table data.
     Stores/loads `DataPreprocessor`'s encoders and imputers for pipelines to decrease optional preprocessing time.
 
-    :param cache_folder: path to the place where cache files should be stored.
+    :param cache_dir: path to the place where cache files should be stored.
     """
 
-    def __init__(self, cache_folder: Optional[str] = None):
-        super().__init__(PreprocessingCacheDB(cache_folder))
+    def __init__(self, cache_dir: Optional[str] = None):
+        super().__init__(PreprocessingCacheDB(cache_dir))
 
     def try_load_preprocessor(self, pipeline: 'Pipeline', fold_id: Union[int, None]):
         """
         Tries to find preprocessor in DB table and load it for pipeline
 
         :param pipeline: pipeline to load preprocessor for
         :param fold_id: number of fold
```

### Comparing `fedot-0.7.0/fedot/core/caching/preprocessing_cache_db.py` & `fedot-0.7.1/fedot/core/caching/preprocessing_cache_db.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 
 
 class PreprocessingCacheDB(BaseCacheDB):
     """
     Database for `PreprocessingCache` class.
     Includes low-level idea of caching pipeline preprocessor items using relational database.
 
-    :param cache_folder: path to the place where cache files should be stored.
+    :param cache_dir: path to the place where cache files should be stored.
     """
 
-    def __init__(self, cache_folder: Optional[str] = None):
-        super().__init__('preprocessors', cache_folder, False, ['preprocessors_hit', 'preprocessors_total'])
+    def __init__(self, cache_dir: Optional[str] = None):
+        super().__init__('preprocessors', cache_dir, False, ['preprocessors_hit', 'preprocessors_total'])
         self._init_db()
 
     def get_preprocessor(self, uid: str) -> Optional[Tuple[
         Dict[str, OneHotEncodingImplementation], Dict[str, ImputationImplementation]
     ]]:
         """
         Tries to return both data processors, None if is not found
```

### Comparing `fedot-0.7.0/fedot/core/composer/composer.py` & `fedot-0.7.1/fedot/core/composer/composer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/composer/composer_builder.py` & `fedot-0.7.1/fedot/core/composer/composer_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import platform
 from multiprocessing import set_start_method
 from pathlib import Path
-from typing import Dict, List, Optional, Sequence, Type, Union
+from typing import List, Optional, Sequence, Type, Union
 
 from golem.core.log import LoggerAdapter, default_log
 from golem.core.optimisers.genetic.gp_optimizer import EvoGraphOptimizer
 from golem.core.optimisers.genetic.gp_params import GPAlgorithmParameters
-from fedot.core.pipelines.pipeline_composer_requirements import PipelineComposerRequirements
 from golem.core.optimisers.initial_graphs_generator import InitialPopulationGenerator, GenerationFunction
 from golem.core.optimisers.optimizer import GraphOptimizer, AlgorithmParameters, GraphGenerationParams
 from golem.core.utilities.data_structures import ensure_wrapped_in_sequence
 
 from fedot.core.caching.pipelines_cache import OperationsCache
 from fedot.core.caching.preprocessing_cache import PreprocessingCache
 from fedot.core.composer.composer import Composer
 from fedot.core.composer.gp_composer.gp_composer import GPComposer
 from fedot.core.optimisers.objective.metrics_objective import MetricsObjective
 from fedot.core.pipelines.pipeline import Pipeline
+from fedot.core.pipelines.pipeline_composer_requirements import PipelineComposerRequirements
 from fedot.core.pipelines.pipeline_graph_generation_params import get_pipeline_generation_params
 from fedot.core.pipelines.verification import rules_by_task
 from fedot.core.repository.operation_types_repository import get_operations_for_task
 from fedot.core.repository.quality_metrics_repository import (
     ComplexityMetricsEnum,
     MetricsEnum,
     MetricType
@@ -42,15 +42,14 @@
         self.log: LoggerAdapter = default_log(self)
 
         self.task: Task = task
         self.metrics: Sequence[MetricsEnum] = MetricByTask.get_default_quality_metrics(task.task_type)
 
         self.optimizer_cls: Type[GraphOptimizer] = EvoGraphOptimizer  # default optimizer class
         self.optimizer_parameters: Optional[AlgorithmParameters] = None
-        self.optimizer_external_parameters: dict = {}
 
         self.composer_cls: Type[Composer] = GPComposer  # default composer class
         self.composer_requirements: Optional[PipelineComposerRequirements] = None
         self.graph_generation_params: Optional[GraphGenerationParams] = None
 
         self.initial_population: Union[Pipeline, Sequence[Pipeline]] = ()
         self.initial_population_generation_function: Optional[GenerationFunction] = None
@@ -68,20 +67,17 @@
 
     def with_optimizer(self, optimizer_cls: Optional[Type[GraphOptimizer]]):
         if optimizer_cls:
             self.optimizer_cls = optimizer_cls
         return self
 
     def with_optimizer_params(self, parameters: Optional[AlgorithmParameters] = None,
-                              external_parameters: Optional[Dict] = None,
                               dispatcher=None):
         if parameters is not None:
             self.optimizer_parameters = parameters
-        if external_parameters is not None:
-            self.optimizer_external_parameters = external_parameters
         if dispatcher is not None:
             self.optimizer_parameters = dispatcher
         return self
 
     def with_requirements(self, requirements: PipelineComposerRequirements):
         self.composer_requirements = requirements
         if self.composer_requirements.max_graph_fit_time:
@@ -153,16 +149,15 @@
             .with_initial_graphs(self.initial_population) \
             .with_custom_generation_function(self.initial_population_generation_function)()
 
         optimiser = self.optimizer_cls(objective=objective,
                                        initial_graphs=initial_population,
                                        requirements=self.composer_requirements,
                                        graph_generation_params=self.graph_generation_params,
-                                       graph_optimizer_params=self.optimizer_parameters,
-                                       **self.optimizer_external_parameters)
+                                       graph_optimizer_params=self.optimizer_parameters)
 
         composer = self.composer_cls(optimiser,
                                      self.composer_requirements,
                                      self.pipelines_cache,
                                      self.preprocessing_cache)
 
         return composer
```

### Comparing `fedot-0.7.0/fedot/core/composer/gp_composer/gp_composer.py` & `fedot-0.7.1/fedot/core/composer/gp_composer/gp_composer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/composer/gp_composer/specific_operators.py` & `fedot-0.7.1/fedot/core/composer/gp_composer/specific_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from random import choice, random
 from typing import List
 
-from golem.core.optimisers.genetic.operators.mutation import Mutation
+from golem.core.optimisers.genetic.operators.base_mutations import get_mutation_prob
 
 from fedot.core.pipelines.node import PipelineNode
 from fedot.core.pipelines.pipeline import Pipeline
 from fedot.core.pipelines.tuning.hyperparams import ParametersChanger
 from fedot.core.repository.operation_types_repository import OperationTypesRepository
 from fedot.core.repository.tasks import TaskTypesEnum
 
 
-def parameter_change_mutation(pipeline: Pipeline, requirements, params, opt_params, **kwargs) -> Pipeline:
+def parameter_change_mutation(pipeline: Pipeline, requirements, graph_gen_params, parameters, **kwargs) -> Pipeline:
     """
     This type of mutation is passed over all nodes and changes
     hyperparameters of the operations with probability - 'node mutation probability'
     which is initialised inside the function
     """
-    node_mutation_probability = Mutation.get_mutation_prob(mut_id=opt_params.mutation_strength,
-                                                           node=pipeline.root_node)
+    node_mutation_probability = get_mutation_prob(mut_id=parameters.mutation_strength,
+                                                  node=pipeline.root_node)
     for node in pipeline.nodes:
         if random() < node_mutation_probability:
             operation_name = node.operation.operation_type
             current_params = node.parameters
 
             # Perform specific change for particular parameter
             changer = ParametersChanger(operation_name, current_params)
@@ -30,19 +30,19 @@
                 if new_params is not None:
                     node.parameters = new_params
             except Exception as ex:
                 pipeline.log.error(ex)
     return pipeline
 
 
-def boosting_mutation(pipeline: Pipeline, requirements, params, **kwargs) -> Pipeline:
+def boosting_mutation(pipeline: Pipeline, requirements, graph_gen_params, **kwargs) -> Pipeline:
     """ This type of mutation adds the additional 'boosting' cascade to the existing pipeline """
 
     # TODO: refactor next line to get task_type more obviously
-    task_type = params.advisor.task.task_type
+    task_type = graph_gen_params.advisor.task.task_type
     decompose_operations = OperationTypesRepository('data_operation').suitable_operation(
         task_type=task_type, tags=['decompose'])
     decompose_operation = decompose_operations[0]
 
     existing_pipeline = pipeline
 
     all_data_operations = OperationTypesRepository('data_operation').suitable_operation(
```

### Comparing `fedot-0.7.0/fedot/core/composer/metrics.py` & `fedot-0.7.1/fedot/core/composer/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from abc import abstractmethod
 
 import numpy as np
-from sklearn.metrics import (accuracy_score, f1_score, log_loss, mean_absolute_error, mean_absolute_percentage_error,
-                             mean_squared_error, mean_squared_log_error, precision_score, r2_score, roc_auc_score,
-                             silhouette_score, roc_curve, auc)
+from sklearn.metrics import (accuracy_score, auc, f1_score, log_loss, mean_absolute_error,
+                             mean_absolute_percentage_error, mean_squared_error, mean_squared_log_error,
+                             precision_score, r2_score, roc_auc_score, roc_curve, silhouette_score)
 
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.pipelines.pipeline import Pipeline
 from fedot.core.pipelines.ts_wrappers import in_sample_ts_forecast
 from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.core.repository.tasks import TaskTypesEnum
 
@@ -184,23 +184,25 @@
     def metric(reference: InputData, predicted: OutputData) -> float:
         return smape(y_true=reference.target, y_pred=predicted.predict)
 
 
 class F1(QualityMetric):
     default_value = 0
     output_mode = 'labels'
+    binary_averaging_mode = 'binary'
+    multiclass_averaging_mode = 'weighted'
 
     @staticmethod
     @from_maximised_metric
     def metric(reference: InputData, predicted: OutputData) -> float:
         n_classes = reference.num_classes
         if n_classes > 2:
-            additional_params = {'average': 'weighted'}
+            additional_params = {'average': F1.multiclass_averaging_mode}
         else:
-            additional_params = {'average': 'micro'}
+            additional_params = {'average': F1.binary_averaging_mode}
         return f1_score(y_true=reference.target, y_pred=predicted.predict,
                         **additional_params)
 
 
 class MAE(QualityMetric):
     default_value = sys.maxsize
```

### Comparing `fedot-0.7.0/fedot/core/composer/random_composer.py` & `fedot-0.7.1/fedot/core/composer/random_composer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/constants.py` & `fedot-0.7.1/fedot/core/constants.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/data/array_utilities.py` & `fedot-0.7.1/fedot/core/data/array_utilities.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/data/data.py` & `fedot-0.7.1/fedot/core/data/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,51 +4,50 @@
 import os
 from copy import copy, deepcopy
 from dataclasses import dataclass, field
 from typing import List, Optional, Tuple, Union, Iterable, Any
 
 import numpy as np
 import pandas as pd
-
 from golem.core.log import default_log
 from golem.utilities.requirements_notificator import warn_requirement
 
-#: The list of keyword for auto-detecting csv *tabular* data index. Used in :py:meth:`Data.from_csv`
-#: and :py:meth:`MultiModalData.from_csv`.
-POSSIBLE_TABULAR_IDX_KEYWORDS = ['idx', 'index', 'id', 'unnamed: 0']
-#: The list of keyword for auto-detecting csv *time-series* data index. Used in :py:meth:`Data.from_csv_time_series`,
-#: :py:meth:`Data.from_csv_multi_time_series` and :py:meth:`MultiModalData.from_csv_time_series`.
-POSSIBLE_TS_IDX_KEYWORDS = ['datetime', 'date', 'time', 'unnamed: 0']
-
 try:
     import cv2
 except ModuleNotFoundError:
     warn_requirement('opencv-python')
     cv2 = None
 
 from fedot.core.data.array_utilities import atleast_2d
 from fedot.core.data.load_data import JSONBatchLoader, TextBatchLoader
 from fedot.core.data.supplementary_data import SupplementaryData
 from fedot.core.repository.dataset_types import DataTypesEnum
 from fedot.core.repository.tasks import Task, TaskTypesEnum
 
+#: The list of keyword for auto-detecting csv *tabular* data index. Used in :py:meth:`Data.from_csv`
+#: and :py:meth:`MultiModalData.from_csv`.
+POSSIBLE_TABULAR_IDX_KEYWORDS = ['idx', 'index', 'id', 'unnamed: 0']
+#: The list of keyword for auto-detecting csv *time-series* data index. Used in :py:meth:`Data.from_csv_time_series`,
+#: :py:meth:`Data.from_csv_multi_time_series` and :py:meth:`MultiModalData.from_csv_time_series`.
+POSSIBLE_TS_IDX_KEYWORDS = ['datetime', 'date', 'time', 'unnamed: 0']
+
 PathType = Union[os.PathLike, str]
 
 
 @dataclass
 class Data:
     """
     Base Data type class
     """
 
-    idx: np.array
+    idx: np.ndarray
     task: Task
     data_type: DataTypesEnum
-    features: np.array
-    target: Optional[np.array] = None
+    features: np.ndarray
+    target: Optional[np.ndarray] = None
 
     # Object with supplementary info
     supplementary_data: SupplementaryData = field(default_factory=SupplementaryData)
 
     @classmethod
     def from_csv(cls,
                  file_path: PathType,
@@ -329,27 +328,27 @@
             raise ValueError("""Path to the directory expected but got file""")
 
         df_data = JSONBatchLoader(path=files_path, label=label, fields_to_use=fields_to_use,
                                   shuffle=shuffle).extract(export_to_meta)
 
         if len(fields_to_use) > 1:
             fields_to_combine = []
-            for field in fields_to_use:
-                fields_to_combine.append(np.array(df_data[field]))
+            for field_to_use in fields_to_use:
+                fields_to_combine.append(np.array(df_data[field_to_use]))
                 # Unite if the element of text data is divided into strings
-                if isinstance(df_data[field][0], list):
-                    df_data[field] = [' '.join(piece) for piece in df_data[field]]
+                if isinstance(df_data[field_to_use][0], list):
+                    df_data[field_to_use] = [' '.join(piece) for piece in df_data[field_to_use]]
 
             features = np.column_stack(tuple(fields_to_combine))
         else:
-            field = df_data[fields_to_use[0]]
-            # process field with nested list
-            if isinstance(field[0], list):
-                field = [' '.join(piece) for piece in field]
-            features = np.array(field)
+            field_to_use = df_data[fields_to_use[0]]
+            # process field_to_use with nested list
+            if isinstance(field_to_use[0], list):
+                field_to_use = [' '.join(piece) for piece in field_to_use]
+            features = np.array(field_to_use)
 
         if is_multilabel:
             target = df_data[label]
             classes = set()
             for el in target:
                 for label in el:
                     classes.add(label)
@@ -579,14 +578,33 @@
         df = pd.read_csv(file_path,
                          parse_dates=[idx_column])
         idx = [str(d) for d in df[idx_column]]
         return idx
     return np.arange(0, len(data_frame))
 
 
+def np_datetime_to_numeric(data: np.ndarray) -> np.ndarray:
+    """
+    Change data's datetime type to integer with milliseconds unit.
+
+    Args:
+        data: table data for converting.
+
+    Returns:
+        The same table data with datetimes (if existed) converted to integer
+    """
+    orig_shape = data.shape
+    out_dtype = np.int64 if 'datetime' in str((dt := data.dtype)) else dt
+    features_df = pd.DataFrame(data, copy=False).infer_objects()
+    date_cols = features_df.select_dtypes('datetime')
+    converted_cols = date_cols.to_numpy(np.int64) // 1e6  # to 'ms' unit from 'ns'
+    features_df[date_cols.columns] = converted_cols
+    return features_df.to_numpy(out_dtype).reshape(orig_shape)
+
+
 def array_to_input_data(features_array: np.array,
                         target_array: np.array,
                         idx: Optional[np.array] = None,
                         task: Task = Task(TaskTypesEnum.classification),
                         data_type: Optional[DataTypesEnum] = None) -> InputData:
     if idx is None:
         idx = np.arange(len(features_array))
@@ -602,15 +620,14 @@
         return DataTypesEnum.table
 
 
 def get_df_from_csv(file_path: PathType, delimiter: str, index_col: Optional[Union[str, int]] = None,
                     possible_idx_keywords: Optional[List[str]] = None, *,
                     columns_to_drop: Optional[List[Union[str, int]]] = None,
                     columns_to_use: Optional[List[Union[str, int]]] = None):
-
     def define_index_column(candidate_columns: List[str]) -> Optional[str]:
         for column_name in candidate_columns:
             if is_column_name_suitable_for_index(column_name):
                 return column_name
 
     def is_column_name_suitable_for_index(column_name: str) -> bool:
         return any(key in column_name.lower() for key in possible_idx_keywords)
```

### Comparing `fedot-0.7.0/fedot/core/data/data_detection.py` & `fedot-0.7.1/fedot/core/data/data_detection.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/data/data_preprocessing.py` & `fedot-0.7.1/fedot/core/data/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/data/data_split.py` & `fedot-0.7.1/fedot/core/data/data_split.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/data/load_data.py` & `fedot-0.7.1/fedot/core/data/load_data.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/data/merge/data_merger.py` & `fedot-0.7.1/fedot/core/data/merge/data_merger.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,13 +163,19 @@
         # Ensure that 1d-column timeseries remains 1d timeseries
         return flatten_extra_dim(merged_predicts)
 
 
 class TextDataMerger(DataMerger):
 
     def merge_predicts(self, predicts: List[np.array]) -> np.array:
+        if any(len(pred.shape) > 2 for pred in predicts):
+            raise ValueError('Merge of arrays with more than 2 dimensions is not supported')
         if len(predicts) > 1:
-            raise ValueError("Text tables and merge of text data is not supported")
+            predicts = [predict.astype(str) for predict in predicts]
+            result = predicts[0]
+            for i in range(1, len(predicts)):
+                result = np.core.defchararray.add(result, predicts[i])
+            return result
         return predicts[0]
 
     def postprocess_predicts(self, merged_predicts: np.array) -> np.array:
         return merged_predicts
```

### Comparing `fedot-0.7.0/fedot/core/data/merge/supplementary_data_merger.py` & `fedot-0.7.1/fedot/core/data/merge/supplementary_data_merger.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/data/multi_modal.py` & `fedot-0.7.1/fedot/core/data/multi_modal.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/data/supplementary_data.py` & `fedot-0.7.1/fedot/core/data/supplementary_data.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/data/visualisation.py` & `fedot-0.7.1/fedot/core/data/visualisation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/atomized_model.py` & `fedot-0.7.1/fedot/core/operations/atomized_model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/atomized_template.py` & `fedot-0.7.1/fedot/core/operations/atomized_template.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/data_operation.py` & `fedot-0.7.1/fedot/core/operations/data_operation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from fedot.core.data.data import OutputData
 from fedot.core.operations.operation import Operation
 from fedot.core.repository.operation_types_repository import OperationMetaInfo, OperationTypesRepository
 
 
 class DataOperation(Operation):
     """Class with ``fit``/``predict`` methods defining the evaluation strategy for the task
```

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/automl.py` & `fedot-0.7.1/fedot/core/operations/evaluation/automl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from typing import Optional
 
 import numpy as np
 
 from h2o import h2o, H2OFrame
 from h2o.automl import H2OAutoML
 from tpot import TPOTClassifier, TPOTRegressor
```

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/classification.py` & `fedot-0.7.1/fedot/core/operations/evaluation/classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/clustering.py` & `fedot-0.7.1/fedot/core/operations/evaluation/clustering.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/common_preprocessing.py` & `fedot-0.7.1/fedot/core/operations/evaluation/common_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/custom.py` & `fedot-0.7.1/fedot/core/operations/evaluation/custom.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,19 @@
 
 warnings.filterwarnings("ignore", category=UserWarning)
 
 
 class CustomModelStrategy(EvaluationStrategy):
     """
     This class defines the default model container for custom of domain-specific implementations
-    :param str operation_type: rudimentary of parent - type of the operation defined in operation or
-           data operation repositories
-    :param dict params: hyperparameters to fit the model with
+
+    Args:
+        operation_type: rudimentary of parent - type of the operation defined in operation or
+            data operation repositories
+        params: hyperparameters to fit the model with
     """
 
     def __init__(self, operation_type: Optional[str], params: Optional[OperationParameters] = None):
         super().__init__(operation_type, params)
         self.operation_impl = CustomModelImplementation(params)
 
     def fit(self, train_data: InputData):
```

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/data_source.py` & `fedot-0.7.1/fedot/core/operations/evaluation/data_source.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/evaluation_interfaces.py` & `fedot-0.7.1/fedot/core/operations/evaluation/evaluation_interfaces.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/gpu/classification.py` & `fedot-0.7.1/fedot/core/operations/evaluation/gpu/classification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/gpu/clustering.py` & `fedot-0.7.1/fedot/core/operations/evaluation/gpu/clustering.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/gpu/common.py` & `fedot-0.7.1/fedot/core/operations/evaluation/gpu/common.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/gpu/regression.py` & `fedot-0.7.1/fedot/core/operations/evaluation/gpu/regression.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/categorical_encoders.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/decompose.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_filters.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_imbalanced_class.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_selectors.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/sklearn_transformations.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/text_pretrained.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/data_operations/ts_transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from copy import copy
+from copy import copy, deepcopy
 from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 from golem.core.log import default_log
 from scipy.ndimage import gaussian_filter
 from sklearn.decomposition import TruncatedSVD
@@ -674,16 +674,17 @@
 
         Args:
             input_data: data with features, target and ids to process
 
         Returns:
             output data with cutted time series
         """
-
+        old_target = deepcopy(input_data.target)
         input_data = self._cut_input_data(input_data)
+        input_data.target = old_target
 
         output_data = self._convert_to_output(input_data,
                                               input_data.features,
                                               data_type=input_data.data_type)
         return output_data
 
     def transform_for_fit(self, input_data: InputData) -> OutputData:
```

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/implementation_interfaces.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/discriminant_analysis.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/keras.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/keras.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/knn.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/knn.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/svc.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/svc.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/arima.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/statsmodels.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,260 +1,314 @@
 from copy import copy
-from typing import Optional
 
 import numpy as np
-from scipy import stats
-from scipy.special import boxcox, inv_boxcox
-from statsmodels.tsa.api import STLForecast
-from statsmodels.tsa.arima.model import ARIMA
+import statsmodels.api as sm
+from statsmodels.genmod.families import Gamma, Gaussian, InverseGaussian
+from statsmodels.genmod.families.links import identity, inverse_power, inverse_squared, log as lg
+from statsmodels.genmod.generalized_linear_model import GLM
+from statsmodels.tsa.ar_model import AutoReg
+from statsmodels.tsa.exponential_smoothing.ets import ETSModel
 
 from fedot.core.data.data import InputData, OutputData
 from fedot.core.operations.evaluation.operation_implementations.data_operations.ts_transformations import ts_to_table
 from fedot.core.operations.evaluation.operation_implementations.implementation_interfaces import ModelImplementation
 from fedot.core.operations.operation_parameters import OperationParameters
 from fedot.core.repository.dataset_types import DataTypesEnum
-from fedot.utilities.ts_gapfilling import SimpleGapFiller
 
 
-class ARIMAImplementation(ModelImplementation):
+class GLMImplementation(ModelImplementation):
+    """ Generalized linear models implementation """
+    # some models are dropped due to instability
+    family_distribution = {
+        "gaussian": {'distribution': Gaussian,
+                     'default_link': 'identity',
+                     'available_links': {'log': lg(),
+                                         'identity': identity(),
+                                         'inverse_power': inverse_power()
+                                         }
+                     },
+        "gamma": {'distribution': Gamma,
+                  'default_link': 'inverse_power',
+                  'available_links': {'log': lg(),
+                                      'identity': identity(),
+                                      'inverse_power': inverse_power()
+                                      }
+                  },
+        "inverse_gaussian": {'distribution': InverseGaussian,
+                             'default_link': 'inverse_squared',
+                             'available_links': {'log': lg(),
+                                                 'identity': identity(),
+                                                 'inverse_squared': inverse_squared(),
+                                                 'inverse_power': inverse_power()
+                                                 }
+                             },
+        "default": Gaussian(identity())
+    }
 
-    def __init__(self, params: Optional[OperationParameters] = None):
+    def __init__(self, params: OperationParameters):
         super().__init__(params)
-        self.arima = None
-        self.lambda_value = None
-        self.scope = None
-        self.actual_ts_len = None
-
-    def fit(self, input_data):
-        """ Class fit arima model on data
-
-        :param input_data: data with features, target and ids to process
-        """
-        source_ts = np.array(input_data.features)
-        # Save actual time series length
-        self.actual_ts_len = len(source_ts)
-
-        # Apply box-cox transformation for positive values
-        transformed_ts = self._apply_boxcox(source_ts)
+        self.model = None
+        self.family_link = None
 
-        # Set parameters
-        p = int(self.params.get('p'))
-        d = int(self.params.get('d'))
-        q = int(self.params.get('q'))
-        params = {'order': (p, d, q)}
+        self.correct_params()
 
-        self.arima = ARIMA(transformed_ts, **params).fit()
+    @property
+    def family(self) -> str:
+        return self.params.get('family')
 
-        return self.arima
+    @property
+    def link(self) -> str:
+        return self.params.get('link')
 
-    def predict(self, input_data: InputData):
-        """ Method for time series prediction on forecast length
-
-        :param input_data: data with features, target and ids to process
+    def fit(self, input_data):
+        self.model = GLM(
+            exog=sm.add_constant(input_data.idx.astype("float64")).reshape(-1, 2),
+            endog=input_data.target.astype("float64").reshape(-1, 1),
+            family=self.family_link
+        ).fit(method="lbfgs")
+        return self.model
 
-        :return output_data: output data with smoothed time series
-        """
+    def predict(self, input_data):
         input_data = copy(input_data)
-        forecast_length = input_data.task.task_params.forecast_length
-        self.handle_new_data(input_data)
+        parameters = input_data.task.task_params
+        forecast_length = parameters.forecast_length
+        old_idx = input_data.idx
+        if forecast_length == 1:
+            predictions = self.model.predict(np.concatenate([np.array([1]),
+                                                             input_data.idx.astype("float64")]).reshape(-1, 2))
+        else:
+            predictions = self.model.predict(sm.add_constant(input_data.idx.astype("float64")).reshape(-1, 2))
 
-        start_id = self.actual_ts_len
-        end_id = start_id + forecast_length - 1
+        start_id = old_idx[-1] - forecast_length + 1
+        end_id = old_idx[-1]
+        predict = predictions
+        predict = np.array(predict).reshape(1, -1)
+        new_idx = np.arange(start_id, end_id + 1)
 
-        predicted = self.arima.predict(start=start_id,
-                                       end=end_id)
-        predicted = self._inverse_boxcox(predicted=predicted,
-                                         lambda_param=self.lambda_value)
-        predict = self._inverse_shift(predicted)
+        input_data.idx = new_idx
 
-        predict = np.array(predict).reshape(1, -1)
         output_data = self._convert_to_output(input_data,
                                               predict=predict,
                                               data_type=DataTypesEnum.table)
-
         return output_data
 
-    def predict_for_fit(self, input_data: InputData):
+    def predict_for_fit(self, input_data: InputData) -> OutputData:
         input_data = copy(input_data)
-        forecast_length = input_data.task.task_params.forecast_length
-        fitted_values = self.arima.fittedvalues
-
-        fitted_values = self._inverse_boxcox(predicted=fitted_values,
-                                             lambda_param=self.lambda_value)
-        fitted_values = self._inverse_shift(fitted_values)
-
-        diff = int(self.actual_ts_len - len(fitted_values))
-        # If first elements skipped
-        if diff != 0:
-            # Fill nans with first values
-            first_element = fitted_values[0]
-            first_elements = [first_element] * diff
-            first_elements.extend(list(fitted_values))
-
-            fitted_values = np.array(first_elements)
-
-        _, predict = ts_to_table(idx=input_data.idx,
-                                 time_series=fitted_values,
+        parameters = input_data.task.task_params
+        forecast_length = parameters.forecast_length
+        old_idx = input_data.idx
+        target = input_data.target
+        predictions = self.model.predict(sm.add_constant(input_data.idx.astype("float64")).reshape(-1, 2))
+        _, predict = ts_to_table(idx=old_idx,
+                                 time_series=predictions,
                                  window_size=forecast_length)
-
-        new_idx, target_columns = ts_to_table(idx=input_data.idx,
-                                              time_series=input_data.target,
+        new_idx, target_columns = ts_to_table(idx=old_idx,
+                                              time_series=target,
                                               window_size=forecast_length)
+
         input_data.idx = new_idx
         input_data.target = target_columns
 
         output_data = self._convert_to_output(input_data,
                                               predict=predict,
                                               data_type=DataTypesEnum.table)
-
         return output_data
 
-    def handle_new_data(self, input_data: InputData):
-        """
-        Method to update x samples inside a model (used when we want to use old model to a new data)
-
-        :param input_data: new input_data
-        """
-        if input_data.idx[0] > self.actual_ts_len:
-            self.arima = self.fit(input_data)
-            self.log.info("Arima refitted for handling a new data")
-
-    def _apply_boxcox(self, source_ts):
-        min_value = np.min(source_ts)
-        if min_value > 0:
-            pass
-        else:
-            # Making a shift to positive values
-            self.scope = abs(min_value) + 1
-            source_ts = source_ts + self.scope
-
-        _, self.lambda_value = stats.boxcox(source_ts)
-        transformed_ts = boxcox(source_ts, self.lambda_value)
-
-        return transformed_ts
-
-    def _inverse_boxcox(self, predicted, lambda_param):
-        """ Method apply inverse Box-Cox transformation """
-        if lambda_param == 0:
-            return np.exp(predicted)
+    def set_default(self):
+        """ Set default value of Family(link) """
+        self.family_link = self.family_distribution['default']
+        self.params.update(family='gaussian')
+        self.log.info("Invalid family. Changed to default value")
+
+    def correct_params(self):
+        """ Correct params if they are not correct """
+        if self.family in self.family_distribution:
+            if self.link not in self.family_distribution[self.family]['available_links']:
+                # get default link for distribution if current invalid
+                default_link = self.family_distribution[self.family]['default_link']
+                self.log.info(
+                    f"Invalid link function {self.link} for {self.family}. Change to default "
+                    f"link {default_link}")
+                self.params.update(link=default_link)
+            # if correct isn't need
+            self.family_link = self.family_distribution[self.family]['distribution'](
+                self.family_distribution[self.family]['available_links'][self.link]
+            )
         else:
-            res = inv_boxcox(predicted, lambda_param)
-            res = self._filling_gaps(res)
-            return res
-
-    def _inverse_shift(self, values):
-        """ Method apply inverse shift operation """
-        if self.scope is None:
-            pass
-        else:
-            values = values - self.scope
-
-        return values
-
-    @staticmethod
-    def _filling_gaps(res):
-        nan_ind = np.argwhere(np.isnan(res))
-        res[nan_ind] = -100.0
+            # get default family for distribution if current invalid
+            self.set_default()
 
-        # Gaps in first and last elements fills with mean value
-        if 0 in nan_ind:
-            res[0] = np.mean(res)
-        if int(len(res) - 1) in nan_ind:
-            res[int(len(res) - 1)] = np.mean(res)
 
-        # Gaps in center of timeseries fills with linear interpolation
-        if len(np.ravel(np.argwhere(np.isnan(res)))) != 0:
-            gf = SimpleGapFiller()
-            res = gf.linear_interpolation(res)
+class AutoRegImplementation(ModelImplementation):
 
-        return res
-
-
-class STLForecastARIMAImplementation(ModelImplementation):
-    def __init__(self, params: Optional[OperationParameters] = None):
+    def __init__(self, params: OperationParameters):
         super().__init__(params)
-        self.model = None
-        self.lambda_param = None
-        self.scope = None
+        self.autoreg = None
         self.actual_ts_len = None
 
     def fit(self, input_data):
-        """ Class fit STLForecast arima model on data
+        """ Class fit ar model on data
 
         :param input_data: data with features, target and ids to process
         """
 
         source_ts = np.array(input_data.features)
-        # Save actual time series length
         self.actual_ts_len = len(source_ts)
 
-        p = int(self.params.setdefault('p', 2))
-        d = int(self.params.setdefault('d', 0))
-        q = int(self.params.setdefault('q', 2))
-        period = int(self.params.setdefault('period', 365))
-        params = {'period': period, 'model_kwargs': {'order': (p, d, q)}}
-        self.model = STLForecast(source_ts, ARIMA, **params).fit()
+        # Correct window size parameter
+        self._check_and_correct_lags(source_ts)
 
-        return self.model
+        lag_1 = int(self.params.get('lag_1'))
+        lag_2 = int(self.params.get('lag_2'))
+        self.autoreg = AutoReg(source_ts, lags=[lag_1, lag_2]).fit()
+        self.actual_ts_len = input_data.idx.shape[0]
+
+        return self.autoreg
 
-    def predict(self, input_data: InputData) -> OutputData:
+    def predict(self, input_data):
         """ Method for time series prediction on forecast length
 
         :param input_data: data with features, target and ids to process
-
         :return output_data: output data with smoothed time series
         """
+        input_data = copy(input_data)
         parameters = input_data.task.task_params
         forecast_length = parameters.forecast_length
 
         # in case in(out) sample forecasting
         self.handle_new_data(input_data)
         start_id = self.actual_ts_len
         end_id = start_id + forecast_length - 1
-        predicted = self.model.get_prediction(start=start_id, end=end_id).predicted_mean
-
+        predicted = self.autoreg.predict(start=start_id, end=end_id)
         predict = np.array(predicted).reshape(1, -1)
+
+        output_data = self._convert_to_output(input_data,
+                                              predict=predict,
+                                              data_type=DataTypesEnum.table)
+        return output_data
+
+    def predict_for_fit(self, input_data: InputData) -> OutputData:
+        input_data = copy(input_data)
+        parameters = input_data.task.task_params
+        forecast_length = parameters.forecast_length
+        idx = input_data.idx
+        target = input_data.target
+        predicted = self.autoreg.predict(start=idx[0], end=idx[-1])
+        # adding nan to target as in predicted
+        nan_mask = np.isnan(predicted)
+        target = target.astype(float)
+        target = target[~nan_mask]
+        idx = idx[~nan_mask]
+        predicted = predicted[~nan_mask]
+        new_idx, predict = ts_to_table(idx=idx,
+                                       time_series=predicted,
+                                       window_size=forecast_length)
+        _, target_columns = ts_to_table(idx=idx,
+                                        time_series=target,
+                                        window_size=forecast_length)
+        input_data.idx = new_idx
+        input_data.target = target_columns
+        output_data = self._convert_to_output(input_data,
+                                              predict=predict,
+                                              data_type=DataTypesEnum.table)
+        return output_data
+
+    def _check_and_correct_lags(self, time_series: np.array):
+        previous_lag_1 = int(self.params.get('lag_1'))
+        previous_lag_2 = int(self.params.get('lag_2'))
+        max_lag = len(time_series) // 2 - 1
+        new_lag_1 = self._check_and_correct_lag(max_lag, previous_lag_1)
+        new_lag_2 = self._check_and_correct_lag(max_lag, previous_lag_2)
+        if new_lag_1 == new_lag_2:
+            new_lag_2 -= 1
+        prefix = "Warning: lag of AutoRegImplementation was changed"
+        if previous_lag_1 != new_lag_1:
+            self.log.info(f"{prefix} from {previous_lag_1} to {new_lag_1}.")
+            self.params.update(lag_1=new_lag_1)
+        if previous_lag_2 != new_lag_2:
+            self.log.info(f"{prefix} from {previous_lag_2} to {new_lag_2}.")
+            self.params.update(lag_2=new_lag_2)
+
+    def _check_and_correct_lag(self, max_lag: int, lag: int):
+        if lag > max_lag:
+            lag = max_lag
+        return lag
+
+    def handle_new_data(self, input_data: InputData):
+        """
+        Method to update x samples inside a model (used when we want to use old model to a new data)
+
+        :param input_data: new input_data
+        """
+        if input_data.idx[0] > self.actual_ts_len:
+            self.autoreg.model.endog = input_data.features[-self.actual_ts_len:]
+            self.autoreg.model._setup_regressors()
+
+
+class ExpSmoothingImplementation(ModelImplementation):
+    """ Exponential smoothing implementation from statsmodels """
+
+    def __init__(self, params: OperationParameters):
+        super().__init__(params)
+        self.model = None
+        if self.params.get("seasonal"):
+            self.seasonal_periods = int(self.params.get("seasonal_periods"))
+        else:
+            self.seasonal_periods = None
+
+    def fit(self, input_data):
+        self.model = ETSModel(
+            input_data.features.astype("float64"),
+            error=self.params.get("error"),
+            trend=self.params.get("trend"),
+            seasonal=self.params.get("seasonal"),
+            damped_trend= self.params.get("damped_trend") if self.params.get("trend") else None,
+            seasonal_periods=self.seasonal_periods
+        )
+        self.model = self.model.fit(disp=False)
+        return self.model
+
+    def predict(self, input_data):
+        input_data = copy(input_data)
+        idx = input_data.idx
+
+        start_id = idx[0]
+        end_id = idx[-1]
+        predictions = self.model.predict(start=start_id,
+                                         end=end_id)
+        predict = predictions
+        predict = np.array(predict).reshape(1, -1)
         new_idx = np.arange(start_id, end_id + 1)
 
         input_data.idx = new_idx
 
         output_data = self._convert_to_output(input_data,
                                               predict=predict,
                                               data_type=DataTypesEnum.table)
         return output_data
 
     def predict_for_fit(self, input_data: InputData) -> OutputData:
+        input_data = copy(input_data)
         parameters = input_data.task.task_params
         forecast_length = parameters.forecast_length
         idx = input_data.idx
         target = input_data.target
-        fitted_values = self.model.get_prediction(start=idx[0], end=idx[-1]).predicted_mean
-        diff = int(self.actual_ts_len) - len(fitted_values)
-        # If first elements skipped
-        if diff != 0:
-            # Fill nans with first values
-            first_element = fitted_values[0]
-            first_elements = [first_element] * diff
-            first_elements.extend(list(fitted_values))
-
-            fitted_values = np.array(first_elements)
 
+        # Indexing for statsmodels is different
+        start_id = idx[0]
+        end_id = idx[-1]
+        predictions = self.model.predict(start=start_id,
+                                         end=end_id)
         _, predict = ts_to_table(idx=idx,
-                                 time_series=fitted_values,
+                                 time_series=predictions,
                                  window_size=forecast_length)
-
         new_idx, target_columns = ts_to_table(idx=idx,
                                               time_series=target,
                                               window_size=forecast_length)
 
         input_data.idx = new_idx
         input_data.target = target_columns
+
         output_data = self._convert_to_output(input_data,
                                               predict=predict,
                                               data_type=DataTypesEnum.table)
         return output_data
-
-    def handle_new_data(self, input_data: InputData):
-        """ Refit model if use new test data"""
-        if input_data.idx[0] > self.actual_ts_len:
-            self.model = self.fit(input_data)
-            self.log.info("STL Arima refitted for handling a new data")
```

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/cgru.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/naive.py`

 * *Files 18% similar despite different names*

```diff
@@ -96,42 +96,41 @@
         return self.params.get('part_for_averaging')
 
     def fit(self, input_data):
         """ Such a simple approach does not support fit method """
         pass
 
     def predict(self, input_data: InputData) -> OutputData:
+        input_data = copy(input_data)
         """ Get desired part of time series for averaging and calculate mean value """
         forecast_length = input_data.task.task_params.forecast_length
 
         elements_to_take = self._how_many_elements_use_for_averaging(input_data.features)
         # Prepare single forecast
         mean_value = np.nanmean(input_data.features[-elements_to_take:])
         forecast = np.array([mean_value] * forecast_length).reshape((1, -1))
 
         output_data = self._convert_to_output(input_data,
                                               predict=forecast,
                                               data_type=DataTypesEnum.table)
         return output_data
 
     def predict_for_fit(self, input_data: InputData) -> OutputData:
+        input_data = copy(input_data)
         forecast_length = input_data.task.task_params.forecast_length
         parts = split_rolling_slices(input_data)
         mean_values_for_chunks = self.average_by_axis(parts)
         forecast = np.repeat(mean_values_for_chunks.reshape((-1, 1)), forecast_length, axis=1)
-        forecast = forecast[:-forecast_length, :]
 
         # Update target
-        _, transformed_target = ts_to_table(idx=input_data.idx, time_series=input_data.target,
-                                            window_size=forecast_length, is_lag=True)
-        input_data.target = transformed_target[1:, :]
-
-        # Update indices - there is no forecast for first element and skip last out of boundaries predictions
-        last_threshold = forecast_length - 1
-        new_idx = input_data.idx[1: -last_threshold]
+        new_idx, transformed_target = ts_to_table(idx=input_data.idx, time_series=input_data.target,
+                                                  window_size=forecast_length)
+
+        input_data.target = transformed_target
+        forecast = forecast[new_idx]
         input_data.idx = new_idx
         output_data = self._convert_to_output(input_data,
                                               predict=forecast,
                                               data_type=DataTypesEnum.table)
         return output_data
 
     def average_by_axis(self, parts: np.array):
```

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py` & `fedot-0.7.1/fedot/core/operations/evaluation/operation_implementations/models/ts_implementations/poly.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/regression.py` & `fedot-0.7.1/fedot/core/operations/evaluation/regression.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/text.py` & `fedot-0.7.1/fedot/core/operations/evaluation/text.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/evaluation/time_series.py` & `fedot-0.7.1/fedot/core/operations/evaluation/time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 
 
 class FedotTsForecastingStrategy(EvaluationStrategy):
     """
     This class defines the certain classical models implementation for time
     series forecasting (e.g. AR, ARIMA)
 
-    :param str operation_type: str type of the operation defined in operation or
-    data operation repositories
-    :param dict params: hyperparameters to fit the model with
+    Args:
+        operation_type: str type of the operation defined in operation or
+            data operation repositories
+        params: hyperparameters to fit the model with
     """
 
     __operations_by_types = {
         'arima': ARIMAImplementation,
         'ar': AutoRegImplementation,
         'stl_arima': STLForecastARIMAImplementation,
         'ets': ExpSmoothingImplementation,
@@ -95,17 +96,18 @@
 
 
 class FedotTsTransformingStrategy(EvaluationStrategy):
     """
     This class defines the certain data operation implementation for time series
     forecasting
 
-    :param str operation_type: str type of the operation defined in operation or
-    data operation repositories
-    :param dict params: hyperparameters to fit the model with
+    Args:
+        operation_type: str type of the operation defined in operation or
+            data operation repositories
+        params: hyperparameters to fit the model with
     """
 
     __operations_by_types = {
         'lagged': LaggedTransformationImplementation,
         'sparse_lagged': SparseLaggedTransformationImplementation,
         'smoothing': TsSmoothingImplementation,
         'exog_ts': ExogDataTransformationImplementation,
```

### Comparing `fedot-0.7.0/fedot/core/operations/factory.py` & `fedot-0.7.1/fedot/core/operations/factory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/hyperparameters_preprocessing.py` & `fedot-0.7.1/fedot/core/operations/hyperparameters_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/model.py` & `fedot-0.7.1/fedot/core/operations/model.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/operation.py` & `fedot-0.7.1/fedot/core/operations/operation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/operations/operation_parameters.py` & `fedot-0.7.1/fedot/core/operations/operation_parameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from copy import deepcopy
-from typing import Optional, Iterable
+from typing import Iterable
 
 from fedot.core.repository.default_params_repository import DefaultOperationParamsRepository
 
 
 class OperationParameters:
     """Stores parameters for models and data operations implementations and records what parameters were changed.
     Uses operation_type to set default parameters from default_parameters_repository if a parameter was not passed
```

### Comparing `fedot-0.7.0/fedot/core/operations/operation_template.py` & `fedot-0.7.1/fedot/core/operations/operation_template.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/optimisers/objective/data_objective_advisor.py` & `fedot-0.7.1/fedot/core/optimisers/objective/data_objective_advisor.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/optimisers/objective/data_objective_eval.py` & `fedot-0.7.1/fedot/core/optimisers/objective/data_objective_eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,31 +27,34 @@
     :param data_producer: Producer of data folds, each fold is a tuple of (train_data, test_data).
     If it returns a single fold, it's effectively a hold-out validation. For many folds it's k-folds.
     :param time_constraint: Optional time constraint for pipeline.fit.
     :param validation_blocks: Number of validation blocks, optional, used only for time series validation.
     :param pipelines_cache: Cache manager for fitted models, optional.
     :param preprocessing_cache: Cache manager for optional preprocessing encoders and imputers, optional.
     :param eval_n_jobs: number of jobs used to evaluate the objective.
+    :params do_unfit: unfit graph after evaluation
     """
 
     def __init__(self,
                  objective: Objective,
                  data_producer: DataSource,
                  time_constraint: Optional[timedelta] = None,
                  validation_blocks: Optional[int] = None,
                  pipelines_cache: Optional[OperationsCache] = None,
                  preprocessing_cache: Optional[PreprocessingCache] = None,
-                 eval_n_jobs: int = 1):
+                 eval_n_jobs: int = 1,
+                 do_unfit: bool = True):
         super().__init__(objective, eval_n_jobs=eval_n_jobs)
         self._data_producer = data_producer
         self._time_constraint = time_constraint
         self._validation_blocks = validation_blocks
         self._pipelines_cache = pipelines_cache
         self._preprocessing_cache = preprocessing_cache
         self._log = default_log(self)
+        self._do_unfit = do_unfit
 
     def evaluate(self, graph: Pipeline) -> Fitness:
         # Seems like a workaround for situation when logger is lost
         #  when adapting and restoring it to/from OptGraph.
         graph.log = self._log
 
         graph_id = graph.root_node.descriptive_id
@@ -75,15 +78,16 @@
                                                 reference_data=test_data,
                                                 validation_blocks=self._validation_blocks)
             if evaluated_fitness.valid:
                 folds_metrics.append(evaluated_fitness.values)
             else:
                 self._log.warning(f'Invalid fitness after objective evaluation. '
                                   f'Skipping the graph: {graph_id}', raise_if_test=True)
-            graph.unfit()
+            if self._do_unfit:
+                graph.unfit()
         if folds_metrics:
             folds_metrics = tuple(np.mean(folds_metrics, axis=0))  # averages for each metric over folds
             self._log.debug(f'Pipeline {graph_id} with evaluated metrics: {folds_metrics}')
         else:
             folds_metrics = None
 
         return to_fitness(folds_metrics, self._objective.is_multi_objective)
@@ -138,7 +142,11 @@
                 n_jobs=self._eval_n_jobs,
             )
             intermediate_fitness = self._objective(intermediate_graph,
                                                    reference_data=test_data,
                                                    validation_blocks=self._validation_blocks)
             # saving only the most important first metric
             node.metadata.metric = intermediate_fitness.values[0]
+
+    @property
+    def input_data(self):
+        return self._data_producer.args[0]
```

### Comparing `fedot-0.7.0/fedot/core/optimisers/objective/data_source_splitter.py` & `fedot-0.7.1/fedot/core/optimisers/objective/data_source_splitter.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/optimisers/objective/metrics_objective.py` & `fedot-0.7.1/fedot/core/optimisers/objective/metrics_objective.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/optimisers/objective/objective_serialization.py` & `fedot-0.7.1/fedot/core/optimisers/objective/objective_serialization.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/adapters.py` & `fedot-0.7.1/fedot/core/pipelines/adapters.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/automl_wrappers.py` & `fedot-0.7.1/fedot/core/pipelines/automl_wrappers.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/node.py` & `fedot-0.7.1/fedot/core/pipelines/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from dataclasses import dataclass
 from typing import Any, List, Optional, Tuple, Union
 
 import numpy as np
 from golem.core.dag.linked_graph_node import LinkedGraphNode
 from golem.core.log import default_log
 from golem.core.optimisers.timer import Timer
@@ -15,15 +17,15 @@
 from fedot.core.repository.operation_types_repository import OperationTypesRepository
 from fedot.core.utils import DEFAULT_PARAMS_STUB
 
 
 @register_serializable
 @dataclass
 class NodeMetadata:
-    """Dataclass. :class:`Node` metadata
+    """Dataclass. :class:`PipelineNode` metadata
 
     Args:
         metric: quality score
     """
 
     metric: Optional[float] = None
 
@@ -34,16 +36,16 @@
     Args:
         operation_type: operation defined in the operation repository
         nodes_from: parent nodes where data comes from
         node_data: ``dict`` with :class:`InputData` for fit and predict stage
         kwargs: optional arguments (i.e. logger)
     """
 
-    def __init__(self, operation_type: Optional[Union[str, 'Operation']] = None,
-                 nodes_from: Optional[List['Node']] = None,
+    def __init__(self, operation_type: Optional[Union[str, Operation]] = None,
+                 nodes_from: Optional[List[PipelineNode]] = None,
                  node_data: Optional[dict] = None,
                  **kwargs):
         if node_data is None:
             self._node_data = {}
             self.direct_set = False
         else:
             self._node_data = node_data
@@ -388,15 +390,14 @@
             prediction = parent.predict(input_data=input_data)
             parent_results.append(prediction)
         elif parent_operation == 'fit':
             prediction = parent.fit(input_data=input_data)
             parent_results.append(prediction)
         else:
             raise NotImplementedError()
-
         if input_data is None:
             # InputData was set to primary nodes
             target = prediction.target
 
     return parent_results, target
```

### Comparing `fedot-0.7.0/fedot/core/pipelines/pipeline.py` & `fedot-0.7.1/fedot/core/pipelines/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 ERROR_PREFIX = 'Invalid pipeline configuration:'
 
 
 class Pipeline(GraphDelegate, Serializable):
     """Base class used for composite model structure definition
 
     Args:
-        nodes: :obj:`Node` object(s)
-        use_input_preprocessing: whether to do input preprocessing or not, True by default
+        nodes: :obj:`PipelineNode` object(s)
+        use_input_preprocessing: whether to do input preprocessing or not, ``True`` by default.
     """
 
     def __init__(self, nodes: Union[PipelineNode, Sequence[PipelineNode]] = (), use_input_preprocessing: bool = True):
         super().__init__(nodes, _graph_nodes_to_pipeline_nodes)
 
         self.computation_time = None
         self.log = default_log(self)
@@ -58,15 +58,15 @@
 
         # Clean all saved states and fit all operations
         self.unfit()
         self.fit(input_data)
 
     def _fit_with_time_limit(self, input_data: Optional[InputData],
                              time: timedelta) -> OutputData:
-        """Runs training process in all of the pipeline nodes starting with root with time limit.
+        """Runs training process in all the pipeline nodes starting with root with time limit.
 
         Todo:
             unresolved sentence
 
         Args:
             input_data: data used for operations training
             time: time constraint for operations fitting process (in minutes)
@@ -116,16 +116,16 @@
             return train_predicted
         else:
             process_state_dict['train_predicted'] = train_predicted
             process_state_dict['computation_time_in_seconds'] = self.computation_time
             for node in self.nodes:
                 fitted_operations.append(node.fitted_operation)
 
-    def _preprocess(self, input_data: Union[InputData, MultiModalData], *, is_fit_stage: bool = True) -> Union[
-        InputData, MultiModalData]:
+    def _preprocess(self, input_data: Union[InputData, MultiModalData], *, is_fit_stage: bool = True) -> \
+            Union[InputData, MultiModalData]:
         """
         Makes obligatory and optional (if needed) steps of data preprocessing
 
         Args:
             input_data: to be copied and preprocessed
             is_fit_stage: True when it's fitting stage
 
@@ -236,14 +236,15 @@
             cache: pipeline nodes cacher
             fold_id: optional part of the cache item UID
                (can be used to specify the number of CV fold)
 
         Returns:
             bool: indicating if at least one node was loaded
         """
+
         if cache is not None:
             cache.try_load_into_pipeline(self, fold_id)
         if preprocessing_cache is not None:
             preprocessing_cache.try_load_preprocessor(self, fold_id)
 
     def predict(self, input_data: Union[InputData, MultiModalData], output_mode: str = 'default') -> OutputData:
         """Runs the predict process in all of the pipeline nodes starting with root
@@ -405,15 +406,15 @@
 
 def _graph_nodes_to_pipeline_nodes(operator: LinkedGraph, nodes: Sequence[PipelineNode]):
     """
     Method to update nodes type after performing some action on the pipeline
         via GraphOperator, if any of them are of GraphNode type
 
     Args:
-        nodes: :obj:`Node` object(s)
+        nodes: :obj:`PipelineNode` object(s)
     """
 
     for node in nodes:
         if not isinstance(node, GraphNode):
             continue
         if not node.nodes_from and not operator.node_children(node) and node != operator.root_node:
             operator.nodes.remove(node)
```

### Comparing `fedot-0.7.0/fedot/core/pipelines/pipeline_advisor.py` & `fedot-0.7.1/fedot/core/pipelines/pipeline_advisor.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         operation_id = node.content['name']
         if 'exog_ts' in operation_id:
             return RemoveType.forbidden
         if 'custom' in operation_id or 'lagged' in operation_id:
             return RemoveType.with_parents
         if 'data_source' in operation_id:
             return RemoveType.with_direct_children
-        return RemoveType.node_only
+        return RemoveType.node_rewire
 
     def propose_change(self, node: OptNode, possible_operations: List[str]) -> List[str]:
         """
         Proposes promising candidates for node replacement
         :param node: node to propose changes for
         :param possible_operations: list of candidates for replace
         :return: list of candidates with str operations
@@ -75,10 +75,10 @@
                     # the sequence of the same parent and child is not meaningful
                     candidates.remove(parent_operation_id)
         return candidates
 
 
 def check_for_specific_operations(operation_id: str):
     if ('data_source' in operation_id or
-            'exog_ts' == operation_id or 'custom' in operation_id):
+            'exog_ts' in operation_id or 'custom' in operation_id):
         return True
     return False
```

### Comparing `fedot-0.7.0/fedot/core/pipelines/pipeline_composer_requirements.py` & `fedot-0.7.1/fedot/core/pipelines/pipeline_composer_requirements.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/pipeline_graph_generation_params.py` & `fedot-0.7.1/fedot/core/pipelines/pipeline_graph_generation_params.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/pipeline_node_factory.py` & `fedot-0.7.1/fedot/core/pipelines/pipeline_node_factory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/random_pipeline_factory.py` & `fedot-0.7.1/fedot/core/pipelines/random_pipeline_factory.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/template.py` & `fedot-0.7.1/fedot/core/pipelines/template.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/ts_wrappers.py` & `fedot-0.7.1/fedot/core/pipelines/ts_wrappers.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/tuning/hyperparams.py` & `fedot-0.7.1/fedot/core/pipelines/tuning/hyperparams.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/tuning/search_space.py` & `fedot-0.7.1/fedot/core/pipelines/tuning/search_space.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional, Dict, Tuple, Callable, List
+
 import numpy as np
 from golem.core.tuning.search_space import SearchSpace
 from hyperopt import hp
 
 
 class PipelineSearchSpace(SearchSpace):
     """
@@ -9,15 +11,15 @@
 
     :param custom_search_space: dictionary of dictionaries of tuples (hyperopt expression (e.g. hp.choice), *params)
      for applying custom hyperparameters search space
     :param replace_default_search_space: whether replace default dictionary (False) or append it (True)
     """
 
     def __init__(self,
-                 custom_search_space: dict = None,
+                 custom_search_space: Optional[Dict[str, Dict[str, Tuple[Callable, List]]]] = None,
                  replace_default_search_space: bool = False):
         self.custom_search_space = custom_search_space
         self.replace_default_search_space = replace_default_search_space
         parameters_per_operation = self.get_parameters_dict()
         super().__init__(parameters_per_operation)
 
     def get_parameters_dict(self):
@@ -255,16 +257,15 @@
                 'reg_lambda': (hp.loguniform, [np.log(1e-8), np.log(10)])
             },
             'catboost': {
                 'max_depth': (hp.uniformint, [1, 11]),
                 'learning_rate': (hp.loguniform, [np.log(0.01), np.log(0.2)]),
                 'min_data_in_leaf': (hp.qloguniform, [0, 6, 1]),
                 'border_count': (hp.uniformint, [2, 255]),
-                'l2_leaf_reg': (hp.loguniform, [np.log(1e-8), np.log(10)]),
-                'loss_function': (hp.choice, [['Logloss', 'CrossEntropy']])
+                'l2_leaf_reg': (hp.loguniform, [np.log(1e-8), np.log(10)])
             },
             'catboostreg': {
                 'max_depth': (hp.uniformint, [1, 11]),
                 'learning_rate': (hp.loguniform, [np.log(0.01), np.log(0.2)]),
                 'min_data_in_leaf': (hp.qloguniform, [0, 6, 1]),
                 'border_count': (hp.uniformint, [2, 255]),
                 'l2_leaf_reg': (hp.loguniform, [np.log(1e-8), np.log(10)])
@@ -288,15 +289,14 @@
                 'ngram_range': (hp.choice, [[(1, 1), (1, 2), (1, 3)]]),
                 'min_df': (hp.uniform, [0.0001, 0.1]),
                 'max_df': (hp.uniform, [0.9, 0.99])
             },
         }
 
         if self.custom_search_space is not None:
-            for operation in self.custom_search_space.keys():
-                if self.replace_default_search_space:
-                    parameters_per_operation[operation] = self.custom_search_space[operation]
-                else:
-                    for key, value in self.custom_search_space[operation].items():
-                        parameters_per_operation[operation][key] = value
+            if self.replace_default_search_space:
+                parameters_per_operation.update(self.custom_search_space)
+            else:
+                for operation_name, operation_dct in self.custom_search_space.items():
+                    parameters_per_operation[operation_name].update(operation_dct)
 
         return parameters_per_operation
```

### Comparing `fedot-0.7.0/fedot/core/pipelines/tuning/tuner_builder.py` & `fedot-0.7.1/fedot/core/pipelines/tuning/tuner_builder.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/verification.py` & `fedot-0.7.1/fedot/core/pipelines/verification.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/pipelines/verification_rules.py` & `fedot-0.7.1/fedot/core/pipelines/verification_rules.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,72 +102,116 @@
     else:
         raise ValueError(f'{ERROR_PREFIX} pipeline not contains operations for time series processing')
 
 
 def has_no_data_flow_conflicts_in_ts_pipeline(pipeline: Pipeline):
     """ Function checks the correctness of connection between nodes """
     task = Task(TaskTypesEnum.ts_forecasting)
-    models = get_operations_for_task(task=task, mode='model')
+    ts_models = get_operations_for_task(task=task, mode='model', tags=["non_lagged"])
+    non_ts_models = list(set(get_operations_for_task(task=task, mode='model')).difference(set(ts_models)))
+
     # Preprocessing not only for time series
     non_ts_data_operations = get_operations_for_task(task=task,
                                                      mode='data_operation',
                                                      tags=["non_applicable_for_ts"])
     ts_data_operations = get_operations_for_task(task=task,
                                                  mode='data_operation',
                                                  tags=["non_lagged"])
     # Remove lagged and sparse lagged transformation
     ts_data_operations.remove('lagged')
     ts_data_operations.remove('sparse_lagged')
     ts_data_operations.remove('exog_ts')
 
+    ts_to_table_operations = ['lagged', 'sparse_lagged', 'exog_ts']
+
     # Dictionary as {'current operation in the node': 'parent operations list'}
-    # TODO refactor
-    wrong_connections = {'lagged': models + non_ts_data_operations + ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'sparse_lagged': models + non_ts_data_operations + ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'ar': models + non_ts_data_operations + ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'arima': models + non_ts_data_operations + ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'ridge': ts_data_operations, 'linear': ts_data_operations,
-                         'lasso': ts_data_operations, 'dtreg': ts_data_operations,
-                         'knnreg': ts_data_operations, 'scaling': ts_data_operations,
-                         'xgbreg': ts_data_operations, 'adareg': ts_data_operations,
-                         'gbr': ts_data_operations, 'treg': ts_data_operations,
-                         'rfr': ts_data_operations, 'svr': ts_data_operations,
-                         'sgdr': ts_data_operations, 'normalization': ts_data_operations,
-                         'kernel_pca': ts_data_operations, 'poly_features': ts_data_operations,
-                         'ransac_lin_reg': ts_data_operations, 'ransac_non_lin_reg': ts_data_operations,
-                         'rfe_lin_reg': ts_data_operations, 'rfe_non_lin_reg': ts_data_operations,
-                         'pca': ts_data_operations,
-                         'gaussian_filter': ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'diff_filter': ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'smoothing': ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'cut': ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'ts_naive_average': ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'locf': ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'ets': ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'polyfit': ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'glm': ['lagged', 'sparse_lagged', 'exog_ts'],
-                         'stl_arima': ['lagged', 'sparse_lagged', 'exog_ts'],
-                         }
+    wrong_connections = get_wrong_links(ts_to_table_operations, ts_data_operations, non_ts_data_operations,
+                                        ts_models, non_ts_models)
+
+    limit_parents_count, need_to_have_parent = get_parent_limits(ts_to_table_operations, ts_data_operations,
+                                                                 non_ts_data_operations,
+                                                                 ts_models)
 
     for node in pipeline.nodes:
         # Operation name in the current node
         current_operation = node.operation.operation_type
         parent_nodes = node.nodes_from
-
+        if current_operation in limit_parents_count:
+            if limit_parents_count[current_operation] < len(parent_nodes):
+                raise ValueError(f'{ERROR_PREFIX} Pipeline has incorrect subgraph with wrong parent nodes combination')
         if parent_nodes is not None:
             # There are several parents for current node or at least 1
             for parent in parent_nodes:
                 parent_operation = parent.operation.operation_type
 
                 forbidden_parents = wrong_connections.get(current_operation)
                 if forbidden_parents is not None:
                     __check_connection(parent_operation, forbidden_parents)
+        else:
+            if current_operation in need_to_have_parent:
+                raise ValueError(f'{ERROR_PREFIX} Pipeline has incorrect subgraph with wrong parent nodes combination')
     return True
 
 
+def get_wrong_links(ts_to_table_operations: list, ts_data_operations: list, non_ts_data_operations: list,
+                    ts_models: list, non_ts_models: list) -> dict:
+    """
+    Function that return wrong ts connections like op_A : [op_B, op_C] that means op_B and op_C
+    can't be a parent for op_A.
+
+    :param ts_to_table_operations: list of ts_to_table operations
+    :param ts_data_operations: list of ts data operations
+    :param non_ts_data_operations: list of non ts data operations
+    :param ts_models: list of ts models
+    :param non_ts_models: list of non ts models
+    :return: dict with wrong connections
+    """
+    limit_lagged_parents = {lagged_op: ts_models + non_ts_models + non_ts_data_operations + ts_to_table_operations
+                            for lagged_op in ts_to_table_operations}
+
+    limit_ts_models_parents = {ts_model: ts_models + non_ts_models + non_ts_data_operations + ts_to_table_operations
+                               for ts_model in ts_models}
+    limit_non_ts_models_parents = {non_ts_model: ts_data_operations
+                                   for non_ts_model in non_ts_models}
+
+    limit_ts_data_operations_parents = {
+        ts_data_op: ts_models + non_ts_models + non_ts_data_operations + ts_to_table_operations
+        for ts_data_op in ts_data_operations}
+    limit_non_ts_data_operations_parents = {non_ts_data_op: ts_data_operations
+                                            for non_ts_data_op in non_ts_data_operations}
+
+    wrong_connections = {**limit_non_ts_data_operations_parents,
+                         **limit_ts_data_operations_parents,
+                         **limit_non_ts_models_parents,
+                         **limit_ts_models_parents,
+                         **limit_lagged_parents}
+    return wrong_connections
+
+
+def get_parent_limits(ts_to_table_operations: list, ts_data_operations: list, non_ts_data_operations: list,
+                      ts_models: list) -> (dict, list):
+    """
+    Function that return some constraints on number of parents for time series forecasting graphs
+
+    :param ts_to_table_operations: list of ts_to_table operations
+    :param ts_data_operations: list of ts data operations
+    :param non_ts_data_operations: list of non ts data operations
+    :param ts_models: list of ts models
+    :return: dict with parent limits and list with operations that must have a parent
+    """
+    limit_ts_model_data_op_parents_count = {ts_model_op: 1
+                                            for ts_model_op in ts_models + ts_data_operations + ts_to_table_operations}
+
+    limit_decompose_parents_count = {'decompose': 1}
+
+    limit_parents_count = {**limit_ts_model_data_op_parents_count, **limit_decompose_parents_count}
+    need_to_have_parent = [op for op in non_ts_data_operations]
+    return limit_parents_count, need_to_have_parent
+
+
 def only_non_lagged_operations_are_primary(pipeline: Pipeline):
     """ Only time series specific operations could be placed in primary nodes """
 
     # Check only primary nodes
     for node in pipeline.nodes:
         if isinstance(node, PipelineNode) and node.is_primary and \
                 DataTypesEnum.ts not in node.operation.metadata.input_types:
```

### Comparing `fedot-0.7.0/fedot/core/repository/data/automl_repository.json` & `fedot-0.7.1/fedot/core/repository/data/automl_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/repository/data/data_operation_repository.json` & `fedot-0.7.1/fedot/core/repository/data/data_operation_repository.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989484126984127%*

 * *Differences: {"'operations'": "{'scaling': {'tags': {insert: [(2, 'non_applicable_for_ts')]}}, 'normalization': "*

 * *                 "{'tags': {insert: [(2, 'non_applicable_for_ts')]}}, 'isolation_forest_reg': "*

 * *                 "{'tags': {insert: [(2, 'non_applicable_for_ts')]}}, 'rfe_lin_reg': {'tags': "*

 * *                 "{insert: [(4, 'non_applicable_for_ts')]}}, 'rfe_non_lin_reg': {'tags': {insert: "*

 * *                 "[(4, 'non_applicable_for_ts')]}}}"}*

```diff
@@ -317,15 +317,16 @@
                 "filtering"
             ]
         },
         "isolation_forest_reg": {
             "meta": "regression_preprocessing",
             "tags": [
                 "non_linear",
-                "filtering"
+                "filtering",
+                "non_applicable_for_ts"
             ]
         },
         "kernel_pca": {
             "meta": "dimension_transformation",
             "presets": [
                 "ts",
                 "*tree"
@@ -372,15 +373,16 @@
             "presets": [
                 "fast_train",
                 "ts",
                 "*tree"
             ],
             "tags": [
                 "simple",
-                "feature_scaling"
+                "feature_scaling",
+                "non_applicable_for_ts"
             ]
         },
         "one_hot_encoding": {
             "meta": "sklearn_categorical",
             "tags": [
                 "encoding",
                 "categorical",
@@ -457,15 +459,16 @@
         },
         "rfe_lin_reg": {
             "meta": "regression_preprocessing",
             "tags": [
                 "linear",
                 "feature_selection",
                 "non_applicable_for_ts",
-                "non-default"
+                "non-default",
+                "non_applicable_for_ts"
             ]
         },
         "rfe_non_lin_class": {
             "meta": "classification_preprocessing",
             "tags": [
                 "non_linear",
                 "feature_selection",
@@ -474,27 +477,29 @@
         },
         "rfe_non_lin_reg": {
             "meta": "regression_preprocessing",
             "tags": [
                 "non_linear",
                 "feature_selection",
                 "non_applicable_for_ts",
-                "non-default"
+                "non-default",
+                "non_applicable_for_ts"
             ]
         },
         "scaling": {
             "meta": "custom_preprocessing",
             "presets": [
                 "fast_train",
                 "ts",
                 "*tree"
             ],
             "tags": [
                 "simple",
-                "feature_scaling"
+                "feature_scaling",
+                "non_applicable_for_ts"
             ]
         },
         "simple_imputation": {
             "meta": "custom_preprocessing",
             "presets": [
                 "fast_train",
                 "*tree"
```

### Comparing `fedot-0.7.0/fedot/core/repository/data/default_operation_params.json` & `fedot-0.7.1/fedot/core/repository/data/default_operation_params.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/repository/data/gpu_models_repository.json` & `fedot-0.7.1/fedot/core/repository/data/gpu_models_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/repository/data/model_repository.json` & `fedot-0.7.1/fedot/core/repository/data/model_repository.json`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/repository/dataset_types.py` & `fedot-0.7.1/fedot/core/repository/dataset_types.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/repository/default_params_repository.py` & `fedot-0.7.1/fedot/core/repository/default_params_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/repository/json_evaluation.py` & `fedot-0.7.1/fedot/core/repository/json_evaluation.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/repository/operation_types_repository.py` & `fedot-0.7.1/fedot/core/repository/operation_types_repository.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/repository/pipeline_operation_repository.py` & `fedot-0.7.1/fedot/core/repository/pipeline_operation_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import itertools
 from typing import List, Optional, Dict
 
-import numpy as np
-
 from fedot.api.api_utils.presets import OperationsPreset
 from fedot.core.repository.graph_operation_repository import GraphOperationRepository
 from fedot.core.repository.operation_types_repository import get_operations_for_task
 from fedot.core.repository.tasks import Task, TaskTypesEnum
 
 
 class PipelineOperationRepository(GraphOperationRepository):
```

### Comparing `fedot-0.7.0/fedot/core/repository/quality_metrics_repository.py` & `fedot-0.7.1/fedot/core/repository/quality_metrics_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 from fedot.core.composer.metrics import (ComputationTime, Accuracy, F1, Logloss, MAE,
                                          MAPE, SMAPE, MSE, MSLE, Metric, NodeNum, Precision, R2,
                                          RMSE, ROCAUC, Silhouette, StructuralComplexity)
 
 
 class MetricsEnum(Enum):
-    pass
+    def __str__(self):
+        return self.value
 
 
 G = TypeVar('G', bound=Graph, covariant=True)
 MetricCallable = Callable[[G], Real]
 MetricType = Union[MetricCallable, MetricsEnum]
```

### Comparing `fedot-0.7.0/fedot/core/repository/tasks.py` & `fedot-0.7.1/fedot/core/repository/tasks.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/utils.py` & `fedot-0.7.1/fedot/core/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import os
 import platform
+import random
 import tempfile
 from pathlib import Path
+from typing import Optional
 
 import numpy as np
 import pandas as pd
+from golem.core.utilities.random import RandomStateHandler
 from sklearn.model_selection import train_test_split
 
 DEFAULT_PARAMS_STUB = 'default_params'
 
 
 def fedot_project_root() -> Path:
     """Returns FEDOT project root folder."""
     return Path(__file__).parent.parent.parent
 
 
 def default_fedot_data_dir() -> str:
     """ Returns the folder where all the output data
-    is recorded to. Default: home/Fedot
+    is recorded to. Default: home/FEDOT
     """
-    temp_folder = Path("/tmp" if platform.system() == "Darwin" else tempfile.gettempdir())
-    default_data_path = os.path.join(temp_folder, 'FEDOT')
+    temp_dir = Path("/tmp" if platform.system() == "Darwin" else tempfile.gettempdir())
+    default_data_path = os.path.join(temp_dir, 'FEDOT')
 
-    if 'FEDOT' not in os.listdir(temp_folder):
+    if 'FEDOT' not in os.listdir(temp_dir):
         os.mkdir(default_data_path)
 
     return default_data_path
 
 
 def labels_to_dummy_probs(prediction: np.array):
     """ Returns converted predictions using one-hot probability encoding """
@@ -74,7 +77,15 @@
 def make_pipeline_generator(pipeline):
     visited_nodes = []
 
     for node in pipeline.nodes:
         if node not in visited_nodes:
             visited_nodes.append(node)
             yield node
+
+
+def set_random_seed(seed: Optional[int]):
+    """ Sets random seed for evaluation of models"""
+    if seed is not None:
+        np.random.seed(seed)
+        random.seed(seed)
+        RandomStateHandler.MODEL_FITTING_SEED = seed
```

### Comparing `fedot-0.7.0/fedot/core/validation/split.py` & `fedot-0.7.1/fedot/core/validation/split.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/core/visualisation/pipeline_specific_visuals.py` & `fedot-0.7.1/fedot/core/visualisation/pipeline_specific_visuals.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/explainability/explainers.py` & `fedot-0.7.1/fedot/explainability/explainers.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/explainability/surrogate_explainer.py` & `fedot-0.7.1/fedot/explainability/surrogate_explainer.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/preprocessing/base_preprocessing.py` & `fedot-0.7.1/fedot/preprocessing/base_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/preprocessing/categorical.py` & `fedot-0.7.1/fedot/preprocessing/categorical.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/preprocessing/data_type_check.py` & `fedot-0.7.1/fedot/preprocessing/data_type_check.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/preprocessing/data_types.py` & `fedot-0.7.1/fedot/preprocessing/data_types.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/preprocessing/dummy_preprocessing.py` & `fedot-0.7.1/fedot/preprocessing/dummy_preprocessing.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/preprocessing/preprocessing.py` & `fedot-0.7.1/fedot/preprocessing/preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 import numpy as np
 import pandas as pd
 from golem.core.log import default_log
 from golem.core.paths import copy_doc
 from sklearn.preprocessing import LabelEncoder
 
-from fedot.core.data.data import InputData, OutputData, data_type_is_table, data_type_is_ts, data_type_is_text
+from fedot.core.data.data import InputData, np_datetime_to_numeric
+from fedot.core.data.data import OutputData, data_type_is_table, data_type_is_ts, data_type_is_text
 from fedot.core.data.data_preprocessing import (
     data_has_categorical_features,
     data_has_missing_values,
     find_categorical_columns,
     replace_inf_with_nans,
     replace_nans_with_empty_strings
 )
@@ -83,15 +84,15 @@
                 self.types_correctors[data_source] = TableTypesCorrector()
         else:
             raise ValueError('Unknown type of data.')
 
     def _init_main_target_source_name(self, multi_data: MultiModalData):
         """
         Defines main_target_source_name for MultiModal data branches with main target and the side ones
-        
+
         Args:
             multi_data: `MultiModalData`
         """
         if self.main_target_source_name is not None:
             # Target name has been already defined
             return None
 
@@ -114,88 +115,93 @@
                 data[data_source_name] = self._prepare_obligatory_unimodal_for_fit(values,
                                                                                    source_name=data_source_name)
 
         BasePreprocessor.mark_as_preprocessed(data)
         return data
 
     @copy_doc(BasePreprocessor.obligatory_prepare_for_predict)
-    def obligatory_prepare_for_predict(self, data: Union[InputData, MultiModalData]) -> Union[
-        InputData, MultiModalData]:
+    def obligatory_prepare_for_predict(self,
+                                       data: Union[InputData, MultiModalData]) -> Union[InputData, MultiModalData]:
         if isinstance(data, InputData):
             data = self._prepare_obligatory_unimodal_for_predict(data, source_name=DEFAULT_SOURCE_NAME)
 
         elif isinstance(data, MultiModalData):
             for data_source_name, values in data.items():
                 data[data_source_name] = self._prepare_obligatory_unimodal_for_predict(values,
                                                                                        source_name=data_source_name)
 
         BasePreprocessor.mark_as_preprocessed(data)
         return data
 
     @copy_doc(BasePreprocessor.optional_prepare_for_fit)
-    def optional_prepare_for_fit(self, pipeline, data: Union[InputData, MultiModalData]) -> Union[
-        InputData, MultiModalData]:
+    def optional_prepare_for_fit(self, pipeline,
+                                 data: Union[InputData, MultiModalData]) -> Union[InputData, MultiModalData]:
         self._init_supplementary_preprocessors(data)
 
         if isinstance(data, InputData):
             self._prepare_optional(pipeline, data, DEFAULT_SOURCE_NAME)
         else:
             # Multimodal data
             self._init_main_target_source_name(data)
             for data_source_name, values in data.items():
                 self._prepare_optional(pipeline, values, data_source_name)
 
         BasePreprocessor.mark_as_preprocessed(data, is_obligatory=False)
         return data
 
     @copy_doc(BasePreprocessor.optional_prepare_for_predict)
-    def optional_prepare_for_predict(self, pipeline, data: Union[InputData, MultiModalData]) -> Union[
-        InputData, MultiModalData]:
+    def optional_prepare_for_predict(self, pipeline,
+                                     data: Union[InputData, MultiModalData]) -> Union[InputData, MultiModalData]:
         if isinstance(data, InputData):
             self._prepare_optional(pipeline, data, DEFAULT_SOURCE_NAME)
         else:
             # Multimodal data
             for data_source_name, values in data.items():
                 self._prepare_optional(pipeline, values, data_source_name)
 
         BasePreprocessor.mark_as_preprocessed(data, is_obligatory=False)
         return data
 
     def _take_only_correct_features(self, data: InputData, source_name: str):
         """
         Takes only correct features from the table
-        
+
         Args:
             data: to take correct features from
             source_name: name of the data source node
         """
         current_relevant_ids = self.ids_relevant_features[source_name]
         if current_relevant_ids:
             data.features = data.features[:, current_relevant_ids]
 
     @exclude_ts
     @exclude_multi_ts
     @exclude_image
     def _prepare_obligatory_unimodal_for_fit(self, data: InputData, source_name: str) -> InputData:
         """
         Processes InputData for pipeline fit method
-        
+
         Args:
             data: to be preprocessed
             source_name: name of the data source node
-        
+
         Returns:
             obligatory-prepared ``data``
         """
         if data.supplementary_data.obligatorily_preprocessed:
             # Preprocessing was already done - return data
             return data
 
-        # Wrap indices in numpy array
-        data.idx = np.array(data.idx)
+        # Convert datetime data to numerical
+        data.features = np_datetime_to_numeric(data.features)
+        if data.target is not None:
+            data.target = np_datetime_to_numeric(data.target)
+
+        # Wrap indices in numpy array if needed
+        data.idx = np.asarray(data.idx)
 
         # Fix tables / time series sizes
         data = self._correct_shapes(data)
         replace_inf_with_nans(data)
 
         # Find incorrect features which must be removed
         self._find_features_full_of_nans(data, source_name)
@@ -225,26 +231,31 @@
 
     @exclude_ts
     @exclude_multi_ts
     @exclude_image
     def _prepare_obligatory_unimodal_for_predict(self, data: InputData, source_name: str) -> InputData:
         """
         Processes InputData for pipeline predict method
-        
+
         Args:
             data: to be preprocessed
             source_name: name of the data source node
-        
+
         Returns:
             obligatory-prepared data
         """
         if data.supplementary_data.obligatorily_preprocessed:
             # Preprocessing was already done - return data
             return data
 
+        # Convert datetime data to numerical
+        data.features = np_datetime_to_numeric(data.features)
+        if data.target is not None:
+            data.target = np_datetime_to_numeric(data.target)
+
         # Wrap indices in numpy array
         data.idx = np.array(data.idx)
 
         # Fix tables / time series sizes
         data = self._correct_shapes(data)
         replace_inf_with_nans(data)
 
@@ -259,15 +270,15 @@
             data = self.binary_categorical_processors[source_name].transform(data)
 
         return data
 
     def _prepare_optional(self, pipeline, data: InputData, source_name: str):
         """
         Performs optional fitting/preprocessing for unimodal data
-        
+
         Args:
             pipeline: determines if optional preprocessing is needed
             data: to be preprocessed
             source_name: name of the data source node
         """
         if not data_type_is_table(data) or data.supplementary_data.optionally_preprocessed:
             return data
@@ -305,18 +316,18 @@
             else:
                 self.ids_incorrect_features[source_name].append(i)
 
     @staticmethod
     def _drop_rows_with_nan_in_target(data: InputData) -> InputData:
         """
         Drops rows with nans in target column
-        
+
         Args:
             data: to be modified
-        
+
         Returns:
             modified ``data``
         """
         features = data.features
         target = data.target
 
         # Find indices of nans rows. Using pd instead of np because it is needed for string columns
@@ -335,15 +346,15 @@
         return data
 
     @staticmethod
     def _clean_extra_spaces(data: InputData) -> InputData:
         """
         Removes extra spaces from data.
             Transforms cells in columns from ' x ' to 'x'
-        
+
         Args:
             data: to be stripped
 
         Returns:
             cleaned ``data``
         """
         features = pd.DataFrame(data.features)
@@ -377,15 +388,15 @@
 
     def _apply_imputation_unidata(self, data: InputData, source_name: str) -> InputData:
         """
         Fills in the gaps in the provided data.
 
         Args:
             data: data for fill in the gaps
-        
+
         Returns:
             imputed ``data``
         """
         imputer = self.features_imputers.get(source_name)
         if not imputer:
             imputer = ImputationImplementation()
             output_data = imputer.fit_transform(data)
@@ -399,15 +410,15 @@
         """
         Transforms the data inplace. Uses the same transformations as for the training data if trained already.
         Otherwise fits appropriate encoder and converts data's categorical features with it.
 
         Args:
             data: data to be transformed
             source_name: name of the data source node
-        
+
         Returns:
             encoded ``data``
         """
         encoder = self.features_encoders.get(source_name)
         if encoder is None:
             encoder = LabelEncodingImplementation() if self.use_label_encoder else OneHotEncodingImplementation()
             encoder.fit(data)
@@ -417,15 +428,15 @@
         data.features = output_data.predict
         data.supplementary_data = output_data.supplementary_data
         return data
 
     def _train_target_encoder(self, data: InputData, source_name: str):
         """
         Trains `LabelEncoder` if the ``data``'s target consists of strings
-        
+
         Args:
             data: data to be encoded
             source_name: name of the data source node
         """
         categorical_ids, _ = find_categorical_columns(data.target, data.supplementary_data.column_types['target'])
 
         if categorical_ids:
@@ -440,15 +451,15 @@
 
         For example, target [['red'], ['green'], ['red']] will be converted into
         [[0], [1], [0]]
 
         Args:
             data: data to be encoded
             source_name: name of the data source node
-        
+
         Returns:
             encoded ``data``'s target
         """
         encoder = self.target_encoders.get(source_name)
         encoded_target = data.target
         if encoder is not None:
             # Target encoders have already been fitted
@@ -479,33 +490,33 @@
         return column_to_transform
 
     def _determine_target_converter(self):
         """
         Determines which encoder target to use.
         Applicable for inverse target transformation (if there are several targets in
             single MultiModal pipeline).
-        
+
         Returns:
             selected data source name
         """
         # Choose data source node name with main target
         if self.main_target_source_name is None:
             return DEFAULT_SOURCE_NAME
         else:
             return self.main_target_source_name
 
     @staticmethod
     def _correct_shapes(data: InputData) -> InputData:
         """
         Corrects shapes of tabular data or time series.
-        
+
         Args:
             data: time series or tabular. In the first case must be 1d-array, in the second case must be
                 two-dimensional arrays or array of (n, 1) for texts.
-        
+
         Returns:
             corrected tabular data
         """
         if data_type_is_table(data) or data.data_type is DataTypesEnum.multi_ts:
             if np.ndim(data.features) < 2:
                 data.features = data.features.reshape((-1, 1))
             if data.target is not None and np.ndim(data.target) < 2:
```

### Comparing `fedot-0.7.0/fedot/preprocessing/structure.py` & `fedot-0.7.1/fedot/preprocessing/structure.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/remote/infrastructure/clients/client.py` & `fedot-0.7.1/fedot/remote/infrastructure/clients/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from fedot.core.utils import default_fedot_data_dir
 
 G = TypeVar('G', bound=Serializable)
 
 
 class Client:
     """
-    Base class for remote evaluation client. It allow fitting the pipelines in external system instead local one.
+    Base class for remote evaluation client. It allows to fit the pipelines in external system instead local one.
     """
 
     def __init__(self, connect_params: dict, exec_params: dict, output_path: Optional[str] = None):
         """
         :param connect_params: parameters for connection to remote server
         :param exec_params: params for remote task execution
         :param output_path: local path for temporary saving of downloaded pipelines
```

### Comparing `fedot-0.7.0/fedot/remote/infrastructure/clients/datamall_client.py` & `fedot-0.7.1/fedot/remote/infrastructure/clients/datamall_client.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/remote/infrastructure/clients/test_client.py` & `fedot-0.7.1/fedot/remote/infrastructure/clients/test_client.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/remote/pipeline_run_config.py` & `fedot-0.7.1/fedot/remote/pipeline_run_config.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/remote/remote_evaluator.py` & `fedot-0.7.1/fedot/remote/remote_evaluator.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/remote/run_pipeline.py` & `fedot-0.7.1/fedot/remote/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/sensitivity/deletion_methods/multi_times_analysis.py` & `fedot-0.7.1/fedot/sensitivity/deletion_methods/multi_times_analysis.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/sensitivity/node_sa_approaches.py` & `fedot-0.7.1/fedot/sensitivity/node_sa_approaches.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,21 +45,21 @@
                 train_data: InputData, test_data: InputData,
                 is_save: bool = False) -> dict:
 
         """Method runs Node analysis within defined approaches
 
         Args:
             is_save: whether the certain node analysis result is needed to ba saved
-            pipeline: :obj:`Pipeline` containing the analyzed :obj:`Node`
-            node: :obj:`Node` object to analyze in :obj:`Pipeline`
+            pipeline: :obj:`Pipeline` containing the analyzed :obj:`PipelineNode`
+            node: :obj:`PipelineNode` object to analyze in :obj:`Pipeline`
             train_data: data used for :obj:`Pipeline` training
             test_data: data used for :obj:`Pipeline` validation
 
         Returns:
-            dict:  :obj:`Node` analysis result per approach
+            dict:  :obj:`PipelineNode` analysis result per approach
         """
 
         results = dict()
         for approach in self.approaches:
             results[f'{approach.__name__}'] = \
                 approach(pipeline=pipeline,
                          train_data=train_data,
@@ -121,15 +121,15 @@
         self.log.info(f'Node Sensitivity analysis results were saved to {result_file}')
 
 
 class NodeAnalyzeApproach(ABC):
     """Base class for analysis approach.
 
     Args:
-        pipeline: :obj:`Pipeline` containing the analyzed :obj:`Node`
+        pipeline: :obj:`Pipeline` containing the analyzed :obj:`PipelineNode`
         train_data: data used for :obj:`Pipeline` training
         test_data: data used for :obj:`Pipeline` validation
         path_to_save: path to save results to. Default: ``~home/Fedot/sensitivity``
     """
 
     def __init__(self, pipeline: Pipeline, train_data, test_data: InputData,
                  requirements: SensitivityAnalysisRequirements = None,
@@ -188,15 +188,15 @@
                  requirements: SensitivityAnalysisRequirements = None, path_to_save=None):
         super().__init__(pipeline, train_data, test_data, requirements,
                          path_to_save)
 
     def analyze(self, node: PipelineNode, **kwargs) -> Union[List[dict], List[float]]:
         """
         Args:
-            node: :obj:`Node` object to analyze
+            node: :obj:`PipelineNode` object to analyze
 
         Returns:
             the ratio of modified pipeline score to origin score
         """
 
         if node is self._pipeline.root_node:
             # TODO or warning?
@@ -210,15 +210,15 @@
                 loss = 1
 
             return [loss]
 
     def sample(self, node: PipelineNode):
         """
         Args:
-            node: :obj:`Node` object to delete from :obj:`Pipeline` object
+            node: :obj:`PipelineNode` object to delete from :obj:`Pipeline` object
         Retuens:
             :obj:`Pipeline`: pipeline without node
         """
 
         pipeline_sample = deepcopy(self._pipeline)
         node_index_to_delete = self._pipeline.nodes.index(node)
         node_to_delete = pipeline_sample.nodes[node_index_to_delete]
@@ -243,15 +243,15 @@
                  requirements: SensitivityAnalysisRequirements = None, path_to_save=None):
         super().__init__(pipeline, train_data, test_data, requirements,
                          path_to_save)
 
     def analyze(self, node: PipelineNode, **kwargs) -> Union[List[dict], List[float]]:
         """
         Args:
-            node: :obj:`Node` object to analyze
+            node: :obj:`PipelineNode` object to analyze
 
         Returns:
             the ratio of modified pipeline score to origin score
         """
 
         requirements: ReplacementAnalysisMetaParams = self._requirements.replacement_meta
         node_id = self._pipeline.nodes.index(node)
@@ -276,15 +276,15 @@
         return loss_values
 
     def sample(self, node: PipelineNode,
                nodes_to_replace_to: Optional[List[PipelineNode]],
                number_of_random_operations: Optional[int] = None) -> Union[List[Pipeline], Pipeline]:
         """
         Args:
-            node: :obj:`Node` object to replace
+            node: :obj:`PipelineNode` object to replace
             nodes_to_replace_to: nodes provided for old_node replacement
             number_of_random_operations: number of replacement operations,
                 if ``nodes_to_replace_to`` not provided
         Returns:
             Union[List[Pipeline], Pipeline]: sequence of :obj:`Pipeline` objects with new operations instead of old one
         """
 
@@ -310,15 +310,15 @@
         # Get models
         app_models, _ = OperationTypesRepository().suitable_operation(task_type=task)
         # Get data operations for such task
         app_data_operations = OperationTypesRepository('data_operation').suitable_operation(
             task_type=task)
 
         # Unit two lists
-        app_operations = app_models
+        app_operations = app_models + app_data_operations
         if number_of_operations:
             random_operations = random.sample(app_operations, number_of_operations)
         else:
             random_operations = app_operations
 
         nodes = []
         for operation in random_operations:
@@ -346,11 +346,11 @@
             original_operation_index = x_values.index(original_operation_type)
             plt.gca().get_xticklabels()[original_operation_index].set_color('red')
 
         file_name = f'{self._pipeline.nodes[node_id].operation.operation_type}_id_{node_id}_replacement.jpg'
         result_file = join(self._path_to_save, file_name)
         plt.savefig(result_file)
         self.log.info(f'NodeReplacementAnalysis for '
-                         f'{original_operation_type}(index:{node_id}) was saved to {result_file}')
+                      f'{original_operation_type}(index:{node_id}) was saved to {result_file}')
 
     def __str__(self):
         return 'NodeReplaceOperationAnalyze'
```

### Comparing `fedot-0.7.0/fedot/sensitivity/nodes_sensitivity.py` & `fedot-0.7.1/fedot/sensitivity/nodes_sensitivity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from os.path import join
 from typing import List, Optional, Type, Sequence
 
 import numpy as np
 from golem.core.dag.convert import graph_structure_as_nx_graph
+from golem.core.dag.graph import Graph
 from golem.core.log import default_log
 from matplotlib import pyplot as plt
 
 from fedot.core.data.data import InputData
 from fedot.core.pipelines.node import PipelineNode
 from fedot.core.pipelines.pipeline import Pipeline
 from fedot.core.utils import default_fedot_data_dir
@@ -67,15 +68,15 @@
                                        approaches_requirements=self.requirements,
                                        path_to_save=self.path_to_save). \
                 analyze(pipeline=self.pipeline, node=node,
                         train_data=self.train_data,
                         test_data=self.test_data)
             operation_types.append(node.operation.operation_type)
 
-            nodes_results[f'id = {self.pipeline.nodes.index(node)}, ' \
+            nodes_results[f'id = {self.pipeline.nodes.index(node)}, '
                           f'operation = {node.content["name"].operation_type}'] = node_result
 
         if self.requirements.visualization:
             self._visualize_result_per_approach(nodes_results, operation_types)
 
         if len(self.nodes_to_analyze) == len(self.pipeline.nodes):
             self._visualize_degree_correlation(nodes_results)
@@ -128,15 +129,15 @@
         for approach in self.approaches:
             approach_result = [np.mean(result[f'{approach.__name__}']) - 1 for result in results.values()]
             gathered_results.append(approach_result)
 
         return gathered_results
 
 
-def get_nodes_degrees(graph: 'Graph') -> Sequence[int]:
+def get_nodes_degrees(graph: Graph) -> Sequence[int]:
     """Nodes degree as the number of edges the node has:
         ``degree = #input_edges + #out_edges``
 
     Returns:
         nodes degrees ordered according to the nx_graph representation of this graph
     """
     graph, _ = graph_structure_as_nx_graph(graph)
```

### Comparing `fedot-0.7.0/fedot/sensitivity/operations_hp_sensitivity/multi_operations_sensitivity.py` & `fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/multi_operations_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/sensitivity/operations_hp_sensitivity/one_operation_sensitivity.py` & `fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/one_operation_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/sensitivity/operations_hp_sensitivity/problem.py` & `fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/problem.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/sensitivity/operations_hp_sensitivity/sa_and_sample_methods.py` & `fedot-0.7.1/fedot/sensitivity/operations_hp_sensitivity/sa_and_sample_methods.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/sensitivity/pipeline_sensitivity.py` & `fedot-0.7.1/fedot/sensitivity/pipeline_sensitivity.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/sensitivity/pipeline_sensitivity_facade.py` & `fedot-0.7.1/fedot/sensitivity/pipeline_sensitivity_facade.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/sensitivity/sa_requirements.py` & `fedot-0.7.1/fedot/sensitivity/sa_requirements.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/utilities/debug.py` & `fedot-0.7.1/fedot/utilities/debug.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/utilities/define_metric_by_task.py` & `fedot-0.7.1/fedot/utilities/define_metric_by_task.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/utilities/golem_imports_transition.py` & `fedot-0.7.1/fedot/utilities/golem_imports_transition.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/utilities/memory.py` & `fedot-0.7.1/fedot/utilities/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import logging
 import tracemalloc
 from typing import Optional
 
+from golem.core.log import default_log
+
 
 class MemoryAnalytics:
     is_active = False
     active_session_label = 'main'
 
     @classmethod
     def start(cls):
@@ -16,15 +18,15 @@
         tracemalloc.start()
 
     @classmethod
     def finish(cls):
         """
         Finish memory monitoring session
         """
-        cls.log(additional_info=f'finish',
+        cls.log(additional_info='finish',
                 logging_level=45)  # message logging level
         tracemalloc.stop()
         cls.is_active = False
 
     @classmethod
     def get_measures(cls):
         """
@@ -46,12 +48,11 @@
         """
         message = ''
         if cls.is_active:
             memory_consumption = cls.get_measures()
             message = f'Memory consumption for {additional_info} in {cls.active_session_label} session: ' \
                       f'current {round(memory_consumption[0], 1)} MiB, ' \
                       f'max: {round(memory_consumption[1], 1)} MiB'
-            if logger is not None:
-                logger.log(logging_level, message)
-            else:
-                print(message)
+            if logger is None:
+                logger = default_log(prefix=cls.__name__)
+            logger.log(logging_level, message)
         return message
```

### Comparing `fedot-0.7.0/fedot/utilities/project_import_export.py` & `fedot-0.7.1/fedot/utilities/project_import_export.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/utilities/synth_dataset_generator.py` & `fedot-0.7.1/fedot/utilities/synth_dataset_generator.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot/utilities/ts_gapfilling.py` & `fedot-0.7.1/fedot/utilities/ts_gapfilling.py`

 * *Files identical despite different names*

### Comparing `fedot-0.7.0/fedot.egg-info/PKG-INFO` & `fedot-0.7.1/fedot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedot
-Version: 0.7.0
+Version: 0.7.1
 Summary: Automated machine learning framework for composite pipelines
 Home-page: https://github.com/aimclub/FEDOT
 Author: NSS Lab
 Author-email: itmo.nss.team@gmail.com
 License: BSD 3-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
@@ -30,62 +30,59 @@
 .. start-badges
 .. list-table::
    :stub-columns: 1
 
    * - package
      - | |pypi| |python|
    * - tests
-     - | |build| |coverage|
+     - | |build| |integration| |coverage|
    * - docs
      - |docs|
    * - license
      - | |license|
    * - stats
      - | |downloads_stats|
    * - support
      - | |tg|
    * - languages
      - | |eng| |rus|
+   * - mirror
+     - | |gitlab|
+   * - funding
+     - | |ITMO| |NCCR|
 .. end-badges
 
 **FEDOT** is an open-source framework for automated modeling and machine learning (AutoML) problems. This framework is distributed under the 3-Clause BSD license.
 
 It provides automatic generative design of machine learning pipelines for various real-world problems. The core of FEDOT is based on an evolutionary approach and supports classification (binary and multiclass), regression, clustering, and time series prediction problems.
 
-.. image:: /docs/pipeline_small.png
-   :alt: The structure of the modeling pipeline that can be optimised by FEDOT
+.. image:: /docs/fedot-workflow.png
+   :alt: The structure of the AutoML workflow in FEDOT
 
 The key feature of the framework is the complex management of interactions between various blocks of pipelines. It is represented as a graph that defines connections between data preprocessing and model blocks.
 
 The project is maintained by the research team of the Natural Systems Simulation Lab, which is a part of the `National Center for Cognitive Research of ITMO University <https://actcognitive.org/>`__.
 
 More details about FEDOT are available in the next video:
 
 
 .. image:: https://res.cloudinary.com/marcomontalbano/image/upload/v1606396758/video_to_markdown/images/youtube--RjbuV6i6de4-c05b58ac6eb4c4700831b2b3070cd403.jpg
    :target: http://www.youtube.com/watch?v=RjbuV6i6de4
    :alt: Introducing Fedot
 
-FEDOT Features
+FEDOT concepts
 ==============
 
-The main features of the framework are as follows:
-
-- **Flexibility.** FEDOT is highly flexible: it can be used to automate the construction of solutions for various problems, data types, and models;
-- **Integration with ML libraries.** FEDOT supports widely used ML libraries (Scikit-Learn, Catboost, Xgboost, etc.) and allows you to integrate custom ones;
-- **Extensibility for new domains.** Pipeline optimization algorithms are data- and task-independent, yet you can use special templates for a specific task class or data type (time series forecasting, NLP, tabular data, etc.) to increase the efficiency;
-- **No limits.** The framework is versatile and is not limited to specific modeling tasks, for example, it can be used in ODE or PDE;
-- **Support of hyper-parameter tuning.** Hyper-parameter tuning methods are supported. Custom methods can also be integrated in FEDOT;
-- **Reproducibility.** You can export the resulting pipelines in JSON format for experiment reproducibility.
-
-Compared to other frameworks:
-
-- There are no limits to specific modeling tasks, therefore FEDOT claims versatility and expandability;
-- Allows managing the complexity of models and thereby achieving better results.
-- Allows building pipelines using different types of input data (texts, images, tables, etc.) and consisting of various models.
+- **Flexibility.** FEDOT can be used to automate the construction of solutions for various `problems <https://fedot.readthedocs.io/en/master/introduction/fedot_features/main_features.html#involved-tasks>`_, `data types <https://fedot.readthedocs.io/en/master/introduction/fedot_features/automation_features.html#data-nature>`_ (texts, images, tables), and `models <https://fedot.readthedocs.io/en/master/advanced/automated_pipelines_design.html>`_;
+- **Extensibility.** Pipeline optimization algorithms are data- and task-independent, yet you can use `special strategies <https://fedot.readthedocs.io/en/master/api/strategies.html>`_ for specific tasks or data types (time-series forecasting, NLP, tabular data, etc.) to increase the efficiency;
+- **Integrability.** FEDOT supports widely used ML libraries (Scikit-learn, CatBoost, XGBoost, etc.) and allows you to integrate `custom ones <https://fedot.readthedocs.io/en/master/api/strategies.html#module-fedot.core.operations.evaluation.custom>`_;
+- **Tuningability.** Various `hyper-parameters tuning methods <https://fedot.readthedocs.io/en/master/advanced/hyperparameters_tuning.html>`_ are supported including models' custom evaluation metrics and search spaces;
+- **Versatility.** FEDOT is `not limited to specific modeling tasks <https://fedot.readthedocs.io/en/master/advanced/architecture.html>`_, for example, it can be used in ODE or PDE;
+- **Reproducibility.** Resulting pipelines can be `exported separately as JSON <https://fedot.readthedocs.io/en/master/advanced/pipeline_import_export.html>`_ or `together with your input data as ZIP archive <https://fedot.readthedocs.io/en/master/advanced/project_import_export.html>`_ for experiments reproducibility;
+- **Customizability.** FEDOT allows `managing models complexity <https://fedot.readthedocs.io/en/master/introduction/fedot_features/automation_features.html#models-used>`_ and thereby achieving desired quality.
 
 Installation
 ============
 
 The simplest way to install FEDOT is using ``pip``:
 
 .. code-block::
@@ -213,16 +210,14 @@
 Also, we are doing several research tasks related to AutoML time-series benchmarking and multi-modal modeling.
 
 Any contribution is welcome. Our R&D team is open for cooperation with other scientific teams as well as with industrial partners.
 
 Documentation
 =============
 
-The general description is available in the `FEDOT.Docs <https://itmo-nss-team.github.io/FEDOT.Miscellaneous>`__ repository.
-
 Also, a detailed FEDOT API description is available in `Read the Docs <https://fedot.readthedocs.io/en/latest/>`__.
 
 Contribution Guide
 ==================
 
 - The contribution guide is available in this `repository <https://github.com/aimclub/FEDOT/blob/master/docs/source/contribution.rst>`__.
 
@@ -273,15 +268,19 @@
 
 .. |docs| image:: https://readthedocs.org/projects/ebonite/badge/?style=flat
    :target: https://fedot.readthedocs.io/en/latest/
    :alt: Documentation Status
 
 .. |build| image:: https://github.com/aimclub/FEDOT/workflows/Build/badge.svg?branch=master
    :alt: Build Status
-   :target: https://github.com/aimclub/FEDOT/actions
+   :target: https://github.com/aimclub/FEDOT/actions/workflows/unit-build.yml
+
+.. |integration| image:: https://github.com/aimclub/FEDOT/workflows/Integration/badge.svg?branch=master
+   :alt: Integration Build Status
+   :target: https://github.com/aimclub/FEDOT/actions/workflows/integration-build.yml
 
 .. |coverage| image:: https://codecov.io/gh/aimclub/FEDOT/branch/master/graph/badge.svg
    :alt: Coverage Status
    :target: https://codecov.io/gh/aimclub/FEDOT
 
 .. |pypi| image:: https://badge.fury.io/py/fedot.svg
    :alt: Supported Python Versions
@@ -297,7 +296,19 @@
 
 .. |downloads_stats| image:: https://static.pepy.tech/personalized-badge/fedot?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads
    :target: https://pepy.tech/project/fedot
 
 .. |tg| image:: https://img.shields.io/badge/Telegram-Group-blue.svg
           :target: https://t.me/FEDOT_helpdesk
           :alt: Telegram Chat
+
+.. |ITMO| image:: https://github.com/ITMO-NSS-team/open-source-ops/blob/add_badge/badges/ITMO_badge_rus.svg
+   :alt: Acknowledgement to ITMO
+   :target: https://itmo.ru
+
+.. |NCCR| image:: https://github.com/ITMO-NSS-team/open-source-ops/blob/add_badge/badges/NCCR_badge.svg
+   :alt: Acknowledgement to NCCR
+   :target: https://actcognitive.org/
+
+.. |gitlab| image:: https://camo.githubusercontent.com/9bd7b8c5b418f1364e72110a83629772729b29e8f3393b6c86bff237a6b784f6/68747470733a2f2f62616467656e2e6e65742f62616467652f6769746c61622f6d6972726f722f6f72616e67653f69636f6e3d6769746c6162
+   :alt: GitLab mirror for this repository
+   :target: https://gitlab.actcognitive.org/itmo-nss-team/FEDOT
```

### Comparing `fedot-0.7.0/fedot.egg-info/SOURCES.txt` & `fedot-0.7.1/fedot.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 examples/advanced/multi_modal_pipeline.py
 examples/advanced/multimodal_text_num_example.py
 examples/advanced/multiobj_optimisation.py
 examples/advanced/multitask_classification_regression.py
 examples/advanced/parallelization_comparison.py
 examples/advanced/pipeline_sensitivity.py
 examples/advanced/profiler_example.py
+examples/advanced/surrogate_optimization.py
 examples/advanced/automl/__init__.py
 examples/advanced/automl/h2o_example.py
 examples/advanced/automl/pipeline_from_automl.py
 examples/advanced/automl/tpot_example.py
 examples/advanced/automl/tpot_vs_fedot.py
 examples/advanced/decompose/__init__.py
 examples/advanced/decompose/classification_refinement_example.py
@@ -94,16 +95,17 @@
 fedot/api/fedot_cli.py
 fedot/api/help.py
 fedot/api/main.py
 fedot/api/time.py
 fedot/api/api_utils/__init__.py
 fedot/api/api_utils/api_composer.py
 fedot/api/api_utils/api_data.py
-fedot/api/api_utils/api_data_analyser.py
+fedot/api/api_utils/api_params_repository.py
 fedot/api/api_utils/data_definition.py
+fedot/api/api_utils/input_analyser.py
 fedot/api/api_utils/metrics.py
 fedot/api/api_utils/params.py
 fedot/api/api_utils/predefined_model.py
 fedot/api/api_utils/presets.py
 fedot/api/api_utils/assumptions/__init__.py
 fedot/api/api_utils/assumptions/assumptions_builder.py
 fedot/api/api_utils/assumptions/assumptions_handler.py
@@ -119,14 +121,15 @@
 fedot/core/caching/pipelines_cache.py
 fedot/core/caching/pipelines_cache_db.py
 fedot/core/caching/preprocessing_cache.py
 fedot/core/caching/preprocessing_cache_db.py
 fedot/core/composer/__init__.py
 fedot/core/composer/composer.py
 fedot/core/composer/composer_builder.py
+fedot/core/composer/meta_rules.py
 fedot/core/composer/metrics.py
 fedot/core/composer/random_composer.py
 fedot/core/composer/gp_composer/__init__.py
 fedot/core/composer/gp_composer/gp_composer.py
 fedot/core/composer/gp_composer/specific_operators.py
 fedot/core/data/__init__.py
 fedot/core/data/array_utilities.py
```

### Comparing `fedot-0.7.0/fedot.egg-info/requires.txt` & `fedot-0.7.1/fedot.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-thegolem>=0.2.0
+thegolem==0.3.1
 numpy!=1.24.0,>=1.16.0
 anytree>=2.8.0
 catboost>=0.25.0
 lightgbm>=3.0.0
 xgboost>=1.4.0
 statsmodels>=0.12.0
 ete3>=3.1.0
```

### Comparing `fedot-0.7.0/setup.py` & `fedot-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 # The directory containing this file
 HERE = Path(__file__).parent.resolve()
 
 # The text of the README file
 NAME = 'fedot'
-VERSION = '0.7.0'
+VERSION = '0.7.1'
 AUTHOR = 'NSS Lab'
 SHORT_DESCRIPTION = 'Automated machine learning framework for composite pipelines'
 README = Path(HERE, 'README_en.rst').read_text(encoding='utf-8')
 URL = 'https://github.com/aimclub/FEDOT'
 REQUIRES_PYTHON = '>=3.8'
 LICENSE = 'BSD 3-Clause'
```

### Comparing `fedot-0.7.0/test/test_gpu_strategy.py` & `fedot-0.7.1/test/test_gpu_strategy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Tuple
 
-from fedot.core.data.data import InputData, OutputData
+from cuml.svm import SVC
 
-from test.unit.models.test_split_train_test import get_synthetic_input_data
-from fedot.core.operations.evaluation.gpu.common import CuMLEvaluationStrategy
+from fedot.core.data.data import InputData, OutputData
 from fedot.core.operations.evaluation.gpu.classification import CuMLClassificationStrategy
-from cuml.svm import SVC
+from fedot.core.operations.evaluation.gpu.common import CuMLEvaluationStrategy
+from test.integration.models.test_split_train_test import get_synthetic_input_data
 
 
 def get_synthetic_data() -> Tuple[InputData, InputData]:
     train_data = get_synthetic_input_data(10000)
     test_data = get_synthetic_input_data(1000)
 
     return train_data, test_data
```

