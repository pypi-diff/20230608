# Comparing `tmp/boonamber-2.0.6.tar.gz` & `tmp/boonamber-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boonamber-2.0.6.tar", last modified: Fri May 26 04:10:57 2023, max compression
+gzip compressed data, was "boonamber-2.0.8.tar", last modified: Thu Jun  8 11:47:16 2023, max compression
```

## Comparing `boonamber-2.0.6.tar` & `boonamber-2.0.8.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:10:57.118345 boonamber-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 04:10:48.000000 boonamber-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-26 04:10:57.118345 boonamber-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-26 04:10:48.000000 boonamber-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:10:57.110345 boonamber-2.0.6/boonamber/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:10:57.110345 boonamber-2.0.6/boonamber/util/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/util/ambererror.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:10:57.110345 boonamber-2.0.6/boonamber/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    48323 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:10:57.110345 boonamber-2.0.6/boonamber/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22682 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/amber_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:10:57.110345 boonamber-2.0.6/boonamber/v2/api/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92075 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:10:57.118345 boonamber-2.0.6/boonamber/v2/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/amber_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/analytic_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/autotuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/feature_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/feature_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/feature_root_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/fusion_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/get_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/get_nano_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/get_pretrain_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/get_root_cause_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/get_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/get_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/get_version_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_amber_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_autotune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_buffer_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_nano.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_nano_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_nano_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_pattern_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_recent_ams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_recent_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_recent_floats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_recent_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_recent_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_recent_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_streaming_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/m_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/magic_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/mncp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/model_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/nano_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/percent_variation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_config_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_data_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_learning_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_learning_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_model_copy_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_oauth2_access_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_oauth2_access_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_oauth2_refresh_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_oauth2_refresh_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_pretrain_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/post_pretrain_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/pretrain_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/put_data_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/put_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/put_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/streaming_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/training_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/models/version_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-05-26 04:10:48.000000 boonamber-2.0.6/boonamber/v2/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:10:57.110345 boonamber-2.0.6/boonamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-26 04:10:57.000000 boonamber-2.0.6/boonamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-26 04:10:57.000000 boonamber-2.0.6/boonamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 04:10:57.000000 boonamber-2.0.6/boonamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 04:10:57.000000 boonamber-2.0.6/boonamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 04:10:57.000000 boonamber-2.0.6/boonamber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-26 04:10:48.000000 boonamber-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 04:10:57.118345 boonamber-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.619071 boonamber-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 11:47:05.000000 boonamber-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 11:47:16.619071 boonamber-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-08 11:47:05.000000 boonamber-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/util/ambererror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    48323 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22682 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/amber_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber/v2/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92075 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.619071 boonamber-2.0.8/boonamber/v2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/amber_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/analytic_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/autotuning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/feature_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/feature_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/feature_root_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/fusion_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_nano_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_pretrain_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_root_cause_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_amber_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_autotune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_buffer_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_nano.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_nano_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_nano_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_pattern_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_ams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_floats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_streaming_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/magic_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/mncp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/model_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/nano_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/percent_variation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_learning_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_learning_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_model_copy_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_oauth2_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_oauth2_access_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_oauth2_refresh_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_oauth2_refresh_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_pretrain_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_pretrain_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/pretrain_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/put_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/put_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/put_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/streaming_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/training_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/version_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 11:47:16.000000 boonamber-2.0.8/boonamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-08 11:47:16.000000 boonamber-2.0.8/boonamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:47:16.000000 boonamber-2.0.8/boonamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 11:47:16.000000 boonamber-2.0.8/boonamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 11:47:16.000000 boonamber-2.0.8/boonamber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-08 11:47:05.000000 boonamber-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:47:16.619071 boonamber-2.0.8/setup.cfg
```

### Comparing `boonamber-2.0.6/LICENSE` & `boonamber-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/PKG-INFO` & `boonamber-2.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boonamber
-Version: 2.0.6
+Version: 2.0.8
 Summary: An SDK for Boon Amber sensor analytics
 Author: BoonLogic
 Author-email: amber-support@boonlogic.com
 License: MIT
 Project-URL: repository, https://github.com/boonlogic/amber-python-sdk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boonamber-2.0.6/README.md` & `boonamber-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/__init__.py` & `boonamber-2.0.8/boonamber/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v1/__init__.py` & `boonamber-2.0.8/boonamber/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/__init__.py` & `boonamber-2.0.8/boonamber/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/amber_client.py` & `boonamber-2.0.8/boonamber/v2/amber_client.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/api/default_api.py` & `boonamber-2.0.8/boonamber/v2/api/default_api.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/api_client.py` & `boonamber-2.0.8/boonamber/v2/api_client.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/configuration.py` & `boonamber-2.0.8/boonamber/v2/configuration.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/__init__.py` & `boonamber-2.0.8/boonamber/v2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/amber_state.py` & `boonamber-2.0.8/boonamber/v2/models/amber_state.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/analytic_results.py` & `boonamber-2.0.8/boonamber/v2/models/analytic_results.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/autotuning.py` & `boonamber-2.0.8/boonamber/v2/models/autotuning.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/config_response.py` & `boonamber-2.0.8/boonamber/v2/models/config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/delete_model_response.py` & `boonamber-2.0.8/boonamber/v2/models/delete_model_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/error.py` & `boonamber-2.0.8/boonamber/v2/models/error.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/feature_config.py` & `boonamber-2.0.8/boonamber/v2/models/feature_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/feature_config_response.py` & `boonamber-2.0.8/boonamber/v2/models/feature_config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/feature_root_cause.py` & `boonamber-2.0.8/boonamber/v2/models/feature_root_cause.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/fusion_feature.py` & `boonamber-2.0.8/boonamber/v2/models/fusion_feature.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/get_models_response.py` & `boonamber-2.0.8/boonamber/v2/models/get_models_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/get_nano_status_response.py` & `boonamber-2.0.8/boonamber/v2/models/get_nano_status_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/get_pretrain_response.py` & `boonamber-2.0.8/boonamber/v2/models/get_pretrain_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/get_root_cause_response.py` & `boonamber-2.0.8/boonamber/v2/models/get_root_cause_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/get_status_response.py` & `boonamber-2.0.8/boonamber/v2/models/get_status_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/get_summary_response.py` & `boonamber-2.0.8/boonamber/v2/models/get_summary_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/get_version_response.py` & `boonamber-2.0.8/boonamber/v2/models/get_version_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_amber_status.py` & `boonamber-2.0.8/boonamber/v2/models/m_amber_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_autotune.py` & `boonamber-2.0.8/boonamber/v2/models/m_autotune.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_buffer_stats.py` & `boonamber-2.0.8/boonamber/v2/models/m_buffer_stats.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_nano.py` & `boonamber-2.0.8/boonamber/v2/models/m_nano.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_nano_backend.py` & `boonamber-2.0.8/boonamber/v2/models/m_nano_backend.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_nano_config.py` & `boonamber-2.0.8/boonamber/v2/models/m_nano_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_pattern_memory.py` & `boonamber-2.0.8/boonamber/v2/models/m_pattern_memory.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_recent_ams.py` & `boonamber-2.0.8/boonamber/v2/models/m_recent_ams.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_recent_analytics.py` & `boonamber-2.0.8/boonamber/v2/models/m_recent_analytics.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_recent_floats.py` & `boonamber-2.0.8/boonamber/v2/models/m_recent_floats.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_recent_ids.py` & `boonamber-2.0.8/boonamber/v2/models/m_recent_ids.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_recent_samples.py` & `boonamber-2.0.8/boonamber/v2/models/m_recent_samples.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_recent_times.py` & `boonamber-2.0.8/boonamber/v2/models/m_recent_times.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_streaming_parameters.py` & `boonamber-2.0.8/boonamber/v2/models/m_streaming_parameters.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/m_training.py` & `boonamber-2.0.8/boonamber/v2/models/m_training.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/magic_number.py` & `boonamber-2.0.8/boonamber/v2/models/magic_number.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/map.py` & `boonamber-2.0.8/boonamber/v2/models/map.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/mncp.py` & `boonamber-2.0.8/boonamber/v2/models/mncp.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/model.py` & `boonamber-2.0.8/boonamber/v2/models/model.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/model_status.py` & `boonamber-2.0.8/boonamber/v2/models/model_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/nano_status.py` & `boonamber-2.0.8/boonamber/v2/models/nano_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/percent_variation.py` & `boonamber-2.0.8/boonamber/v2/models/percent_variation.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_config_request.py` & `boonamber-2.0.8/boonamber/v2/models/post_config_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_config_response.py` & `boonamber-2.0.8/boonamber/v2/models/post_config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_data_request.py` & `boonamber-2.0.8/boonamber/v2/models/post_data_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_data_response.py` & `boonamber-2.0.8/boonamber/v2/models/post_data_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_learning_request.py` & `boonamber-2.0.8/boonamber/v2/models/post_learning_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_learning_response.py` & `boonamber-2.0.8/boonamber/v2/models/post_learning_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_model_copy_request.py` & `boonamber-2.0.8/boonamber/v2/models/post_model_copy_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_model_request.py` & `boonamber-2.0.8/boonamber/v2/models/post_model_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_model_response.py` & `boonamber-2.0.8/boonamber/v2/models/post_model_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_oauth2_access_request.py` & `boonamber-2.0.8/boonamber/v2/models/post_oauth2_access_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_oauth2_access_response.py` & `boonamber-2.0.8/boonamber/v2/models/post_oauth2_access_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_oauth2_refresh_request.py` & `boonamber-2.0.8/boonamber/v2/models/post_oauth2_refresh_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_oauth2_refresh_response.py` & `boonamber-2.0.8/boonamber/v2/models/post_oauth2_refresh_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_pretrain_request.py` & `boonamber-2.0.8/boonamber/v2/models/post_pretrain_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/post_pretrain_response.py` & `boonamber-2.0.8/boonamber/v2/models/post_pretrain_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/pretrain_status.py` & `boonamber-2.0.8/boonamber/v2/models/pretrain_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/put_data_request.py` & `boonamber-2.0.8/boonamber/v2/models/put_data_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/put_data_response.py` & `boonamber-2.0.8/boonamber/v2/models/put_data_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/put_model_request.py` & `boonamber-2.0.8/boonamber/v2/models/put_model_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/streaming_window.py` & `boonamber-2.0.8/boonamber/v2/models/streaming_window.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/training_config.py` & `boonamber-2.0.8/boonamber/v2/models/training_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/models/version_number.py` & `boonamber-2.0.8/boonamber/v2/models/version_number.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber/v2/rest.py` & `boonamber-2.0.8/boonamber/v2/rest.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/boonamber.egg-info/PKG-INFO` & `boonamber-2.0.8/boonamber.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boonamber
-Version: 2.0.6
+Version: 2.0.8
 Summary: An SDK for Boon Amber sensor analytics
 Author: BoonLogic
 Author-email: amber-support@boonlogic.com
 License: MIT
 Project-URL: repository, https://github.com/boonlogic/amber-python-sdk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boonamber-2.0.6/boonamber.egg-info/SOURCES.txt` & `boonamber-2.0.8/boonamber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.6/pyproject.toml` & `boonamber-2.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "boonamber"
-version = "2.0.6"
+version = "2.0.8"
 authors = [
     {name = "BoonLogic"},
     {email = "amber-support@boonlogic.com"}
 ]
 urls = {repository = "https://github.com/boonlogic/amber-python-sdk"}
 license = {text = "MIT"}
 description = "An SDK for Boon Amber sensor analytics"
```

