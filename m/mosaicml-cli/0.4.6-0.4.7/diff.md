# Comparing `tmp/mosaicml-cli-0.4.6.tar.gz` & `tmp/mosaicml-cli-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.4.6.tar", last modified: Tue Jun  6 23:19:16 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.4.7.tar", last modified: Thu Jun  8 20:36:22 2023, max compression
```

## Comparing `mosaicml-cli-0.4.6.tar` & `mosaicml-cli-0.4.7.tar`

### file list

```diff
@@ -1,199 +1,200 @@
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.337015 mosaicml-cli-0.4.6/
--rw-r--r--   0 margaretqian   (501) staff       (20)      696 2023-06-06 23:19:16.336822 mosaicml-cli-0.4.6/PKG-INFO
--rw-r--r--   0 margaretqian   (501) staff       (20)     7193 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/README.md
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.302299 mosaicml-cli-0.4.6/mcli/
--rw-r--r--   0 margaretqian   (501) staff       (20)     2092 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/__init__.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.303186 mosaicml-cli-0.4.6/mcli/api/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/api/__init__.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.303864 mosaicml-cli-0.4.6/mcli/api/cluster/
--rw-r--r--   0 margaretqian   (501) staff       (20)      134 2022-10-27 18:49:21.000000 mosaicml-cli-0.4.6/mcli/api/cluster/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4237 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.304325 mosaicml-cli-0.4.6/mcli/api/engine/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/api/engine/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    25914 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/engine/engine.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10685 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/exceptions.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.306545 mosaicml-cli-0.4.6/mcli/api/inference_deployments/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1521 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3297 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5105 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3603 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     8450 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2053 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_ping.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2356 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_predict_inference_deployment.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6483 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_update_inference_deployments.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.307054 mosaicml-cli-0.4.6/mcli/api/mint/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-03-06 23:35:18.000000 mosaicml-cli-0.4.6/mcli/api/mint/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     7759 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/mint/shell.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2676 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/mint/tty.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.307802 mosaicml-cli-0.4.6/mcli/api/model/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1114 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/model/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6322 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/model/cluster_details.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4583 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/model/inference_deployment.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10439 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/model/run.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.310526 mosaicml-cli-0.4.6/mcli/api/runs/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1199 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.6/mcli/api/runs/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2804 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_create_run.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4211 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     8906 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10933 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5213 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_start_run.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5405 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3937 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_update_run_metadata.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10619 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.311020 mosaicml-cli-0.4.6/mcli/api/schema/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/api/schema/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      636 2022-08-23 17:34:43.000000 mosaicml-cli-0.4.6/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.312652 mosaicml-cli-0.4.6/mcli/api/secrets/
--rw-r--r--   0 margaretqian   (501) staff       (20)      309 2022-09-22 23:36:49.000000 mosaicml-cli-0.4.6/mcli/api/secrets/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2386 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3019 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3718 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2354 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/api/typing_future.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.313308 mosaicml-cli-0.4.6/mcli/api/users/
--rw-r--r--   0 margaretqian   (501) staff       (20)      139 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.6/mcli/api/users/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2715 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.313599 mosaicml-cli-0.4.6/mcli/cli/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/__init__.py
--rwxr-xr-x   0 margaretqian   (501) staff       (20)     6387 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/cli.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.314079 mosaicml-cli-0.4.6/mcli/cli/common/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-02-02 19:35:37.000000 mosaicml-cli-0.4.6/mcli/cli/common/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2560 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6922 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.314411 mosaicml-cli-0.4.6/mcli/cli/m_connect/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-03-06 23:35:18.000000 mosaicml-cli-0.4.6/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1935 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.6/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.315221 mosaicml-cli-0.4.6/mcli/cli/m_create/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_create/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2385 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_create/m_create.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    16900 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.315914 mosaicml-cli-0.4.6/mcli/cli/m_delete/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6448 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_delete/delete.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5805 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.316349 mosaicml-cli-0.4.6/mcli/cli/m_deploy/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4001 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.317349 mosaicml-cli-0.4.6/mcli/cli/m_describe/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-02-02 19:35:37.000000 mosaicml-cli-0.4.6/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3929 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     9988 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2002 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.319114 mosaicml-cli-0.4.6/mcli/cli/m_get/
--rw-r--r--   0 margaretqian   (501) staff       (20)      467 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6226 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/clusters.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6447 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/display.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5669 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4803 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/m_get.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     9800 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/runs.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2189 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/secrets.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1580 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.6/mcli/cli/m_get/users.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.319515 mosaicml-cli-0.4.6/mcli/cli/m_init/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_init/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4115 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.6/mcli/cli/m_init/m_init.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.320525 mosaicml-cli-0.4.6/mcli/cli/m_interactive/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10916 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.6/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    44284 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_interactive/kube_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     9493 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_interactive/m_interactive.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.321369 mosaicml-cli-0.4.6/mcli/cli/m_kube/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_kube/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5523 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_kube/m_get_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1398 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_kube/m_kube.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2050 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_kube/m_merge_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6946 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_kube/utils.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.321685 mosaicml-cli-0.4.6/mcli/cli/m_log/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_log/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    11398 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.6/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.322103 mosaicml-cli-0.4.6/mcli/cli/m_ping/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1103 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.322409 mosaicml-cli-0.4.6/mcli/cli/m_predict/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1661 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.322714 mosaicml-cli-0.4.6/mcli/cli/m_root/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_root/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      536 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.323012 mosaicml-cli-0.4.6/mcli/cli/m_run/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/cli/m_run/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     8267 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.324228 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-10-11 22:54:49.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2973 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1802 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/feature_flag.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1940 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1421 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      881 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.6/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.324640 mosaicml-cli-0.4.6/mcli/cli/m_stop/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-09-27 16:43:54.000000 mosaicml-cli-0.4.6/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4066 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.325118 mosaicml-cli-0.4.6/mcli/cli/m_util/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-07-14 21:04:39.000000 mosaicml-cli-0.4.6/mcli/cli/m_util/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      797 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_util/m_util.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6837 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/cli/m_util/util.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    12876 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.6/mcli/config.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.326295 mosaicml-cli-0.4.6/mcli/models/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1047 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2103 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/gpu_type.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10317 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/inference_deployment_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      427 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/mcli_cluster.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      456 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/mcli_envvar.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6724 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/mcli_secret.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    19547 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/models/run_config.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.326534 mosaicml-cli-0.4.6/mcli/objects/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/objects/__init__.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.328307 mosaicml-cli-0.4.6/mcli/objects/secrets/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1090 2022-12-07 22:00:09.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/__init__.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.330107 mosaicml-cli-0.4.6/mcli/objects/secrets/create/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1646 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/base.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2244 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2408 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6377 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3858 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3001 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5342 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      783 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1017 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/env_var.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      556 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/gcp.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1267 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/mounted.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      967 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/oci.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      961 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/s3.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1718 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.330567 mosaicml-cli-0.4.6/mcli/proto/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.6/mcli/proto/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1477 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.6/mcli/proto/mint_pb2.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.330957 mosaicml-cli-0.4.6/mcli/sdk/
--rw-r--r--   0 margaretqian   (501) staff       (20)     1976 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/sdk/__init__.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.334695 mosaicml-cli-0.4.6/mcli/utils/
--rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/utils/__init__.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5306 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/utils/utils_cli.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6073 2023-04-13 22:08:13.000000 mosaicml-cli-0.4.6/mcli/utils/utils_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)      740 2022-09-27 16:43:54.000000 mosaicml-cli-0.4.6/mcli/utils/utils_date.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10749 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_docker.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2225 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_epilog.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10774 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_interactive.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4527 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_logging.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     2160 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.6/mcli/utils/utils_message_decoding.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6614 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/utils/utils_pypi.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3115 2022-08-31 05:37:31.000000 mosaicml-cli-0.4.6/mcli/utils/utils_rich.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     5033 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.6/mcli/utils/utils_run_status.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     4350 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1103 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.6/mcli/utils/utils_spinner.py
--rw-r--r--   0 margaretqian   (501) staff       (20)    10751 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_string_functions.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1677 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/mcli/utils/utils_types.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     1001 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/mcli/utils/utils_yaml.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     3885 2023-06-06 23:17:23.000000 mosaicml-cli-0.4.6/mcli/version.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.335603 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/
--rw-r--r--   0 margaretqian   (501) staff       (20)      696 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 margaretqian   (501) staff       (20)     4868 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 margaretqian   (501) staff       (20)        1 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 margaretqian   (501) staff       (20)       75 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 margaretqian   (501) staff       (20)     1655 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 margaretqian   (501) staff       (20)        5 2023-06-06 23:19:16.000000 mosaicml-cli-0.4.6/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 margaretqian   (501) staff       (20)    31087 2023-05-16 20:27:59.000000 mosaicml-cli-0.4.6/pyproject.toml
--rw-r--r--   0 margaretqian   (501) staff       (20)       38 2023-06-06 23:19:16.337077 mosaicml-cli-0.4.6/setup.cfg
--rw-r--r--   0 margaretqian   (501) staff       (20)     3057 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/setup.py
-drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-06 23:19:16.336390 mosaicml-cli-0.4.6/tests/
--rw-r--r--   0 margaretqian   (501) staff       (20)     5991 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.6/tests/test_config.py
--rw-r--r--   0 margaretqian   (501) staff       (20)       62 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.6/tests/test_simple.py
--rw-r--r--   0 margaretqian   (501) staff       (20)     6116 2023-04-11 21:00:01.000000 mosaicml-cli-0.4.6/tests/test_upgrade.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.787793 mosaicml-cli-0.4.7/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      696 2023-06-08 20:36:22.787561 mosaicml-cli-0.4.7/PKG-INFO
+-rw-r--r--   0 margaretqian   (501) staff       (20)     7089 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/README.md
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.760093 mosaicml-cli-0.4.7/mcli/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2092 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/__init__.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.760685 mosaicml-cli-0.4.7/mcli/api/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/api/__init__.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.760963 mosaicml-cli-0.4.7/mcli/api/cluster/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      134 2022-10-27 18:49:21.000000 mosaicml-cli-0.4.7/mcli/api/cluster/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4237 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.761223 mosaicml-cli-0.4.7/mcli/api/engine/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/api/engine/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    26003 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/mcli/api/engine/engine.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10685 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/exceptions.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.762380 mosaicml-cli-0.4.7/mcli/api/inference_deployments/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1521 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3297 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5105 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3603 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_get_inference_deployment_logs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     8450 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2053 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_ping.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2356 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_predict_inference_deployment.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6483 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_update_inference_deployments.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.762753 mosaicml-cli-0.4.7/mcli/api/mint/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-03-06 23:35:18.000000 mosaicml-cli-0.4.7/mcli/api/mint/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     7849 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/mcli/api/mint/shell.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2676 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/mint/tty.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.763281 mosaicml-cli-0.4.7/mcli/api/model/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1114 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/model/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6322 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/model/cluster_details.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4583 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10439 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/model/run.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.764573 mosaicml-cli-0.4.7/mcli/api/runs/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1199 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.7/mcli/api/runs/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2804 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4211 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     8906 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10933 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5213 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_start_run.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5405 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3937 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_update_run_metadata.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10619 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.764836 mosaicml-cli-0.4.7/mcli/api/schema/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/api/schema/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      636 2022-08-23 17:34:43.000000 mosaicml-cli-0.4.7/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.765387 mosaicml-cli-0.4.7/mcli/api/secrets/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      309 2022-09-22 23:36:49.000000 mosaicml-cli-0.4.7/mcli/api/secrets/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2386 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3019 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3718 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2354 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/api/typing_future.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.765659 mosaicml-cli-0.4.7/mcli/api/users/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      139 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.7/mcli/api/users/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2715 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/api/users/api_get_users.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1091 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/mcli/api/utils.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.765895 mosaicml-cli-0.4.7/mcli/cli/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/__init__.py
+-rwxr-xr-x   0 margaretqian   (501) staff       (20)     6387 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/cli.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.766290 mosaicml-cli-0.4.7/mcli/cli/common/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-02-02 19:35:37.000000 mosaicml-cli-0.4.7/mcli/cli/common/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2560 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6922 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.766531 mosaicml-cli-0.4.7/mcli/cli/m_connect/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-03-06 23:35:18.000000 mosaicml-cli-0.4.7/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1935 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.7/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.766910 mosaicml-cli-0.4.7/mcli/cli/m_create/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2385 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    16900 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.767327 mosaicml-cli-0.4.7/mcli/cli/m_delete/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6448 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5805 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.767585 mosaicml-cli-0.4.7/mcli/cli/m_deploy/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4001 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.768141 mosaicml-cli-0.4.7/mcli/cli/m_describe/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-02-02 19:35:37.000000 mosaicml-cli-0.4.7/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3929 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     9988 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2002 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.769225 mosaicml-cli-0.4.7/mcli/cli/m_get/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      467 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6226 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6447 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/display.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5669 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4803 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     9800 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/runs.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2189 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1580 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.7/mcli/cli/m_get/users.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.769476 mosaicml-cli-0.4.7/mcli/cli/m_init/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4115 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.7/mcli/cli/m_init/m_init.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.770112 mosaicml-cli-0.4.7/mcli/cli/m_interactive/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10916 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.7/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    44284 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_interactive/kube_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     9493 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_interactive/m_interactive.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.770777 mosaicml-cli-0.4.7/mcli/cli/m_kube/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_kube/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5523 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_kube/m_get_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1398 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_kube/m_kube.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2050 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_kube/m_merge_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6946 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_kube/utils.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.771027 mosaicml-cli-0.4.7/mcli/cli/m_log/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    11398 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.7/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.775512 mosaicml-cli-0.4.7/mcli/cli/m_ping/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1103 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.775854 mosaicml-cli-0.4.7/mcli/cli/m_predict/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1661 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.776142 mosaicml-cli-0.4.7/mcli/cli/m_root/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      536 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.776582 mosaicml-cli-0.4.7/mcli/cli/m_run/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     8267 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.777468 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-10-11 22:54:49.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2973 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1802 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/feature_flag.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1940 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1421 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      881 2023-02-02 20:09:34.000000 mosaicml-cli-0.4.7/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.777751 mosaicml-cli-0.4.7/mcli/cli/m_stop/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-09-27 16:43:54.000000 mosaicml-cli-0.4.7/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4066 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.778152 mosaicml-cli-0.4.7/mcli/cli/m_util/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-07-14 21:04:39.000000 mosaicml-cli-0.4.7/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      797 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6837 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/cli/m_util/util.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    12876 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.7/mcli/config.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.779133 mosaicml-cli-0.4.7/mcli/models/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1047 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2103 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/gpu_type.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10374 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      427 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/mcli_cluster.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      456 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/mcli_envvar.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6724 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/mcli_secret.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    19547 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/models/run_config.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.779293 mosaicml-cli-0.4.7/mcli/objects/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/objects/__init__.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.780555 mosaicml-cli-0.4.7/mcli/objects/secrets/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1090 2022-12-07 22:00:09.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/__init__.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.782249 mosaicml-cli-0.4.7/mcli/objects/secrets/create/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1646 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2244 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2408 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6377 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3858 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3001 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5342 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      783 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1017 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      556 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1267 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      967 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/oci.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      961 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/s3.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1718 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.782580 mosaicml-cli-0.4.7/mcli/proto/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.7/mcli/proto/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1477 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.7/mcli/proto/mint_pb2.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.783027 mosaicml-cli-0.4.7/mcli/sdk/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1976 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/sdk/__init__.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.785760 mosaicml-cli-0.4.7/mcli/utils/
+-rw-r--r--   0 margaretqian   (501) staff       (20)        0 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/utils/__init__.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5306 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/utils/utils_cli.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6073 2023-04-13 22:08:13.000000 mosaicml-cli-0.4.7/mcli/utils/utils_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)      740 2022-09-27 16:43:54.000000 mosaicml-cli-0.4.7/mcli/utils/utils_date.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10749 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_docker.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2225 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_epilog.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10774 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_interactive.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4527 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_logging.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     2160 2023-05-01 16:10:33.000000 mosaicml-cli-0.4.7/mcli/utils/utils_message_decoding.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6614 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/utils/utils_pypi.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3115 2022-08-31 05:37:31.000000 mosaicml-cli-0.4.7/mcli/utils/utils_rich.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5033 2023-06-06 23:17:16.000000 mosaicml-cli-0.4.7/mcli/utils/utils_run_status.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4350 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1103 2023-04-11 21:00:00.000000 mosaicml-cli-0.4.7/mcli/utils/utils_spinner.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)    10751 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1677 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/mcli/utils/utils_types.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1001 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/mcli/utils/utils_yaml.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3885 2023-06-08 20:35:56.000000 mosaicml-cli-0.4.7/mcli/version.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.786816 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/
+-rw-r--r--   0 margaretqian   (501) staff       (20)      696 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 margaretqian   (501) staff       (20)     4886 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 margaretqian   (501) staff       (20)        1 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 margaretqian   (501) staff       (20)       75 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 margaretqian   (501) staff       (20)     1655 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 margaretqian   (501) staff       (20)        5 2023-06-08 20:36:22.000000 mosaicml-cli-0.4.7/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 margaretqian   (501) staff       (20)    31087 2023-05-16 20:27:59.000000 mosaicml-cli-0.4.7/pyproject.toml
+-rw-r--r--   0 margaretqian   (501) staff       (20)       38 2023-06-08 20:36:22.787870 mosaicml-cli-0.4.7/setup.cfg
+-rw-r--r--   0 margaretqian   (501) staff       (20)     3057 2023-06-08 20:35:34.000000 mosaicml-cli-0.4.7/setup.py
+drwxr-xr-x   0 margaretqian   (501) staff       (20)        0 2023-06-08 20:36:22.787302 mosaicml-cli-0.4.7/tests/
+-rw-r--r--   0 margaretqian   (501) staff       (20)     5991 2023-06-06 22:51:56.000000 mosaicml-cli-0.4.7/tests/test_config.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)       62 2022-06-27 19:47:20.000000 mosaicml-cli-0.4.7/tests/test_simple.py
+-rw-r--r--   0 margaretqian   (501) staff       (20)     6116 2023-04-11 21:00:01.000000 mosaicml-cli-0.4.7/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.4.6/PKG-INFO` & `mosaicml-cli-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.6
+Version: 0.4.7
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.6/README.md` & `mosaicml-cli-0.4.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 ## Understanding MCLI
 
 MCLI is a command line interface and python SDK for the MosaicML platform.
 
 To understand MCLI use cases, read the [customer-facing docs](https://mcli.docs.mosaicml.com/) and go through installation and tutorials.
 
-There is also documentation specific to [internal use cases](https://internal.mcli.docs.mosaicml.com).
-
 ## Development environment setup
 
 ### Pre-requisites
 
 **Git**
 
 We’re using git and GitHub for source control. In case your dev box does not have git installed, [this is a good resource on installing git](https://github.com/git-guides/install-git#install-git) (and it has [even more resources](https://github.com/git-guides/) to help get started with git concepts and commands).
```

### Comparing `mosaicml-cli-0.4.6/mcli/__init__.py` & `mosaicml-cli-0.4.7/mcli/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.4.7/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/engine/engine.py` & `mosaicml-cli-0.4.7/mcli/api/engine/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from gql.transport.exceptions import TransportQueryError
 from gql.transport.websockets import WebsocketsTransport
 from graphql import DocumentNode
 from websockets.exceptions import ConnectionClosed, PayloadTooBig, WebSocketException
 
 from mcli.api.exceptions import MAPIException, MCLIConfigError, MultiMAPIException
 from mcli.api.schema.generic_model import DeserializableModel
+from mcli.api.utils import check_python_certificates
 from mcli.config import MESSAGE, get_timeout
 
 logger = logging.getLogger(__name__)
 
 # pylint: disable-next=invalid-name
 THREADPOOL_WORKERS = 10
 THREADPOOL: Optional[ThreadPoolExecutor] = None
@@ -195,14 +196,15 @@
                     self._loop,
                 )
 
         finally:
             async_gen.aclose()
 
     async def init_session(self):
+        check_python_certificates()
         session = await self.client.connect_async(
             reconnecting=True,
             retry_connect=on_exception(
                 expo,
                 # This needs to be Exception - do not change to more specific subclass
                 # https://github.com/graphql-python/gql/blob/master/gql/client.py#L1304
                 Exception,
```

### Comparing `mosaicml-cli-0.4.6/mcli/api/exceptions.py` & `mosaicml-cli-0.4.7/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.4.7/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_get_inference_deployment_logs.py` & `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_get_inference_deployment_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_ping.py` & `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/inference_deployments/api_update_inference_deployments.py` & `mosaicml-cli-0.4.7/mcli/api/inference_deployments/api_update_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/mint/shell.py` & `mosaicml-cli-0.4.7/mcli/api/mint/shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import backoff
 from websockets.client import WebSocketClientProtocol
 from websockets.client import connect as ws_connect
 
 from mcli.api.exceptions import MintConnectionException, MintServerException, handle_mint_errors
 from mcli.api.mint import tty
 from mcli.api.model.run import Run
+from mcli.api.utils import check_python_certificates
 from mcli.proto.mint_pb2 import MINTMessage, TerminalSize, UserInput
 from mcli.utils.utils_logging import WARN
 from mcli.utils.utils_message_decoding import MessageDecoder
 
 logger = logging.getLogger(__name__)
 
 
@@ -202,11 +203,13 @@
 
         return response
 
     def connect(self, command: Optional[str] = None) -> None:
         """
         Connect to a run using the MINT Shell
         """
+
+        check_python_certificates()
         if not tty.TTY_SUPPORTED:
             logger.warning(f'{WARN} MCLI Connect does not currently support TTY for your OS')
 
         return self._loop.run_until_complete(self._connect(self._uri, command=command))
```

### Comparing `mosaicml-cli-0.4.6/mcli/api/mint/tty.py` & `mosaicml-cli-0.4.7/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/model/__init__.py` & `mosaicml-cli-0.4.7/mcli/api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.4.7/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.4.7/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/model/run.py` & `mosaicml-cli-0.4.7/mcli/api/model/run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/runs/__init__.py` & `mosaicml-cli-0.4.7/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.4.7/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.4.7/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.4.7/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.4.7/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/runs/api_start_run.py` & `mosaicml-cli-0.4.7/mcli/api/runs/api_start_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.4.7/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/runs/api_update_run_metadata.py` & `mosaicml-cli-0.4.7/mcli/api/runs/api_update_run_metadata.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.4.7/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.4.7/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.4.7/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.4.7/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.4.7/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/typing_future.py` & `mosaicml-cli-0.4.7/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.4.7/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/cli.py` & `mosaicml-cli-0.4.7/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.4.7/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.4.7/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.4.7/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.4.7/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.4.7/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.4.7/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.4.7/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.4.7/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.4.7/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.4.7/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.4.7/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.4.7/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_get/display.py` & `mosaicml-cli-0.4.7/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.4.7/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.4.7/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.4.7/mcli/cli/m_get/runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.4.7/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_get/users.py` & `mosaicml-cli-0.4.7/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.4.7/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.4.7/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_interactive/kube_config.py` & `mosaicml-cli-0.4.7/mcli/cli/m_interactive/kube_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.4.7/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_kube/m_get_config.py` & `mosaicml-cli-0.4.7/mcli/cli/m_kube/m_get_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_kube/m_kube.py` & `mosaicml-cli-0.4.7/mcli/cli/m_kube/m_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_kube/m_merge_config.py` & `mosaicml-cli-0.4.7/mcli/cli/m_kube/m_merge_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_kube/utils.py` & `mosaicml-cli-0.4.7/mcli/cli/m_kube/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.4.7/mcli/cli/m_log/m_log.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.4.7/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.4.7/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.4.7/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.4.7/mcli/cli/m_run/m_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.4.7/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_set_unset/feature_flag.py` & `mosaicml-cli-0.4.7/mcli/cli/m_set_unset/feature_flag.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.4.7/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.4.7/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.4.7/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.4.7/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.4.7/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/cli/m_util/util.py` & `mosaicml-cli-0.4.7/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/config.py` & `mosaicml-cli-0.4.7/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/models/__init__.py` & `mosaicml-cli-0.4.7/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/models/gpu_type.py` & `mosaicml-cli-0.4.7/mcli/models/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.4.7/mcli/models/inference_deployment_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 class ModelConfig(TypedDict, total=False):
     """Typed dictionary for model configs"""
     downloader: str
     download_parameters: Dict[str, str]
     model_handler: str
     model_parameters: Dict[str, str]
+    backend: Optional[str]
 
 
 @dataclass
 class FinalInferenceDeploymentConfig(DeserializableModel):
     """A finalized deployment configuration
     This configuration must be complete, with enough details to submit a new deployment to the
     MosaicML Cloud.
@@ -252,14 +253,15 @@
     """Translate model configs to and from MAPI"""
 
     _property_translations = {
         'downloader': 'downloader',
         'download_parameters': 'downloadParameters',
         'model_handler': 'modelHandler',
         'model_parameters': 'modelParameters',
+        'backend': 'backend',
     }
 
     @classmethod
     def from_mapi(cls, value: Dict[str, Any]) -> ModelConfig:
         translated_config = {}
         for mcli_key, mapi_key in cls._property_translations.items():
             translated_config[mcli_key] = value.get(mapi_key)
```

### Comparing `mosaicml-cli-0.4.6/mcli/models/mcli_secret.py` & `mosaicml-cli-0.4.7/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/models/run_config.py` & `mosaicml-cli-0.4.7/mcli/models/run_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.4.7/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/proto/mint_pb2.py` & `mosaicml-cli-0.4.7/mcli/proto/mint_pb2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/sdk/__init__.py` & `mosaicml-cli-0.4.7/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_cli.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_config.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_date.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_docker.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_logging.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_message_decoding.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_message_decoding.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_rich.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_types.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.4.7/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/mcli/version.py` & `mosaicml-cli-0.4.7/mcli/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = '0.4.6'
+__version__ = '0.4.7'
 
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.4.6/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.4.7/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.4.6
+Version: 0.4.7
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.4.6/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.4.7/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 mcli/__init__.py
 mcli/config.py
 mcli/version.py
 mcli/api/__init__.py
 mcli/api/exceptions.py
 mcli/api/typing_future.py
+mcli/api/utils.py
 mcli/api/cluster/__init__.py
 mcli/api/cluster/api_get_clusters.py
 mcli/api/engine/__init__.py
 mcli/api/engine/engine.py
 mcli/api/inference_deployments/__init__.py
 mcli/api/inference_deployments/api_create_inference_deployment.py
 mcli/api/inference_deployments/api_delete_inference_deployments.py
```

### Comparing `mosaicml-cli-0.4.6/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.4.7/mosaicml_cli.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,54 +9,54 @@
 questionary>=1.10.0
 rich>=10.16.2
 ruamel.yaml>=0.17.21
 typing_extensions>=4.0.1
 validators>=0.20.0
 
 [all]
-sphinxcontrib-serializinghtml==1.1.5
-myst-parser>=0.16.1
-sphinxemoji==0.2.0
-sphinx-copybutton==0.5.2
-sphinx_external_toc==0.3.0
-pytest-cov>=4.0.0
-sphinx==4.4.0
-radon>=5.1.0
 yapf>=0.33.0
-sphinx-markdown-tables==0.0.17
-twine>=4.0.2
+sphinxcontrib-applehelp>=1.0.2
+sphinxcontrib-images>=0.9.4
+myst-parser>=0.16.1
 pre-commit>=2.17.0
-sphinxcontrib-devhelp>=1.0.2
-sphinxcontrib-katex==0.9.4
-sphinxext-opengraph==0.8.2
+sphinx-markdown-tables==0.0.17
+sphinx_external_toc==0.3.0
+sphinx-panels==0.6.0
+sphinxemoji==0.2.0
 sphinx-argparse==0.4.0
-furo==2022.9.29
+radon>=5.1.0
 docutils>=0.17.0
 sphinx-design
-sphinxcontrib-applehelp>=1.0.2
-sphinxcontrib-htmlhelp>=2.0.0
-toml>=0.10.2
+isort>=5.9.3
+sphinxcontrib-katex==0.9.4
+furo==2022.9.29
 pylint>=2.12.2
 pytest-mock>=3.7.0
-pyright>=1.1.256
-sphinx-rtd-theme==1.0.0
-sphinxcontrib-images>=0.9.4
-build>=0.10.0
-pytest>=6.2.5
-isort>=5.9.3
-sphinx-panels==0.6.0
+sphinx-copybutton==0.5.2
 sphinxcontrib-qthelp>=1.0.3
+sphinxcontrib-devhelp>=1.0.2
 sphinxcontrib-jsmath>=1.0.1
+sphinx==4.4.0
+sphinxcontrib-htmlhelp>=2.0.0
+sphinx-rtd-theme==1.0.0
+twine>=4.0.2
+sphinxcontrib-serializinghtml==1.1.5
+pytest>=6.2.5
+sphinxext-opengraph==0.8.2
+toml>=0.10.2
+build>=0.10.0
+pyright==1.1.256
+pytest-cov>=4.0.0
 
 [dev]
 build>=0.10.0
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
-pyright>=1.1.256
+pyright==1.1.256
 pytest-cov>=4.0.0
 pytest-mock>=3.7.0
 pytest>=6.2.5
 radon>=5.1.0
 twine>=4.0.2
 toml>=0.10.2
 yapf>=0.33.0
```

### Comparing `mosaicml-cli-0.4.6/pyproject.toml` & `mosaicml-cli-0.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/setup.py` & `mosaicml-cli-0.4.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 extra_deps = {}
 
 extra_deps['dev'] = [
     'build>=0.10.0',
     'isort>=5.9.3',
     'pre-commit>=2.17.0',
     'pylint>=2.12.2',
-    'pyright>=1.1.256',
+    'pyright==1.1.256',
     'pytest-cov>=4.0.0',
     'pytest-mock>=3.7.0',
     'pytest>=6.2.5',
     'radon>=5.1.0',
     'twine>=4.0.2',
     'toml>=0.10.2',
     'yapf>=0.33.0',
```

### Comparing `mosaicml-cli-0.4.6/tests/test_config.py` & `mosaicml-cli-0.4.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.4.6/tests/test_upgrade.py` & `mosaicml-cli-0.4.7/tests/test_upgrade.py`

 * *Files identical despite different names*

