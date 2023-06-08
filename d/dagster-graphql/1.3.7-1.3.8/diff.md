# Comparing `tmp/dagster-graphql-1.3.7.tar.gz` & `tmp/dagster-graphql-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.3.7.tar", last modified: Thu Jun  1 18:22:47 2023, max compression
+gzip compressed data, was "dagster-graphql-1.3.8.tar", last modified: Thu Jun  8 16:30:52 2023, max compression
```

## Comparing `dagster-graphql-1.3.7.tar` & `dagster-graphql-1.3.8.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.821929 dagster-graphql-1.3.7/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-01 18:22:47.821929 dagster-graphql-1.3.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.749929 dagster-graphql-1.3.7/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.753929 dagster-graphql-1.3.7/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17963 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2715 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6886 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.769929 dagster-graphql-1.3.7/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18592 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.773929 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    11422 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9455 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3725 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4586 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4396 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7270 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)    25777 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1120 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12470 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    14972 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     8157 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)     9554 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2910 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)    21120 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3093 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      933 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     8078 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.801929 dagster-graphql-1.3.7/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2907 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40571 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     6280 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)      838 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16867 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4785 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    18061 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5489 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    16323 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    10983 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)     5072 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28430 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/instigation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.801929 dagster-graphql-1.3.7/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    20983 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     4473 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)    17622 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.813929 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11062 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39668 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1261 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.817929 dagster-graphql-1.3.7/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    25389 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    37798 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2915 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     5940 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.821929 dagster-graphql-1.3.7/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     3904 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8306 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)     7983 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    29569 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     1328 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1411 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.821929 dagster-graphql-1.3.7/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6364 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:22:47.749929 dagster-graphql-1.3.7/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4286 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       81 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-01 18:22:47.000000 dagster-graphql-1.3.7/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-01 18:22:47.825929 dagster-graphql-1.3.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1527 2023-06-01 18:14:54.000000 dagster-graphql-1.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.470056 dagster-graphql-1.3.8/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 16:30:52.470056 dagster-graphql-1.3.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.306056 dagster-graphql-1.3.8/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.314056 dagster-graphql-1.3.8/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17963 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6886 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.346056 dagster-graphql-1.3.8/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18592 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.362056 dagster-graphql-1.3.8/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    11422 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3725 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4586 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4396 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7270 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)    25777 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12470 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    14972 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)     9554 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2910 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)    21120 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      933 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     8078 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.410056 dagster-graphql-1.3.8/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2907 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40571 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     8183 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)      838 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16867 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4785 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    18061 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5489 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    16323 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28430 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/instigation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.434056 dagster-graphql-1.3.8/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    20983 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     4473 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)    17622 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.446056 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11062 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39668 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.462056 dagster-graphql-1.3.8/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    26830 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    37813 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     5940 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.466056 dagster-graphql-1.3.8/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8306 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)     7983 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    29569 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.466056 dagster-graphql-1.3.8/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6364 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:30:52.310056 dagster-graphql-1.3.8/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 16:30:52.000000 dagster-graphql-1.3.8/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-06-08 16:30:52.000000 dagster-graphql-1.3.8/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:30:52.000000 dagster-graphql-1.3.8/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-08 16:30:52.000000 dagster-graphql-1.3.8/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-08 16:30:52.000000 dagster-graphql-1.3.8/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-08 16:30:52.000000 dagster-graphql-1.3.8/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-08 16:30:52.470056 dagster-graphql-1.3.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-08 16:23:49.000000 dagster-graphql-1.3.8/setup.py
```

### Comparing `dagster-graphql-1.3.7/LICENSE` & `dagster-graphql-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/PKG-INFO` & `dagster-graphql-1.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.7
+Version: 1.3.8
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.7/dagster_graphql/__init__.py` & `dagster-graphql-1.3.8/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/cli.py` & `dagster-graphql-1.3.8/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/client/client.py` & `dagster-graphql-1.3.8/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.3.8/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/client/query.py` & `dagster-graphql-1.3.8/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/client/utils.py` & `dagster-graphql-1.3.8/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/events.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/external.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,59 @@
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from dagster import AssetKey, DagsterInstance
+from dagster import AssetKey
+from dagster._daemon.asset_daemon import get_current_evaluation_id
 
+from dagster_graphql.implementation.fetch_assets import get_asset_nodes_by_asset_key
 from dagster_graphql.schema.auto_materialize_asset_evaluations import (
     GrapheneAutoMaterializeAssetEvaluationNeedsMigrationError,
     GrapheneAutoMaterializeAssetEvaluationRecord,
     GrapheneAutoMaterializeAssetEvaluationRecords,
 )
 from dagster_graphql.schema.inputs import GrapheneAssetKeyInput
 
+if TYPE_CHECKING:
+    from ..schema.util import ResolveInfo
+
 
 def fetch_auto_materialize_asset_evaluations(
-    instance: DagsterInstance,
-    asset_key: GrapheneAssetKeyInput,
+    graphene_info: "ResolveInfo",
+    graphene_asset_key: GrapheneAssetKeyInput,
     limit: int,
     cursor: Optional[str],
 ):
     """Fetch asset policy evaluations from storage."""
-    if instance.schedule_storage is None:
+    if graphene_info.context.instance.schedule_storage is None:
         return GrapheneAutoMaterializeAssetEvaluationNeedsMigrationError(
             message="Instance does not have schedule storage configured, cannot fetch evaluations."
         )
-    if not instance.schedule_storage.supports_auto_materialize_asset_evaluations:
+    if (
+        not graphene_info.context.instance.schedule_storage.supports_auto_materialize_asset_evaluations
+    ):
         return GrapheneAutoMaterializeAssetEvaluationNeedsMigrationError(
             message=(
                 "Auto materialize evaluations are not getting logged. Run `dagster instance"
                 " migrate` to enable."
             )
         )
 
+    asset_key = AssetKey.from_graphql_input(graphene_asset_key)
+    asset_node = get_asset_nodes_by_asset_key(graphene_info).get(asset_key)
+    partitions_def = (
+        asset_node.external_asset_node.partitions_def_data.get_partitions_definition()
+        if asset_node and asset_node.external_asset_node.partitions_def_data
+        else None
+    )
+
+    current_evaluation_id = get_current_evaluation_id(graphene_info.context.instance)
+
     return GrapheneAutoMaterializeAssetEvaluationRecords(
         records=[
-            GrapheneAutoMaterializeAssetEvaluationRecord(record)
-            for record in instance.schedule_storage.get_auto_materialize_asset_evaluations(
-                asset_key=AssetKey.from_graphql_input(asset_key),
+            GrapheneAutoMaterializeAssetEvaluationRecord(record, partitions_def=partitions_def)
+            for record in graphene_info.context.instance.schedule_storage.get_auto_materialize_asset_evaluations(
+                asset_key=asset_key,
                 limit=limit,
                 cursor=int(cursor) if cursor else None,
             )
-        ]
+        ],
+        currentEvaluationId=current_evaluation_id,
     )
```

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.3.8/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import List, Optional, Tuple
+from typing import Optional, Tuple
 
 import dagster._check as check
 import graphene
+from dagster import PartitionsDefinition
 from dagster._core.definitions.auto_materialize_condition import (
     AutoMaterializeCondition,
     AutoMaterializeDecisionType,
     DownstreamFreshnessAutoMaterializeCondition,
     FreshnessAutoMaterializeCondition,
     MaxMaterializationsExceededAutoMaterializeCondition,
     MissingAutoMaterializeCondition,
@@ -18,16 +19,38 @@
 from dagster_graphql.schema.errors import GrapheneError
 
 from .util import non_null_list
 
 GrapheneAutoMaterializeDecisionType = graphene.Enum.from_enum(AutoMaterializeDecisionType)
 
 
+class GraphenePartitionKeys(graphene.ObjectType):
+    partitionKeys = non_null_list(graphene.String)
+
+    class Meta:
+        name = "PartitionKeys"
+
+
+class GraphenePartitionSubsetDeserializationError(graphene.ObjectType):
+    message = graphene.NonNull(graphene.String)
+
+    class Meta:
+        interfaces = (GrapheneError,)
+        name = "PartitionSubsetDeserializationError"
+
+
+class GraphenePartitionKeysOrError(graphene.Union):
+    class Meta:
+        types = (GraphenePartitionKeys, GraphenePartitionSubsetDeserializationError)
+        name = "PartitionKeysOrError"
+
+
 class GrapheneAutoMaterializeConditionWithDecisionType(graphene.Interface):
     decisionType = graphene.NonNull(GrapheneAutoMaterializeDecisionType)
+    partitionKeysOrError = graphene.Field(GraphenePartitionKeysOrError)
 
     class Meta:
         name = "AutoMaterializeConditionWithDecisionType"
 
 
 class GrapheneFreshnessAutoMaterializeCondition(graphene.ObjectType):
     class Meta:
@@ -75,34 +98,59 @@
             GrapheneMissingAutoMaterializeCondition,
             GrapheneParentOutdatedAutoMaterializeCondition,
             GrapheneMaxMaterializationsExceededAutoMaterializeCondition,
         )
 
 
 def create_graphene_auto_materialize_condition(
-    condition_tuple: Tuple[AutoMaterializeCondition, Optional[SerializedPartitionsSubset]]
+    condition_tuple: Tuple[AutoMaterializeCondition, Optional[SerializedPartitionsSubset]],
+    partitions_def: Optional[PartitionsDefinition],
 ):
-    condition, _ = condition_tuple
+    condition, serialized_partition_subset = condition_tuple
+
+    if not serialized_partition_subset:
+        partition_keys_or_error = None
+    elif not partitions_def:
+        partition_keys_or_error = GraphenePartitionSubsetDeserializationError(
+            message="PartitionsDefinition not found, cannot display partition keys"
+        )
+    elif not serialized_partition_subset.can_deserialize(partitions_def):
+        partition_keys_or_error = GraphenePartitionSubsetDeserializationError(
+            message=(
+                "Partition subset cannot be deserialized. The PartitionsDefinition may have"
+                " changed."
+            )
+        )
+    else:
+        subset = serialized_partition_subset.deserialize(partitions_def)
+        partition_keys_or_error = GraphenePartitionKeys(partitionKeys=subset.get_partition_keys())
+
     if isinstance(condition, FreshnessAutoMaterializeCondition):
-        return GrapheneFreshnessAutoMaterializeCondition(decisionType=condition.decision_type)
+        return GrapheneFreshnessAutoMaterializeCondition(
+            decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
+        )
     elif isinstance(condition, DownstreamFreshnessAutoMaterializeCondition):
         return GrapheneDownstreamFreshnessAutoMaterializeCondition(
-            decisionType=condition.decision_type
+            decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
         )
     elif isinstance(condition, ParentMaterializedAutoMaterializeCondition):
         return GrapheneParentMaterializedAutoMaterializeCondition(
-            decisionType=condition.decision_type
+            decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
         )
     elif isinstance(condition, MissingAutoMaterializeCondition):
-        return GrapheneMissingAutoMaterializeCondition(decisionType=condition.decision_type)
+        return GrapheneMissingAutoMaterializeCondition(
+            decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
+        )
     elif isinstance(condition, ParentOutdatedAutoMaterializeCondition):
-        return GrapheneParentOutdatedAutoMaterializeCondition(decisionType=condition.decision_type)
+        return GrapheneParentOutdatedAutoMaterializeCondition(
+            decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
+        )
     elif isinstance(condition, MaxMaterializationsExceededAutoMaterializeCondition):
         return GrapheneMaxMaterializationsExceededAutoMaterializeCondition(
-            decisionType=condition.decision_type
+            decisionType=condition.decision_type, partitionKeysOrError=partition_keys_or_error
         )
     else:
         check.failed(f"Unexpected condition type {type(condition)}")
 
 
 class GrapheneAutoMaterializeAssetEvaluationRecord(graphene.ObjectType):
     id = graphene.NonNull(graphene.ID)
@@ -112,38 +160,40 @@
     numDiscarded = graphene.NonNull(graphene.Int)
     conditions = non_null_list(GrapheneAutoMaterializeCondition)
     timestamp = graphene.NonNull(graphene.Float)
 
     class Meta:
         name = "AutoMaterializeAssetEvaluationRecord"
 
-    def __init__(self, record: AutoMaterializeAssetEvaluationRecord):
+    def __init__(
+        self,
+        record: AutoMaterializeAssetEvaluationRecord,
+        partitions_def: Optional[PartitionsDefinition],
+    ):
         super().__init__(
             id=record.id,
             evaluationId=record.evaluation_id,
             numRequested=record.evaluation.num_requested,
             numSkipped=record.evaluation.num_skipped,
             numDiscarded=record.evaluation.num_discarded,
             conditions=[
-                create_graphene_auto_materialize_condition(c)
+                create_graphene_auto_materialize_condition(c, partitions_def)
                 for c in record.evaluation.partition_subsets_by_condition
             ],
             timestamp=record.timestamp,
         )
 
 
 class GrapheneAutoMaterializeAssetEvaluationRecords(graphene.ObjectType):
     records = non_null_list(GrapheneAutoMaterializeAssetEvaluationRecord)
+    currentEvaluationId = graphene.Int()
 
     class Meta:
         name = "AutoMaterializeAssetEvaluationRecords"
 
-    def __init__(self, records: List[AutoMaterializeAssetEvaluationRecord]):
-        super().__init__(records=records)
-
 
 class GrapheneAutoMaterializeAssetEvaluationNeedsMigrationError(graphene.ObjectType):
     message = graphene.NonNull(graphene.String)
 
     class Meta:
         interfaces = (GrapheneError,)
         name = "AutoMaterializeAssetEvaluationNeedsMigrationError"
```

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/errors.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/execution.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/external.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/instance.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/instance.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import dagster._check as check
 import graphene
 from dagster._core.instance import DagsterInstance
 from dagster._core.launcher.base import RunLauncher
 from dagster._core.storage.captured_log_manager import CapturedLogManager
 from dagster._daemon.asset_daemon import get_auto_materialize_paused
 from dagster._daemon.types import DaemonStatus
+from dagster._utils.concurrency import ConcurrencyKeyInfo
 
 from .errors import GraphenePythonError
 from .util import ResolveInfo, non_null_list
 
 
 class GrapheneRunLauncher(graphene.ObjectType):
     name = graphene.NonNull(graphene.String)
@@ -84,24 +85,51 @@
     def resolve_allDaemonStatuses(self, _graphene_info: ResolveInfo):
         return [
             GrapheneDaemonStatus(daemon_status)
             for daemon_status in self._instance.get_daemon_statuses().values()
         ]
 
 
+class GrapheneConcurrencyKeyInfo(graphene.ObjectType):
+    concurrencyKey = graphene.NonNull(graphene.String)
+    slotCount = graphene.NonNull(graphene.Int)
+    activeSlotCount = graphene.NonNull(graphene.Int)
+    activeRunIds = non_null_list(graphene.String)
+    pendingStepCount = graphene.NonNull(graphene.Int)
+    pendingStepRunIds = non_null_list(graphene.String)
+    assignedStepCount = graphene.NonNull(graphene.Int)
+    assignedStepRunIds = non_null_list(graphene.String)
+
+    class Meta:
+        name = "ConcurrencyKeyInfo"
+
+    def __init__(self, concurrency_key_info: ConcurrencyKeyInfo):
+        super().__init__(
+            concurrencyKey=concurrency_key_info.concurrency_key,
+            slotCount=concurrency_key_info.slot_count,
+            activeSlotCount=concurrency_key_info.active_slot_count,
+            activeRunIds=list(concurrency_key_info.active_run_ids),
+            pendingStepCount=concurrency_key_info.pending_step_count,
+            pendingStepRunIds=list(concurrency_key_info.pending_run_ids),
+            assignedStepCount=concurrency_key_info.assigned_step_count,
+            assignedStepRunIds=list(concurrency_key_info.assigned_run_ids),
+        )
+
+
 class GrapheneInstance(graphene.ObjectType):
     id = graphene.NonNull(graphene.String)
     info = graphene.Field(graphene.String)
     runLauncher = graphene.Field(GrapheneRunLauncher)
     runQueuingSupported = graphene.NonNull(graphene.Boolean)
     executablePath = graphene.NonNull(graphene.String)
     daemonHealth = graphene.NonNull(GrapheneDaemonHealth)
     hasInfo = graphene.NonNull(graphene.Boolean)
     hasCapturedLogManager = graphene.NonNull(graphene.Boolean)
     autoMaterializePaused = graphene.NonNull(graphene.Boolean)
+    concurrencyLimits = non_null_list(GrapheneConcurrencyKeyInfo)
 
     class Meta:
         name = "Instance"
 
     def __init__(self, instance):
         super().__init__()
         self._instance = check.inst_param(instance, "instance", DagsterInstance)
@@ -134,7 +162,14 @@
         return GrapheneDaemonHealth(instance=self._instance)
 
     def resolve_hasCapturedLogManager(self, _graphene_info: ResolveInfo):
         return isinstance(self._instance.compute_log_manager, CapturedLogManager)
 
     def resolve_autoMaterializePaused(self, _graphene_info: ResolveInfo):
         return get_auto_materialize_paused(self._instance)
+
+    def resolve_concurrencyLimits(self, _graphene_info: ResolveInfo):
+        res = []
+        for key in self._instance.event_log_storage.get_concurrency_keys():
+            key_info = self._instance.event_log_storage.get_concurrency_info(key)
+            res.append(GrapheneConcurrencyKeyInfo(key_info))
+        return res
```

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/resources.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/roots/mutation.py`

 * *Files 12% similar despite different names*

```diff
@@ -705,14 +705,53 @@
     @capture_error
     @check_permission(Permissions.TOGGLE_AUTO_MATERIALIZE)
     def mutate(self, graphene_info, paused: bool):
         set_auto_materialize_paused(graphene_info.context.instance, paused)
         return paused
 
 
+class GrapheneSetConcurrencyLimitMutation(graphene.Mutation):
+    """Sets the concurrency limit for a given concurrency key."""
+
+    Output = graphene.NonNull(graphene.Boolean)
+
+    class Meta:
+        name = "SetConcurrencyLimitMutation"
+
+    class Arguments:
+        concurrencyKey = graphene.Argument(graphene.NonNull(graphene.String))
+        limit = graphene.Argument(graphene.NonNull(graphene.Int))
+
+    @capture_error
+    @check_permission(Permissions.EDIT_CONCURRENCY_LIMIT)
+    def mutate(self, graphene_info, concurrencyKey: str, limit: int):
+        graphene_info.context.instance.event_log_storage.set_concurrency_slots(
+            concurrencyKey, limit
+        )
+        return True
+
+
+class GrapheneFreeConcurrencySlotsForRunMutation(graphene.Mutation):
+    """Frees the concurrency slots occupied by a specific run."""
+
+    Output = graphene.NonNull(graphene.Boolean)
+
+    class Meta:
+        name = "FreeConcurrencySlotsForRunMutation"
+
+    class Arguments:
+        runId = graphene.Argument(graphene.NonNull(graphene.String))
+
+    @capture_error
+    @check_permission(Permissions.EDIT_CONCURRENCY_LIMIT)
+    def mutate(self, graphene_info, runId: str):
+        graphene_info.context.instance.event_log_storage.free_concurrency_slots_for_run(runId)
+        return True
+
+
 class GrapheneDagitMutation(graphene.ObjectType):
     """The root for all mutations to modify data in your Dagster instance."""
 
     class Meta:
         name = "DagitMutation"
 
     launch_pipeline_execution = GrapheneLaunchRunMutation.Field()
@@ -737,7 +776,9 @@
     launch_partition_backfill = GrapheneLaunchBackfillMutation.Field()
     resume_partition_backfill = GrapheneResumeBackfillMutation.Field()
     cancel_partition_backfill = GrapheneCancelBackfillMutation.Field()
     log_telemetry = GrapheneLogTelemetryMutation.Field()
     set_nux_seen = GrapheneSetNuxSeenMutation.Field()
     add_dynamic_partition = GrapheneAddDynamicPartitionMutation.Field()
     setAutoMaterializePaused = GrapheneSetAutoMaterializePausedMutation.Field()
+    setConcurrencyLimit = GrapheneSetConcurrencyLimitMutation.Field()
+    freeConcurrencySlotsForRun = GrapheneFreeConcurrencySlotsForRunMutation.Field()
```

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/roots/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,15 +467,15 @@
     test = graphene.Field(
         GrapheneTestFields,
         description="Provides fields for testing behavior",
     )
 
     autoMaterializeAssetEvaluationsOrError = graphene.Field(
         GrapheneAutoMaterializeAssetEvaluationRecordsOrError,
-        assetKey=graphene.Argument(GrapheneAssetKeyInput),
+        assetKey=graphene.Argument(graphene.NonNull(GrapheneAssetKeyInput)),
         limit=graphene.Argument(graphene.NonNull(graphene.Int)),
         cursor=graphene.Argument(graphene.String),
         description="Retrieve the auto materialization evaluation records for all assets.",
     )
 
     @capture_error
     def resolve_repositoriesOrError(
@@ -991,9 +991,9 @@
         self,
         graphene_info: ResolveInfo,
         assetKey: GrapheneAssetKeyInput,
         limit: int,
         cursor: Optional[str] = None,
     ):
         return fetch_auto_materialize_asset_evaluations(
-            instance=graphene_info.context.instance, asset_key=assetKey, cursor=cursor, limit=limit
+            graphene_info=graphene_info, graphene_asset_key=assetKey, cursor=cursor, limit=limit
         )
```

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/runs.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/solids.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/table.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/tags.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/schema/util.py` & `dagster-graphql-1.3.8/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql/test/utils.py` & `dagster-graphql-1.3.8/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.3.8/dagster_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.3.7
+Version: 1.3.8
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dagster-graphql-1.3.7/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.3.8/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.3.7/setup.py` & `dagster-graphql-1.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     install_requires=[
-        "dagster==1.3.7",
+        "dagster==1.3.8",
         "graphene>=3",
         "gql[requests]>=3.0.0",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
         "urllib3<2.0.0",  # https://github.com/psf/requests/issues/6432
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
```

