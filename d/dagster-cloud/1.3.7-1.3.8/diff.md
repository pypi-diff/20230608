# Comparing `tmp/dagster_cloud-1.3.7.tar.gz` & `tmp/dagster_cloud-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud-1.3.7.tar", last modified: Thu Jun  1 18:27:19 2023, max compression
+gzip compressed data, was "dagster_cloud-1.3.8.tar", last modified: Thu Jun  8 16:34:35 2023, max compression
```

## Comparing `dagster_cloud-1.3.7.tar` & `dagster_cloud-1.3.8.tar`

### file list

```diff
@@ -1,114 +1,110 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.957537 dagster_cloud-1.3.7/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-06-01 18:27:19.957537 dagster_cloud-1.3.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.905537 dagster_cloud-1.3.7/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      140 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.909537 dagster_cloud-1.3.7/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.909537 dagster_cloud-1.3.7/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43075 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.909537 dagster_cloud-1.3.7/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16984 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.913537 dagster_cloud-1.3.7/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/auth/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.913537 dagster_cloud-1.3.7/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.913537 dagster_cloud-1.3.7/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.913537 dagster_cloud-1.3.7/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    14188 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.917537 dagster_cloud-1.3.7/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.917537 dagster_cloud-1.3.7/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    18147 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.917537 dagster_cloud-1.3.7/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.921537 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.921537 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7786 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4541 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.925537 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.925537 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10312 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)     9912 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    11492 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.929537 dagster_cloud-1.3.7/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.929537 dagster_cloud-1.3.7/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4616 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.933537 dagster_cloud-1.3.7/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.933537 dagster_cloud-1.3.7/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4582 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.937537 dagster_cloud-1.3.7/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9532 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    26988 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.941537 dagster_cloud-1.3.7/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19041 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.941537 dagster_cloud-1.3.7/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1927 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7209 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.941537 dagster_cloud-1.3.7/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2248 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.941537 dagster_cloud-1.3.7/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.945537 dagster_cloud-1.3.7/dagster_cloud/workspace/cli/
--rw-r--r--   0 root         (0) root         (0)     6948 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.945537 dagster_cloud-1.3.7/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)     8613 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     5365 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.949537 dagster_cloud-1.3.7/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12011 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.953537 dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23300 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    22551 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     1748 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.953537 dagster_cloud-1.3.7/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17127 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/kubernetes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.957537 dagster_cloud-1.3.7/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    74026 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:27:19.905537 dagster_cloud-1.3.7/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-06-01 18:27:19.000000 dagster_cloud-1.3.7/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3216 2023-06-01 18:27:19.000000 dagster_cloud-1.3.7/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:27:19.000000 dagster_cloud-1.3.7/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:27:19.000000 dagster_cloud-1.3.7/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-01 18:27:19.000000 dagster_cloud-1.3.7/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 18:27:19.957537 dagster_cloud-1.3.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2890 2023-06-01 18:15:11.000000 dagster_cloud-1.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.097891 dagster_cloud-1.3.8/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-06-08 16:34:35.097891 dagster_cloud-1.3.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.957891 dagster_cloud-1.3.8/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      223 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.961891 dagster_cloud-1.3.8/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.961891 dagster_cloud-1.3.8/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42585 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.965891 dagster_cloud-1.3.8/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16984 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.965891 dagster_cloud-1.3.8/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/auth/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.965891 dagster_cloud-1.3.8/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.965891 dagster_cloud-1.3.8/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    14913 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.969891 dagster_cloud-1.3.8/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.969891 dagster_cloud-1.3.8/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    18147 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.969891 dagster_cloud-1.3.8/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.973891 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.977891 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4541 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.993891 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.993891 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10999 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    12930 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.005891 dagster_cloud-1.3.8/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.005891 dagster_cloud-1.3.8/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4641 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.009891 dagster_cloud-1.3.8/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.009891 dagster_cloud-1.3.8/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.021891 dagster_cloud-1.3.8/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11717 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    32380 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.021891 dagster_cloud-1.3.8/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19041 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.029891 dagster_cloud-1.3.8/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1927 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.033891 dagster_cloud-1.3.8/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.037891 dagster_cloud-1.3.8/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.037891 dagster_cloud-1.3.8/dagster_cloud/workspace/cli/
+-rw-r--r--   0 root         (0) root         (0)     6948 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.077891 dagster_cloud-1.3.8/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6018 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.081891 dagster_cloud-1.3.8/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12030 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.089891 dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23381 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    23524 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.093891 dagster_cloud-1.3.8/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17127 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11407 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/kubernetes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:35.097891 dagster_cloud-1.3.8/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    74026 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:34:34.957891 dagster_cloud-1.3.8/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-06-08 16:34:34.000000 dagster_cloud-1.3.8/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-08 16:34:34.000000 dagster_cloud-1.3.8/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:34:34.000000 dagster_cloud-1.3.8/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 16:34:34.000000 dagster_cloud-1.3.8/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 16:34:34.000000 dagster_cloud-1.3.8/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 16:34:35.097891 dagster_cloud-1.3.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-06-08 16:24:05.000000 dagster_cloud-1.3.8/setup.py
```

### Comparing `dagster_cloud-1.3.7/PKG-INFO` & `dagster_cloud-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_cloud
-Version: 1.3.7
+Version: 1.3.8
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.7/README.md` & `dagster_cloud-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/agent/cli/__init__.py` & `dagster_cloud-1.3.8/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster_cloud-1.3.8/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,22 +120,14 @@
     def __exit__(self, _exception_type, _exception_value, _traceback):
         self._exit_stack.close()
 
     @property
     def _active_deployment_names(self):
         return [deployment[0] for deployment in self._active_deployments]
 
-    @property
-    def _active_production_deployment_names(self):
-        return [
-            deployment
-            for deployment, is_branch_deployment in self._active_deployments
-            if not is_branch_deployment
-        ]
-
     def _check_initial_deployment_names(self, instance: DagsterCloudAgentInstance):
         if instance.deployment_names:
             result = instance.organization_scoped_graphql_client().execute(
                 DEPLOYMENTS_QUERY, variable_values={"deploymentNames": instance.deployment_names}
             )
             deployments = result["data"]["deployments"]
             existing_deployment_names = {deployment["deploymentName"] for deployment in deployments}
@@ -261,17 +253,14 @@
             return
 
         errors = [
             TimestampedError(timestamp.float_timestamp, error)
             for (error, timestamp) in self._errors
         ]
 
-        # Get a run worker status object for every deployment since AgentHeartbeat requires one
-        # - it will just always be empty for branch deployments since those didn't even check for
-        # run worker statuses
         run_worker_statuses_dict = instance.user_code_launcher.get_cloud_run_worker_statuses(
             self._active_deployment_names
         )
 
         code_server_heartbeats_dict = instance.user_code_launcher.get_grpc_server_heartbeats()
 
         agent_image_tag = os.getenv("DAGSTER_CLOUD_AGENT_IMAGE_TAG")
@@ -504,17 +493,15 @@
 
         if upload_all:
             user_code_launcher.add_upload_metadata(deployment_map)
         else:
             user_code_launcher.update_grpc_metadata(deployment_map)
 
         # Tell run worker monitoring which deployments it should care about
-        user_code_launcher.update_run_worker_monitoring_deployments(
-            self._active_production_deployment_names
-        )
+        user_code_launcher.update_run_worker_monitoring_deployments(self._active_deployment_names)
 
         # In the rare event that there are pending requests that are no longer in the workspace at
         # all (if, say, a location is removed while requests are enqueued), they should be forcibly
         # moved to ready so that they don't stay pending forever - callsites will get an error
         # about the location not existing, but that's preferable to slowly timing out
         pending_requests_copy = self._pending_requests.copy()
         self._pending_requests = []
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/agent/queries.py` & `dagster_cloud-1.3.8/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/api/dagster_cloud_api.py` & `dagster_cloud-1.3.8/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/auth/constants.py` & `dagster_cloud-1.3.8/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/execution/monitoring/__init__.py` & `dagster_cloud-1.3.8/dagster_cloud/execution/monitoring/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 import logging
 import sys
 import threading
 from enum import Enum
-from typing import Dict, Iterable, List, Mapping, NamedTuple, Optional, Sequence, Set, Tuple, Union
+from typing import (
+    Dict,
+    Iterable,
+    List,
+    Mapping,
+    NamedTuple,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Union,
+)
 
 import dagster._check as check
 import grpc
 from dagster import DagsterInstance, DagsterRunStatus
 from dagster._core.launcher import CheckRunHealthResult, WorkerStatus
 from dagster._core.storage.dagster_run import IN_PROGRESS_RUN_STATUSES, RunsFilter
 from dagster._serdes import whitelist_for_serdes
@@ -52,31 +63,53 @@
 class CloudRunWorkerStatus(
     NamedTuple(
         "_CloudRunWorkerStatus",
         [
             ("run_id", str),
             ("status_type", WorkerStatus),
             ("message", Optional[str]),
+            ("transient", Optional[bool]),  # If the run worker failed, is there reason to retry?
+            (
+                "run_worker_id",
+                Optional[str],
+            ),  # unique identifier for a particular run worker
         ],
     )
 ):
-    def __new__(cls, run_id: str, status_type: WorkerStatus, message: Optional[str] = None):
+    def __new__(
+        cls,
+        run_id: str,
+        status_type: WorkerStatus,
+        message: Optional[str] = None,
+        transient: Optional[bool] = None,
+        run_worker_id: Optional[str] = None,
+    ):
         return super(CloudRunWorkerStatus, cls).__new__(
             cls,
             run_id=check.str_param(run_id, "run_id"),
             status_type=check.inst_param(status_type, "status_type", WorkerStatus),
             message=check.opt_str_param(message, "message"),
+            transient=check.opt_bool_param(transient, "transient", default=False),
+            run_worker_id=check.opt_str_param(run_worker_id, "run_worker_id"),
         )
 
     @classmethod
     def from_check_run_health_result(
-        cls, run_id: str, result: CheckRunHealthResult
+        cls,
+        run_id: str,
+        result: CheckRunHealthResult,
     ) -> "CloudRunWorkerStatus":
         check.inst_param(result, "result", CheckRunHealthResult)
-        return CloudRunWorkerStatus(run_id, result.status, result.msg)
+        return CloudRunWorkerStatus(
+            run_id,
+            result.status,
+            result.msg,
+            transient=result.transient,
+            run_worker_id=result.run_worker_id,
+        )
 
 
 @whitelist_for_serdes
 class CloudRunWorkerStatuses(
     NamedTuple(
         "_CloudRunWorkerStatuses",
         [
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/execution/utils/process.py` & `dagster_cloud-1.3.8/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/instance/__init__.py` & `dagster_cloud-1.3.8/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster_cloud-1.3.8/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster_cloud-1.3.8/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/pex/grpc/client.py` & `dagster_cloud-1.3.8/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/pex/grpc/compile.py` & `dagster_cloud-1.3.8/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/manager.py` & `dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,183 +1,184 @@
 import logging
 import os
 import subprocess
+import sys
 import threading
 from contextlib import AbstractContextManager
-from typing import Dict, List, NamedTuple, Optional, Set
+from typing import Dict, List, Optional, Set, Union, cast
 
 import dagster._seven as seven
 from dagster import _check as check
 from dagster._core.errors import DagsterUserCodeUnreachableError
 from dagster._core.instance.ref import InstanceRef
 from dagster._grpc.client import DagsterGrpcClient, client_heartbeat_thread
 from dagster._serdes.ipc import open_ipc_subprocess
 from dagster._utils import find_free_port, safe_tempfile_path_unmanaged
+from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
+from pydantic import BaseModel, Extra
 
 from ..types import PexServerHandle
 from .registry import PexS3Registry
 
 
-class PexProcessEntry(
-    NamedTuple(
-        "_PexProcessEntry",
-        [
-            ("pex_server_handle", PexServerHandle),
-            ("grpc_server_process", subprocess.Popen),
-            ("grpc_client", DagsterGrpcClient),
-            ("heartbeat_shutdown_event", threading.Event),
-            ("heartbeat_thread", threading.Thread),
-        ],
-    )
-):
-    def __new__(
-        cls,
-        pex_server_handle: PexServerHandle,
-        grpc_server_process: subprocess.Popen,
-        grpc_client: DagsterGrpcClient,
-        heartbeat_shutdown_event: threading.Event,
-        heartbeat_thread: threading.Thread,
-    ):
-        return super(PexProcessEntry, cls).__new__(
-            cls,
-            check.inst_param(pex_server_handle, "pex_server_handle", PexServerHandle),
-            check.inst_param(grpc_server_process, "grpc_server_process", subprocess.Popen),
-            check.inst_param(grpc_client, "grpc_client", DagsterGrpcClient),
-            check.inst_param(heartbeat_shutdown_event, "heartbeat_shutdown_event", threading.Event),
-            check.inst_param(heartbeat_thread, "heartbeat_thread", threading.Thread),
-        )
+class PexProcessEntry(BaseModel, frozen=True, extra=Extra.forbid, arbitrary_types_allowed=True):
+    pex_server_handle: PexServerHandle
+    grpc_server_process: subprocess.Popen
+    grpc_client: DagsterGrpcClient
+    heartbeat_shutdown_event: threading.Event
+    heartbeat_thread: threading.Thread
+
+
+class PexErrorEntry(BaseModel, frozen=True, extra=Extra.forbid, arbitrary_types_allowed=True):
+    pex_server_handle: PexServerHandle
+    error: SerializableErrorInfo
 
 
 class MultiPexManager(AbstractContextManager):
     def __init__(
         self,
         local_pex_files_dir: Optional[str] = None,
     ):
         # Keyed by hash of PexServerHandle
-        self._pex_servers: Dict[str, PexProcessEntry] = {}
+        self._pex_servers: Dict[str, Union[PexProcessEntry, PexErrorEntry]] = {}
         self._pending_startup_pex_servers: Set[str] = set()
         self._pending_shutdown_pex_servers: Set[str] = set()
         self._pex_servers_lock = threading.Lock()
         self._heartbeat_ttl = 60
         self._registry = PexS3Registry(local_pex_files_dir)
 
-    def get_pex_grpc_client(self, server_handle: PexServerHandle):
+    def get_pex_grpc_client_or_error(
+        self, server_handle: PexServerHandle
+    ) -> Union[DagsterGrpcClient, SerializableErrorInfo]:
         handle_id = server_handle.get_id()
         with self._pex_servers_lock:
             if handle_id not in self._pex_servers:
                 if handle_id in self._pending_startup_pex_servers:
                     raise Exception("This server is still starting up")
                 else:
                     raise Exception("No server created with the given handle")
 
-            return self._pex_servers[handle_id].grpc_client
+            pex_server_or_error = self._pex_servers[handle_id]
+            if isinstance(pex_server_or_error, PexErrorEntry):
+                return pex_server_or_error.error
+
+            return cast(PexProcessEntry, self._pex_servers[handle_id]).grpc_client
 
-    def get_pex_servers(self, deployment_name, location_name: str) -> List[PexServerHandle]:
+    def get_pex_server_handles(self, deployment_name, location_name: str) -> List[PexServerHandle]:
         with self._pex_servers_lock:
             return [
                 server.pex_server_handle
                 for server in self._pex_servers.values()
                 if server.pex_server_handle.deployment_name == deployment_name
                 and server.pex_server_handle.location_name == location_name
             ]
 
-    def get_all_pex_grpc_clients(self) -> List[DagsterGrpcClient]:
-        with self._pex_servers_lock:
-            return [server.grpc_client for server in self._pex_servers.values()]
-
     def get_all_pex_grpc_clients_map(self) -> Dict[str, DagsterGrpcClient]:
         with self._pex_servers_lock:
             return {
                 server.pex_server_handle.get_id(): server.grpc_client
                 for server in self._pex_servers.values()
+                if isinstance(server, PexProcessEntry)
             }
 
     def is_server_active(self, server_handle_id: str) -> bool:
         """Server is present and not pending shutdown."""
         with self._pex_servers_lock:
             return (
                 server_handle_id in self._pex_servers
                 and server_handle_id not in self._pending_shutdown_pex_servers
+                and isinstance(self._pex_servers[server_handle_id], PexProcessEntry)
             )
 
     def create_pex_server(
         self,
         server_handle: PexServerHandle,
         code_deployment_metadata: CodeDeploymentMetadata,
         instance_ref: Optional[InstanceRef],
     ):
         # install pex files and launch them - do it asynchronously to not block this call
         def _create_pex_server() -> None:
-            pex_executable = self._registry.get_pex_executable(
-                check.not_none(code_deployment_metadata.pex_metadata)
-            )
-            logging.info(
-                "Installed pex executable %s at %s",
-                code_deployment_metadata.pex_metadata,
-                pex_executable.source_path,
-            )
+            try:
+                pex_executable = self._registry.get_pex_executable(
+                    check.not_none(code_deployment_metadata.pex_metadata)
+                )
+                logging.info(
+                    "Installed pex executable %s at %s",
+                    code_deployment_metadata.pex_metadata,
+                    pex_executable.source_path,
+                )
 
-            metadata = code_deployment_metadata
-            logging.info("Launching subprocess %s", pex_executable.source_path)
-            subprocess_args = [
-                pex_executable.source_path,
-                "-m",
-                "dagster",
-                "api",
-                "grpc",
-                "--heartbeat",
-                "--heartbeat-timeout",
-                str(self._heartbeat_ttl),
-            ]
+                metadata = code_deployment_metadata
+                logging.info("Launching subprocess %s", pex_executable.source_path)
+                subprocess_args = [
+                    pex_executable.source_path,
+                    "-m",
+                    "dagster",
+                    "api",
+                    "grpc",
+                    "--heartbeat",
+                    "--heartbeat-timeout",
+                    str(self._heartbeat_ttl),
+                ]
+
+                if seven.IS_WINDOWS:
+                    port = find_free_port()
+                    socket = None
+                else:
+                    port = None
+                    socket = safe_tempfile_path_unmanaged()
 
-            if seven.IS_WINDOWS:
-                port = find_free_port()
-                socket = None
-            else:
-                port = None
-                socket = safe_tempfile_path_unmanaged()
-
-            additional_env = metadata.get_grpc_server_env(
-                port=port,
-                location_name=server_handle.location_name,
-                instance_ref=instance_ref,
-                socket=socket,
-            )
+                additional_env = metadata.get_grpc_server_env(
+                    port=port,
+                    location_name=server_handle.location_name,
+                    instance_ref=instance_ref,
+                    socket=socket,
+                )
 
-            server_process = open_ipc_subprocess(
-                subprocess_args,
-                env={
-                    **os.environ.copy(),
-                    **pex_executable.environ,
-                    **additional_env,
-                },
-                cwd=pex_executable.working_directory,
-            )
+                server_process = open_ipc_subprocess(
+                    subprocess_args,
+                    env={
+                        **os.environ.copy(),
+                        **pex_executable.environ,
+                        **additional_env,
+                    },
+                    cwd=pex_executable.working_directory,
+                )
 
-            client = DagsterGrpcClient(
-                port=port,
-                socket=socket,
-                host="localhost",
-                use_ssl=False,
-            )
+                client = DagsterGrpcClient(
+                    port=port,
+                    socket=socket,
+                    host="localhost",
+                    use_ssl=False,
+                )
 
-            heartbeat_shutdown_event = threading.Event()
-            heartbeat_thread = threading.Thread(
-                target=client_heartbeat_thread,
-                args=(client, heartbeat_shutdown_event),
-            )
-            heartbeat_thread.daemon = True
-            heartbeat_thread.start()
+                heartbeat_shutdown_event = threading.Event()
+                heartbeat_thread = threading.Thread(
+                    target=client_heartbeat_thread,
+                    args=(client, heartbeat_shutdown_event),
+                )
+                heartbeat_thread.daemon = True
+                heartbeat_thread.start()
 
-            logging.info("Created a heartbeat thread %s", heartbeat_thread.name)
+                logging.info("Created a heartbeat thread %s", heartbeat_thread.name)
+            except Exception:
+                with self._pex_servers_lock:
+                    self._pex_servers[server_handle.get_id()] = PexErrorEntry(
+                        pex_server_handle=server_handle,
+                        error=serializable_error_info_from_exc_info(sys.exc_info()),
+                    )
+                    self._pending_startup_pex_servers.remove(server_handle.get_id())
+                logging.exception(
+                    "Creating new pex server for %s:%s failed",
+                    server_handle.deployment_name,
+                    server_handle.location_name,
+                )
+                return
 
-            # open question - how do we know when to spin down old pexes / how do you reload a pex
-            # in a zero-downtime way (very similar questions to the process agent really)
-            # we probably want a TTL on these subprocesses
             with self._pex_servers_lock:
                 self._pex_servers[server_handle.get_id()] = PexProcessEntry(
                     pex_server_handle=server_handle,
                     grpc_server_process=server_process,
                     grpc_client=client,
                     heartbeat_shutdown_event=heartbeat_shutdown_event,
                     heartbeat_thread=heartbeat_thread,
@@ -220,14 +221,19 @@
             # request shutdown for processes that we have not tried to shutdown yet
             for handle_id in self._pending_shutdown_pex_servers:
                 pex_server = self._pex_servers.get(handle_id)
                 if not pex_server:
                     # still in _pending_startup_pex_servers
                     logging.info("Server %s not up yet, will request shutdown later", handle_id)
                     continue
+
+                if isinstance(pex_server, PexErrorEntry):
+                    logging.info("Server %s was in an error state, no shutdown needed", handle_id)
+                    continue
+
                 if pex_server.heartbeat_shutdown_event.is_set():
                     # already requested shutdown
                     logging.info("Already requested shutdown for server %s", handle_id)
                     continue
 
                 logging.info("Requesting shutdown for server %s", handle_id)
                 pex_server.heartbeat_shutdown_event.set()
@@ -236,18 +242,20 @@
                     pex_server.grpc_client.shutdown_server()
                 except DagsterUserCodeUnreachableError:
                     # Server already shutdown
                     pass
 
     def __exit__(self, exception_type, exception_value, traceback):
         for _handle, pex_server in self._pex_servers.items():
-            pex_server.heartbeat_shutdown_event.set()
-            pex_server.heartbeat_thread.join()
+            if isinstance(pex_server, PexProcessEntry):
+                pex_server.heartbeat_shutdown_event.set()
+                pex_server.heartbeat_thread.join()
 
         for _handle, pex_server in self._pex_servers.items():
-            try:
-                pex_server.grpc_client.shutdown_server()
-            except DagsterUserCodeUnreachableError:
-                # Server already shutdown
-                pass
-            if pex_server.grpc_server_process.poll() is None:
-                pex_server.grpc_server_process.communicate(timeout=30)
+            if isinstance(pex_server, PexProcessEntry):
+                try:
+                    pex_server.grpc_client.shutdown_server()
+                except DagsterUserCodeUnreachableError:
+                    # Server already shutdown
+                    pass
+                if pex_server.grpc_server_process.poll() is None:
+                    pex_server.grpc_server_process.communicate(timeout=30)
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/registry.py` & `dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DEFAULT_PEX_FILES_DIR = "/tmp/pex-files"
 
 
 def _download_from_s3(filename: str, local_filepath: str):
     # Lazy import boto3 to avoid a hard dependency during module load
     import boto3
 
-    s3 = boto3.client("s3")
+    s3 = boto3.client("s3", region_name="us-west-2")
 
     # TODO: move the bucket and prefix to pex_metdata
     s3_bucket_name = os.environ["DAGSTER_CLOUD_SERVERLESS_STORAGE_S3_BUCKET"]
     # prefix is typically org-storage/{org_public_id}
     s3_prefix = os.environ["DAGSTER_CLOUD_SERVERLESS_STORAGE_S3_PREFIX"]
 
     s3_key = f"{s3_prefix}/pex/{filename}"
@@ -155,16 +155,16 @@
 
     def venv_for(self, pex_filepath) -> PexVenv:
         _, pex_filename = os.path.split(pex_filepath)
         venv_dir = self.venv_dir_for(pex_filepath)
         if os.path.exists(venv_dir):
             logging.info("Reusing existing venv %r for %r", venv_dir, pex_filepath)
         else:
-            installed = self.install_venv(venv_dir, pex_filepath)
-            if not installed or not os.path.exists(venv_dir):
+            self.install_venv(venv_dir, pex_filepath)
+            if not os.path.exists(venv_dir):
                 raise PexInstallationError("Could not install venv", pex_filepath)
         venv_path = Path(venv_dir).absolute()
         return PexVenv(
             path=venv_path,
             site_packages=self.get_site_packages_dir_for_venv(venv_path),
             bin=venv_path / "bin",
             entrypoint=venv_path / "pex",
@@ -173,15 +173,15 @@
 
     def venv_dir_for(self, pex_filepath: str):
         # Use a short name for better stack traces
         short_hash = hashlib.shake_256(pex_filepath.encode("utf-8")).hexdigest(6)
         venv_root = os.getenv("VENVS_ROOT", "/venvs")
         return os.path.join(venv_root, short_hash)
 
-    def install_venv(self, venv_dir: str, pex_filepath: str) -> bool:
+    def install_venv(self, venv_dir: str, pex_filepath: str):
         # Unpacks the pex file into a venv at venv_dir
         try:
             subprocess.check_output(
                 [
                     "pex-tools",
                     pex_filepath,
                     "venv",
@@ -190,28 +190,24 @@
                     "--collisions-ok",
                     # since we combine multiple venvs, we need non hermetic scripts
                     "--non-hermetic-scripts",
                     venv_dir,
                 ],
                 stderr=subprocess.STDOUT,
             )
-        except subprocess.CalledProcessError as err:
+        except subprocess.CalledProcessError as e:
             shutil.rmtree(venv_dir, ignore_errors=True)  # don't leave invalid dir behind
-            logging.exception(
-                "Failure to unpack pex file %r into a venv: %r",
-                pex_filepath,
-                err.output,
-            )
-            return False
+            raise PexInstallationError(
+                f"Could not install venv. Pex output: {e.output}", pex_filepath
+            ) from e
         logging.info(
             "Unpacked pex file %r into venv at %r",
             pex_filepath,
             venv_dir,
         )
-        return True
 
     def get_site_packages_dir_for_venv(self, venv_path: Path) -> Path:
         python = venv_path / "bin" / "python3"
         proc = subprocess.run(
             [python, "-c", "import site; print(site.getsitepackages()[0])"],
             capture_output=True,
             check=False,
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/pex/grpc/server/server.py` & `dagster_cloud-1.3.8/dagster_cloud/pex/grpc/server/server.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     DagsterApiServicer,
     add_DagsterApiServicer_to_server,
 )
 from dagster._grpc.server import server_termination_target
 from dagster._grpc.types import GetCurrentRunsResult
 from dagster._grpc.utils import max_rx_bytes, max_send_bytes
 from dagster._serdes import deserialize_value, serialize_value
-from dagster._utils.error import serializable_error_info_from_exc_info
+from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from grpc_health.v1 import health, health_pb2, health_pb2_grpc
 
 from ..__generated__ import multi_pex_api_pb2
 from ..__generated__.multi_pex_api_pb2_grpc import (
     MultiPexApiServicer,
     add_MultiPexApiServicer_to_server,
 )
@@ -66,15 +66,15 @@
         return multi_pex_api_pb2.CreatePexServerReply(
             create_pex_server_response=serialize_value(response)
         )
 
     def GetPexServers(self, request, _context):
         get_pex_servers_args = deserialize_value(request.get_pex_servers_args, GetPexServersArgs)
         try:
-            pex_server_handles = self._pex_manager.get_pex_servers(
+            pex_server_handles = self._pex_manager.get_pex_server_handles(
                 get_pex_servers_args.deployment_name,
                 get_pex_servers_args.location_name,
             )
             response = GetPexServersResponse(server_handles=pex_server_handles)
         except:
             response = serializable_error_info_from_exc_info(sys.exc_info())
 
@@ -124,30 +124,54 @@
         return PexServerHandle(
             deployment_name=metadict["deployment"],
             location_name=metadict["location"],
             metadata_update_timestamp=int(metadict["timestamp"]),
         )
 
     def _query(self, api_name: str, request, context):
-        return self._pex_manager.get_pex_grpc_client(  # noqa: SLF001
+        client_or_error = self._pex_manager.get_pex_grpc_client_or_error(
             self._get_handle_from_metadata(context)
-        )._get_response(api_name, request)
+        )
+        if isinstance(client_or_error, SerializableErrorInfo):
+            raise Exception("Server failed to start up, no available client")
+        return client_or_error._get_response(api_name, request)  # noqa: SLF001
 
     def _streaming_query(self, api_name: str, request, context):
-        return self._pex_manager.get_pex_grpc_client(  # noqa: SLF001
+        client_or_error = self._pex_manager.get_pex_grpc_client_or_error(
             self._get_handle_from_metadata(context)
-        )._get_streaming_response(api_name, request)
+        )
+        if isinstance(client_or_error, SerializableErrorInfo):
+            raise Exception("Server failed to start up, no available client")
+        return client_or_error._get_streaming_response(api_name, request)  # noqa: SLF001
 
     def ExecutionPlanSnapshot(self, request, context):
         return self._query("ExecutionPlanSnapshot", request, context)
 
     def ListRepositories(self, request, context):
-        return self._query("ListRepositories", request, context)
+        client_or_error = self._pex_manager.get_pex_grpc_client_or_error(
+            self._get_handle_from_metadata(context)
+        )
+        if isinstance(client_or_error, SerializableErrorInfo):
+            return api_pb2.ListRepositoriesReply(
+                serialized_list_repositories_response_or_error=serialize_value(client_or_error)
+            )
+        return client_or_error._get_response("ListRepositories", request)  # noqa: SLF001
 
     def Ping(self, request, context):
+        client_or_error = self._pex_manager.get_pex_grpc_client_or_error(
+            self._get_handle_from_metadata(context)
+        )
+        # This is hacky, but if the server failed to start up, it's 'ready' in the sense that it
+        # will return an error as soon as ListRepositories is called, even though the server
+        # can't serve requests. TODO Find a better way to model that in a backwards compatible way
+        # so that _wait_for_dagster_server_process returns immediately
+        if isinstance(client_or_error, SerializableErrorInfo):
+            echo = request.echo
+            return api_pb2.PingReply(echo=echo)
+
         return self._query("Ping", request, context)
 
     def GetServerId(self, request, context):
         return self._query("GetServerId", request, context)
 
     def GetCurrentImage(self, request, context):
         return self._query("GetCurrentImage", request, context)
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/pex/grpc/types.py` & `dagster_cloud-1.3.8/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/secrets/loader.py` & `dagster_cloud-1.3.8/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/serverless/io_manager.py` & `dagster_cloud-1.3.8/dagster_cloud/serverless/io_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     @property
     def _s3(self):
         if self._boto_session_expiration <= datetime.datetime.now(
             self._boto_session_expiration.tzinfo
         ) + datetime.timedelta(minutes=5):
             self._boto_session, self._boto_session_expiration = self._refresh_boto_session()
-        return self._boto_session.client("s3")
+        return self._boto_session.client("s3", region_name="us-west-2")
 
     def _get_path(self, context: Union[InputContext, OutputContext]) -> str:
         path: Sequence[str]
         if context.has_asset_key:
             path = context.get_asset_identifier()
         else:
             path = ["storage", *context.get_identifier()]
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/storage/client.py` & `dagster_cloud-1.3.8/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster_cloud-1.3.8/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence
 
 import dagster._seven as _seven
 import requests
 from dagster import (
     Field,
+    IntSource,
     StringSource,
     _check as check,
 )
 from dagster._core.storage.cloud_storage_compute_log_manager import CloudStorageComputeLogManager
 from dagster._core.storage.compute_log_manager import ComputeIOType
 from dagster._core.storage.local_compute_log_manager import (
     IO_TYPE_EXTENSION,
@@ -26,49 +27,52 @@
 
 class CloudComputeLogManager(
     CloudStorageComputeLogManager["DagsterCloudAgentInstance"], ConfigurableClass
 ):
     def __init__(
         self,
         local_dir=None,
+        upload_interval=None,
         inst_data=None,
     ):
         # proxy calls to local compute log manager (for subscriptions, etc)
         if not local_dir:
             local_dir = _seven.get_system_temp_directory()
 
         self._upload_session = requests.Session()
         adapter = HTTPAdapter(max_retries=3)
         self._upload_session.mount("http://", adapter)
         self._upload_session.mount("https://", adapter)
 
         self._local_manager = LocalComputeLogManager(local_dir)
+        self._upload_interval = check.opt_int_param(upload_interval, "upload_interval")
         self._inst_data = check.opt_inst_param(inst_data, "inst_data", ConfigurableClassData)
 
     @property
     def inst_data(self):
         return self._inst_data
 
     @classmethod
     def config_type(cls):
         return {
             "local_dir": Field(StringSource, is_required=False),
+            "upload_interval": Field(IntSource, is_required=False),
         }
 
     @classmethod
     def from_config_value(cls, inst_data: ConfigurableClassData, config_value: Any) -> Self:
         return CloudComputeLogManager(inst_data=inst_data, **config_value)
 
     @property
     def local_manager(self) -> LocalComputeLogManager:
         return self._local_manager
 
     @property
     def upload_interval(self) -> Optional[int]:
-        return None
+        return self._upload_interval
 
     def delete_logs(
         self, log_key: Optional[Sequence[str]] = None, prefix: Optional[Sequence[str]] = None
     ):
         raise NotImplementedError("User Agent should not need to delete compute logs")
 
     def download_url_for_type(self, log_key: Sequence[str], io_type: ComputeIOType):
@@ -82,17 +86,15 @@
     ) -> bool:
         """Returns whether the cloud storage contains logs for a given log key."""
         return False
 
     def upload_to_cloud_storage(
         self, log_key: Sequence[str], io_type: ComputeIOType, partial=False
     ):
-        path = self.local_manager.get_captured_local_path(
-            log_key, IO_TYPE_EXTENSION[io_type], partial=partial
-        )
+        path = self.local_manager.get_captured_local_path(log_key, IO_TYPE_EXTENSION[io_type])
         ensure_file(path)
         params: Dict[str, Any] = {
             "log_key": log_key,
             "io_type": io_type.value,
             # for back-compat
             "run_id": log_key[0],
             "key": log_key[-1],
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/storage/event_logs/queries.py` & `dagster_cloud-1.3.8/dagster_cloud/storage/event_logs/queries.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 }
 """
 
 PYTHON_ERROR_FRAGMENT = """
 fragment PythonErrorFragment on PythonError {
   __typename
   message
+  className
   stack
   cause {
     message
     stack
   }
 }
 """
@@ -414,7 +415,96 @@
         eventLogs {
             DeleteDynamicPartition(partitionsDefName: $partitionsDefName, partitionKey: $partitionKey) {
                 ok
             }
         }
     }
 """
+
+SET_CONCURRENCY_SLOTS_MUTATION = (
+    PYTHON_ERROR_FRAGMENT
+    + """
+mutation SetConcurrencySlots($concurrencyKey: String!, $num: Int!) {
+    eventLogs {
+        SetConcurrencySlots(concurrencyKey: $concurrencyKey, num: $num) {
+            success
+            error {
+                ...PythonErrorFragment
+            }
+        }
+    }
+}
+"""
+)
+
+GET_CONCURRENCY_KEYS_QUERY = """
+query getConcurrencyKeys {
+    eventLogs {
+        getConcurrencyKeys
+    }
+}
+"""
+
+GET_CONCURRENCY_INFO_QUERY = """
+query getConcurrencyInfo($concurrencyKey: String!) {
+    eventLogs {
+        getConcurrencyInfo(concurrencyKey: $concurrencyKey) {
+            concurrencyKey
+            slotCount
+            activeSlotCount
+            activeRunIds
+            pendingStepCount
+            pendingStepRunIds
+            assignedStepCount
+            assignedStepRunIds
+        }
+    }
+}
+"""
+
+CLAIM_CONCURRENCY_SLOT_MUTATION = """
+mutation ClaimConcurrencySlot($concurrencyKey: String!, $runId: String!, $stepKey: String!, $priority: Int!) {
+    eventLogs {
+        ClaimConcurrencySlot(concurrencyKey: $concurrencyKey, runId: $runId, stepKey: $stepKey, priority: $priority) {
+            status {
+                slotStatus
+                priority
+                assignedTimestamp
+                enqueuedTimestamp
+            }
+        }
+    }
+}
+"""
+
+CHECK_CONCURRENCY_CLAIM_QUERY = """
+query getCheckConcurrencyClaim($concurrencyKey: String!, $runId: String!, $stepKey: String!) {
+    eventLogs {
+        getCheckConcurrencyClaim(concurrencyKey: $concurrencyKey, runId: $runId, stepKey: $stepKey) {
+            slotStatus
+            priority
+            assignedTimestamp
+            enqueuedTimestamp
+        }
+    }
+}
+"""
+
+FREE_CONCURRENCY_SLOTS_FOR_RUN_MUTATION = """
+mutation FreeConcurrencySlotsForRun($runId: String!) {
+    eventLogs {
+        FreeConcurrencySlotsForRun(runId: $runId) {
+            success
+        }
+    }
+}
+"""
+
+FREE_CONCURRENCY_SLOT_FOR_STEP_MUTATION = """
+mutation FreeConcurrencySlotForStep($runId: String!, $stepKey: String!) {
+    eventLogs {
+        FreeConcurrencySlotForStep(runId: $runId, stepKey: $stepKey) {
+            success
+        }
+    }
+}
+"""
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/storage/event_logs/storage.py` & `dagster_cloud-1.3.8/dagster_cloud/storage/event_logs/storage.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Tuple,
     Union,
     cast,
 )
 from uuid import uuid4
 
 import dagster._check as check
+from dagster import DagsterInvalidInvocationError
 from dagster._core.assets import AssetDetails
 from dagster._core.definitions.events import AssetKey, ExpectationResult
 from dagster._core.event_api import EventLogRecord, EventRecordsFilter, RunShardedEventsCursor
 from dagster._core.events import DagsterEvent, DagsterEventType
 from dagster._core.events.log import EventLogEntry
 from dagster._core.execution.stats import RunStepKeyStatsSnapshot, RunStepMarker, StepEventStatus
 from dagster._core.storage.dagster_run import DagsterRunStatsSnapshot
@@ -33,44 +34,56 @@
 from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
 from dagster._serdes import (
     ConfigurableClass,
     ConfigurableClassData,
     serialize_value,
 )
 from dagster._serdes.serdes import deserialize_value
-from dagster._utils import datetime_as_float
+from dagster._utils import datetime_as_float, utc_datetime_from_timestamp
+from dagster._utils.concurrency import (
+    ConcurrencyClaimStatus,
+    ConcurrencyKeyInfo,
+    ConcurrencySlotStatus,
+)
 from dagster._utils.error import SerializableErrorInfo
 from dagster._utils.merger import merge_dicts
 from dagster_cloud_cli.core.errors import GraphQLStorageError
 from typing_extensions import Self
 
 from dagster_cloud.storage.event_logs.utils import truncate_event
 
 from .queries import (
     ADD_DYNAMIC_PARTITIONS_MUTATION,
+    CHECK_CONCURRENCY_CLAIM_QUERY,
+    CLAIM_CONCURRENCY_SLOT_MUTATION,
     DELETE_DYNAMIC_PARTITION_MUTATION,
     DELETE_EVENTS_MUTATION,
     ENABLE_SECONDARY_INDEX_MUTATION,
+    FREE_CONCURRENCY_SLOT_FOR_STEP_MUTATION,
+    FREE_CONCURRENCY_SLOTS_FOR_RUN_MUTATION,
     GET_ALL_ASSET_KEYS_QUERY,
     GET_ASSET_RECORDS_QUERY,
     GET_ASSET_RUN_IDS_QUERY,
+    GET_CONCURRENCY_INFO_QUERY,
+    GET_CONCURRENCY_KEYS_QUERY,
     GET_DYNAMIC_PARTITIONS_QUERY,
     GET_EVENT_RECORDS_QUERY,
     GET_EVENT_TAGS_FOR_ASSET,
     GET_LATEST_ASSET_PARTITION_MATERIALIZATION_ATTEMPTS_WITHOUT_MATERIALIZATIONS,
     GET_LATEST_MATERIALIZATION_EVENTS_QUERY,
     GET_MATERIALIZATION_COUNT_BY_PARTITION,
     GET_RECORDS_FOR_RUN_QUERY,
     GET_STATS_FOR_RUN_QUERY,
     GET_STEP_STATS_FOR_RUN_QUERY,
     HAS_ASSET_KEY_QUERY,
     HAS_DYNAMIC_PARTITION_QUERY,
     IS_ASSET_AWARE_QUERY,
     IS_PERSISTENT_QUERY,
     REINDEX_MUTATION,
+    SET_CONCURRENCY_SLOTS_MUTATION,
     STORE_EVENT_MUTATION,
     UPDATE_ASSET_CACHED_STATUS_DATA_MUTATION,
     UPGRADE_EVENT_LOG_STORAGE_MUTATION,
     WIPE_ASSET_CACHED_STATUS_DATA_MUTATION,
     WIPE_ASSET_MUTATION,
     WIPE_EVENT_LOG_STORAGE_MUTATION,
 )
@@ -681,7 +694,125 @@
         )
 
     def wipe_asset(self, asset_key: AssetKey):
         res = self._execute_query(
             WIPE_ASSET_MUTATION, variables={"assetKey": asset_key.to_string()}
         )
         return res
+
+    @property
+    def supports_global_concurrency_limits(self) -> bool:
+        return True
+
+    def set_concurrency_slots(self, concurrency_key: str, num: int) -> None:
+        check.str_param(concurrency_key, "concurrency_key")
+        check.int_param(num, "num")
+        res = self._execute_query(
+            SET_CONCURRENCY_SLOTS_MUTATION,
+            variables={"concurrencyKey": concurrency_key, "num": num},
+        )
+        result = res["data"]["eventLogs"]["SetConcurrencySlots"]
+        error = result.get("error")
+
+        if error:
+            if error["className"] == "DagsterInvalidInvocationError":
+                raise DagsterInvalidInvocationError(error["message"])
+            else:
+                raise GraphQLStorageError(res)
+        return res
+
+    def get_concurrency_keys(self) -> Set[str]:
+        res = self._execute_query(GET_CONCURRENCY_KEYS_QUERY)
+        return set(res["data"]["eventLogs"]["getConcurrencyKeys"])
+
+    def get_concurrency_info(self, concurrency_key: str) -> ConcurrencyKeyInfo:
+        check.str_param(concurrency_key, "concurrency_key")
+        res = self._execute_query(
+            GET_CONCURRENCY_INFO_QUERY,
+            variables={"concurrencyKey": concurrency_key},
+        )
+        info = res["data"]["eventLogs"]["getConcurrencyInfo"]
+        return ConcurrencyKeyInfo(
+            concurrency_key=concurrency_key,
+            slot_count=info["slotCount"],
+            active_slot_count=info["activeSlotCount"],
+            active_run_ids=set(info["activeRunIds"]),
+            pending_step_count=info["pendingStepCount"],
+            pending_run_ids=set(info["pendingStepRunIds"]),
+            assigned_step_count=info["assignedStepCount"],
+            assigned_run_ids=set(info["assignedStepRunIds"]),
+        )
+
+    def claim_concurrency_slot(
+        self, concurrency_key: str, run_id: str, step_key: str, priority: Optional[int] = None
+    ) -> ConcurrencyClaimStatus:
+        check.str_param(concurrency_key, "concurrency_key")
+        check.str_param(run_id, "run_id")
+        check.str_param(step_key, "step_key")
+        check.opt_int_param(priority, "priority")
+        res = self._execute_query(
+            CLAIM_CONCURRENCY_SLOT_MUTATION,
+            variables={
+                "concurrencyKey": concurrency_key,
+                "runId": run_id,
+                "stepKey": step_key,
+                "priority": priority,
+            },
+        )
+        claim_status = res["data"]["eventLogs"]["ClaimConcurrencySlot"]["status"]
+        return ConcurrencyClaimStatus(
+            concurrency_key=concurrency_key,
+            slot_status=ConcurrencySlotStatus(claim_status["slotStatus"]),
+            priority=claim_status["priority"],
+            assigned_timestamp=utc_datetime_from_timestamp(claim_status["assignedTimestamp"])
+            if claim_status["assignedTimestamp"]
+            else None,
+            enqueued_timestamp=utc_datetime_from_timestamp(claim_status["enqueuedTimestamp"])
+            if claim_status["enqueuedTimestamp"]
+            else None,
+        )
+
+    def check_concurrency_claim(
+        self, concurrency_key: str, run_id: str, step_key: str
+    ) -> ConcurrencyClaimStatus:
+        check.str_param(concurrency_key, "concurrency_key")
+        check.str_param(run_id, "run_id")
+        check.str_param(step_key, "step_key")
+        res = self._execute_query(
+            CHECK_CONCURRENCY_CLAIM_QUERY,
+            variables={
+                "concurrencyKey": concurrency_key,
+                "runId": run_id,
+                "stepKey": step_key,
+            },
+        )
+        claim_status = res["data"]["eventLogs"]["getCheckConcurrencyClaim"]
+        return ConcurrencyClaimStatus(
+            concurrency_key=concurrency_key,
+            slot_status=ConcurrencySlotStatus(claim_status["slotStatus"]),
+            priority=claim_status["priority"],
+            assigned_timestamp=utc_datetime_from_timestamp(claim_status["assignedTimestamp"])
+            if claim_status["assignedTimestamp"]
+            else None,
+            enqueued_timestamp=utc_datetime_from_timestamp(claim_status["enqueuedTimestamp"])
+            if claim_status["enqueuedTimestamp"]
+            else None,
+        )
+
+    def get_concurrency_run_ids(self) -> Set[str]:
+        raise NotImplementedError("Not callable from user cloud")
+
+    def free_concurrency_slots_for_run(self, run_id: str) -> None:
+        check.str_param(run_id, "run_id")
+        res = self._execute_query(
+            FREE_CONCURRENCY_SLOTS_FOR_RUN_MUTATION, variables={"runId": run_id}
+        )
+        return res
+
+    def free_concurrency_slot_for_step(self, run_id: str, step_key: str) -> None:
+        check.str_param(run_id, "run_id")
+        check.opt_str_param(step_key, "step_key")
+        res = self._execute_query(
+            FREE_CONCURRENCY_SLOT_FOR_STEP_MUTATION,
+            variables={"runId": run_id, "stepKey": step_key},
+        )
+        return res
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/storage/event_logs/utils.py` & `dagster_cloud-1.3.8/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/storage/runs/queries.py` & `dagster_cloud-1.3.8/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/storage/runs/storage.py` & `dagster_cloud-1.3.8/dagster_cloud/storage/runs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/storage/schedules/queries.py` & `dagster_cloud-1.3.8/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/storage/schedules/storage.py` & `dagster_cloud-1.3.8/dagster_cloud/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/util/__init__.py` & `dagster_cloud-1.3.8/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/cli/__init__.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/config_schema/__init__.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/config_schema/docker.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/config_schema/ecs.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,14 +96,34 @@
         description="Additional sidecar containers to include in code server task definitions.",
     ),
     "run_sidecar_containers": Field(
         Array(Permissive({})),
         is_required=False,
         description="Additional sidecar containers to include in run task definitions.",
     ),
+    "run_ecs_tags": Field(
+        Array(
+            {
+                "key": Field(StringSource, is_required=True),
+                "value": Field(StringSource, is_required=False),
+            }
+        ),
+        is_required=False,
+        description="Additional tags to apply to the launched ECS task.",
+    ),
+    "server_ecs_tags": Field(
+        Array(
+            {
+                "key": Field(StringSource, is_required=True),
+                "value": Field(StringSource, is_required=False),
+            }
+        ),
+        is_required=False,
+        description="Additional tags to apply to the launched ECS task for a code server.",
+    ),
 }
 
 
 ECS_CONTAINER_CONTEXT_CONFIG = {
     "secrets": Field(
         Noneable(Array(Shape({"name": StringSource, "valueFrom": StringSource}))),
         is_required=False,
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/docker/__init__.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/docker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             DagsterDockerContainer(container=container)
             for container in client.containers.list(
                 all=True,
                 filters={
                     "label": [
                         GRPC_SERVER_LABEL,
                         deterministic_label_for_location(deployment_name, location_name),
-                        self._instance.instance_uuid,
+                        f"{AGENT_LABEL}={self._instance.instance_uuid}",
                     ]
                 },
             )
         ]
 
     def _get_multipex_server_handles_for_location(
         self, deployment_name: str, location_name: str
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/client.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,15 +415,18 @@
         )
         params["networkConfiguration"] = self.network_configuration
 
         if service_registry_arn:
             params["serviceRegistries"] = [{"registryArn": service_registry_arn}]
 
         if tags and self.taggable:
-            params["tags"] = [{"key": key, "value": value} for key, value in tags.items()]
+            params["tags"] = [
+                {"key": key, **({"value": value} if value is not None else {})}
+                for key, value in tags.items()
+            ]
 
         arn = self.ecs.create_service(**params).get("service").get("serviceArn")
 
         return Service(client=self, arn=arn)
 
     def wait_for_new_service(self, service, container_name, logger=None) -> str:
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/launcher.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/launcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     DagsterCloudUserCodeLauncher,
     ServerEndpoint,
 )
 from dagster_cloud.workspace.user_code_launcher.utils import deterministic_label_for_location
 
 from .client import get_debug_ecs_prompt
 from .run_launcher import CloudEcsRunLauncher
-from .utils import get_task_definition_family
+from .utils import get_server_task_definition_family
 
 EcsServerHandleType = Service
 
 CONTAINER_NAME = "dagster"
 PORT = 4000
 
 
@@ -62,14 +62,16 @@
         server_resources: Optional[Mapping[str, Any]] = None,
         run_resources: Optional[Mapping[str, Any]] = None,
         runtime_platform: Optional[Mapping[str, Any]] = None,
         mount_points: Optional[Sequence[Mapping[str, Any]]] = None,
         volumes: Optional[Sequence[Mapping[str, Any]]] = None,
         server_sidecar_containers: Optional[Sequence[Mapping[str, Any]]] = None,
         run_sidecar_containers: Optional[Sequence[Mapping[str, Any]]] = None,
+        server_ecs_tags: Optional[Sequence[Mapping[str, Optional[str]]]] = None,
+        run_ecs_tags: Optional[Sequence[Mapping[str, Optional[str]]]] = None,
         **kwargs,
     ):
         self.ecs = boto3.client("ecs")
         self.logs = boto3.client("logs")
         self.service_discovery = boto3.client("servicediscovery")
         self.secrets_manager = boto3.client("secretsmanager")
 
@@ -119,14 +121,17 @@
         self.server_sidecar_containers = check.opt_sequence_param(
             server_sidecar_containers, "server_sidecar_containers"
         )
         self.run_sidecar_containers = check.opt_sequence_param(
             run_sidecar_containers, "run_sidecar_containers"
         )
 
+        self.server_ecs_tags = check.opt_sequence_param(server_ecs_tags, "server_ecs_tags")
+        self.run_ecs_tags = check.opt_sequence_param(run_ecs_tags, "run_ecs_tags")
+
         self.client = Client(
             cluster_name=self.cluster,
             subnet_ids=self.subnets,
             security_group_ids=security_group_ids,
             service_discovery_namespace_id=self.service_discovery_namespace_id,
             log_group=self.log_group,
             show_debug_cluster_info=self.show_debug_cluster_info,
@@ -311,39 +316,51 @@
             task_role_arn=self.task_role_arn,
             execution_role_arn=self.execution_role_arn,
             runtime_platform=self.runtime_platform,
             mount_points=self.mount_points,
             volumes=self.volumes,
             server_sidecar_containers=self.server_sidecar_containers,
             run_sidecar_containers=self.run_sidecar_containers,
+            server_ecs_tags=self.server_ecs_tags,
+            run_ecs_tags=self.run_ecs_tags,
         ).merge(EcsContainerContext.create_from_config(metadata.container_context))
 
         environment = merge_dicts(
             container_context.get_environment_dict(),
             additional_env,
             self._get_additional_grpc_server_env(),
         )
 
         self._logger.info(f"Creating a new service for {deployment_name}:{location_name}...")
 
-        family = get_task_definition_family(
-            "server", self._instance.organization_name, deployment_name, location_name
+        family = get_server_task_definition_family(
+            self._instance.organization_name, deployment_name, location_name
         )
 
+        system_tags = {**self._get_dagster_tags(deployment_name, location_name), **tags}
+        system_tag_keys = set(system_tags)
+
+        invalid_user_keys = [
+            tag["key"] for tag in container_context.server_ecs_tags if tag["key"] in system_tag_keys
+        ]
+        if invalid_user_keys:
+            raise Exception(f"Cannot override system ECS tags: {', '.join(invalid_user_keys)}")
+
         service = self.client.create_service(
             name=unique_ecs_resource_name(deployment_name, location_name),
             family=family,
             image=metadata.image,
             container_name=CONTAINER_NAME,
             command=command,
             execution_role_arn=container_context.execution_role_arn,
             env=environment,
             tags={
                 **self._get_dagster_tags(deployment_name, location_name),
                 **tags,
+                **{tag["key"]: tag.get("value") for tag in container_context.server_ecs_tags},
             },
             task_role_arn=container_context.task_role_arn,
             secrets=container_context.get_secrets_dict(self.secrets_manager),
             sidecars=self._get_grpc_server_sidecars(container_context),
             logger=self._logger,
             cpu=self._get_service_cpu_override(container_context),
             memory=self._get_service_memory_override(container_context),
@@ -513,14 +530,15 @@
             env_vars=self.env_vars,
             use_current_ecs_task_config=False,
             run_task_kwargs={
                 "cluster": self.cluster,
                 "networkConfiguration": self.client.network_configuration,
                 "launchType": self.launch_type,
             },
+            run_ecs_tags=self.run_ecs_tags,
             container_name=CONTAINER_NAME,
             run_resources=self.run_resources,
         )
 
     def run_launcher(self) -> CloudEcsRunLauncher:
         launcher = CloudEcsRunLauncher(**self._run_launcher_kwargs())
         launcher.register_instance(self._instance)
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/service.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/ecs/utils.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/ecs/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import hashlib
 import re
 from typing import Optional
 
+from dagster._core.host_representation.origin import ExternalJobOrigin
 from dagster_aws.ecs.utils import sanitize_family
 
 from ..user_code_launcher.utils import get_human_readable_label, unique_resource_name
 
 
 def unique_ecs_resource_name(deployment_name, location_name):
     return unique_resource_name(
@@ -20,33 +21,56 @@
     return get_human_readable_label(
         name,
         length_limit=60,  # Service discovery name must satisfy DNS
         sanitize_fn=lambda name: re.sub("[^a-z0-9-]", "", name).strip("-"),
     )
 
 
-def get_task_definition_family(
-    prefix: str,
+def _get_family_hash(name, max_length=32, hash_size=8):
+    m = hashlib.sha1()
+    m.update(name.encode("utf-8"))
+    name_hash = m.hexdigest()[:hash_size]
+    return f"{name[:(max_length-hash_size-1)]}_{name_hash}"
+
+
+def get_server_task_definition_family(
     organization_name: Optional[str],
     deployment_name: str,
     location_name: str,
 ) -> str:
     # Truncate the location name if it's too long (but add a unique suffix at the end so that no matter what it's unique)
     # Relies on the fact that org name and deployment name are always <= 64 characters long to
     # stay well underneath the 255 character limit imposed by ECS
     m = hashlib.sha1()
     m.update(location_name.encode("utf-8"))
-    location_name_hash = m.hexdigest()[:8]
+
+    truncated_location_name = _get_family_hash(location_name, max_length=64)
+
+    final_family = f"server_{organization_name}_{deployment_name}_{truncated_location_name}"
+
+    assert len(final_family) <= 255
+
+    return sanitize_family(final_family)
+
+
+def get_run_task_definition_family(
+    organization_name: Optional[str],
+    deployment_name: str,
+    job_origin: ExternalJobOrigin,
+) -> str:
+    # Truncate the location name if it's too long (but add a unique suffix at the end so that no matter what it's unique)
+    # Relies on the fact that org name and deployment name are always <= 64 characters long to
+    # stay well underneath the 255 character limit imposed by ECS
+    job_name = job_origin.job_name
+    repo_name = job_origin.external_repository_origin.repository_name
+    location_name = job_origin.external_repository_origin.code_location_origin.location_name
 
     assert len(str(organization_name)) <= 64
     assert len(deployment_name) <= 64
-    assert len(prefix) <= 32
 
-    # Make a unique location name that's still under 64 characters
-    truncated_location_name = f"{location_name[:55]}_{location_name_hash}"
-    assert len(truncated_location_name) <= 64
+    # '{16}_{64}_{64}_{32}_{32}_{32}': max 245 characters
 
-    final_family = f"{prefix}_{organization_name}_{deployment_name}_{truncated_location_name}"
+    final_family = f"run_{organization_name}_{deployment_name}_{_get_family_hash(location_name)}_{_get_family_hash(repo_name)}_{_get_family_hash(job_name)}"
 
     assert len(final_family) <= 255
 
     return sanitize_family(final_family)
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/kubernetes/utils.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/origin.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/origin.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster_cloud-1.3.8/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.7/dagster_cloud.egg-info/PKG-INFO` & `dagster_cloud-1.3.8/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.3.7
+Version: 1.3.8
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.7/dagster_cloud.egg-info/SOURCES.txt` & `dagster_cloud-1.3.8/dagster_cloud.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 dagster_cloud/agent/queries.py
 dagster_cloud/agent/cli/__init__.py
 dagster_cloud/api/__init__.py
 dagster_cloud/api/dagster_cloud_api.py
 dagster_cloud/auth/__init__.py
 dagster_cloud/auth/constants.py
 dagster_cloud/execution/__init__.py
-dagster_cloud/execution/cloud_run_launcher/__init__.py
-dagster_cloud/execution/cloud_run_launcher/k8s.py
-dagster_cloud/execution/cloud_run_launcher/process.py
 dagster_cloud/execution/monitoring/__init__.py
 dagster_cloud/execution/utils/__init__.py
 dagster_cloud/execution/utils/process.py
 dagster_cloud/instance/__init__.py
 dagster_cloud/pex/__init__.py
 dagster_cloud/pex/grpc/__init__.py
 dagster_cloud/pex/grpc/client.py
```

### Comparing `dagster_cloud-1.3.7/setup.py` & `dagster_cloud-1.3.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.7",
-        "dagster-cloud-cli==1.3.7",
+        "dagster==1.3.8",
+        "dagster-cloud-cli==1.3.8",
         "pex",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -58,19 +58,19 @@
             "mypy",
             "paramiko",
             "pylint",
             "pytest",
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
-            "dagster_k8s==0.19.7",
+            "dagster_k8s==0.19.8",
         ],
-        "docker": ["docker", "dagster_docker==0.19.7"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.19.7"],
-        "ecs": ["dagster_aws==0.19.7", "boto3"],
+        "docker": ["docker", "dagster_docker==0.19.8"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.19.8"],
+        "ecs": ["dagster_aws==0.19.8", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

