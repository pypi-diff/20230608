# Comparing `tmp/simba_ml-1.0.0rc7.tar.gz` & `tmp/simba_ml-1.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simba_ml-1.0.0rc7.tar", last modified: Tue Jun  6 08:32:34 2023, max compression
+gzip compressed data, was "simba_ml-1.0.0rc8.tar", last modified: Thu Jun  8 13:17:19 2023, max compression
```

## Comparing `simba_ml-1.0.0rc7.tar` & `simba_ml-1.0.0rc8.tar`

### file list

```diff
@@ -1,177 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.568078 simba_ml-1.0.0rc7/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-06 08:32:34.568078 simba_ml-1.0.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-06 08:32:34.568078 simba_ml-1.0.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.568078 simba_ml-1.0.0rc7/simba_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-06 08:32:34.568078 simba_ml-1.0.0rc7/simba_ml/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.556078 simba_ml-1.0.0rc7/simba_ml/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/cli/generate_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.556078 simba_ml-1.0.0rc7/simba_ml/cli/problem_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/cli/problem_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/cli/problem_viewer/problem_viewer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/cli/problem_viewer/run_problem_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/cli/start_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/error_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.556078 simba_ml-1.0.0rc7/simba_ml/example_problems/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/example_problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/example_problems/constant_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/example_problems/salt_and_brine_tanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/example_problems/sir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/example_problems/sird.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/example_problems/trigonometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/logging/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/logging/wandb_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/config/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/config/steady_state_data_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/data_loader/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/data_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/data_loader/dataset_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/data_loader/splits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/mixed_data_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/mixed_data_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/mixed_data_pipeline/data_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/synthetic_data_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/synthetic_data_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/synthetic_data_pipeline/data_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/time_series_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/transfer_learning_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/transfer_learning_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/transfer_learning_pipeline/data_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/splits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/window_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/metrics/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.560078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/average_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.564078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/keras/dense_neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/keras/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/last_value_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.564078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.564078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/transfer_learning_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/transfer_learning_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.564078 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.564078 simba_ml-1.0.0rc7/simba_ml/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.564078 simba_ml-1.0.0rc7/simba_ml/simulation/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/constraints/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/constraints/keep_species_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/constraints/species_value_in_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/constraints/species_value_truncator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.564078 simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/derivative_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.564078 simba_ml-1.0.0rc7/simba_ml/simulation/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/distributions/beta_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/distributions/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/distributions/continuous_uniform_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/distributions/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/distributions/lognormal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/distributions/normal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/distributions/vector_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.568078 simba_ml-1.0.0rc7/simba_ml/simulation/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/generators/generator_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/generators/pertubation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/generators/steady_state_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/generators/time_points_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/generators/time_series_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.568078 simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.568078 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/additive_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/adjusting_mean_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/column_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/elastic_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/multi_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/multiplicative_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/no_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/noisers/sequential_noiser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.568078 simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/constant_suffix_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/interval_sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/no_sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/random_sample_sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/sequential_sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/species.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.568078 simba_ml-1.0.0rc7/simba_ml/simulation/system_model/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/system_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/system_model/system_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/simba_ml/simulation/system_model/system_model_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:32:34.556078 simba_ml-1.0.0rc7/simba_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-06 08:32:34.000000 simba_ml-1.0.0rc7/simba_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-06 08:32:34.000000 simba_ml-1.0.0rc7/simba_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:32:34.000000 simba_ml-1.0.0rc7/simba_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 08:32:34.000000 simba_ml-1.0.0rc7/simba_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 08:32:34.000000 simba_ml-1.0.0rc7/simba_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 08:32:34.000000 simba_ml-1.0.0rc7/simba_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-06 08:28:49.000000 simba_ml-1.0.0rc7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.634576 simba_ml-1.0.0rc8/simba_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-08 13:17:19.634576 simba_ml-1.0.0rc8/simba_ml/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.618576 simba_ml-1.0.0rc8/simba_ml/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/generate_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.618576 simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/problem_viewer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/run_problem_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/start_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/example_problems/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/constant_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/salt_and_brine_tanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/sir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/sird.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/trigonometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/logging/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/logging/wandb_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/config/steady_state_data_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/dataset_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/splits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/data_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/data_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/time_series_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/transfer_learning_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/transfer_learning_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/transfer_learning_pipeline/data_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/splits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/window_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/average_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/dense_neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/last_value_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/transfer_learning_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/transfer_learning_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/keep_species_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/species_value_in_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/species_value_truncator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/derivative_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/beta_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/continuous_uniform_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/lognormal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/normal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/vector_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/generator_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/pertubation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/steady_state_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/time_points_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/time_series_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/additive_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/adjusting_mean_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/column_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/elastic_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/multi_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/multiplicative_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/no_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/sequential_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/random_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/constant_suffix_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/interval_sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/no_sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/random_sample_sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/sequential_sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/species.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/system_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/system_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/system_model/system_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/system_model/system_model_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.618576 simba_ml-1.0.0rc8/simba_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/versioneer.py
```

### Comparing `simba_ml-1.0.0rc7/PKG-INFO` & `simba_ml-1.0.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simba_ml
-Version: 1.0.0rc7
+Version: 1.0.0rc8
 Summary: Simulation-Based Machine Learning
 Home-page: UNKNOWN
 Author: Maximilian Kleissl, Björn Heyder, Julian Zabbarov, Lukas Drews
 Author-email: maximilian.kleissl@student.hpi.de,bjoern.heyder@student.hpi.de,julian.zabbarov@student.hpi.de,lukas.drews@student.hpi.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/DILiS-lab/SimbaML/issues
 Project-URL: Source Code, https://github.com/DILiS-lab/SimbaML
```

### Comparing `simba_ml-1.0.0rc7/README.md` & `simba_ml-1.0.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/setup.cfg` & `simba_ml-1.0.0rc8/setup.cfg`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/setup.py` & `simba_ml-1.0.0rc8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     version=VERSION,
     cmdclass=versioneer.get_cmdclass(),
     author="Maximilian Kleissl, Björn Heyder, Julian Zabbarov, Lukas Drews",
     author_email="maximilian.kleissl@student.hpi.de,bjoern.heyder@student.hpi.de,julian.zabbarov@student.hpi.de,lukas.drews@student.hpi.de",
     project_urls={
         "Bug Tracker": "https://github.com/DILiS-lab/SimbaML/issues",
         "Source Code": "https://github.com/DILiS-lab/SimbaML",
-        "Documentation": "https://simbaml.readthedocs.io"
+        "Documentation": "https://simbaml.readthedocs.io",
     },
     description=DESCRIPTION,
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         "streamlit",
@@ -47,9 +47,9 @@
     ],
     classifiers=[],
     entry_points={
         "console_scripts": [
             "simba_ml = simba_ml.cli.__main__:main",
         ],
     },
-    license_files=("LICENSE.txt",)
+    license_files=("LICENSE.txt",),
 )
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/cli/generate_data.py` & `simba_ml-1.0.0rc8/simba_ml/cli/generate_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import importlib
 import os
 import sys
 
 import click
 
 from simba_ml.simulation import generators
+from simba_ml.simulation import random_generator
 
 
 GENERATORS: dict[str, type[generators.GeneratorInterface]] = {
     "TimeSeriesGenerator": generators.TimeSeriesGenerator,
     "SteadyStateGenerator": generators.SteadyStateGenerator,
 }
 
@@ -42,19 +43,30 @@
 @click.option(
     "--output-dir",
     default="./data/",
     type=str,
     required=True,
     help="Path to the output directory.",
 )
-def generate_data(generator: str, config_module: str, n: int, output_dir: str) -> None:
+@click.option(
+    "--seed",
+    required=False,
+    default=0,
+    type=int,
+    help="The random seed for the simulation part.",
+)
+def generate_data(
+    generator: str, config_module: str, n: int, output_dir: str, seed: int
+) -> None:
     """Command for generating data.
 
     Args:
         generator: Type of generator
         config_module: Path to the config file, that contains a System Model called sm.
         n: Number of samples to generate.
         output_dir: Path to the output directory.
+        seed: The random seed
     """
     sys.path.append(os.getcwd())
+    random_generator.set_seed(seed)
     sm = importlib.import_module(__normalize_module_name(config_module)).sm
     GENERATORS[generator](sm).generate_csvs(n, output_dir)
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/cli/problem_viewer/problem_viewer.py` & `simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/problem_viewer.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/cli/problem_viewer/run_problem_viewer.py` & `simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/run_problem_viewer.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/cli/start_prediction.py` & `simba_ml-1.0.0rc8/simba_ml/cli/start_prediction.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/error_handler.py` & `simba_ml-1.0.0rc8/simba_ml/error_handler.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/example_problems/constant_function.py` & `simba_ml-1.0.0rc8/simba_ml/example_problems/constant_function.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/example_problems/salt_and_brine_tanks.py` & `simba_ml-1.0.0rc8/simba_ml/example_problems/salt_and_brine_tanks.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/example_problems/sir.py` & `simba_ml-1.0.0rc8/simba_ml/example_problems/sir.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/example_problems/sird.py` & `simba_ml-1.0.0rc8/simba_ml/example_problems/sird.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/example_problems/trigonometry.py` & `simba_ml-1.0.0rc8/simba_ml/example_problems/trigonometry.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/export.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/export.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/logging/wandb_logger.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/logging/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/normalizer.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/normalizer.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/plugin_loader.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/preprocessing.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/preprocessing.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/data_loader/dataset_generator.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/steady_state/data_loader/splits.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/splits.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/mixed_data_pipeline/data_config.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/data_config.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/synthetic_data_pipeline/data_config.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/data_config.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/splits.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/splits.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/data_loader/window_generator.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/window_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/metrics/factory.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/factory.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/metrics/metrics.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/average_predictor.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/average_predictor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/factory.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/factory.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/keras/__init__.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/keras/dense_neural_network.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/dense_neural_network.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/keras/keras_model.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/keras_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,14 @@
     def set_seed(self, seed: int) -> None:
         """Sets the seed for the model.
 
         Args:
             seed: seed to set.
         """
         tf.random.set_seed(seed)
-        np.random.seed(seed)
 
     def train(self, train: list[pd.DataFrame]) -> None:
         """Trains the model with the given data.
 
         Args:
             train: training data.
         """
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/last_value_predictor.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/last_value_predictor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/model.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/pytorch_lightning/__init__.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,14 @@
     def set_seed(self, seed: int) -> None:
         """Sets the seed for the model.
 
         Args:
             seed: seed to set.
         """
         torch.manual_seed(seed)
-        np.random.seed(seed)
 
     def train(self, train: list[pd.DataFrame]) -> None:
         """Trains the model with the given data.
 
         Args:
             train: training data.
         """
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/__init__.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/transfer_learning_factory.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/transfer_learning_factory.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/models/transfer_learning_model.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     config = dacite.from_dict(
         data_class=pipeline_config.PipelineConfig,
         data=config_json,
         config=dacite.Config(strict=True),
     )
 
     # set seed
-    np.random.seed(config.seed)
     random.seed(config.seed)
 
     # set up wandb
     wandb_logger = wandb.WandbLogger(config.logging)
     wandb_logger.login()
 
     # instantiate models
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
     config = dacite.from_dict(
         data_class=pipeline_config.PipelineConfig,
         data=config_json,
         config=dacite.Config(strict=True),
     )
 
     # set seed
-    np.random.seed(config.seed)
     random.seed(config.seed)
 
     # set up wandb
     wandb_logger = wandb.WandbLogger(config.logging)
     wandb_logger.login()
 
     # instantiate models
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py` & `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
     config = dacite.from_dict(
         data_class=transfer_learning_pipeline.PipelineConfig,
         data=config_json,
         config=dacite.Config(strict=True),
     )
 
     # set seed
-    np.random.seed(config.seed)
     random.seed(config.seed)
 
     # set up wandb
     wandb_logger = wandb.WandbLogger(config.logging)
     wandb_logger.login()
 
     # instantiate models
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/constraints/__init__.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/constraints/constraint.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/constraints/keep_species_sum.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/constraints/keep_species_sum.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/constraints/species_value_in_range.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/constraints/species_value_in_range.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/constraints/species_value_truncator.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/constraints/species_value_truncator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/__init__.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/derivative_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/derivative_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/distributions/__init__.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/distributions/beta_distribution.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/beta_distribution.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Defines Beta Distribution."""
 
 import typing
 
-import numpy as np
 from scipy import stats
 
 from simba_ml import error_handler
 
+from simba_ml.simulation import random_generator
+
 
 class BetaDistribution:
     """An object which samples values from a beta distributions.
 
     Attributes:
         alpha: Alpha parameter of the distributions.
         beta: Beta parameter of the distributions.
@@ -38,27 +39,31 @@
         error_handler.confirm_number_is_greater_than_0(self.alpha, "alpha")
         error_handler.confirm_number_is_greater_than_0(self.beta, "beta")
 
     def get_random_values(self, n: int) -> list[float]:
         """Samples an array of values with the given shape from the distributions.
 
         Args:
-            n: The number of values.
+            n: The number ofnp.random values.
 
         Returns:
             an array of randomly sampled values.
 
         """
-        return np.random.default_rng().beta(self.alpha, self.beta, n).tolist()
+        return random_generator.get_rng().beta(self.alpha, self.beta, n).tolist()
 
     def get_samples_from_hypercube(self, n: int) -> list[float]:
         """Samples n values from a hypercube.
 
         Args:
             n: the number of samples.
 
         Returns:
             Samples of the distribution, sampled from a hypercube.
         """
         rv = stats.beta(self.alpha, self.beta)
-        p = [np.random.uniform(low=i / n, high=(i + 1) / n) for i in range(n)]
+        p = [
+            random_generator.get_rng().uniform(low=i / n, high=(i + 1) / n)
+            for i in range(n)
+        ]
+        rv.random_state = random_generator.get_rng()
         return rv.ppf(p)
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/distributions/constant.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/constant.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/distributions/continuous_uniform_distribution.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/continuous_uniform_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Defines Continuous Uniform Distribution."""
 
 import typing
 
 import numpy as np
 
 from simba_ml import error_handler
+from simba_ml.simulation import random_generator
 
 
 class ContinuousUniformDistribution:
     """An object which samples values from a continuous uniform distributions.
 
     Attributes:
         min_value: the minimal value of the distributions.
@@ -39,29 +40,29 @@
         Args:
             n: The number of values.
 
         Returns:
             np.ndarray[float]
         """
         return (
-            np.random.default_rng()
+            random_generator.get_rng()
             .uniform(self.min_value, self.max_value, size=n)
             .tolist()
         )
 
     def get_samples_from_hypercube(self, n: int) -> list[float]:
         """Samples n values from a hypercube.
 
         Args:
             n: the number of samples.
 
         Returns:
             Samples of the distributions, sampled from a hypercube.
         """
-        rng = np.random.default_rng()
+        rng = random_generator.get_rng()
         res = [
             rng.uniform(min_value, min_value + (self.max_value - self.min_value) / n)
             for min_value in np.arange(
                 self.min_value, self.max_value, (self.max_value - self.min_value) / n
             )
         ]
         rng.shuffle(res)
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/distributions/distribution.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/distributions/helper_functions.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/helper_functions.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/distributions/lognormal_distribution.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/lognormal_distribution.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Defines Lognormal Distribution."""
 
 import typing
 
-import numpy as np
 from scipy import stats
 
 from simba_ml import error_handler
+from simba_ml.simulation import random_generator
 
 
 class LogNormalDistribution:
     """An object which samples values from a log-normal distributions.
 
     Attributes:
         mu: Mean ("centre") of the distributions.
@@ -44,20 +44,25 @@
 
         Args:
             n: The number of values.
 
         Returns:
             np.ndarray[float]
         """
-        return np.random.default_rng().lognormal(self.mu, self.sigma, size=n).tolist()
+        return (
+            random_generator.get_rng().lognormal(self.mu, self.sigma, size=n).tolist()
+        )
 
     def get_samples_from_hypercube(self, n: int) -> list[float]:
         """Samples n values from a hypercube.
 
         Args:
             n: the number of samples.
 
         Returns:
             Samples of the distribution, sampled from a hypercube.
         """
-        p = [np.random.uniform(low=i / n, high=(i + 1) / n) for i in range(n)]
+        p = [
+            random_generator.get_rng().uniform(low=i / n, high=(i + 1) / n)
+            for i in range(n)
+        ]
         return stats.lognorm.ppf(p, 1, self.mu, self.sigma)
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/distributions/normal_distribution.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/normal_distribution.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Defines the Normal Distribution."""
 
 import typing
 
-import numpy as np
 from scipy import stats
 
 from simba_ml import error_handler
+from simba_ml.simulation import random_generator
 
 
 class NormalDistribution:
     """An object which samples values from a normal distributions.
 
     Attributes:
         mu: Mean ("centre") of the distributions.
@@ -43,21 +43,25 @@
 
         Args:
             n: The number of values.
 
         Returns:
             np.ndarray[float]
         """
-        return np.random.default_rng().normal(self.mu, self.sigma, size=n).tolist()
+        return random_generator.get_rng().normal(self.mu, self.sigma, size=n).tolist()
 
     def get_samples_from_hypercube(self, n: int) -> list[float]:
         """Samples n values from a hypercube.
 
         Args:
             n: the number of samples.
 
         Returns:
             Samples of the distribution, sampled from a hypercube.
         """
         rv = stats.norm(self.mu, self.sigma)
-        p = [np.random.uniform(low=i / n, high=(i + 1) / n) for i in range(n)]
+        p = [
+            random_generator.get_rng().uniform(low=i / n, high=(i + 1) / n)
+            for i in range(n)
+        ]
+        rv.random_state = random_generator.get_rng()
         return rv.ppf(p)
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/distributions/vector_distribution.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/vector_distribution.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Defines Vector Distribution."""
 
 import typing
 
-import numpy as np
-
 from simba_ml import error_handler
+from simba_ml.simulation import random_generator
 
 
 class VectorDistribution:
     """An object which samples values from a list of numbers.
 
     Attributes:
         values: A list containing values.
@@ -35,24 +34,24 @@
 
         Args:
             n: The number of values.
 
         Returns:
             np.ndarray[float]
         """
-        return np.random.default_rng().choice(self.values, size=n).tolist()
+        return random_generator.get_rng().choice(self.values, size=n).tolist()
 
     def get_samples_from_hypercube(self, n: int) -> list[float]:
         """Samples n values from a hypercube.
 
         Args:
             n: the number of samples.
 
         Returns:
             Samples of the distributions, sampled from a hypercube.
         """
-        rng = np.random.default_rng()
+        rng = random_generator.get_rng()
         res = (
             self.values * (n // len(self.values)) + self.values[: n % len(self.values)]
         )
         rng.shuffle(res)
         return res
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/generators/__init__.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/generators/generator_interface.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/generators/generator_interface.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/generators/pertubation_generator.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/generators/pertubation_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/generators/steady_state_generator.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/generators/steady_state_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Provides the generator for `PredictionTask` signals."""
 import os
 import typing
-
 import math
-import numpy as np
 
 import pandas as pd
 
 from simba_ml.simulation.system_model import system_model_interface
+from simba_ml.simulation import random_generator
 
 
 class SteadyStateGenerator:
     """Defines how to generate signals from a PredictionTask."""
 
     def __init__(self, sm: system_model_interface.SystemModelInterface):
         """Initializes the `PredictionTaskBuilder`.
@@ -100,15 +99,15 @@
         if not self.__check_if_signal_has_steady_state(clean_signal):
             raise ValueError("Signal has no steady state.")
 
         pertubation_std = 0.01
         for key in start_values["specieses"]:
             start_values["specieses"][key][sample_id] = clean_signal[key].iloc[
                 -1
-            ] * np.random.normal(1, pertubation_std)
+            ] * random_generator.get_rng().normal(1, pertubation_std)
 
         pertubated_signal = self.sm.get_clean_signal(
             start_values=start_values, sample_id=sample_id
         )
         if self.__check_if_signal_has_steady_state(pertubated_signal):
             self.sm.apply_noisifier(clean_signal)
             return clean_signal.iloc[-1]
```

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/generators/time_points_generator.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/generators/time_points_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/generators/time_series_generator.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/generators/time_series_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/__init__.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/noisers/__init__.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/noisers/additive_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/additive_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/noisers/adjusting_mean_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/adjusting_mean_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/noisers/column_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/column_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/noisers/elastic_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/elastic_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/noisers/multi_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/multi_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/noisers/multiplicative_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/multiplicative_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/noisers/sequential_noiser.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/sequential_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/__init__.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/constant_suffix_remover.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/constant_suffix_remover.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/interval_sparsifier.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/interval_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/no_sparsifier.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/no_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/random_sample_sparsifier.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/random_sample_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/sparsifier/sequential_sparsifier.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/sequential_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/species.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/species.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/system_model/system_model.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/system_model/system_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml/simulation/system_model/system_model_interface.py` & `simba_ml-1.0.0rc8/simba_ml/simulation/system_model/system_model_interface.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc7/simba_ml.egg-info/PKG-INFO` & `simba_ml-1.0.0rc8/simba_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simba-ml
-Version: 1.0.0rc7
+Version: 1.0.0rc8
 Summary: Simulation-Based Machine Learning
 Home-page: UNKNOWN
 Author: Maximilian Kleissl, Björn Heyder, Julian Zabbarov, Lukas Drews
 Author-email: maximilian.kleissl@student.hpi.de,bjoern.heyder@student.hpi.de,julian.zabbarov@student.hpi.de,lukas.drews@student.hpi.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/DILiS-lab/SimbaML/issues
 Project-URL: Source Code, https://github.com/DILiS-lab/SimbaML
```

### Comparing `simba_ml-1.0.0rc7/simba_ml.egg-info/SOURCES.txt` & `simba_ml-1.0.0rc8/simba_ml.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py
 simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py
 simba_ml/prediction/time_series/pipelines/__init__.py
 simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py
 simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py
 simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py
 simba_ml/simulation/__init__.py
+simba_ml/simulation/random_generator.py
 simba_ml/simulation/species.py
 simba_ml/simulation/constraints/__init__.py
 simba_ml/simulation/constraints/constraint.py
 simba_ml/simulation/constraints/keep_species_sum.py
 simba_ml/simulation/constraints/species_value_in_range.py
 simba_ml/simulation/constraints/species_value_truncator.py
 simba_ml/simulation/derivative_noiser/__init__.py
```

### Comparing `simba_ml-1.0.0rc7/versioneer.py` & `simba_ml-1.0.0rc8/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # Version: 0.28
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -344,33 +343,37 @@
     versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
         versioneer_py = os.path.join(root, "versioneer.py")
     if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
-        err = ("Versioneer was unable to run the project root directory. "
-               "Versioneer requires setup.py to be executed from "
-               "its immediate directory (like 'python setup.py COMMAND'), "
-               "or in a way that lets it use sys.argv[0] to find the root "
-               "(like 'python path/to/setup.py COMMAND').")
+        err = (
+            "Versioneer was unable to run the project root directory. "
+            "Versioneer requires setup.py to be executed from "
+            "its immediate directory (like 'python setup.py COMMAND'), "
+            "or in a way that lets it use sys.argv[0] to find the root "
+            "(like 'python path/to/setup.py COMMAND')."
+        )
         raise VersioneerBadRootError(err)
     try:
         # Certain runtime workflows (setup.py install/develop in a setuptools
         # tree) execute all dependencies in a single python process, so
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
         if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
-            print("Warning: build in %s is using versioneer.py from %s"
-                  % (os.path.dirname(my_path), versioneer_py))
+            print(
+                "Warning: build in %s is using versioneer.py from %s"
+                % (os.path.dirname(my_path), versioneer_py)
+            )
     except NameError:
         pass
     return root
 
 
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
@@ -380,29 +383,29 @@
     # the top of versioneer.py for instructions on writing your setup.cfg .
     root = Path(root)
     pyproject_toml = root / "pyproject.toml"
     setup_cfg = root / "setup.cfg"
     section = None
     if pyproject_toml.exists() and have_tomllib:
         try:
-            with open(pyproject_toml, 'rb') as fobj:
+            with open(pyproject_toml, "rb") as fobj:
                 pp = tomllib.load(fobj)
-            section = pp['tool']['versioneer']
+            section = pp["tool"]["versioneer"]
         except (tomllib.TOMLDecodeError, KeyError):
             pass
     if not section:
         parser = configparser.ConfigParser()
         with open(setup_cfg) as cfg_file:
             parser.read_file(cfg_file)
         parser.get("versioneer", "VCS")  # raise error if missing
 
         section = parser["versioneer"]
 
     cfg = VersioneerConfig()
-    cfg.VCS = section['VCS']
+    cfg.VCS = section["VCS"]
     cfg.style = section.get("style", "")
     cfg.versionfile_source = section.get("versionfile_source")
     cfg.versionfile_build = section.get("versionfile_build")
     cfg.tag_prefix = section.get("tag_prefix")
     if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
@@ -417,23 +420,24 @@
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY: Dict[str, str] = {}
 HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
 def register_vcs_handler(vcs, method):  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
+
     def decorate(f):
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
+
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
 
     popen_kwargs = {}
     if sys.platform == "win32":
         # This hides the console window if pythonw.exe is used
@@ -441,18 +445,22 @@
         startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
         popen_kwargs["startupinfo"] = startupinfo
 
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
-            process = subprocess.Popen([command] + args, cwd=cwd, env=env,
-                                       stdout=subprocess.PIPE,
-                                       stderr=(subprocess.PIPE if hide_stderr
-                                               else None), **popen_kwargs)
+            process = subprocess.Popen(
+                [command] + args,
+                cwd=cwd,
+                env=env,
+                stdout=subprocess.PIPE,
+                stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
+            )
             break
         except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
@@ -467,15 +475,17 @@
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-LONG_VERSION_PY['git'] = r'''
+LONG_VERSION_PY[
+    "git"
+] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain.
@@ -1183,49 +1193,56 @@
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
     refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG):] for r in refs if r.startswith(TAG)}
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r'\d', r)}
+        tags = {r for r in refs if re.search(r"\d", r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
-            r = ref[len(tag_prefix):]
+            r = ref[len(tag_prefix) :]
             # Filter out refs that exactly match prefix or that don't start
             # with a number once the prefix is stripped (mostly a concern
             # when prefix is '')
-            if not re.match(r'\d', r):
+            if not re.match(r"\d", r):
                 continue
             if verbose:
                 print("picking %s" % r)
-            return {"version": r,
-                    "full-revisionid": keywords["full"].strip(),
-                    "dirty": False, "error": None,
-                    "date": date}
+            return {
+                "version": r,
+                "full-revisionid": keywords["full"].strip(),
+                "dirty": False,
+                "error": None,
+                "date": date,
+            }
     # no suitable tags, so version is "0+unknown", but full hex is still there
     if verbose:
         print("no suitable tags, using unknown + full revision id")
-    return {"version": "0+unknown",
-            "full-revisionid": keywords["full"].strip(),
-            "dirty": False, "error": "no suitable tags", "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": keywords["full"].strip(),
+        "dirty": False,
+        "error": "no suitable tags",
+        "date": None,
+    }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
 def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
@@ -1239,43 +1256,50 @@
     # GIT_DIR can interfere with correct operation of Versioneer.
     # It may be intended to be passed to the Versioneer-versioned project,
     # but that should not change where we get our version from.
     env = os.environ.copy()
     env.pop("GIT_DIR", None)
     runner = functools.partial(runner, env=env)
 
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=not verbose)
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, [
-        "describe", "--tags", "--dirty", "--always", "--long",
-        "--match", f"{tag_prefix}[[:digit:]]*"
-    ], cwd=root)
+    describe_out, rc = runner(
+        GITS,
+        [
+            "describe",
+            "--tags",
+            "--dirty",
+            "--always",
+            "--long",
+            "--match",
+            f"{tag_prefix}[[:digit:]]*",
+        ],
+        cwd=root,
+    )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
     pieces = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
-    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
-                             cwd=root)
+    branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
         raise NotThisMethod("'git rev-parse --abbrev-ref' returned error")
     branch_name = branch_name.strip()
 
     if branch_name == "HEAD":
         # If we aren't exactly on a branch, pick a branch which represents
@@ -1307,37 +1331,38 @@
     # TAG might have hyphens.
     git_describe = describe_out
 
     # look for -dirty suffix
     dirty = git_describe.endswith("-dirty")
     pieces["dirty"] = dirty
     if dirty:
-        git_describe = git_describe[:git_describe.rindex("-dirty")]
+        git_describe = git_describe[: git_describe.rindex("-dirty")]
 
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
-        mo = re.search(r'^(.+)-(\d+)-g([0-9a-f]+)$', git_describe)
+        mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparsable. Maybe git-describe is misbehaving?
-            pieces["error"] = ("unable to parse git-describe output: '%s'"
-                               % describe_out)
+            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = ("tag '%s' doesn't start with prefix '%s'"
-                               % (full_tag, tag_prefix))
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
+                full_tag,
+                tag_prefix,
+            )
             return pieces
-        pieces["closest-tag"] = full_tag[len(tag_prefix):]
+        pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
@@ -1403,23 +1428,29 @@
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
 
     for _ in range(3):
         dirname = os.path.basename(root)
         if dirname.startswith(parentdir_prefix):
-            return {"version": dirname[len(parentdir_prefix):],
-                    "full-revisionid": None,
-                    "dirty": False, "error": None, "date": None}
+            return {
+                "version": dirname[len(parentdir_prefix) :],
+                "full-revisionid": None,
+                "dirty": False,
+                "error": None,
+                "date": None,
+            }
         rootdirs.append(root)
         root = os.path.dirname(root)  # up a level
 
     if verbose:
-        print("Tried directories %s but none started with prefix %s" %
-              (str(rootdirs), parentdir_prefix))
+        print(
+            "Tried directories %s but none started with prefix %s"
+            % (str(rootdirs), parentdir_prefix)
+        )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
 # This file was generated by 'versioneer.py' (0.28) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
@@ -1440,29 +1471,30 @@
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except OSError:
         raise NotThisMethod("unable to read _version.py")
-    mo = re.search(r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-                   contents, re.M | re.S)
+    mo = re.search(
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+    )
     if not mo:
-        mo = re.search(r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-                       contents, re.M | re.S)
+        mo = re.search(
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
+        )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
-    contents = json.dumps(versions, sort_keys=True,
-                          indent=1, separators=(",", ": "))
+    contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
@@ -1486,16 +1518,15 @@
         if pieces["distance"] or pieces["dirty"]:
             rendered += plus_or_dot(pieces)
             rendered += "%d.g%s" % (pieces["distance"], pieces["short"])
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
-        rendered = "0+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def render_pep440_branch(pieces):
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
@@ -1516,16 +1547,15 @@
             if pieces["dirty"]:
                 rendered += ".dirty"
     else:
         # exception #1
         rendered = "0"
         if pieces["branch"] != "master":
             rendered += ".dev0"
-        rendered += "+untagged.%d.g%s" % (pieces["distance"],
-                                          pieces["short"])
+        rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
 def pep440_split_post(ver):
     """Split pep440 version string at the post-release segment.
@@ -1678,19 +1708,21 @@
         rendered += "-dirty"
     return rendered
 
 
 def render(pieces, style):
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
-        return {"version": "unknown",
-                "full-revisionid": pieces.get("long"),
-                "dirty": None,
-                "error": pieces["error"],
-                "date": None}
+        return {
+            "version": "unknown",
+            "full-revisionid": pieces.get("long"),
+            "dirty": None,
+            "error": pieces["error"],
+            "date": None,
+        }
 
     if not style or style == "default":
         style = "pep440"  # the default
 
     if style == "pep440":
         rendered = render_pep440(pieces)
     elif style == "pep440-branch":
@@ -1706,17 +1738,21 @@
     elif style == "git-describe":
         rendered = render_git_describe(pieces)
     elif style == "git-describe-long":
         rendered = render_git_describe_long(pieces)
     else:
         raise ValueError("unknown style '%s'" % style)
 
-    return {"version": rendered, "full-revisionid": pieces["long"],
-            "dirty": pieces["dirty"], "error": None,
-            "date": pieces.get("date")}
+    return {
+        "version": rendered,
+        "full-revisionid": pieces["long"],
+        "dirty": pieces["dirty"],
+        "error": None,
+        "date": pieces.get("date"),
+    }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
 def get_versions(verbose=False):
@@ -1731,16 +1767,17 @@
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
     verbose = verbose or cfg.verbose
-    assert cfg.versionfile_source is not None, \
-        "please set versioneer.versionfile_source"
+    assert (
+        cfg.versionfile_source is not None
+    ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
     # extract version from first of: _version.py, VCS command (e.g. 'git
     # describe'), parentdir. This is meant to work for developers using a
     # source checkout, for users of a tarball created by 'setup.py sdist',
@@ -1786,17 +1823,21 @@
             return ver
     except NotThisMethod:
         pass
 
     if verbose:
         print("unable to compute version")
 
-    return {"version": "0+unknown", "full-revisionid": None,
-            "dirty": None, "error": "unable to compute version",
-            "date": None}
+    return {
+        "version": "0+unknown",
+        "full-revisionid": None,
+        "dirty": None,
+        "error": "unable to compute version",
+        "date": None,
+    }
 
 
 def get_version():
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
@@ -1841,14 +1882,15 @@
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
+
     cmds["version"] = cmd_version
 
     # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
@@ -1862,16 +1904,16 @@
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
     # pip install -e . and setuptool/editable_wheel will invoke build_py
     # but the build_py command is not expected to copy any files.
 
     # we override different "build_py" commands for both environments
-    if 'build_py' in cmds:
-        _build_py = cmds['build_py']
+    if "build_py" in cmds:
+        _build_py = cmds["build_py"]
     else:
         from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
@@ -1880,22 +1922,22 @@
             if getattr(self, "editable_mode", False):
                 # During editable installs `.py` and data files are
                 # not copied to build_lib
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
-                target_versionfile = os.path.join(self.build_lib,
-                                                  cfg.versionfile_build)
+                target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
+
     cmds["build_py"] = cmd_build_py
 
-    if 'build_ext' in cmds:
-        _build_ext = cmds['build_ext']
+    if "build_ext" in cmds:
+        _build_ext = cmds["build_ext"]
     else:
         from setuptools.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
         def run(self):
             root = get_root()
             cfg = get_config_from_root(root)
@@ -1907,27 +1949,30 @@
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if not cfg.versionfile_build:
                 return
-            target_versionfile = os.path.join(self.build_lib,
-                                              cfg.versionfile_build)
+            target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
             if not os.path.exists(target_versionfile):
-                print(f"Warning: {target_versionfile} does not exist, skipping "
-                      "version update. This can happen if you are running build_ext "
-                      "without first running build_py.")
+                print(
+                    f"Warning: {target_versionfile} does not exist, skipping "
+                    "version update. This can happen if you are running build_ext "
+                    "without first running build_py."
+                )
                 return
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
+
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
         from cx_Freeze.dist import build_exe as _build_exe
+
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
@@ -1940,25 +1985,29 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _build_exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
-    if 'py2exe' in sys.modules:  # py2exe enabled?
+    if "py2exe" in sys.modules:  # py2exe enabled?
         try:
             from py2exe.setuptools_buildexe import py2exe as _py2exe
         except ImportError:
             from py2exe.distutils_buildexe import py2exe as _py2exe
 
         class cmd_py2exe(_py2exe):
             def run(self):
@@ -1969,63 +2018,70 @@
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
                 _py2exe.run(self)
                 os.unlink(target_versionfile)
                 with open(cfg.versionfile_source, "w") as f:
                     LONG = LONG_VERSION_PY[cfg.VCS]
-                    f.write(LONG %
-                            {"DOLLAR": "$",
-                             "STYLE": cfg.style,
-                             "TAG_PREFIX": cfg.tag_prefix,
-                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                             })
+                    f.write(
+                        LONG
+                        % {
+                            "DOLLAR": "$",
+                            "STYLE": cfg.style,
+                            "TAG_PREFIX": cfg.tag_prefix,
+                            "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                            "VERSIONFILE_SOURCE": cfg.versionfile_source,
+                        }
+                    )
+
         cmds["py2exe"] = cmd_py2exe
 
     # sdist farms its file list building out to egg_info
-    if 'egg_info' in cmds:
-        _egg_info = cmds['egg_info']
+    if "egg_info" in cmds:
+        _egg_info = cmds["egg_info"]
     else:
         from setuptools.command.egg_info import egg_info as _egg_info
 
     class cmd_egg_info(_egg_info):
         def find_sources(self):
             # egg_info.find_sources builds the manifest list and writes it
             # in one shot
             super().find_sources()
 
             # Modify the filelist and normalize it
             root = get_root()
             cfg = get_config_from_root(root)
-            self.filelist.append('versioneer.py')
+            self.filelist.append("versioneer.py")
             if cfg.versionfile_source:
                 # There are rare cases where versionfile_source might not be
                 # included by default, so we must be explicit
                 self.filelist.append(cfg.versionfile_source)
             self.filelist.sort()
             self.filelist.remove_duplicates()
 
             # The write method is hidden in the manifest_maker instance that
             # generated the filelist and was thrown away
             # We will instead replicate their final normalization (to unicode,
             # and POSIX-style paths)
             from setuptools import unicode_utils
-            normalized = [unicode_utils.filesys_decode(f).replace(os.sep, '/')
-                          for f in self.filelist.files]
 
-            manifest_filename = os.path.join(self.egg_info, 'SOURCES.txt')
-            with open(manifest_filename, 'w') as fobj:
-                fobj.write('\n'.join(normalized))
+            normalized = [
+                unicode_utils.filesys_decode(f).replace(os.sep, "/")
+                for f in self.filelist.files
+            ]
+
+            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
+            with open(manifest_filename, "w") as fobj:
+                fobj.write("\n".join(normalized))
 
-    cmds['egg_info'] = cmd_egg_info
+    cmds["egg_info"] = cmd_egg_info
 
     # we override different "sdist" commands for both environments
-    if 'sdist' in cmds:
-        _sdist = cmds['sdist']
+    if "sdist" in cmds:
+        _sdist = cmds["sdist"]
     else:
         from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
         def run(self):
             versions = get_versions()
             self._versioneer_generated_versions = versions
@@ -2039,16 +2095,18 @@
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
             print("UPDATING %s" % target_versionfile)
-            write_to_version_file(target_versionfile,
-                                  self._versioneer_generated_versions)
+            write_to_version_file(
+                target_versionfile, self._versioneer_generated_versions
+            )
+
     cmds["sdist"] = cmd_sdist
 
     return cmds
 
 
 CONFIG_ERROR = """
 setup.cfg is missing the necessary Versioneer configuration. You need
@@ -2100,36 +2158,37 @@
 
 
 def do_setup():
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (OSError, configparser.NoSectionError,
-            configparser.NoOptionError) as e:
+    except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
         if isinstance(e, (OSError, configparser.NoSectionError)):
-            print("Adding sample versioneer config to setup.cfg",
-                  file=sys.stderr)
+            print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
     print(" creating %s" % cfg.versionfile_source)
     with open(cfg.versionfile_source, "w") as f:
         LONG = LONG_VERSION_PY[cfg.VCS]
-        f.write(LONG % {"DOLLAR": "$",
-                        "STYLE": cfg.style,
-                        "TAG_PREFIX": cfg.tag_prefix,
-                        "PARENTDIR_PREFIX": cfg.parentdir_prefix,
-                        "VERSIONFILE_SOURCE": cfg.versionfile_source,
-                        })
+        f.write(
+            LONG
+            % {
+                "DOLLAR": "$",
+                "STYLE": cfg.style,
+                "TAG_PREFIX": cfg.tag_prefix,
+                "PARENTDIR_PREFIX": cfg.parentdir_prefix,
+                "VERSIONFILE_SOURCE": cfg.versionfile_source,
+            }
+        )
 
-    ipy = os.path.join(os.path.dirname(cfg.versionfile_source),
-                       "__init__.py")
+    ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
```

