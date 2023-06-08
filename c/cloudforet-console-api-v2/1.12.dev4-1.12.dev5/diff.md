# Comparing `tmp/cloudforet-console-api-v2-1.12.dev4.tar.gz` & `tmp/cloudforet-console-api-v2-1.12.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudforet-console-api-v2-1.12.dev4.tar", last modified: Wed May 10 09:25:40 2023, max compression
+gzip compressed data, was "cloudforet-console-api-v2-1.12.dev5.tar", last modified: Thu Jun  8 09:04:33 2023, max compression
```

## Comparing `cloudforet-console-api-v2-1.12.dev4.tar` & `cloudforet-console-api-v2-1.12.dev5.tar`

### file list

```diff
@@ -1,135 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.264825 cloudforet-console-api-v2-1.12.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.252825 cloudforet-console-api-v2-1.12.dev4/cloudforet/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.252825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.252825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/conf/global_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/conf/router_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.252825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/error/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/error/cloudforet.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/error/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.252825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.252825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.252825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/budget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/budget_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/cost_query_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/custom_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/data_source_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/job_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/public_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/user_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.252825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/dashboard/custom_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/dashboard/domain_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/dashboard/project_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.252825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/extension/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.256825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/domain_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/project_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.256825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/change_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/cloud_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/cloud_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/job_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/resource_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.256825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/notification_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/project_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/quota.py
--rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.256825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/repository/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/repository/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/repository/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/repository/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.256825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/cloudforet_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/resource_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/resource_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/resource_manager/cost_analysis_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/resource_manager/inventory_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/cost_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/cost_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/cost_analysis/cost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/dashboard/custom_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/dashboard/domain_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/dashboard/project_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/extension/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/identity/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/identity/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/identity/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/change_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/cloud_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/cloud_service_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/region.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/repository/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/repository/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/repository/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/repository/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/repository/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/service/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/service/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/service/common/proxy_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/service/extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/service/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/service/extension/resource_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:25:40.260825 cloudforet-console-api-v2-1.12.dev4/cloudforet_console_api_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-10 09:25:40.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet_console_api_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-10 09:25:40.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet_console_api_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:25:40.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet_console_api_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:25:40.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet_console_api_v2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 09:25:40.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet_console_api_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-10 09:25:40.000000 cloudforet-console-api-v2-1.12.dev4/cloudforet_console_api_v2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 09:25:40.264825 cloudforet-console-api-v2-1.12.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-10 09:25:27.000000 cloudforet-console-api-v2-1.12.dev4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.692668 cloudforet-console-api-v2-1.12.dev5/cloudforet/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.692668 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.692668 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/conf/global_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/conf/router_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.692668 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/error/cloudforet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/error/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.696668 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.696668 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.700667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/budget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/budget_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/cost_query_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/custom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/data_source_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/job_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/public_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/user_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.700667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/dashboard/custom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/dashboard/domain_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/dashboard/project_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.700667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/extension/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.700667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/domain_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/project_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.700667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/change_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/cloud_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/cloud_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/job_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/resource_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.700667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/notification_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/project_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.700667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/repository/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/repository/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/repository/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/repository/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/cloudforet_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/resource_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/resource_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/resource_manager/cost_analysis_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/resource_manager/inventory_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/cost_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/cost_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/cost_analysis/cost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/dashboard/custom_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/dashboard/domain_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/dashboard/project_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/extension/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/identity/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/identity/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/identity/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/change_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/cloud_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/cloud_service_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/region.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/repository/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/repository/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/repository/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/repository/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/service/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/service/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/service/common/proxy_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/service/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/service/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/service/extension/resource_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/cloudforet_console_api_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 09:04:33.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet_console_api_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-08 09:04:33.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet_console_api_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:04:33.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet_console_api_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:04:33.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet_console_api_v2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 09:04:33.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet_console_api_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 09:04:33.000000 cloudforet-console-api-v2-1.12.dev5/cloudforet_console_api_v2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:04:33.704667 cloudforet-console-api-v2-1.12.dev5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-08 09:04:20.000000 cloudforet-console-api-v2-1.12.dev5/setup.py
```

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/conf/global_conf.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/conf/router_conf.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/conf/router_conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,9 +330,16 @@
     },
     {
         'router_path': 'cloudforet.console_api_v2.interface.rest.dashboard.custom_widget:router',
         'router_options': {
             'prefix': '/dashboard/custom-widget',
             'tags': ['dashboard > custom-widget'],
         }
+    },
+    {
+        'router_path': 'cloudforet.console_api_v2.interface.rest.plugin.plugin:router',
+        'router_options': {
+            'prefix': '/plugin/plugin',
+            'tags': ['plugin > plugin'],
+        }
     }
 ]
```

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/budget.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/budget.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/budget_usage.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/budget_usage.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/cost.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/cost.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/cost_query_set.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/cost_query_set.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/custom_widget.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/custom_widget.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/data_source.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/data_source.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/data_source_rule.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/data_source_rule.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/exchange_rate.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/job.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/job.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/job_task.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/job_task.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/public_dashboard.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/public_dashboard.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/cost_analysis/user_dashboard.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/cost_analysis/user_dashboard.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/dashboard/custom_widget.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/dashboard/custom_widget.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/dashboard/domain_dashboard.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/dashboard/domain_dashboard.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/dashboard/project_dashboard.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/dashboard/project_dashboard.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/extension/resource.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/extension/resource.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/api_key.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/api_key.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/domain.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/domain.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/domain_owner.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/domain_owner.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/endpoint.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/endpoint.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/policy.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/policy.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/project.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/project.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/project_group.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/project_group.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/provider.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/provider.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/role.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/role.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/role_binding.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/role_binding.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/service_account.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/service_account.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/token.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/token.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/identity/user.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/identity/user.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/change_history.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/change_history.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/cloud_service.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/cloud_service.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/cloud_service_type.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/cloud_service_type.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/collector.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/collector.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/job.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/note.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,46 +9,64 @@
 _LOGGER = logging.getLogger(__name__)
 _AUTH_SCHEME = HTTPBearer()
 
 router = InferringRouter()
 
 
 @cbv(router)
-class Job(BaseAPI):
+class Note(BaseAPI):
     token: HTTPAuthorizationCredentials = Depends(_AUTH_SCHEME)
     service = 'console-api'
 
+    @router.post('/create')
+    @exception_handler
+    async def create(self, request: Request, body: dict = Body(...)):
+        params, metadata = await self.parse_request(request, self.token.credentials)
+
+        with self.locator.get_service(ProxyService, metadata) as proxy_service:
+            params['grpc_method'] = 'inventory.Note.create'
+            return proxy_service.dispatch_api(params)
+
+    @router.post('/update')
+    @exception_handler
+    async def update(self, request: Request):
+        params, metadata = await self.parse_request(request, self.token.credentials)
+
+        with self.locator.get_service(ProxyService, metadata) as proxy_service:
+            params['grpc_method'] = 'inventory.Note.update'
+            return proxy_service.dispatch_api(params)
+
     @router.post('/delete')
     @exception_handler
     async def delete(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.Job.delete'
+            params['grpc_method'] = 'inventory.Note.delete'
             return proxy_service.dispatch_api(params)
 
     @router.post('/get')
     @exception_handler
     async def get(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.Job.get'
+            params['grpc_method'] = 'inventory.Note.get'
             return proxy_service.dispatch_api(params)
 
     @router.post('/list')
     @exception_handler
     async def list(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.Job.list'
+            params['grpc_method'] = 'inventory.Note.list'
             return proxy_service.dispatch_api(params)
 
     @router.post('/stat')
     @exception_handler
     async def stat(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.Job.stat'
+            params['grpc_method'] = 'inventory.Note.stat'
             return proxy_service.dispatch_api(params)
```

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/job_task.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/job_task.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/note.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/resource_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,64 +9,64 @@
 _LOGGER = logging.getLogger(__name__)
 _AUTH_SCHEME = HTTPBearer()
 
 router = InferringRouter()
 
 
 @cbv(router)
-class Note(BaseAPI):
+class ResourceGroup(BaseAPI):
     token: HTTPAuthorizationCredentials = Depends(_AUTH_SCHEME)
     service = 'console-api'
 
     @router.post('/create')
     @exception_handler
     async def create(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.Note.create'
+            params['grpc_method'] = 'inventory.ResourceGroup.create'
             return proxy_service.dispatch_api(params)
 
     @router.post('/update')
     @exception_handler
     async def update(self, request: Request):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.Note.update'
+            params['grpc_method'] = 'inventory.ResourceGroup.update'
             return proxy_service.dispatch_api(params)
 
     @router.post('/delete')
     @exception_handler
     async def delete(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.Note.delete'
+            params['grpc_method'] = 'inventory.ResourceGroup.delete'
             return proxy_service.dispatch_api(params)
 
     @router.post('/get')
     @exception_handler
     async def get(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.Note.get'
+            params['grpc_method'] = 'inventory.ResourceGroup.get'
             return proxy_service.dispatch_api(params)
 
     @router.post('/list')
     @exception_handler
     async def list(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.Note.list'
+            params['grpc_method'] = 'inventory.ResourceGroup.list'
             return proxy_service.dispatch_api(params)
 
     @router.post('/stat')
     @exception_handler
     async def stat(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.Note.stat'
+            params['grpc_method'] = 'inventory.ResourceGroup.stat'
             return proxy_service.dispatch_api(params)
```

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/region.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/region.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/inventory/resource_group.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/notification.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,64 +9,64 @@
 _LOGGER = logging.getLogger(__name__)
 _AUTH_SCHEME = HTTPBearer()
 
 router = InferringRouter()
 
 
 @cbv(router)
-class ResourceGroup(BaseAPI):
+class Notification(BaseAPI):
     token: HTTPAuthorizationCredentials = Depends(_AUTH_SCHEME)
     service = 'console-api'
 
     @router.post('/create')
     @exception_handler
-    async def create(self, request: Request, body: dict = Body(...)):
+    async def create(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.ResourceGroup.create'
+            params['grpc_method'] = 'notification.Notification.create'
             return proxy_service.dispatch_api(params)
 
-    @router.post('/update')
+    @router.post('/delete')
     @exception_handler
-    async def update(self, request: Request):
+    async def delete(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.ResourceGroup.update'
+            params['grpc_method'] = 'notification.Notification.delete'
             return proxy_service.dispatch_api(params)
 
-    @router.post('/delete')
+    @router.post('/set-read')
     @exception_handler
-    async def delete(self, request: Request, body: dict = Body(...)):
+    async def set_read(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.ResourceGroup.delete'
+            params['grpc_method'] = 'notification.Notification.set_read'
             return proxy_service.dispatch_api(params)
 
     @router.post('/get')
     @exception_handler
-    async def get(self, request: Request, body: dict = Body(...)):
+    async def get(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.ResourceGroup.get'
+            params['grpc_method'] = 'notification.Notification.get'
             return proxy_service.dispatch_api(params)
 
     @router.post('/list')
     @exception_handler
-    async def list(self, request: Request, body: dict = Body(...)):
+    async def list(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.ResourceGroup.list'
+            params['grpc_method'] = 'notification.Notification.list'
             return proxy_service.dispatch_api(params)
 
     @router.post('/stat')
     @exception_handler
-    async def stat(self, request: Request, body: dict = Body(...)):
+    async def stat(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'inventory.ResourceGroup.stat'
+            params['grpc_method'] = 'notification.Notification.stat'
             return proxy_service.dispatch_api(params)
```

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/notification.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/quota.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,64 +9,64 @@
 _LOGGER = logging.getLogger(__name__)
 _AUTH_SCHEME = HTTPBearer()
 
 router = InferringRouter()
 
 
 @cbv(router)
-class Notification(BaseAPI):
+class Quota(BaseAPI):
     token: HTTPAuthorizationCredentials = Depends(_AUTH_SCHEME)
     service = 'console-api'
 
     @router.post('/create')
     @exception_handler
     async def create(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Notification.create'
+            params['grpc_method'] = 'notification.Quota.create'
             return proxy_service.dispatch_api(params)
 
-    @router.post('/delete')
+    @router.post('/update')
     @exception_handler
-    async def delete(self, request: Request, body: dict = Body()):
+    async def update(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Notification.delete'
+            params['grpc_method'] = 'notification.Quota.update'
             return proxy_service.dispatch_api(params)
 
-    @router.post('/set-read')
+    @router.post('/delete')
     @exception_handler
-    async def set_read(self, request: Request, body: dict = Body()):
+    async def delete(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Notification.set_read'
+            params['grpc_method'] = 'notification.Quota.delete'
             return proxy_service.dispatch_api(params)
 
     @router.post('/get')
     @exception_handler
     async def get(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Notification.get'
+            params['grpc_method'] = 'notification.Quota.get'
             return proxy_service.dispatch_api(params)
 
     @router.post('/list')
     @exception_handler
     async def list(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Notification.list'
+            params['grpc_method'] = 'notification.Quota.list'
             return proxy_service.dispatch_api(params)
 
     @router.post('/stat')
     @exception_handler
     async def stat(self, request: Request, body: dict = Body()):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Notification.stat'
+            params['grpc_method'] = 'notification.Quota.stat'
             return proxy_service.dispatch_api(params)
```

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/notification_usage.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/notification_usage.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/project_channel.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/project_channel.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/protocol.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/protocol.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/quota.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/inventory/job.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,64 +9,55 @@
 _LOGGER = logging.getLogger(__name__)
 _AUTH_SCHEME = HTTPBearer()
 
 router = InferringRouter()
 
 
 @cbv(router)
-class Quota(BaseAPI):
+class Job(BaseAPI):
     token: HTTPAuthorizationCredentials = Depends(_AUTH_SCHEME)
     service = 'console-api'
 
-    @router.post('/create')
-    @exception_handler
-    async def create(self, request: Request, body: dict = Body()):
-        params, metadata = await self.parse_request(request, self.token.credentials)
-
-        with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Quota.create'
-            return proxy_service.dispatch_api(params)
-
-    @router.post('/update')
+    @router.post('/delete')
     @exception_handler
-    async def update(self, request: Request, body: dict = Body()):
+    async def delete(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Quota.update'
+            params['grpc_method'] = 'inventory.Job.delete'
             return proxy_service.dispatch_api(params)
 
-    @router.post('/delete')
+    @router.post('/get')
     @exception_handler
-    async def delete(self, request: Request, body: dict = Body()):
+    async def get(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Quota.delete'
+            params['grpc_method'] = 'inventory.Job.get'
             return proxy_service.dispatch_api(params)
 
-    @router.post('/get')
+    @router.post('/list')
     @exception_handler
-    async def get(self, request: Request, body: dict = Body()):
+    async def list(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Quota.get'
+            params['grpc_method'] = 'inventory.Job.list'
             return proxy_service.dispatch_api(params)
 
-    @router.post('/list')
+    @router.post('/analyze')
     @exception_handler
-    async def list(self, request: Request, body: dict = Body()):
+    async def analyze(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Quota.list'
+            params['grpc_method'] = 'inventory.Job.analyze'
             return proxy_service.dispatch_api(params)
 
     @router.post('/stat')
     @exception_handler
-    async def stat(self, request: Request, body: dict = Body()):
+    async def stat(self, request: Request, body: dict = Body(...)):
         params, metadata = await self.parse_request(request, self.token.credentials)
 
         with self.locator.get_service(ProxyService, metadata) as proxy_service:
-            params['grpc_method'] = 'notification.Quota.stat'
+            params['grpc_method'] = 'inventory.Job.stat'
             return proxy_service.dispatch_api(params)
```

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/notification/user_channel.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/notification/user_channel.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/repository/plugin.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/repository/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/repository/policy.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/repository/policy.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/repository/repository.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/repository/repository.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/interface/rest/repository/schema.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/interface/rest/repository/schema.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/cloudforet_manager.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/cloudforet_manager.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/resource_manager/__init__.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/resource_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/resource_manager/cost_analysis_manager.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/resource_manager/cost_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/manager/resource_manager/inventory_manager.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/manager/resource_manager/inventory_manager.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/cost_analysis/cost.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/cost_analysis/cost.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/dashboard/custom_widget.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/dashboard/custom_widget.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/dashboard/domain_dashboard.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/dashboard/domain_dashboard.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/dashboard/project_dashboard.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/dashboard/project_dashboard.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/extension/resource.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/extension/resource.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/identity/project.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/identity/project.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/identity/token.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/identity/token.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/identity/user.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/identity/user.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/change_history.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/change_history.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/cloud_service.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/cloud_service.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/cloud_service_type.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/cloud_service_type.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/note.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/note.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/inventory/region.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/inventory/region.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/repository/plugin.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/repository/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/repository/policy.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/repository/policy.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/repository/repository.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/repository/repository.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/model/repository/schema.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/model/repository/schema.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/service/common/proxy_service.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/service/common/proxy_service.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet/console_api_v2/service/extension/resource_service.py` & `cloudforet-console-api-v2-1.12.dev5/cloudforet/console_api_v2/service/extension/resource_service.py`

 * *Files identical despite different names*

### Comparing `cloudforet-console-api-v2-1.12.dev4/cloudforet_console_api_v2.egg-info/SOURCES.txt` & `cloudforet-console-api-v2-1.12.dev5/cloudforet_console_api_v2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 cloudforet/console_api_v2/interface/rest/notification/__init__.py
 cloudforet/console_api_v2/interface/rest/notification/notification.py
 cloudforet/console_api_v2/interface/rest/notification/notification_usage.py
 cloudforet/console_api_v2/interface/rest/notification/project_channel.py
 cloudforet/console_api_v2/interface/rest/notification/protocol.py
 cloudforet/console_api_v2/interface/rest/notification/quota.py
 cloudforet/console_api_v2/interface/rest/notification/user_channel.py
+cloudforet/console_api_v2/interface/rest/plugin/__init__.py
+cloudforet/console_api_v2/interface/rest/plugin/plugin.py
 cloudforet/console_api_v2/interface/rest/repository/__init__.py
 cloudforet/console_api_v2/interface/rest/repository/plugin.py
 cloudforet/console_api_v2/interface/rest/repository/policy.py
 cloudforet/console_api_v2/interface/rest/repository/repository.py
 cloudforet/console_api_v2/interface/rest/repository/schema.py
 cloudforet/console_api_v2/manager/__init__.py
 cloudforet/console_api_v2/manager/cloudforet_manager.py
```

### Comparing `cloudforet-console-api-v2-1.12.dev4/setup.py` & `cloudforet-console-api-v2-1.12.dev5/setup.py`

 * *Files identical despite different names*
