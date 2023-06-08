# Comparing `tmp/frequenz-api-dispatch-0.8.0.tar.gz` & `tmp/frequenz-api-dispatch-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-dispatch-0.8.0.tar", last modified: Tue Jun  6 14:04:09 2023, max compression
+gzip compressed data, was "frequenz-api-dispatch-0.8.1.tar", last modified: Thu Jun  8 12:27:21 2023, max compression
```

## Comparing `frequenz-api-dispatch-0.8.0.tar` & `frequenz-api-dispatch-0.8.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.220717 frequenz-api-dispatch-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (122)      258 2023-06-06 14:03:46.000000 frequenz-api-dispatch-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-06-06 14:04:09.220717 frequenz-api-dispatch-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-06 14:03:46.000000 frequenz-api-dispatch-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-06 14:03:46.000000 frequenz-api-dispatch-0.8.0/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-06-06 14:03:46.000000 frequenz-api-dispatch-0.8.0/ci.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.204716 frequenz-api-dispatch-0.8.0/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.204716 frequenz-api-dispatch-0.8.0/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.204716 frequenz-api-dispatch-0.8.0/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/proto/frequenz/api/dispatch/
--rw-r--r--   0 runner    (1001) docker     (122)     5506 2023-06-06 14:03:46.000000 frequenz-api-dispatch-0.8.0/proto/frequenz/api/dispatch/dispatch.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/proto/frequenz/api/dispatch/fcr/
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-06 14:03:46.000000 frequenz-api-dispatch-0.8.0/proto/frequenz/api/dispatch/fcr/prequalification.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.204716 frequenz-api-dispatch-0.8.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.204716 frequenz-api-dispatch-0.8.0/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.204716 frequenz-api-dispatch-0.8.0/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/py/frequenz/api/dispatch/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-06 14:03:46.000000 frequenz-api-dispatch-0.8.0/py/frequenz/api/dispatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 14:03:46.000000 frequenz-api-dispatch-0.8.0/py/frequenz/api/dispatch/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/py/frequenz_api_dispatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-06-06 14:04:09.000000 frequenz-api-dispatch-0.8.0/py/frequenz_api_dispatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-06-06 14:04:09.000000 frequenz-api-dispatch-0.8.0/py/frequenz_api_dispatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 14:04:09.000000 frequenz-api-dispatch-0.8.0/py/frequenz_api_dispatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      524 2023-06-06 14:04:09.000000 frequenz-api-dispatch-0.8.0/py/frequenz_api_dispatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-06 14:04:09.000000 frequenz-api-dispatch-0.8.0/py/frequenz_api_dispatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-06 14:03:46.000000 frequenz-api-dispatch-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 14:04:09.220717 frequenz-api-dispatch-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.204716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.216716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.216716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.216716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.216716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.216716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.216716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.216716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.216716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.216716 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.220717 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-06-06 14:03:48.000000 frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/timeofday.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.208716 frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.220717 frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-06-06 14:03:49.000000 frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 14:04:09.220717 frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-06-06 14:03:49.000000 frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-06-06 14:03:49.000000 frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      518 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1666 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/ci.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/proto/frequenz/api/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (122)     5467 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/proto/frequenz/api/dispatch/dispatch.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/proto/frequenz/api/dispatch/fcr/
+-rw-r--r--   0 runner    (1001) docker     (122)      631 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/proto/frequenz/api/dispatch/fcr/prequalification.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/py/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/py/frequenz/api/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/py/frequenz/api/dispatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/py/frequenz/api/dispatch/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.207757 frequenz-api-dispatch-0.8.1/py/frequenz_api_dispatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1730 2023-06-08 12:27:21.000000 frequenz-api-dispatch-0.8.1/py/frequenz_api_dispatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3839 2023-06-08 12:27:21.000000 frequenz-api-dispatch-0.8.1/py/frequenz_api_dispatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 12:27:21.000000 frequenz-api-dispatch-0.8.1/py/frequenz_api_dispatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      524 2023-06-08 12:27:21.000000 frequenz-api-dispatch-0.8.1/py/frequenz_api_dispatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-08 12:27:21.000000 frequenz-api-dispatch-0.8.1/py/frequenz_api_dispatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.207757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.207757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.207757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-06-08 12:26:58.000000 frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.203757 frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-06-08 12:26:59.000000 frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 12:27:21.211757 frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-06-08 12:26:59.000000 frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-06-08 12:26:59.000000 frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
```

### Comparing `frequenz-api-dispatch-0.8.0/PKG-INFO` & `frequenz-api-dispatch-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-dispatch
-Version: 0.8.0
+Version: 0.8.1
 Summary: Frequenz dispatch gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-dispatch/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-dispatch
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-dispatch/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-dispatch/discussions/categories/support
```

### Comparing `frequenz-api-dispatch-0.8.0/README.md` & `frequenz-api-dispatch-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/ci.yaml` & `frequenz-api-dispatch-0.8.1/ci.yaml`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/proto/frequenz/api/dispatch/dispatch.proto` & `frequenz-api-dispatch-0.8.1/proto/frequenz/api/dispatch/dispatch.proto`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 syntax = "proto3";
 
 package frequenz.api.dispatch;
 
 import "google/api/annotations.proto";
 import "google/protobuf/empty.proto";
-import "google/protobuf/struct.proto";
 import "google/protobuf/timestamp.proto";
 
 import "frequenz/api/common/components.proto";
 
 import "frequenz/api/dispatch/fcr/prequalification.proto";
 
 service DispatchService {
```

### Comparing `frequenz-api-dispatch-0.8.0/proto/frequenz/api/dispatch/fcr/prequalification.proto` & `frequenz-api-dispatch-0.8.1/proto/frequenz/api/dispatch/fcr/prequalification.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/py/frequenz_api_dispatch.egg-info/PKG-INFO` & `frequenz-api-dispatch-0.8.1/py/frequenz_api_dispatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-dispatch
-Version: 0.8.0
+Version: 0.8.1
 Summary: Frequenz dispatch gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-dispatch/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-dispatch
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-dispatch/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-dispatch/discussions/categories/support
```

### Comparing `frequenz-api-dispatch-0.8.0/py/frequenz_api_dispatch.egg-info/SOURCES.txt` & `frequenz-api-dispatch-0.8.1/py/frequenz_api_dispatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/py/frequenz_api_dispatch.egg-info/requires.txt` & `frequenz-api-dispatch-0.8.1/py/frequenz_api_dispatch.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/pyproject.toml` & `frequenz-api-dispatch-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-dispatch-0.8.1/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto` & `frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto` & `frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-dispatch-0.8.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto` & `frequenz-api-dispatch-0.8.1/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto`

 * *Files identical despite different names*

