# Comparing `tmp/dagster-1.3.7.tar.gz` & `tmp/dagster-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.3.7.tar", last modified: Thu Jun  1 18:15:21 2023, max compression
+gzip compressed data, was "dagster-1.3.8.tar", last modified: Thu Jun  8 16:24:08 2023, max compression
```

## Comparing `dagster-1.3.7.tar` & `dagster-1.3.8.tar`

### file list

```diff
@@ -1,629 +1,634 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.218557 dagster-1.3.7/
--rw-r--r--   0 root         (0) root         (0)      549 2023-06-01 18:14:54.000000 dagster-1.3.7/COPYING
--rw-r--r--   0 root         (0) root         (0)    11344 2023-06-01 18:14:54.000000 dagster-1.3.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-01 18:14:54.000000 dagster-1.3.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8790 2023-06-01 18:15:21.218557 dagster-1.3.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7167 2023-06-01 18:14:54.000000 dagster-1.3.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.066558 dagster-1.3.7/dagster/
--rw-r--r--   0 root         (0) root         (0)    26213 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)     5456 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.070558 dagster-1.3.7/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     2882 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5479 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     2901 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.070558 dagster-1.3.7/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    51637 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.070558 dagster-1.3.7/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27021 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8263 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     7730 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3540 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     5867 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     2280 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    29907 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     5852 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5129 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19958 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15707 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.070558 dagster-1.3.7/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28391 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.082558 dagster-1.3.7/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15864 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    19601 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    15269 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    16880 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9466 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.082558 dagster-1.3.7/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)    71109 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)     6217 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)      577 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/pythonic_config/utils.py
--rw-r--r--   0 root         (0) root         (0)    12143 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17162 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.090558 dagster-1.3.7/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      994 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13645 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.090558 dagster-1.3.7/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.114558 dagster-1.3.7/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7626 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30229 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    10704 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3816 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    36842 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     5685 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    58554 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_reconciliation_sensor.py
--rw-r--r--   0 root         (0) root         (0)    18474 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7164 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    64846 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    24005 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/assets_job.py
--rw-r--r--   0 root         (0) root         (0)     2806 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/auto_materialize_condition.py
--rw-r--r--   0 root         (0) root         (0)     5297 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    16105 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    45671 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4287 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    10845 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    20795 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    18695 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.118558 dagster-1.3.7/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43205 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8250 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9444 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10676 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    17845 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    14396 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8656 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    11936 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)     7085 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5275 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    21205 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    39988 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    31576 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21013 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)    10548 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/external_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     8010 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16195 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    44740 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3205 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    22898 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     5386 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    51157 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    20308 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     6845 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8841 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.118558 dagster-1.3.7/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)    32319 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    56090 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    20758 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11927 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8041 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    22629 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    19256 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7509 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    18908 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    39032 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47274 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)     8811 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27231 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/reconstruct.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.122558 dagster-1.3.7/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6670 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    18856 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    17401 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    16917 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1336 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    16162 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7806 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)    24105 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15824 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    38400 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    37556 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5189 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    10837 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    46882 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    15391 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2298 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/test_op_definition.py
--rw-r--r--   0 root         (0) root         (0)    12374 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    76525 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15645 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7992 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     2930 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    25453 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)     6241 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.126558 dagster-1.3.7/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    64981 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7783 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.130558 dagster-1.3.7/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38315 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    36589 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    14710 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.134558 dagster-1.3.7/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21992 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)    15991 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9369 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    26845 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    27349 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    33974 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    44193 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18501 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5149 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5426 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9183 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8544 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14451 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6487 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.138558 dagster-1.3.7/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23031 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     7279 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    12550 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16270 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    27355 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    10000 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    37831 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     1159 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5395 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7057 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    57790 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    15616 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15920 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19280 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1651 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)    10329 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4233 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.138558 dagster-1.3.7/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5990 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     2840 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15667 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.138558 dagster-1.3.7/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14328 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.138558 dagster-1.3.7/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.142558 dagster-1.3.7/dagster/_core/host_representation/
--rw-r--r--   0 root         (0) root         (0)     2789 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33518 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    32089 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    70934 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)    12283 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4333 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19051 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3610 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/host_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.142558 dagster-1.3.7/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   104144 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12808 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24084 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.146558 dagster-1.3.7/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6808 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1586 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    17249 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     3691 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.146558 dagster-1.3.7/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    11030 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.146558 dagster-1.3.7/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    21903 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)     9410 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.146558 dagster-1.3.7/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.146558 dagster-1.3.7/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18247 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.150558 dagster-1.3.7/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2815 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9421 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12099 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16654 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4495 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14452 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.158558 dagster-1.3.7/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.158558 dagster-1.3.7/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6676 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.178557 dagster-1.3.7/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      598 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      972 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2548 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      431 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1569 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      420 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      530 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      403 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      415 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      426 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2480 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1176 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7204 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/base_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.178557 dagster-1.3.7/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8736 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9545 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    24055 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11640 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.182558 dagster-1.3.7/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14381 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3630 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7211 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     7911 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     5090 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)    78441 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.182558 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.182558 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7408 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    18950 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10912 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13217 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8915 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10638 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    27079 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17301 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)      876 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4293 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.182558 dagster-1.3.7/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14469 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3186 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    23189 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/root.py
--rw-r--r--   0 root         (0) root         (0)     8509 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/root_input_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.182558 dagster-1.3.7/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15454 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8635 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     5982 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    46394 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1040 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6822 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6358 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4095 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     3710 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    22541 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)     1039 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3664 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7375 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4863 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.186558 dagster-1.3.7/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13981 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    14855 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    27932 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    19369 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.190558 dagster-1.3.7/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7298 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    35761 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3579 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4881 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3712 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1438 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     4003 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.190558 dagster-1.3.7/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    27515 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11881 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4684 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     3952 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     1912 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1930 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6111 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9123 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     4447 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17838 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    10457 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10032 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/monitoring/monitoring_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16247 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39799 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)     6639 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.194558 dagster-1.3.7/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2720 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.066558 dagster-1.3.7/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.198557 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.202558 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      267 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.202558 dagster-1.3.7/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.202558 dagster-1.3.7/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29251 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39700 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2051 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    18451 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4202 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    21967 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.202558 dagster-1.3.7/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5551 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    12415 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    51761 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5301 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    26559 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     2323 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      222 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     3781 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_loggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34303 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1361 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      629 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8004 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7467 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    37613 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5496 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.206558 dagster-1.3.7/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.214558 dagster-1.3.7/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    23319 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8732 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     6965 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/backcompat.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     4116 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    24259 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     2563 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      883 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)     9813 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    12340 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)     3289 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.214558 dagster-1.3.7/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    10412 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     9330 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    28864 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.214558 dagster-1.3.7/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     3334 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4915 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-01 18:14:54.000000 dagster-1.3.7/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 18:15:21.066558 dagster-1.3.7/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8790 2023-06-01 18:15:20.000000 dagster-1.3.7/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25185 2023-06-01 18:15:21.000000 dagster-1.3.7/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 18:15:20.000000 dagster-1.3.7/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-01 18:15:20.000000 dagster-1.3.7/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1450 2023-06-01 18:15:20.000000 dagster-1.3.7/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-01 18:15:20.000000 dagster-1.3.7/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-06-01 18:15:21.218557 dagster-1.3.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6827 2023-06-01 18:14:54.000000 dagster-1.3.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.206350 dagster-1.3.8/
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-08 16:23:49.000000 dagster-1.3.8/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-06-08 16:23:49.000000 dagster-1.3.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-08 16:23:49.000000 dagster-1.3.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-06-08 16:24:08.206350 dagster-1.3.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7167 2023-06-08 16:23:49.000000 dagster-1.3.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.142350 dagster-1.3.8/dagster/
+-rw-r--r--   0 root         (0) root         (0)    26213 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     5456 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.142350 dagster-1.3.8/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     2882 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5479 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.142350 dagster-1.3.8/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    51637 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.146350 dagster-1.3.8/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26292 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8263 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     7730 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3540 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     5867 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     4154 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    29907 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5129 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19958 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15707 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.146350 dagster-1.3.8/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28391 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.146350 dagster-1.3.8/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15864 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    19601 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    15269 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    16880 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.146350 dagster-1.3.8/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)    71995 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)      577 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/pythonic_config/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12143 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17162 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.150350 dagster-1.3.8/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      994 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13645 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.150350 dagster-1.3.8/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.158350 dagster-1.3.8/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7626 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30543 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    10704 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    37134 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    59306 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/asset_reconciliation_sensor.py
+-rw-r--r--   0 root         (0) root         (0)    18474 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7164 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    63783 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    24376 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/assets_job.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/auto_materialize_condition.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16105 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    45671 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4287 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    10845 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    20795 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    18695 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.162350 dagster-1.3.8/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44389 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8250 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9444 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10676 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    17845 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    14396 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8656 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    11936 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     7085 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5275 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    21205 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    39988 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    31576 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21013 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    10548 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/external_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     8010 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16195 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    44740 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    22898 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     5386 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    51157 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20308 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     6845 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8841 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.162350 dagster-1.3.8/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)    32319 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    56090 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    20153 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8041 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    22119 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19256 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7509 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    18908 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    39191 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47274 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     8902 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27231 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/reconstruct.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.162350 dagster-1.3.8/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    18860 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    17401 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    16917 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1336 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    16162 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7806 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    24105 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15824 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    38400 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    37556 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5189 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    10837 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    47376 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    15391 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/test_op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    12374 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    78072 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    16744 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7992 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2930 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    26237 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)     6241 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.162350 dagster-1.3.8/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    64981 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7783 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.166350 dagster-1.3.8/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38315 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    36589 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    14710 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.166350 dagster-1.3.8/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21992 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    15991 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9369 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    26845 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    27349 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    33974 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    44193 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18501 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5426 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9183 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8544 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    14451 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.170350 dagster-1.3.8/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25252 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     7279 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    12550 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16658 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    27355 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    10000 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    37831 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1159 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5395 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7057 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    58041 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    15616 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15920 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19280 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)    10329 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4233 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.170350 dagster-1.3.8/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3431 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15592 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.170350 dagster-1.3.8/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15580 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.170350 dagster-1.3.8/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.170350 dagster-1.3.8/dagster/_core/host_representation/
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33518 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    32089 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    70934 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)    12517 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19051 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/host_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.170350 dagster-1.3.8/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   104144 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12956 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24084 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.170350 dagster-1.3.8/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3758 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6808 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1586 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    17249 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.170350 dagster-1.3.8/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    11030 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.170350 dagster-1.3.8/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    21903 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.174350 dagster-1.3.8/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.174350 dagster-1.3.8/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18247 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.174350 dagster-1.3.8/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2815 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9421 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12099 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16654 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4495 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14452 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.178350 dagster-1.3.8/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.178350 dagster-1.3.8/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.186350 dagster-1.3.8/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1485 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      598 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      972 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2548 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      431 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1569 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      420 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      530 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      403 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      634 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      415 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1176 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7204 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1215 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/base_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.186350 dagster-1.3.8/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8736 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16247 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9545 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    24055 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11640 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.186350 dagster-1.3.8/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16268 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7273 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     7911 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   100680 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7526 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    19093 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10912 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13217 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8915 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10638 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    28589 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17301 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)      876 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4293 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14469 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3186 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    23189 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/root.py
+-rw-r--r--   0 root         (0) root         (0)     8509 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/root_input_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15454 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8697 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    46286 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6818 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6358 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    22626 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)     1039 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7210 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4863 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13981 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    14855 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    27932 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    18936 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.190350 dagster-1.3.8/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3163 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7298 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    35761 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3579 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3712 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    28195 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11881 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4684 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4099 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9123 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     4447 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18221 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    10611 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    10036 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16326 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39892 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)     6639 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.138350 dagster-1.3.8/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.194350 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.198350 dagster-1.3.8/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.198350 dagster-1.3.8/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29251 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39700 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    18451 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4202 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    21967 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.198350 dagster-1.3.8/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5551 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    51532 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5301 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    26559 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.198350 dagster-1.3.8/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.198350 dagster-1.3.8/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_loggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.198350 dagster-1.3.8/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34396 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1361 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.202350 dagster-1.3.8/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8004 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    37613 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.202350 dagster-1.3.8/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5496 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.202350 dagster-1.3.8/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.206350 dagster-1.3.8/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    23319 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8732 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     6965 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/backcompat.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     4116 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    25123 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     3813 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     2563 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      883 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)     9113 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    12340 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.206350 dagster-1.3.8/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    12640 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     9330 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    28864 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.206350 dagster-1.3.8/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)      170 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 16:23:49.000000 dagster-1.3.8/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 16:24:08.142350 dagster-1.3.8/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-06-08 16:24:08.000000 dagster-1.3.8/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25431 2023-06-08 16:24:08.000000 dagster-1.3.8/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 16:24:08.000000 dagster-1.3.8/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-08 16:24:08.000000 dagster-1.3.8/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-08 16:24:08.000000 dagster-1.3.8/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-08 16:24:08.000000 dagster-1.3.8/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2023-06-08 16:24:08.206350 dagster-1.3.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6820 2023-06-08 16:23:49.000000 dagster-1.3.8/setup.py
```

### Comparing `dagster-1.3.7/COPYING` & `dagster-1.3.8/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/LICENSE` & `dagster-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/PKG-INFO` & `dagster-1.3.8/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.7
+Version: 1.3.8
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.7/README.md` & `dagster-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/__init__.py` & `dagster-1.3.8/dagster/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_annotations.py` & `dagster-1.3.8/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_api/get_server_id.py` & `dagster-1.3.8/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_api/list_repositories.py` & `dagster-1.3.8/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_api/notebook_data.py` & `dagster-1.3.8/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_api/snapshot_execution_plan.py` & `dagster-1.3.8/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_api/snapshot_job.py` & `dagster-1.3.8/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_api/snapshot_partition.py` & `dagster-1.3.8/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_api/snapshot_repository.py` & `dagster-1.3.8/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_api/snapshot_schedule.py` & `dagster-1.3.8/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_api/snapshot_sensor.py` & `dagster-1.3.8/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_check/README.md` & `dagster-1.3.8/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_check/__init__.py` & `dagster-1.3.8/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/__init__.py` & `dagster-1.3.8/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/api.py` & `dagster-1.3.8/dagster/_cli/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import base64
 import json
 import logging
 import os
 import sys
 import threading
 import zlib
-from contextlib import ExitStack
 from typing import Any, Callable, Optional, cast
 
 import click
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._cli.workspace.cli_target import (
@@ -546,23 +545,14 @@
     required=False,
     help=(
         "[INTERNAL] This option should generally not be used by users. Internal param used by "
         "dagster to spawn a gRPC server with the specified server id."
     ),
 )
 @click.option(
-    "--override-system-timezone",
-    type=click.STRING,
-    required=False,
-    help=(
-        "[INTERNAL] This option should generally not be used by users. Override the system "
-        "timezone for tests."
-    ),
-)
-@click.option(
     "--log-level",
     type=click.Choice(["critical", "error", "warning", "info", "debug"], case_sensitive=False),
     show_default=True,
     required=False,
     default="info",
     help="Level at which to log output from the code server process",
 )
@@ -610,26 +600,23 @@
     socket=None,
     host=None,
     max_workers=None,
     heartbeat=False,
     heartbeat_timeout=30,
     lazy_load_user_code=False,
     fixed_server_id=None,
-    override_system_timezone=None,
     log_level="INFO",
     use_python_environment_entry_point=False,
     container_image=None,
     container_context=None,
     location_name=None,
     instance_ref=None,
     inject_env_vars_from_instance=False,
     **kwargs,
 ):
-    from dagster._core.test_utils import mock_system_timezone
-
     check.invariant(heartbeat_timeout > 0, "heartbeat_timeout must be greater than 0")
 
     check.invariant(
         max_workers is None or max_workers > 1 if heartbeat else True,
         (
             "max_workers must be greater than 1 or set to None if heartbeat is True. "
             "If set to None, the server will use the gRPC default."
@@ -675,74 +662,70 @@
                 else get_working_directory_from_kwargs(kwargs)
             ),
             module_name=module_name,
             python_file=python_file,
             package_name=kwargs["package_name"],
         )
 
-    with ExitStack() as exit_stack:
-        if override_system_timezone:
-            exit_stack.enter_context(mock_system_timezone(override_system_timezone))
-
-        server_termination_event = threading.Event()
-        api_servicer = DagsterApiServer(
-            server_termination_event=server_termination_event,
-            logger=logger,
-            loadable_target_origin=loadable_target_origin,
-            heartbeat=heartbeat,
-            heartbeat_timeout=heartbeat_timeout,
-            lazy_load_user_code=lazy_load_user_code,
-            fixed_server_id=fixed_server_id,
-            entry_point=(
-                get_python_environment_entry_point(sys.executable)
-                if use_python_environment_entry_point
-                else DEFAULT_DAGSTER_ENTRY_POINT
-            ),
-            container_image=container_image,
-            container_context=(
-                json.loads(container_context) if container_context is not None else None
-            ),
-            inject_env_vars_from_instance=inject_env_vars_from_instance,
-            instance_ref=deserialize_value(instance_ref, InstanceRef) if instance_ref else None,
-            location_name=location_name,
-        )
-
-        server = DagsterGrpcServer(
-            server_termination_event=server_termination_event,
-            dagster_api_servicer=api_servicer,
-            port=port,
-            socket=socket,
-            host=host,
-            max_workers=max_workers,
-        )
-
-        code_desc = " "
-        if loadable_target_origin:
-            if loadable_target_origin.python_file:
-                code_desc = f" for file {loadable_target_origin.python_file} "
-            elif loadable_target_origin.package_name:
-                code_desc = f" for package {loadable_target_origin.package_name} "
-            elif loadable_target_origin.module_name:
-                code_desc = f" for module {loadable_target_origin.module_name} "
-
-        server_desc = (
-            f"Dagster code server{code_desc}on port {port} in process {os.getpid()}"
-            if port
-            else f"Dagster code server{code_desc}in process {os.getpid()}"
-        )
-
-        logger.info("Started %s", server_desc)
-
-        try:
-            server.serve()
-        except KeyboardInterrupt:
-            # Terminate cleanly on interrupt
-            logger.info("Code server was interrupted")
-        finally:
-            logger.info("Shutting down %s", server_desc)
+    server_termination_event = threading.Event()
+    api_servicer = DagsterApiServer(
+        server_termination_event=server_termination_event,
+        logger=logger,
+        loadable_target_origin=loadable_target_origin,
+        heartbeat=heartbeat,
+        heartbeat_timeout=heartbeat_timeout,
+        lazy_load_user_code=lazy_load_user_code,
+        fixed_server_id=fixed_server_id,
+        entry_point=(
+            get_python_environment_entry_point(sys.executable)
+            if use_python_environment_entry_point
+            else DEFAULT_DAGSTER_ENTRY_POINT
+        ),
+        container_image=container_image,
+        container_context=(
+            json.loads(container_context) if container_context is not None else None
+        ),
+        inject_env_vars_from_instance=inject_env_vars_from_instance,
+        instance_ref=deserialize_value(instance_ref, InstanceRef) if instance_ref else None,
+        location_name=location_name,
+    )
+
+    server = DagsterGrpcServer(
+        server_termination_event=server_termination_event,
+        dagster_api_servicer=api_servicer,
+        port=port,
+        socket=socket,
+        host=host,
+        max_workers=max_workers,
+    )
+
+    code_desc = " "
+    if loadable_target_origin:
+        if loadable_target_origin.python_file:
+            code_desc = f" for file {loadable_target_origin.python_file} "
+        elif loadable_target_origin.package_name:
+            code_desc = f" for package {loadable_target_origin.package_name} "
+        elif loadable_target_origin.module_name:
+            code_desc = f" for module {loadable_target_origin.module_name} "
+
+    server_desc = (
+        f"Dagster code server{code_desc}on port {port} in process {os.getpid()}"
+        if port
+        else f"Dagster code server{code_desc}in process {os.getpid()}"
+    )
+
+    logger.info("Started %s", server_desc)
+
+    try:
+        server.serve()
+    except KeyboardInterrupt:
+        # Terminate cleanly on interrupt
+        logger.info("Code server was interrupted")
+    finally:
+        logger.info("Shutting down %s", server_desc)
 
 
 @api_cli.command(name="grpc-health-check", help="Check the status of a dagster GRPC server")
 @click.option(
     "--port",
     "-p",
     type=click.INT,
```

### Comparing `dagster-1.3.7/dagster/_cli/asset.py` & `dagster-1.3.8/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/code_server.py` & `dagster-1.3.8/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/config_scaffolder.py` & `dagster-1.3.8/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/debug.py` & `dagster-1.3.8/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/dev.py` & `dagster-1.3.8/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/job.py` & `dagster-1.3.8/dagster/_cli/job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/load_handle.py` & `dagster-1.3.8/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/project.py` & `dagster-1.3.8/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/run.py` & `dagster-1.3.8/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/schedule.py` & `dagster-1.3.8/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/sensor.py` & `dagster-1.3.8/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/utils.py` & `dagster-1.3.8/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_cli/workspace/cli_target.py` & `dagster-1.3.8/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/__init__.py` & `dagster-1.3.8/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/config_schema.py` & `dagster-1.3.8/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/config_type.py` & `dagster-1.3.8/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/errors.py` & `dagster-1.3.8/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/evaluate_value_result.py` & `dagster-1.3.8/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/field.py` & `dagster-1.3.8/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/field_utils.py` & `dagster-1.3.8/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/post_process.py` & `dagster-1.3.8/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/primitive_mapping.py` & `dagster-1.3.8/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/pythonic_config/__init__.py` & `dagster-1.3.8/dagster/_config/pythonic_config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from pydantic import ConstrainedFloat, ConstrainedInt, ConstrainedStr
 from typing_extensions import TypeAlias, TypeGuard, get_args
 
 from dagster import (
     Enum as DagsterEnum,
     Field as DagsterField,
 )
+from dagster._annotations import deprecated
 from dagster._config.config_type import (
     Array,
     ConfigFloatInstance,
     ConfigType,
     Noneable,
 )
 from dagster._config.field_utils import config_dictionary_from_values
@@ -48,15 +49,15 @@
 from dagster._core.errors import (
     DagsterInvalidConfigDefinitionError,
     DagsterInvalidConfigError,
     DagsterInvalidDefinitionError,
     DagsterInvalidInvocationError,
     DagsterInvalidPythonicConfigDefinitionError,
 )
-from dagster._core.execution.context.init import InitResourceContext
+from dagster._core.execution.context.init import InitResourceContext, build_init_resource_context
 from dagster._utils.cached_method import CACHED_METHOD_FIELD_SUFFIX, cached_method
 
 from .attach_other_object_to_context import (
     IAttachDifferentObjectToOpContext as IAttachDifferentObjectToOpContext,
 )
 
 try:
@@ -91,15 +92,15 @@
     ResourceFunction,
     ResourceFunctionWithContext,
     ResourceFunctionWithoutContext,
     has_at_least_one_parameter,
 )
 from dagster._core.storage.io_manager import IOManager, IOManagerDefinition
 
-from .typing_utils import BaseResourceMeta, LateBoundTypesForResourceTypeChecking
+from .typing_utils import BaseConfigMeta, BaseResourceMeta, LateBoundTypesForResourceTypeChecking
 from .utils import safe_is_subclass
 
 Self = TypeVar("Self", bound="ConfigurableResourceFactory")
 
 INTERNAL_MARKER = "__internal__"
 
 # ensure that this ends with the internal marker so we can do a single check
@@ -172,15 +173,15 @@
             else:
                 raise
 
     def _is_field_internal(self, name: str) -> bool:
         return name.endswith(INTERNAL_MARKER)
 
 
-class Config(MakeConfigCacheable):
+class Config(MakeConfigCacheable, metaclass=BaseConfigMeta):
     """Base class for Dagster configuration models, used to specify config schema for
     ops and assets. Subclasses :py:class:`pydantic.BaseModel`.
 
     Example definition:
 
     .. code-block:: python
 
@@ -911,41 +912,47 @@
                 for attr_name, resource in resources_to_update.items()
                 if attr_name not in partial_resources_to_update
             }
 
             to_update = {**resources_to_update, **partial_resources_to_update}
             yield self._with_updated_values(to_update)
 
+    @deprecated
     def with_resource_context(
         self, resource_context: InitResourceContext
     ) -> "ConfigurableResourceFactory[TResValue]":
+        return self.with_replaced_resource_context(resource_context)
+
+    def with_replaced_resource_context(
+        self, resource_context: InitResourceContext
+    ) -> "ConfigurableResourceFactory[TResValue]":
         """Returns a new instance of the resource with the given resource init context bound."""
         # This utility is used to create a copy of this resource, without adjusting
         # any values in this case
         copy = self._with_updated_values({})
         copy._state__internal__ = copy._state__internal__._replace(  # noqa: SLF001
             resource_context=resource_context
         )
         return copy
 
     def _initialize_and_run(self, context: InitResourceContext) -> TResValue:
         with self._resolve_and_update_nested_resources(context) as has_nested_resource:
-            updated_resource = has_nested_resource.with_resource_context(  # noqa: SLF001
+            updated_resource = has_nested_resource.with_replaced_resource_context(  # noqa: SLF001
                 context
             )._with_updated_values(context.resource_config)
 
             updated_resource.setup_for_execution(context)
             return updated_resource.create_resource(context)
 
     @contextlib.contextmanager
     def _initialize_and_run_cm(
         self, context: InitResourceContext
     ) -> Generator[TResValue, None, None]:
         with self._resolve_and_update_nested_resources(context) as has_nested_resource:
-            updated_resource = has_nested_resource.with_resource_context(  # noqa: SLF001
+            updated_resource = has_nested_resource.with_replaced_resource_context(  # noqa: SLF001
                 context
             )._with_updated_values(context.resource_config)
 
             with updated_resource.yield_for_execution(context) as value:
                 yield value
 
     def setup_for_execution(self, context: InitResourceContext) -> None:
@@ -981,14 +988,28 @@
     def get_resource_context(self) -> InitResourceContext:
         """Returns the context that this resource was initialized with."""
         return check.not_none(
             self._state__internal__.resource_context,
             additional_message="Attempted to get context before resource was initialized.",
         )
 
+    def process_config_and_initialize(self) -> TResValue:
+        """Initializes this resource, fully processing its config and returning the prepared
+        resource value.
+        """
+        from dagster._config.post_process import post_process_config
+
+        return self.from_resource_context(
+            build_init_resource_context(
+                config=post_process_config(
+                    self._config_schema.config_type, self._convert_to_config_dictionary()
+                ).value
+            )
+        )
+
     @classmethod
     def from_resource_context(cls, context: InitResourceContext) -> TResValue:
         """Creates a new instance of this resource from a populated InitResourceContext.
         Useful when creating a resource from a function-based resource, for backwards
         compatibility purposes.
 
         For resources that have custom teardown behavior, use from_resource_context_cm instead.
```

### Comparing `dagster-1.3.7/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.3.8/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.3.8/dagster/_config/pythonic_config/typing_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from typing import TYPE_CHECKING, Any, Generic, Optional, Type, TypeVar, Union, cast
 
 import pydantic
 from pydantic import Field
 from typing_extensions import dataclass_transform, get_origin
 
+from dagster._core.errors import DagsterInvalidDagsterTypeInPythonicConfigDefinitionError
+
 from .utils import safe_is_subclass
 
 if TYPE_CHECKING:
     from dagster._config.pythonic_config import PartialResource
 
 
 # Since a metaclass is invoked by Resource before Resource or PartialResource is defined, we need to
@@ -47,15 +49,37 @@
         LateBoundTypesForResourceTypeChecking._Resource = resource_type  # noqa: SLF001
         LateBoundTypesForResourceTypeChecking._PartialResource = (  # noqa: SLF001
             partial_resource_type
         )
 
 
 @dataclass_transform(kw_only_default=True, field_specifiers=(Field,))
-class BaseResourceMeta(pydantic.main.ModelMetaclass):
+class BaseConfigMeta(pydantic.main.ModelMetaclass):
+    def __new__(cls, name, bases, namespaces, **kwargs) -> Any:
+        annotations = namespaces.get("__annotations__", {})
+
+        # Need try/catch because DagsterType may not be loaded when some of the base Config classes are
+        # being created
+        # Any user-created Config class will have DagsterType loaded by the time it's created, so this
+        # will only affect the base Config classes (where this error won't be an issue)
+        try:
+            from dagster._core.types.dagster_type import DagsterType
+
+            for field in annotations:
+                if isinstance(annotations[field], DagsterType):
+                    raise DagsterInvalidDagsterTypeInPythonicConfigDefinitionError(name, field)
+
+        except ImportError:
+            pass
+
+        return super().__new__(cls, name, bases, namespaces, **kwargs)
+
+
+@dataclass_transform(kw_only_default=True, field_specifiers=(Field,))
+class BaseResourceMeta(BaseConfigMeta):
     """Custom metaclass for Resource and PartialResource. This metaclass is responsible for
     transforming the type annotations on the class so that Pydantic constructor-time validation
     does not error when users provide partially configured resources to resource params.
 
     For example, the following code would ordinarily fail Pydantic validation:
 
     .. code-block:: python
```

### Comparing `dagster-1.3.7/dagster/_config/pythonic_config/utils.py` & `dagster-1.3.8/dagster/_config/pythonic_config/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/snap.py` & `dagster-1.3.8/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/source.py` & `dagster-1.3.8/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/stack.py` & `dagster-1.3.8/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/traversal_context.py` & `dagster-1.3.8/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/type_printer.py` & `dagster-1.3.8/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_config/validate.py` & `dagster-1.3.8/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/assets.py` & `dagster-1.3.8/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/code_pointer.py` & `dagster-1.3.8/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/container_context/config.py` & `dagster-1.3.8/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/debug.py` & `dagster-1.3.8/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/decorator_utils.py` & `dagster-1.3.8/dagster/_core/decorator_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,16 +72,16 @@
         else:
             first_newline_pos = docstring.find("\n")
             if first_newline_pos == -1:
                 return docstring
             else:
                 return (
                     docstring[: first_newline_pos + 1]
-                    + textwrap.dedent(docstring[first_newline_pos + 1 :]).strip()
-                )
+                    + textwrap.dedent(docstring[first_newline_pos + 1 :])
+                ).strip()
     else:
         return None
 
 
 # Type-ignores are used throughout the codebase when this function returns False to ignore the type
 # error arising from assuming
 # When/if `StrictTypeGuard` is supported, we can drop `is_context_not_provided` since a False from
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/__init__.py` & `dagster-1.3.8/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/asset_graph.py` & `dagster-1.3.8/dagster/_core/definitions/asset_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,20 @@
 
 from .assets import AssetsDefinition
 from .events import AssetKey, AssetKeyPartitionKey
 from .freshness_policy import FreshnessPolicy
 from .partition import PartitionsDefinition, PartitionsSubset
 from .partition_mapping import PartitionMapping, infer_partition_mapping
 from .source_asset import SourceAsset
-from .time_window_partitions import TimeWindowPartitionsDefinition
+from .time_window_partitions import (
+    TimeWindowPartitionsDefinition,
+    get_time_partition_key,
+    get_time_partitions_def,
+    has_one_dimension_time_window_partitioning,
+)
 
 if TYPE_CHECKING:
     from dagster._core.definitions.asset_graph_subset import AssetGraphSubset
 
 
 class AssetGraph:
     def __init__(
@@ -655,38 +660,44 @@
         level = max(
             self._toposort_level_by_asset_key[required_asset_key]
             for required_asset_key in required_multi_asset_keys
         )
 
         def _sort_key_for_time_window_partition(
             partitions_def: TimeWindowPartitionsDefinition,
+            time_partition_key: str,
         ) -> float:
             # A sort key such that time window partitions are sorted from oldest to newest
             return pendulum.instance(
-                datetime.strptime(cast(str, asset_partition.partition_key), partitions_def.fmt),
+                datetime.strptime(time_partition_key, partitions_def.fmt),
                 tz=partitions_def.timezone,
             ).timestamp()
 
         partitions_def = self._asset_graph.get_partitions_def(asset_key)
         if self._asset_graph.has_self_dependency(asset_key):
-            if partitions_def is not None and isinstance(
-                partitions_def, TimeWindowPartitionsDefinition
+            if partitions_def is None or not has_one_dimension_time_window_partitioning(
+                partitions_def
             ):
-                # sort self dependencies from oldest to newest, as older partitions must exist before
-                # new ones can execute
-                partition_sort_key = _sort_key_for_time_window_partition(partitions_def)
-            else:
                 check.failed(
                     "Assets with self-dependencies must have time-window partitions, but"
                     f" {asset_key} does not."
                 )
+
+            # sort self dependencies from oldest to newest, as older partitions must exist before
+            # new ones can execute
+            partition_sort_key = _sort_key_for_time_window_partition(
+                get_time_partitions_def(partitions_def),
+                get_time_partition_key(partitions_def, asset_partition.partition_key),
+            )
         elif isinstance(partitions_def, TimeWindowPartitionsDefinition):
             # sort non-self dependencies from newest to oldest, as newer partitions are more relevant
             # than older ones
-            partition_sort_key = -1 * _sort_key_for_time_window_partition(partitions_def)
+            partition_sort_key = -1 * _sort_key_for_time_window_partition(
+                partitions_def, cast(str, asset_partition.partition_key)
+            )
         else:
             partition_sort_key = None
 
         return ToposortedPriorityQueue.QueueItem(
             level,
             partition_sort_key,
             [
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.3.8/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/asset_in.py` & `dagster-1.3.8/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/asset_layer.py` & `dagster-1.3.8/dagster/_core/definitions/asset_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,18 @@
     Set,
     Tuple,
     Union,
     cast,
 )
 
 import dagster._check as check
+from dagster._core.definitions.hook_definition import HookDefinition
 from dagster._core.definitions.metadata import (
     ArbitraryMetadataMapping,
+    RawMetadataValue,
 )
 from dagster._core.selector.subset_selector import AssetSelectionData
 
 from ..errors import DagsterInvalidSubsetError
 from .config import ConfigMapping
 from .dependency import NodeHandle, NodeInputHandle, NodeOutput, NodeOutputHandle
 from .events import AssetKey
@@ -737,16 +739,18 @@
     source_assets: Iterable["SourceAsset"],
     executor_def: Optional[ExecutorDefinition] = None,
     config: Optional[Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig"]] = None,
     partitions_def: Optional["PartitionsDefinition"] = None,
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
     description: Optional[str] = None,
     tags: Optional[Mapping[str, Any]] = None,
+    metadata: Optional[Mapping[str, RawMetadataValue]] = None,
     asset_selection: Optional[AbstractSet[AssetKey]] = None,
     asset_selection_data: Optional[AssetSelectionData] = None,
+    hooks: Optional[AbstractSet[HookDefinition]] = None,
 ) -> "JobDefinition":
     from dagster._core.definitions.assets_job import (
         build_assets_job,
         build_source_asset_observation_job,
     )
 
     if asset_selection is not None:
@@ -776,26 +780,29 @@
             config=config,
             source_assets=[*source_assets, *excluded_assets],
             resource_defs=resource_defs,
             executor_def=executor_def,
             partitions_def=partitions_def,
             description=description,
             tags=tags,
+            metadata=metadata,
+            hooks=hooks,
             _asset_selection_data=asset_selection_data,
         )
     else:
         asset_job = build_source_asset_observation_job(
             name=name,
             source_assets=included_source_assets,
             config=config,
             resource_defs=resource_defs,
             executor_def=executor_def,
             partitions_def=partitions_def,
             description=description,
             tags=tags,
+            hooks=hooks,
             _asset_selection_data=asset_selection_data,
         )
 
     return asset_job
 
 
 def _subset_assets_defs(
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/asset_out.py` & `dagster-1.3.8/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/asset_reconciliation_sensor.py` & `dagster-1.3.8/dagster/_core/definitions/asset_reconciliation_sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,16 @@
                 for partition_key in partitions_def.get_partition_keys_in_time_window(
                     reconciliation_window
                 )
                 if partition_key not in materialized_or_requested_subset
             ]
         else:
             return materialized_or_requested_subset.get_partition_keys_not_in_subset(
-                dynamic_partitions_store=dynamic_partitions_store
+                current_time=current_time,
+                dynamic_partitions_store=dynamic_partitions_store,
             )
 
     def with_updates(
         self,
         latest_storage_id: Optional[int],
         run_requests: Sequence[RunRequest],
         newly_materialized_root_asset_keys: AbstractSet[AssetKey],
@@ -396,14 +397,20 @@
                 AssetKey.from_user_string(key_str)
                 for key_str in serialized_materialized_or_requested_root_asset_keys
             },
             materialized_or_requested_root_partitions_by_asset_key=materialized_or_requested_root_partitions_by_asset_key,
             evaluation_id=evaluation_id,
         )
 
+    @classmethod
+    def get_evaluation_id_from_serialized(cls, cursor: str) -> Optional[int]:
+        data = json.loads(cursor)
+        check.invariant(len(data) in [3, 4], "Invalid serialized cursor")
+        return data[3] if len(data) == 4 else None
+
     def serialize(self) -> str:
         serializable_materialized_or_requested_root_partitions_by_asset_key = {
             key.to_user_string(): subset.serialize()
             for key, subset in self.materialized_or_requested_root_partitions_by_asset_key.items()
         }
         serialized = json.dumps(
             (
@@ -707,14 +714,20 @@
     )
 
     backfill_target_asset_graph_subset = get_active_backfill_target_asset_graph_subset(
         asset_graph=asset_graph,
         instance=instance_queryer.instance,
     )
 
+    def will_be_materialized_for_freshness(asset_partition: AssetKeyPartitionKey) -> bool:
+        return asset_partition in conditions_by_asset_partition_for_freshness and all(
+            condition.decision_type == AutoMaterializeDecisionType.MATERIALIZE
+            for condition in conditions_by_asset_partition_for_freshness[asset_partition]
+        )
+
     def parents_will_be_reconciled(
         asset_graph: AssetGraph,
         candidate: AssetKeyPartitionKey,
     ) -> bool:
         from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 
         for parent in asset_graph.get_parents_partitions(
@@ -797,15 +810,19 @@
             or candidate in backfill_target_asset_graph_subset
             # do not reconcile assets if they are not in the target selection
             or candidate.asset_key not in target_asset_keys
             for candidate in candidates_unit
         ):
             return False
 
-        if all(parents_will_be_reconciled(asset_graph, candidate) for candidate in candidates_unit):
+        if all(
+            will_be_materialized_for_freshness(candidate)
+            or parents_will_be_reconciled(asset_graph, candidate)
+            for candidate in candidates_unit
+        ):
             unit_conditions = set().union(
                 *(conditions_for_candidate(candidate) for candidate in candidates_unit)
             )
             # all candidates in the unit share the same conditions
             if unit_conditions:
                 for candidate in candidates_unit:
                     conditions_by_asset_partition[candidate].update(unit_conditions)
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/asset_selection.py` & `dagster-1.3.8/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.3.8/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/assets.py` & `dagster-1.3.8/dagster/_core/definitions/assets.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 
 import dagster._check as check
 from dagster._annotations import public
 from dagster._core.decorator_utils import get_function_params
 from dagster._core.definitions.asset_layer import get_dep_node_handles_of_graph_backed_asset
 from dagster._core.definitions.auto_materialize_policy import AutoMaterializePolicy
 from dagster._core.definitions.freshness_policy import FreshnessPolicy
-from dagster._core.definitions.input import In
 from dagster._core.definitions.metadata import ArbitraryMetadataMapping
+from dagster._core.definitions.multi_dimensional_partitions import MultiPartitionsDefinition
 from dagster._core.definitions.op_selection import get_graph_subset
+from dagster._core.definitions.partition_mapping import MultiPartitionMapping
 from dagster._core.definitions.time_window_partition_mapping import TimeWindowPartitionMapping
 from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
 from dagster._core.errors import DagsterInvalidDefinitionError, DagsterInvalidInvocationError
-from dagster._core.types.dagster_type import Nothing
 from dagster._utils import IHasInternalInit
 from dagster._utils.backcompat import (
     ExperimentalWarning,
     deprecation_warning,
     experimental_arg_warning,
 )
 from dagster._utils.merger import merge_dicts
@@ -232,14 +232,15 @@
             value_type=AutoMaterializePolicy,
         )
 
         _validate_self_deps(
             input_keys=self._keys_by_input_name.values(),
             output_keys=self._selected_asset_keys,
             partition_mappings=self._partition_mappings,
+            partitions_def=self._partitions_def,
         )
 
     @staticmethod
     def dagster_internal_init(
         *,
         keys_by_input_name: Mapping[str, AssetKey],
         keys_by_output_name: Mapping[str, AssetKey],
@@ -779,14 +780,15 @@
         return self.node_def.resolve_output_to_origin_op_def(output_name)
 
     def with_attributes(
         self,
         output_asset_key_replacements: Optional[Mapping[AssetKey, AssetKey]] = None,
         input_asset_key_replacements: Optional[Mapping[AssetKey, AssetKey]] = None,
         group_names_by_key: Optional[Mapping[AssetKey, str]] = None,
+        descriptions_by_key: Optional[Mapping[AssetKey, str]] = None,
         freshness_policy: Optional[
             Union[FreshnessPolicy, Mapping[AssetKey, FreshnessPolicy]]
         ] = None,
         auto_materialize_policy: Optional[
             Union[AutoMaterializePolicy, Mapping[AssetKey, AutoMaterializePolicy]]
         ] = None,
     ) -> "AssetsDefinition":
@@ -801,14 +803,17 @@
             "input_asset_key_replacements",
             key_type=AssetKey,
             value_type=AssetKey,
         )
         group_names_by_key = check.opt_mapping_param(
             group_names_by_key, "group_names_by_key", key_type=AssetKey, value_type=str
         )
+        descriptions_by_key = check.opt_mapping_param(
+            descriptions_by_key, "descriptions_by_key", key_type=AssetKey, value_type=str
+        )
 
         if group_names_by_key:
             group_name_conflicts = [
                 asset_key
                 for asset_key in group_names_by_key
                 if asset_key in self.group_names_by_key
                 and self.group_names_by_key[asset_key] != DEFAULT_GROUP_NAME
@@ -874,15 +879,15 @@
             if replaced_auto_materialize_policy:
                 replaced_auto_materialize_policies_by_key[
                     output_asset_key_replacements.get(key, key)
                 ] = replaced_auto_materialize_policy
 
         replaced_descriptions_by_key = {
             output_asset_key_replacements.get(key, key): description
-            for key, description in self._descriptions_by_key.items()
+            for key, description in descriptions_by_key.items()
         }
 
         return __class__.dagster_internal_init(
             keys_by_input_name={
                 input_name: input_asset_key_replacements.get(key, key)
                 for input_name, key in self._keys_by_input_name.items()
             },
@@ -921,83 +926,14 @@
                 for key, value in self.metadata_by_key.items()
             },
             freshness_policies_by_key=replaced_freshness_policies_by_key,
             auto_materialize_policies_by_key=replaced_auto_materialize_policies_by_key,
             descriptions_by_key=replaced_descriptions_by_key,
         )
 
-    def _subset_op_backed_asset(
-        self, asset_subselection: AbstractSet[AssetKey], selected_asset_keys: AbstractSet[AssetKey]
-    ) -> "AssetsDefinition":
-        """Creates a new AssetsDefinition which will only materialize the given asset keys. In some
-        cases, this subset will have a new set of root assets, which were previously produced within
-        the subset itself. In this case, we will create new inputs for those assets, and generate a
-        new copy of the op with the new inputs.
-
-        Args:
-            asset_subselection (AbstractSet[AssetKey]): The set of asset keys that should be selected
-                from this AssetsDefinition.
-            selected_asset_keys (AbstractSet[AssetKey]): The total set of asset keys that have been
-                selected from the broader asset graph.
-        """
-        # the set of keys that are not selected but are upstream of the selected keys
-        input_keys = {
-            dep_key for key in asset_subselection for dep_key in self.asset_deps[key]
-        }.difference(asset_subselection)
-        ins = {}
-
-        input_names_by_key = {v: k for k, v in self.keys_by_input_name.items()}
-        op_valid = True
-        input_index = 0
-        for input_key in input_keys:
-            input_name = input_names_by_key.get(input_key)
-            if input_name is not None:
-                # just copy over existing input
-                ins[input_name] = self.op.ins[input_name]
-            elif input_key in selected_asset_keys:
-                # There is no input existing for this key, meaning this is something that is produced
-                # within the op if it is not subsetted. If this input is part of the larger
-                # selection that we want to make a job out of, then this would require us to create
-                # a new input such that the dependency would be respected, and therefore a new copy
-                # of the underlying op.
-                op_valid = False
-                # create a new input for this key
-                input_name = f"artificial_input_{input_index}"
-                input_index += 1
-                ins[input_name] = In(Nothing)
-                input_names_by_key[input_key] = input_name
-
-        # must create a new copy of the op
-        if op_valid:
-            op_def = self.op
-        else:
-            # create a hash of the selected keys to generate a unique name for this subsetted op
-            suffix = hashlib.md5((str(list(sorted(asset_subselection)))).encode()).hexdigest()[-5:]
-            op_def = self.op.with_replaced_properties(
-                name=f"{self.op.name}_subset_{suffix}", ins=ins
-            )
-
-        return AssetsDefinition.dagster_internal_init(
-            keys_by_input_name={**{v: k for k, v in input_names_by_key.items()}},
-            # keep track of the original mapping
-            keys_by_output_name=self.node_keys_by_output_name,
-            node_def=op_def,
-            partitions_def=self.partitions_def,
-            partition_mappings=self._partition_mappings,
-            asset_deps=self._asset_deps,
-            can_subset=self.can_subset,
-            selected_asset_keys=asset_subselection,
-            resource_defs=self.resource_defs,
-            group_names_by_key=self.group_names_by_key,
-            metadata_by_key=self.metadata_by_key,
-            freshness_policies_by_key=self.freshness_policies_by_key,
-            auto_materialize_policies_by_key=self.auto_materialize_policies_by_key,
-            descriptions_by_key=self.descriptions_by_key,
-        )
-
     def _subset_graph_backed_asset(
         self,
         selected_asset_keys: AbstractSet[AssetKey],
     ):
         from dagster._core.definitions.graph_definition import GraphDefinition
 
         if not isinstance(self.node_def, GraphDefinition):
@@ -1088,15 +1024,31 @@
                 metadata_by_key=self.metadata_by_key,
                 freshness_policies_by_key=self.freshness_policies_by_key,
                 auto_materialize_policies_by_key=self.auto_materialize_policies_by_key,
                 descriptions_by_key=self.descriptions_by_key,
             )
         else:
             # multi_asset subsetting
-            return self._subset_op_backed_asset(asset_subselection, selected_asset_keys)
+            return AssetsDefinition.dagster_internal_init(
+                # keep track of the original mapping
+                keys_by_input_name=self._keys_by_input_name,
+                keys_by_output_name=self._keys_by_output_name,
+                node_def=self.node_def,
+                partitions_def=self.partitions_def,
+                partition_mappings=self._partition_mappings,
+                asset_deps=self._asset_deps,
+                can_subset=self.can_subset,
+                selected_asset_keys=asset_subselection,
+                resource_defs=self.resource_defs,
+                group_names_by_key=self.group_names_by_key,
+                metadata_by_key=self.metadata_by_key,
+                freshness_policies_by_key=self.freshness_policies_by_key,
+                auto_materialize_policies_by_key=self.auto_materialize_policies_by_key,
+                descriptions_by_key=self.descriptions_by_key,
+            )
 
     @public
     def to_source_assets(self) -> Sequence[SourceAsset]:
         """Returns a SourceAsset for each asset in this definition.
 
         Each produced SourceAsset will have the same key, metadata, io_manager_key, etc. as the
         corresponding asset
@@ -1373,24 +1325,54 @@
     )
 
 
 def _validate_self_deps(
     input_keys: Iterable[AssetKey],
     output_keys: Iterable[AssetKey],
     partition_mappings: Mapping[AssetKey, PartitionMapping],
+    partitions_def: Optional[PartitionsDefinition],
 ) -> None:
     output_keys_set = set(output_keys)
     for input_key in input_keys:
         if input_key in output_keys_set:
             if input_key in partition_mappings:
                 partition_mapping = partition_mappings[input_key]
+                time_window_partition_mapping = get_self_dep_time_window_partition_mapping(
+                    partition_mapping, partitions_def
+                )
                 if (
-                    isinstance(partition_mapping, TimeWindowPartitionMapping)
-                    and (partition_mapping.start_offset or 0) < 0
-                    and (partition_mapping.end_offset or 0) < 0
+                    time_window_partition_mapping is not None
+                    and (time_window_partition_mapping.start_offset or 0) < 0
+                    and (time_window_partition_mapping.end_offset or 0) < 0
                 ):
                     continue
 
             raise DagsterInvalidDefinitionError(
-                "Assets can only depend on themselves if they are time-partitioned and each"
-                " partition depends on earlier partitions"
+                "Assets can only depend on themselves if they are:\n(a) time-partitioned and each"
+                " partition depends on earlier partitions\n(b) multipartitioned, with one time"
+                " dimension that depends on earlier time partitions"
             )
+
+
+def get_self_dep_time_window_partition_mapping(
+    partition_mapping: Optional[PartitionMapping], partitions_def: Optional[PartitionsDefinition]
+) -> Optional[TimeWindowPartitionMapping]:
+    """Returns a time window partition mapping dimension of the provided partition mapping,
+    if exists.
+    """
+    if isinstance(partition_mapping, TimeWindowPartitionMapping):
+        return partition_mapping
+    elif isinstance(partition_mapping, MultiPartitionMapping):
+        if not isinstance(partitions_def, MultiPartitionsDefinition):
+            return None
+
+        time_partition_mapping = partition_mapping.downstream_mappings_by_upstream_dimension.get(
+            partitions_def.time_window_dimension.name
+        )
+
+        if time_partition_mapping is None or not isinstance(
+            time_partition_mapping.partition_mapping, TimeWindowPartitionMapping
+        ):
+            return None
+
+        return time_partition_mapping.partition_mapping
+    return None
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/assets_job.py` & `dagster-1.3.8/dagster/_core/definitions/assets_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from collections import defaultdict
 from typing import (
     TYPE_CHECKING,
+    AbstractSet,
     Any,
     Dict,
     Iterable,
     List,
     Mapping,
     Optional,
     Sequence,
@@ -12,14 +13,15 @@
     Tuple,
     Union,
 )
 
 from toposort import CircularDependencyError, toposort
 
 import dagster._check as check
+from dagster._core.definitions.hook_definition import HookDefinition
 from dagster._core.errors import DagsterInvalidDefinitionError
 from dagster._core.selector.subset_selector import AssetSelectionData
 from dagster._utils.merger import merge_dicts
 
 from .asset_layer import AssetLayer
 from .assets import AssetsDefinition
 from .config import ConfigMapping
@@ -30,14 +32,15 @@
     NodeHandle,
     NodeInvocation,
 )
 from .events import AssetKey
 from .executor_definition import ExecutorDefinition
 from .graph_definition import GraphDefinition
 from .job_definition import JobDefinition, default_job_io_manager
+from .metadata import RawMetadataValue
 from .partition import PartitionedConfig, PartitionsDefinition
 from .resolved_asset_deps import ResolvedAssetDependencies
 from .resource_definition import ResourceDefinition
 from .resource_requirement import ensure_requirements_satisfied
 from .source_asset import SourceAsset
 from .utils import DEFAULT_IO_MANAGER_KEY
 
@@ -112,16 +115,18 @@
     source_assets: Optional[Sequence[Union[SourceAsset, AssetsDefinition]]] = None,
     resource_defs: Optional[Mapping[str, object]] = None,
     description: Optional[str] = None,
     config: Optional[
         Union[ConfigMapping, Mapping[str, object], PartitionedConfig, "RunConfig"]
     ] = None,
     tags: Optional[Mapping[str, str]] = None,
+    metadata: Optional[Mapping[str, RawMetadataValue]] = None,
     executor_def: Optional[ExecutorDefinition] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
+    hooks: Optional[AbstractSet[HookDefinition]] = None,
     _asset_selection_data: Optional[AssetSelectionData] = None,
 ) -> JobDefinition:
     """Builds a job that materializes the given assets.
 
     The dependencies between the ops in the job are determined by the asset dependencies defined
     in the metadata on the provided asset nodes.
 
@@ -225,30 +230,33 @@
             version_strategy=original_job.version_strategy,
         )
 
     return graph.to_job(
         resource_defs=all_resource_defs,
         config=config,
         tags=tags,
+        metadata=metadata,
         executor_def=executor_def,
         partitions_def=partitions_def,
         asset_layer=asset_layer,
+        hooks=hooks,
         _asset_selection_data=_asset_selection_data,
     )
 
 
 def build_source_asset_observation_job(
     name: str,
     source_assets: Sequence[SourceAsset],
     resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
     description: Optional[str] = None,
     config: Optional[Union[ConfigMapping, Mapping[str, object], PartitionedConfig]] = None,
     tags: Optional[Mapping[str, str]] = None,
     executor_def: Optional[ExecutorDefinition] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
+    hooks: Optional[AbstractSet[HookDefinition]] = None,
     _asset_selection_data: Optional[AssetSelectionData] = None,
 ) -> JobDefinition:
     """Builds a job that observes the given source assets.
 
     There are never any dependencies between the ops in the job.
 
     Args:
@@ -327,14 +335,15 @@
     return graph.to_job(
         resource_defs=all_resource_defs,
         config=config,
         tags=tags,
         executor_def=executor_def,
         partitions_def=partitions_def,
         asset_layer=asset_layer,
+        hooks=hooks,
         _asset_selection_data=_asset_selection_data,
     )
 
 
 def build_job_partitions_from_assets(
     assets: Iterable[Union[AssetsDefinition, SourceAsset]],
 ) -> Optional[PartitionsDefinition]:
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/auto_materialize_condition.py` & `dagster-1.3.8/dagster/_core/definitions/auto_materialize_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.3.8/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.3.8/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/composition.py` & `dagster-1.3.8/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/config.py` & `dagster-1.3.8/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/configurable.py` & `dagster-1.3.8/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/data_time.py` & `dagster-1.3.8/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/data_version.py` & `dagster-1.3.8/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,18 @@
 ) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     """Create a combined definition of multiple assets that are computed using the same op and same
     upstream assets.
 
     Each argument to the decorated function references an upstream asset that this asset depends on.
     The name of the argument designates the name of the upstream asset.
 
+    You can set I/O managers keys, auto-materialize policies, freshness policies, group names, etc.
+    on an individual asset within the multi-asset by attaching them to the :py:class:`AssetOut`
+    corresponding to that asset in the `outs` parameter.
+
     Args:
         name (Optional[str]): The name of the op.
         outs: (Optional[Dict[str, AssetOut]]): The AssetOuts representing the produced assets.
         ins (Optional[Mapping[str, AssetIn]]): A dictionary that maps input names to information
             about the input.
         non_argument_deps (Optional[Union[Set[AssetKey], Set[str]]]): Set of asset keys that are upstream
             dependencies, but do not pass an input to the multi_asset.
@@ -447,14 +451,42 @@
             will be initialized during execution, and can be accessed from the
             context within the body of the function.
         group_name (Optional[str]): A string name used to organize multiple assets into groups. This
             group name will be applied to all assets produced by this multi_asset.
         retry_policy (Optional[RetryPolicy]): The retry policy for the op that computes the asset.
         code_version (Optional[str]): (Experimental) Version of the code encapsulated by the multi-asset. If set,
             this is used as a default code version for all defined assets.
+
+    Examples:
+        .. code-block:: python
+
+            # Use IO managers to handle I/O:
+            @multi_asset(
+                outs={
+                    "my_string_asset": AssetOut(),
+                    "my_int_asset": AssetOut(),
+                }
+            )
+            def my_function(upstream_asset: int):
+                result = upstream_asset + 1
+                return str(result), result
+
+            # Handle I/O on your own:
+            @multi_asset(
+                outs={
+                    "asset1": AssetOut(),
+                    "asset2": AssetOut(),
+                },
+                non_argument_deps={"asset0"},
+            )
+            def my_function():
+                asset0_value = load(path="asset0")
+                asset1_result, asset2_result = do_some_transformation(asset0_value)
+                write(asset1_result, path="asset1")
+                write(asset2_result, path="asset2")
     """
     from dagster._core.execution.build_resources import wrap_resources_for_execution
 
     if resource_defs is not None:
         experimental_arg_warning("resource_defs", "multi_asset")
 
     asset_deps = check.opt_mapping_param(
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.3.8/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.3.8/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/definitions_class.py` & `dagster-1.3.8/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/dependency.py` & `dagster-1.3.8/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/events.py` & `dagster-1.3.8/dagster/_core/definitions/events.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/executor_definition.py` & `dagster-1.3.8/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/external_asset_graph.py` & `dagster-1.3.8/dagster/_core/definitions/external_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/freshness_policy.py` & `dagster-1.3.8/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.3.8/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/graph_definition.py` & `dagster-1.3.8/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/hook_definition.py` & `dagster-1.3.8/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/hook_invocation.py` & `dagster-1.3.8/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/inference.py` & `dagster-1.3.8/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/input.py` & `dagster-1.3.8/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/instigation_logger.py` & `dagster-1.3.8/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/job_base.py` & `dagster-1.3.8/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/job_definition.py` & `dagster-1.3.8/dagster/_core/definitions/job_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.3.8/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/logger_definition.py` & `dagster-1.3.8/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/logger_invocation.py` & `dagster-1.3.8/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/materialize.py` & `dagster-1.3.8/dagster/_core/definitions/materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.3.8/dagster/_core/definitions/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/metadata/table.py` & `dagster-1.3.8/dagster/_core/definitions/metadata/table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.3.8/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.3.8/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,31 +410,14 @@
             if isinstance(dim.partitions_def, TimeWindowPartitionsDefinition)
         ]
         check.invariant(
             len(time_window_dims) == 1, "Expected exactly one time window partitioned dimension"
         )
         return next(iter(time_window_dims))
 
-    def get_cron_schedule(
-        self,
-        minute_of_hour: Optional[int] = None,
-        hour_of_day: Optional[int] = None,
-        day_of_week: Optional[int] = None,
-        day_of_month: Optional[int] = None,
-    ) -> str:
-        return cast(
-            TimeWindowPartitionsDefinition, self.time_window_dimension.partitions_def
-        ).get_cron_schedule(minute_of_hour, hour_of_day, day_of_week, day_of_month)
-
-    @property
-    def timezone(self) -> Optional[str]:
-        return cast(
-            TimeWindowPartitionsDefinition, self.time_window_dimension.partitions_def
-        ).timezone
-
     def time_window_for_partition_key(self, partition_key: str) -> TimeWindow:
         if not isinstance(partition_key, MultiPartitionKey):
             partition_key = self.get_partition_key_from_str(partition_key)
 
         time_window_dimension = self.time_window_dimension
         return cast(
             TimeWindowPartitionsDefinition, time_window_dimension.partitions_def
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/node_container.py` & `dagster-1.3.8/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/node_definition.py` & `dagster-1.3.8/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/observe.py` & `dagster-1.3.8/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/op_definition.py` & `dagster-1.3.8/dagster/_core/definitions/op_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -477,27 +477,14 @@
             else:
                 context = None
                 if len(args) > 0 and isinstance(args[0], UnboundOpExecutionContext):
                     context = cast(UnboundOpExecutionContext, args[0])
                     args = args[1:]
                 return op_invocation_result(self, context, *args, **kwargs)
 
-    def __eq__(self, other) -> bool:
-        if not isinstance(other, OpDefinition):
-            return False
-        return (
-            self.compute_fn == other.compute_fn
-            and self.name == other.name
-            and self.description == other.description
-            and self.config_schema == other.config_schema
-            and self.required_resource_keys == other.required_resource_keys
-            and self.tags == other.tags
-            and self.retry_policy == other.retry_policy
-        )
-
 
 def _resolve_output_defs_from_outs(
     compute_fn: Union[Callable[..., Any], "DecoratedOpFunction"],
     outs: Optional[Mapping[str, Out]],
     default_code_version: Optional[str],
 ) -> Sequence[OutputDefinition]:
     from .decorators.op_decorator import DecoratedOpFunction
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/op_invocation.py` & `dagster-1.3.8/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/op_selection.py` & `dagster-1.3.8/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/output.py` & `dagster-1.3.8/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/partition.py` & `dagster-1.3.8/dagster/_core/definitions/partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -926,14 +926,17 @@
 
         return partitions_def.can_deserialize_subset(
             self.serialized_subset,
             serialized_partitions_def_unique_id=self.serialized_partitions_def_unique_id,
             serialized_partitions_def_class_name=self.serialized_partitions_def_class_name,
         )
 
+    def deserialize(self, partitions_def: PartitionsDefinition) -> PartitionsSubset:
+        return partitions_def.deserialize_subset(self.serialized_subset)
+
 
 class DefaultPartitionsSubset(PartitionsSubset[T_str]):
     # Every time we change the serialization format, we should increment the version number.
     # This will ensure that we can gracefully degrade when deserializing old data.
     SERIALIZATION_VERSION = 1
 
     def __init__(
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/partition_mapping.py` & `dagster-1.3.8/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.3.8/dagster/_core/definitions/partitioned_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     DefaultScheduleStatus,
     RunRequestIterator,
     ScheduleDefinition,
     ScheduleEvaluationContext,
 )
 from .time_window_partitions import (
     TimeWindowPartitionsDefinition,
+    get_time_partitions_def,
     has_one_dimension_time_window_partitioning,
 )
 from .unresolved_asset_job_definition import UnresolvedAssetJobDefinition
 
 
 class UnresolvedPartitionedAssetScheduleDefinition(NamedTuple):
     """Points to an unresolved asset job. The asset selection isn't resolved yet, so we can't resolve
@@ -41,25 +42,24 @@
         if partitions_def is None:
             check.failed(
                 f"Job '{resolved_job.name}' provided to build_schedule_from_partitioned_job must"
                 " contain partitioned assets or a partitions definition."
             )
 
         partitions_def = _check_valid_schedule_partitions_def(partitions_def)
-
-        cron_schedule = partitions_def.get_cron_schedule(
-            self.minute_of_hour, self.hour_of_day, self.day_of_week, self.day_of_month
-        )
+        time_partitions_def = get_time_partitions_def(partitions_def)
 
         return ScheduleDefinition(
             job=resolved_job,
             name=self.name,
             execution_fn=_get_schedule_evaluation_fn(partitions_def, resolved_job, self.tags),
-            execution_timezone=partitions_def.timezone,
-            cron_schedule=cron_schedule,
+            execution_timezone=time_partitions_def.timezone,
+            cron_schedule=time_partitions_def.get_cron_schedule(
+                self.minute_of_hour, self.hour_of_day, self.day_of_week, self.day_of_month
+            ),
         )
 
 
 def build_schedule_from_partitioned_job(
     job: Union[JobDefinition, UnresolvedAssetJobDefinition],
     description: Optional[str] = None,
     name: Optional[str] = None,
@@ -140,25 +140,24 @@
             tags=tags,
         )
     else:
         partitions_def = job.partitions_def
         if partitions_def is None:
             check.failed("The provided job is not partitioned")
 
-        time_window_partitions_def = _check_valid_schedule_partitions_def(partitions_def)
-
-        cron_schedule = time_window_partitions_def.get_cron_schedule(
-            minute_of_hour, hour_of_day, day_of_week, day_of_month
-        )
+        partitions_def = _check_valid_schedule_partitions_def(partitions_def)
+        time_partitions_def = get_time_partitions_def(partitions_def)
 
         return schedule(
-            cron_schedule=cron_schedule,
+            cron_schedule=time_partitions_def.get_cron_schedule(
+                minute_of_hour, hour_of_day, day_of_week, day_of_month
+            ),
             job=job,
             default_status=default_status,
-            execution_timezone=time_window_partitions_def.timezone,
+            execution_timezone=time_partitions_def.timezone,
             name=check.opt_str_param(name, "name", f"{job.name}_schedule"),
             description=check.opt_str_param(description, "description"),
         )(_get_schedule_evaluation_fn(partitions_def, job, tags))
 
 
 def _get_schedule_evaluation_fn(
     partitions_def: PartitionsDefinition,
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/policy.py` & `dagster-1.3.8/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/reconstruct.py` & `dagster-1.3.8/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.3.8/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.3.8/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.3.8/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -462,15 +462,15 @@
                 if isinstance(node_def, SubselectedGraphDefinition):
                     break
 
                 if node_def.name not in node_defs:
                     node_defs[node_def.name] = node_def
                     node_to_job[node_def.name] = job_def.name
 
-                if node_defs[node_def.name] != node_def:
+                if node_defs[node_def.name] is not node_def:
                     first_name, second_name = sorted([node_to_job[node_def.name], job_def.name])
                     raise DagsterInvalidDefinitionError(
                         f"Conflicting definitions found in repository with name '{node_def.name}'."
                         " Op/Graph definition names must be unique within a repository."
                         f" {node_def.__class__.__name__} is defined in"
                         f" job '{first_name}' and in"
                         f" job '{second_name}'."
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.3.8/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.3.8/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.3.8/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.3.8/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/resource_annotation.py` & `dagster-1.3.8/dagster/_core/definitions/resource_annotation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/resource_definition.py` & `dagster-1.3.8/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/resource_invocation.py` & `dagster-1.3.8/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/resource_requirement.py` & `dagster-1.3.8/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/run_config.py` & `dagster-1.3.8/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/run_config_schema.py` & `dagster-1.3.8/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/run_request.py` & `dagster-1.3.8/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.3.8/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/schedule_definition.py` & `dagster-1.3.8/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.3.8/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/selector.py` & `dagster-1.3.8/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/sensor_definition.py` & `dagster-1.3.8/dagster/_core/definitions/sensor_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,15 +374,15 @@
     SkipReason,
     RunRequest,
     DagsterRunReaction,
     SensorResult,
 ]
 RawSensorEvaluationFunction: TypeAlias = Callable[..., RawSensorEvaluationFunctionReturn]
 
-SensorEvaluationFunction: TypeAlias = Callable[..., Iterator[Union[SkipReason, RunRequest]]]
+SensorEvaluationFunction: TypeAlias = Callable[..., Sequence[Union[SkipReason, RunRequest]]]
 
 
 def get_context_param_name(fn: Callable) -> Optional[str]:
     """Determines the sensor's context parameter name by excluding all resource parameters."""
     resource_params = {param.name for param in get_resource_args(fn)}
 
     return next(
@@ -482,15 +482,15 @@
 
         Args:
             job (ExecutableDefinition): The job that should execute when this
                 schedule runs.
         """
         return SensorDefinition.dagster_internal_init(
             name=self.name,
-            evaluation_fn=self._evaluation_fn,
+            evaluation_fn=self._raw_fn,
             minimum_interval_seconds=self.minimum_interval_seconds,
             description=self.description,
             job_name=None,  # if original init was passed job name, was resolved to a job
             jobs=new_jobs if len(new_jobs) > 1 else None,
             job=new_jobs[0] if len(new_jobs) == 1 else None,
             default_status=self.default_status,
             asset_selection=self.asset_selection,
@@ -566,15 +566,15 @@
         self._raw_fn: RawSensorEvaluationFunction = check.callable_param(
             evaluation_fn, "evaluation_fn"
         )
         self._evaluation_fn: Union[
             SensorEvaluationFunction,
             Callable[
                 [SensorEvaluationContext],
-                Iterator[Union[SkipReason, RunRequest, DagsterRunReaction]],
+                List[Union[SkipReason, RunRequest, DagsterRunReaction]],
             ],
         ] = wrap_sensor_evaluation(self._name, evaluation_fn)
         self._min_interval = check.opt_int_param(
             minimum_interval_seconds, "minimum_interval_seconds", DEFAULT_SENSOR_DAEMON_INTERVAL
         )
         self._description = check.opt_str_param(description, "description")
         self._targets: Sequence[Union[RepoRelativeTarget, DirectTarget]] = check.opt_list_param(
@@ -696,15 +696,15 @@
 
         Returns:
             SensorExecutionData: Contains list of run requests, or skip message if present.
 
         """
         context = check.inst_param(context, "context", SensorEvaluationContext)
 
-        result = list(self._evaluation_fn(context))
+        result = self._evaluation_fn(context)
 
         skip_message: Optional[str] = None
         run_requests: List[RunRequest] = []
         dagster_run_reactions: List[DagsterRunReaction] = []
         dynamic_partitions_requests: Optional[
             Sequence[Union[AddDynamicPartitionsRequest, DeleteDynamicPartitionsRequest]]
         ] = []
@@ -972,30 +972,42 @@
             context.resources, sensor_name, resource_arg_names
         )
 
         context_param_name_if_present = get_context_param_name(fn)
         context_param = (
             {context_param_name_if_present: context} if context_param_name_if_present else {}
         )
-        result = fn(**context_param, **resource_args_populated)
+        raw_evaluation_result = fn(**context_param, **resource_args_populated)
 
-        if inspect.isgenerator(result) or isinstance(result, list):
-            for item in result:
-                yield item
-        elif isinstance(result, (SkipReason, RunRequest, SensorResult)):
-            yield result
-
-        elif result is not None:
-            raise Exception(
-                (
-                    "Error in sensor {sensor_name}: Sensor unexpectedly returned output "
-                    "{result} of type {type_}.  Should only return SkipReason or "
+        def check_returned_scalar(scalar):
+            if isinstance(scalar, (SkipReason, RunRequest, SensorResult)):
+                return scalar
+            elif scalar is not None:
+                raise Exception(
+                    f"Error in sensor {sensor_name}: Sensor unexpectedly returned output "
+                    f"{scalar} of type {type(scalar)}.  Should only return SkipReason or "
                     "RunRequest objects."
-                ).format(sensor_name=sensor_name, result=result, type_=type(result))
-            )
+                )
+
+        if inspect.isgenerator(raw_evaluation_result):
+            result = []
+            try:
+                while True:
+                    result.append(next(raw_evaluation_result))
+            except StopIteration as e:
+                # captures the case where the evaluation function has a yield and also returns a
+                # value
+                if e.value is not None:
+                    result.append(check_returned_scalar(e.value))
+
+            return result
+        elif isinstance(raw_evaluation_result, list):
+            return raw_evaluation_result
+        else:
+            return [check_returned_scalar(raw_evaluation_result)]
 
     return _wrapped_fn
 
 
 def build_sensor_context(
     instance: Optional[DagsterInstance] = None,
     cursor: Optional[str] = None,
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/source_asset.py` & `dagster-1.3.8/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/step_launcher.py` & `dagster-1.3.8/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/target.py` & `dagster-1.3.8/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.3.8/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.3.8/dagster/_core/definitions/time_window_partitions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1805,7 +1805,46 @@
             for dim in partitions_def.partitions_defs
             if isinstance(dim.partitions_def, TimeWindowPartitionsDefinition)
         ]
         if len(time_window_dims) == 1:
             return True
 
     return False
+
+
+def get_time_partitions_def(
+    partitions_def: Optional[PartitionsDefinition],
+) -> TimeWindowPartitionsDefinition:
+    from .multi_dimensional_partitions import MultiPartitionsDefinition
+
+    if partitions_def is None:
+        check.failed("Cannot get time partitions def from None object")
+    elif isinstance(partitions_def, TimeWindowPartitionsDefinition):
+        return partitions_def
+    elif isinstance(partitions_def, MultiPartitionsDefinition):
+        return cast(
+            TimeWindowPartitionsDefinition, partitions_def.time_window_dimension.partitions_def
+        )
+    else:
+        check.failed(
+            f"Cannot return time partitions def from non-time partitions def {partitions_def}"
+        )
+
+
+def get_time_partition_key(
+    partitions_def: Optional[PartitionsDefinition], partition_key: Optional[str]
+) -> str:
+    from .multi_dimensional_partitions import MultiPartitionsDefinition
+
+    if partitions_def is None or partition_key is None:
+        check.failed(
+            "Cannot get time partitions key from when partitions def is None or partition key is"
+            " None"
+        )
+    elif isinstance(partitions_def, TimeWindowPartitionsDefinition):
+        return partition_key
+    elif isinstance(partitions_def, MultiPartitionsDefinition):
+        return partitions_def.get_partition_key_from_str(partition_key).keys_by_dimension[
+            partitions_def.time_window_dimension.name
+        ]
+    else:
+        check.failed(f"Cannot get time partition from non-time partitions def {partitions_def}")
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.3.8/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from collections import defaultdict
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, Mapping, NamedTuple, Optional, Sequence, Union
+from typing import TYPE_CHECKING, AbstractSet, Any, Mapping, NamedTuple, Optional, Sequence, Union
 
 import dagster._check as check
 from dagster._core.definitions import AssetKey
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.errors import DagsterInvalidDefinitionError
 from dagster._utils.backcompat import deprecation_warning
 
 from .asset_layer import build_asset_selection_job
 from .config import ConfigMapping
+from .metadata import RawMetadataValue
 
 if TYPE_CHECKING:
     from dagster._core.definitions import (
         AssetsDefinition,
         AssetSelection,
         ExecutorDefinition,
+        HookDefinition,
         JobDefinition,
         PartitionedConfig,
         PartitionsDefinition,
         SourceAsset,
     )
     from dagster._core.definitions.asset_graph import InternalAssetGraph
     from dagster._core.definitions.asset_selection import CoercibleToAssetSelection
@@ -34,49 +36,56 @@
             ("selection", "AssetSelection"),
             (
                 "config",
                 Optional[Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig"]],
             ),
             ("description", Optional[str]),
             ("tags", Optional[Mapping[str, Any]]),
+            ("metadata", Optional[Mapping[str, RawMetadataValue]]),
             ("partitions_def", Optional["PartitionsDefinition"]),
             ("executor_def", Optional["ExecutorDefinition"]),
+            ("hooks", Optional[AbstractSet["HookDefinition"]]),
         ],
     )
 ):
     def __new__(
         cls,
         name: str,
         selection: "AssetSelection",
         config: Optional[
             Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig", "RunConfig"]
         ] = None,
         description: Optional[str] = None,
         tags: Optional[Mapping[str, Any]] = None,
+        metadata: Optional[Mapping[str, RawMetadataValue]] = None,
         partitions_def: Optional["PartitionsDefinition"] = None,
         executor_def: Optional["ExecutorDefinition"] = None,
+        hooks: Optional[AbstractSet["HookDefinition"]] = None,
     ):
         from dagster._core.definitions import (
             AssetSelection,
             ExecutorDefinition,
+            HookDefinition,
             PartitionsDefinition,
         )
         from dagster._core.definitions.run_config import convert_config_input
 
         return super(UnresolvedAssetJobDefinition, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             selection=check.inst_param(selection, "selection", AssetSelection),
             config=convert_config_input(config),
             description=check.opt_str_param(description, "description"),
             tags=check.opt_mapping_param(tags, "tags"),
+            metadata=check.opt_mapping_param(metadata, "metadata"),
             partitions_def=check.opt_inst_param(
                 partitions_def, "partitions_def", PartitionsDefinition
             ),
             executor_def=check.opt_inst_param(executor_def, "partitions_def", ExecutorDefinition),
+            hooks=check.opt_nullable_set_param(hooks, "hooks", of_type=HookDefinition),
         )
 
     def run_request_for_partition(
         self,
         partition_key: str,
         run_key: Optional[str] = None,
         tags: Optional[Mapping[str, str]] = None,
@@ -226,30 +235,34 @@
         return build_asset_selection_job(
             name=self.name,
             assets=assets,
             config=self.config,
             source_assets=source_assets,
             description=self.description,
             tags=self.tags,
+            metadata=self.metadata,
             asset_selection=selected_asset_keys,
             partitions_def=self.partitions_def if self.partitions_def else inferred_partitions_def,
             executor_def=self.executor_def or default_executor_def,
+            hooks=self.hooks,
         )
 
 
 def define_asset_job(
     name: str,
     selection: Optional["CoercibleToAssetSelection"] = None,
     config: Optional[
         Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig", "RunConfig"]
     ] = None,
     description: Optional[str] = None,
     tags: Optional[Mapping[str, Any]] = None,
+    metadata: Optional[Mapping[str, RawMetadataValue]] = None,
     partitions_def: Optional["PartitionsDefinition"] = None,
     executor_def: Optional["ExecutorDefinition"] = None,
+    hooks: Optional[AbstractSet["HookDefinition"]] = None,
 ) -> UnresolvedAssetJobDefinition:
     """Creates a definition of a job which will either materialize a selection of assets or observe
     a selection of source assets. This will only be resolved to a JobDefinition once placed in a
     code location.
 
     Args:
         name (str):
@@ -285,14 +298,18 @@
             determined by the config mapping, and the ConfigMapping, which should return
             configuration in the standard format to configure the job.
         tags (Optional[Mapping[str, Any]]):
             Arbitrary information that will be attached to the execution of the Job.
             Values that are not strings will be json encoded and must meet the criteria that
             `json.loads(json.dumps(value)) == value`.  These tag values may be overwritten by tag
             values provided at invocation time.
+        metadata (Optional[Mapping[str, RawMetadataValue]]): Arbitrary metadata about the job.
+            Keys are displayed string labels, and values are one of the following: string, float,
+            int, JSON-serializable dict, JSON-serializable list, and one of the data classes
+            returned by a MetadataValue static method.
         description (Optional[str]):
             A description for the Job.
         partitions_def (Optional[PartitionsDefinition]):
             Defines the set of partitions for this job. All AssetDefinitions selected for this job
             must have a matching PartitionsDefinition. If no PartitionsDefinition is provided, the
             PartitionsDefinition will be inferred from the selected AssetDefinitions.
         executor_def (Optional[ExecutorDefinition]):
@@ -365,10 +382,12 @@
 
     return UnresolvedAssetJobDefinition(
         name=name,
         selection=resolved_selection,
         config=config,
         description=description,
         tags=tags,
+        metadata=metadata,
         partitions_def=partitions_def,
         executor_def=executor_def,
+        hooks=hooks,
     )
```

### Comparing `dagster-1.3.7/dagster/_core/definitions/utils.py` & `dagster-1.3.8/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/definitions/version_strategy.py` & `dagster-1.3.8/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/errors.py` & `dagster-1.3.8/dagster/_core/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,14 +132,33 @@
                 invalid_type=invalid_type,
                 is_resource=is_resource,
             ),
             **kwargs,
         )
 
 
+class DagsterInvalidDagsterTypeInPythonicConfigDefinitionError(DagsterError):
+    """Indicates that you have attempted to construct a Pythonic config or resource class with a DagsterType
+    annotated field.
+    """
+
+    def __init__(
+        self,
+        config_class_name: str,
+        field_name: Optional[str],
+        **kwargs,
+    ):
+        self.field_name = field_name
+        super(DagsterInvalidDagsterTypeInPythonicConfigDefinitionError, self).__init__(
+            f"""Error defining Dagster config class '{config_class_name}' on field '{field_name}'. DagsterTypes cannot be used to annotate a config type. DagsterType is meant only for type checking and coercion in op and asset inputs and outputs.
+{PYTHONIC_CONFIG_ERROR_VERBIAGE}""",
+            **kwargs,
+        )
+
+
 CONFIG_ERROR_VERBIAGE = """
 This value can be a:
     - Field
     - Python primitive types that resolve to dagster config types
         - int, float, bool, str, list.
     - A dagster config type: Int, Float, Bool, Array, Optional, Selector, Shape, Permissive, Map
     - A bare python dictionary, which is wrapped in Field(Shape(...)). Any values
```

### Comparing `dagster-1.3.7/dagster/_core/event_api.py` & `dagster-1.3.8/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/events/__init__.py` & `dagster-1.3.8/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/events/log.py` & `dagster-1.3.8/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/events/utils.py` & `dagster-1.3.8/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/api.py` & `dagster-1.3.8/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/asset_backfill.py` & `dagster-1.3.8/dagster/_core/execution/asset_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/backfill.py` & `dagster-1.3.8/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/build_resources.py` & `dagster-1.3.8/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/compute_logs.py` & `dagster-1.3.8/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/context/compute.py` & `dagster-1.3.8/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/context/hook.py` & `dagster-1.3.8/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/context/init.py` & `dagster-1.3.8/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/context/input.py` & `dagster-1.3.8/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/context/invocation.py` & `dagster-1.3.8/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/context/logger.py` & `dagster-1.3.8/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/context/output.py` & `dagster-1.3.8/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/context/system.py` & `dagster-1.3.8/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/context_creation_job.py` & `dagster-1.3.8/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/execute_in_process.py` & `dagster-1.3.8/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.3.8/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/execution_result.py` & `dagster-1.3.8/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/host_mode.py` & `dagster-1.3.8/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/job_backfill.py` & `dagster-1.3.8/dagster/_core/execution/job_backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/job_execution_result.py` & `dagster-1.3.8/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/memoization.py` & `dagster-1.3.8/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/active.py` & `dagster-1.3.8/dagster/_core/execution/plan/active.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,43 +27,49 @@
 from dagster._core.execution.context.system import (
     IPlanContext,
     PlanExecutionContext,
     PlanOrchestrationContext,
 )
 from dagster._core.execution.plan.state import KnownExecutionState
 from dagster._core.execution.retries import RetryMode, RetryState
-from dagster._core.storage.tags import PRIORITY_TAG
+from dagster._core.storage.tags import GLOBAL_CONCURRENCY_TAG, PRIORITY_TAG
 from dagster._utils.interrupts import pop_captured_interrupt
 from dagster._utils.tags import TagConcurrencyLimitsCounter
 
+from .instance_concurrency_context import InstanceConcurrencyContext
 from .outputs import StepOutputData, StepOutputHandle
 from .plan import ExecutionPlan
 from .step import ExecutionStep
 
 
 def _default_sort_key(step: ExecutionStep) -> float:
     return int(step.tags.get(PRIORITY_TAG, 0)) * -1
 
 
+CONCURRENCY_CLAIM_BLOCKED_INTERVAL = 1
+
+
 class ActiveExecution:
     """State machine used to track progress through execution of an ExecutionPlan."""
 
     def __init__(
         self,
         execution_plan: ExecutionPlan,
         retry_mode: RetryMode,
         sort_key_fn: Optional[Callable[[ExecutionStep], float]] = None,
         max_concurrent: Optional[int] = None,
         tag_concurrency_limits: Optional[List[Dict[str, Any]]] = None,
+        instance_concurrency_context: Optional[InstanceConcurrencyContext] = None,
     ):
         self._plan: ExecutionPlan = check.inst_param(
             execution_plan, "execution_plan", ExecutionPlan
         )
         self._retry_mode = check.inst_param(retry_mode, "retry_mode", RetryMode)
         self._retry_state = self._plan.known_state.get_retry_state()
+        self._instance_concurrency_context = instance_concurrency_context
 
         self._sort_key_fn: Callable[[ExecutionStep], float] = (
             check.opt_callable_param(
                 sort_key_fn,
                 "sort_key_fn",
             )
             or _default_sort_key
@@ -119,38 +125,32 @@
         self._update()
 
     def __enter__(self) -> Self:
         self._context_guard = True
         return self
 
     def __exit__(
-        self, exc_type: Type[Exception], exc_value: Exception, traceback: TracebackType
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_value: Optional[BaseException],
+        traceback: Optional[TracebackType],
     ) -> None:
         self._context_guard = False
 
         # Exiting due to exception, return to allow exception to bubble
         if exc_type or exc_value or traceback:
             return
 
         if not self.is_complete:
-            pending_action = (
-                self._executable + self._pending_abandon + self._pending_retry + self._pending_skip
-            )
-            state_str = "{pending_str}{in_flight_str}{action_str}{retry_str}".format(
-                in_flight_str=f"\nSteps still in flight: {self._in_flight}"
-                if self._in_flight
-                else "",
-                pending_str=f"\nSteps pending processing: {self._pending.keys()}"
-                if self._pending
-                else "",
-                action_str=f"\nSteps pending action: {pending_action}" if pending_action else "",
-                retry_str=f"\nSteps waiting to retry: {self._waiting_to_retry.keys()}"
-                if self._waiting_to_retry
-                else "",
-            )
+            # generate the state string before exiting the concurrency context
+            state_str = self._pending_state_str()
+        else:
+            state_str = ""
+
+        if not self.is_complete:
             if self._interrupted:
                 raise DagsterExecutionInterruptedError(
                     f"Execution was interrupted before completing the execution plan. {state_str}"
                 )
             else:
                 raise DagsterInvariantViolationError(
                     f"Execution finished without completing the execution plan. {state_str}"
@@ -167,14 +167,37 @@
             else:
                 raise DagsterUnknownStepStateError(
                     "Execution exited with steps {step_list} in an unknown state to this"
                     " process.\nThis was likely caused by losing communication with the process"
                     " performing step execution.".format(step_list=self._unknown_state)
                 )
 
+    def _pending_state_str(self) -> str:
+        assert not self.is_complete
+        pending_action = (
+            self._executable + self._pending_abandon + self._pending_retry + self._pending_skip
+        )
+        return "{pending_str}{in_flight_str}{action_str}{retry_str}{claim_str}".format(
+            in_flight_str=f"\nSteps still in flight: {self._in_flight}" if self._in_flight else "",
+            pending_str=f"\nSteps pending processing: {self._pending.keys()}"
+            if self._pending
+            else "",
+            action_str=f"\nSteps pending action: {pending_action}" if pending_action else "",
+            retry_str=f"\nSteps waiting to retry: {self._waiting_to_retry.keys()}"
+            if self._waiting_to_retry
+            else "",
+            claim_str=(
+                "\nSteps waiting to claim:"
+                f" {self._instance_concurrency_context.pending_claim_steps()}"
+            )
+            if self._instance_concurrency_context
+            and self._instance_concurrency_context.has_pending_claims()
+            else "",
+        )
+
     def _update(self) -> None:
         """Moves steps from _pending to _executable / _pending_skip / _pending_retry
         as a function of what has been _completed.
         """
         new_steps_to_execute: List[str] = []
         new_steps_to_skip: List[str] = []
         new_steps_to_abandon: List[str] = []
@@ -243,34 +266,46 @@
             if tick_time >= at_time:
                 ready_to_retry.append(key)
 
         for key in ready_to_retry:
             self._executable.append(key)
             del self._waiting_to_retry[key]
 
-    def sleep_til_ready(self) -> None:
+    def sleep_interval(self):
         now = time.time()
-        sleep_amt = min([ready_at - now for ready_at in self._waiting_to_retry.values()])
+        intervals = []
+        if self._waiting_to_retry:
+            for t in self._waiting_to_retry.values():
+                intervals.append(t - now)
+        if (
+            self._instance_concurrency_context
+            and self._instance_concurrency_context.has_pending_claims()
+        ):
+            intervals.append(
+                self._instance_concurrency_context.interval_to_next_pending_claim_check()
+            )
+        if intervals:
+            return min(intervals)
+
+        return 0
+
+    def sleep_til_ready(self) -> None:
+        sleep_amt = self.sleep_interval()
         if sleep_amt > 0:
             time.sleep(sleep_amt)
 
-    def get_next_step(self) -> ExecutionStep:
+    def get_next_step(self) -> Optional[ExecutionStep]:
         check.invariant(not self.is_complete, "Can not call get_next_step when is_complete is True")
 
         steps = self.get_steps_to_execute(limit=1)
-        step = None
 
-        if steps:
-            step = steps[0]
-        elif self._waiting_to_retry:
-            self.sleep_til_ready()
-            step = self.get_next_step()
+        if not steps:
+            return None
 
-        check.invariant(step is not None, "Unexpected ActiveExecution state")
-        return step  # type: ignore  # (possible none)
+        return steps[0]
 
     def get_step_by_key(self, step_key: str) -> ExecutionStep:
         step = self._plan.get_step_by_key(step_key)
         return cast(ExecutionStep, check.inst(step, ExecutionStep))
 
     def get_steps_to_execute(
         self,
@@ -285,18 +320,18 @@
         self._update()
 
         steps = sorted(
             [self.get_step_by_key(key) for key in self._executable],
             key=self._sort_key_fn,
         )
 
-        tag_concurrency_limits_counter = None
+        run_scoped_concurrency_limits_counter = None
         if self._tag_concurrency_limits:
             in_flight_steps = [self.get_step_by_key(key) for key in self._in_flight]
-            tag_concurrency_limits_counter = TagConcurrencyLimitsCounter(
+            run_scoped_concurrency_limits_counter = TagConcurrencyLimitsCounter(
                 self._tag_concurrency_limits,
                 in_flight_steps,
             )
 
         batch: List[ExecutionStep] = []
 
         for step in steps:
@@ -305,19 +340,32 @@
 
             if (
                 self._max_concurrent is not None
                 and len(batch) + len(self._in_flight) >= self._max_concurrent
             ):
                 break
 
-            if tag_concurrency_limits_counter:
-                if tag_concurrency_limits_counter.is_blocked(step):
+            if run_scoped_concurrency_limits_counter:
+                if run_scoped_concurrency_limits_counter.is_blocked(step):
                     continue
 
-                tag_concurrency_limits_counter.update_counters_with_launched_item(step)
+            if run_scoped_concurrency_limits_counter:
+                run_scoped_concurrency_limits_counter.update_counters_with_launched_item(step)
+
+            step_concurrency_key = step.tags.get(GLOBAL_CONCURRENCY_TAG)
+            if step_concurrency_key and self._instance_concurrency_context:
+                try:
+                    priority = int(step.tags.get(PRIORITY_TAG, 0))
+                except ValueError:
+                    priority = 0
+
+                if not self._instance_concurrency_context.claim(
+                    step_concurrency_key, step.key, priority
+                ):
+                    continue
 
             batch.append(step)
 
         for step in batch:
             self._in_flight.add(step.key)
             self._executable.remove(step.key)
             self._prep_for_dynamic_outputs(step)
@@ -453,25 +501,31 @@
 
     def handle_event(self, dagster_event: DagsterEvent) -> None:
         check.inst_param(dagster_event, "dagster_event", DagsterEvent)
 
         step_key = cast(str, dagster_event.step_key)
         if dagster_event.is_step_failure:
             self.mark_failed(step_key)
+            if self._instance_concurrency_context:
+                self._instance_concurrency_context.free_step(step_key)
         elif dagster_event.is_resource_init_failure:
             # Resources are only initialized without a step key in the
             # in-process case, and resource initalization happens before the
             # ActiveExecution object is created.
             check.invariant(
                 dagster_event.step_key is not None,
                 "Resource init failure was reported during execution without a step key.",
             )
             self.mark_failed(step_key)
+            if self._instance_concurrency_context:
+                self._instance_concurrency_context.free_step(step_key)
         elif dagster_event.is_step_success:
             self.mark_success(step_key)
+            if self._instance_concurrency_context:
+                self._instance_concurrency_context.free_step(step_key)
         elif dagster_event.is_step_skipped:
             # Skip events are generated by this class. They should not be sent via handle_event
             raise DagsterInvariantViolationError(
                 f"Step {step_key} was reported as skipped from outside the ActiveExecution."
             )
         elif dagster_event.is_step_up_for_retry:
             self.mark_up_for_retry(
@@ -517,14 +571,18 @@
             len(self._pending) == 0
             and len(self._in_flight) == 0
             and len(self._executable) == 0
             and len(self._pending_skip) == 0
             and len(self._pending_retry) == 0
             and len(self._pending_abandon) == 0
             and len(self._waiting_to_retry) == 0
+            and (
+                not self._instance_concurrency_context
+                or not self._instance_concurrency_context.has_pending_claims()
+            )
         )
 
     @property
     def retry_state(self) -> RetryState:
         return self._retry_state
 
     def get_known_state(self) -> KnownExecutionState:
```

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/compute.py` & `dagster-1.3.8/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.3.8/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.3.8/dagster/_core/execution/plan/execute_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from contextlib import ExitStack
-from typing import Iterator, Sequence, cast
+from typing import Iterator, Optional, Sequence, cast
 
 import dagster._check as check
 from dagster._core.definitions import Failure, HookExecutionResult, RetryRequested
 from dagster._core.errors import (
     DagsterError,
     DagsterExecutionInterruptedError,
     DagsterMaxRetriesExceededError,
@@ -12,34 +12,40 @@
     HookExecutionError,
     user_code_error_boundary,
 )
 from dagster._core.events import DagsterEvent, EngineEventData
 from dagster._core.execution.compute_logs import create_compute_log_file_key
 from dagster._core.execution.context.system import PlanExecutionContext, StepExecutionContext
 from dagster._core.execution.plan.execute_step import core_dagster_event_sequence_for_step
+from dagster._core.execution.plan.instance_concurrency_context import InstanceConcurrencyContext
 from dagster._core.execution.plan.objects import (
     ErrorSource,
     StepFailureData,
     StepRetryData,
     UserFailureData,
     step_failure_event_from_exc_info,
 )
 from dagster._core.execution.plan.plan import ExecutionPlan
 from dagster._core.storage.captured_log_manager import CapturedLogManager
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 
 
 def inner_plan_execution_iterator(
-    job_context: PlanExecutionContext, execution_plan: ExecutionPlan
+    job_context: PlanExecutionContext,
+    execution_plan: ExecutionPlan,
+    instance_concurrency_context: Optional[InstanceConcurrencyContext] = None,
 ) -> Iterator[DagsterEvent]:
     check.inst_param(job_context, "pipeline_context", PlanExecutionContext)
     check.inst_param(execution_plan, "execution_plan", ExecutionPlan)
     compute_log_manager = job_context.instance.compute_log_manager
     step_keys = [step.key for step in execution_plan.get_steps_to_execute_in_topo_order()]
-    with execution_plan.start(retry_mode=job_context.retry_mode) as active_execution:
+    with execution_plan.start(
+        retry_mode=job_context.retry_mode,
+        instance_concurrency_context=instance_concurrency_context,
+    ) as active_execution:
         with ExitStack() as capture_stack:
             # begin capturing logs for the whole process if this is a captured log manager
             if isinstance(compute_log_manager, CapturedLogManager):
                 file_key = create_compute_log_file_key()
                 log_key = compute_log_manager.build_log_key_for_run(job_context.run_id, file_key)
                 try:
                     log_context = capture_stack.enter_context(
@@ -50,14 +56,19 @@
                     yield from _handle_compute_log_setup_error(job_context, sys.exc_info())
 
             # It would be good to implement a reference tracking algorithm here to
             # garbage collect results that are no longer needed by any steps
             # https://github.com/dagster-io/dagster/issues/811
             while not active_execution.is_complete:
                 step = active_execution.get_next_step()
+
+                if not step:
+                    active_execution.sleep_til_ready()
+                    continue
+
                 step_context = cast(
                     StepExecutionContext,
                     job_context.for_step(step, active_execution.get_known_state()),
                 )
                 step_event_list = []
 
                 missing_resources = [
```

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/execute_step.py` & `dagster-1.3.8/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/external_step.py` & `dagster-1.3.8/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/handle.py` & `dagster-1.3.8/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/inputs.py` & `dagster-1.3.8/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.3.8/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/objects.py` & `dagster-1.3.8/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/outputs.py` & `dagster-1.3.8/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/plan.py` & `dagster-1.3.8/dagster/_core/execution/plan/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     DagsterUnmetExecutorRequirementsError,
 )
 from dagster._core.execution.plan.handle import (
     ResolvedFromDynamicStepHandle,
     StepHandle,
     UnresolvedStepHandle,
 )
+from dagster._core.execution.plan.instance_concurrency_context import InstanceConcurrencyContext
 from dagster._core.execution.retries import RetryMode
 from dagster._core.instance import DagsterInstance, InstanceRef
 from dagster._core.storage.mem_io_manager import mem_io_manager
 from dagster._core.system_config.objects import ResolvedRunConfig
 from dagster._core.utils import toposort
 
 from ..context.output import get_output_context
@@ -915,23 +916,25 @@
 
     def start(
         self,
         retry_mode: RetryMode,
         sort_key_fn: Optional[Callable[[ExecutionStep], float]] = None,
         max_concurrent: Optional[int] = None,
         tag_concurrency_limits: Optional[List[Dict[str, Any]]] = None,
+        instance_concurrency_context: Optional[InstanceConcurrencyContext] = None,
     ) -> "ActiveExecution":
         from .active import ActiveExecution
 
         return ActiveExecution(
             self,
             retry_mode,
             sort_key_fn,
             max_concurrent,
             tag_concurrency_limits,
+            instance_concurrency_context=instance_concurrency_context,
         )
 
     def step_handle_for_single_step_plans(
         self,
     ) -> Optional[Union[StepHandle, ResolvedFromDynamicStepHandle]]:
         # Temporary hack to isolate single-step plans, which are often the representation of
         # sub-plans in a multiprocessing execution environment.  We want to attribute pipeline
```

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/state.py` & `dagster-1.3.8/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/step.py` & `dagster-1.3.8/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/plan/utils.py` & `dagster-1.3.8/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.3.8/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/resolve_versions.py` & `dagster-1.3.8/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/resources_init.py` & `dagster-1.3.8/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/retries.py` & `dagster-1.3.8/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.3.8/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/stats.py` & `dagster-1.3.8/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/tags.py` & `dagster-1.3.8/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/validate_run_config.py` & `dagster-1.3.8/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/watch_orphans.py` & `dagster-1.3.8/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/execution/with_resources.py` & `dagster-1.3.8/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/executor/base.py` & `dagster-1.3.8/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/executor/child_process_executor.py` & `dagster-1.3.8/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/executor/in_process.py` & `dagster-1.3.8/dagster/_core/executor/in_process.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 import os
 from typing import Iterator, Optional
 
 import dagster._check as check
 from dagster._core.events import DagsterEvent, EngineEventData
 from dagster._core.execution.api import ExecuteRunWithPlanIterable
-from dagster._core.execution.context.system import PlanOrchestrationContext
+from dagster._core.execution.context.system import PlanExecutionContext, PlanOrchestrationContext
 from dagster._core.execution.context_creation_job import PlanExecutionContextManager
 from dagster._core.execution.plan.execute_plan import inner_plan_execution_iterator
+from dagster._core.execution.plan.instance_concurrency_context import InstanceConcurrencyContext
 from dagster._core.execution.plan.plan import ExecutionPlan
 from dagster._core.execution.retries import RetryMode
 from dagster._utils.timing import format_duration, time_execution_scope
 
 from .base import Executor
 
 
+def inprocess_execution_iterator(
+    job_context: PlanExecutionContext,
+    execution_plan: ExecutionPlan,
+    instance_concurrency_context: Optional[InstanceConcurrencyContext] = None,
+) -> Iterator[DagsterEvent]:
+    with InstanceConcurrencyContext(
+        job_context.instance, job_context.run_id
+    ) as instance_concurrency_context:
+        yield from inner_plan_execution_iterator(
+            job_context, execution_plan, instance_concurrency_context
+        )
+
+
 class InProcessExecutor(Executor):
     def __init__(self, retries: RetryMode, marker_to_close: Optional[str] = None):
         self._retries = check.inst_param(retries, "retries", RetryMode)
         self.marker_to_close = check.opt_str_param(marker_to_close, "marker_to_close")
 
     @property
     def retries(self) -> RetryMode:
@@ -37,15 +51,15 @@
             event_specific_data=EngineEventData.in_process(os.getpid(), step_keys_to_execute),
         )
 
         with time_execution_scope() as timer_result:
             yield from iter(
                 ExecuteRunWithPlanIterable(
                     execution_plan=plan_context.execution_plan,
-                    iterator=inner_plan_execution_iterator,
+                    iterator=inprocess_execution_iterator,
                     execution_context_manager=PlanExecutionContextManager(
                         job=plan_context.job,
                         retry_mode=plan_context.retry_mode,
                         execution_plan=plan_context.execution_plan,
                         run_config=plan_context.run_config,
                         dagster_run=plan_context.dagster_run,
                         instance=plan_context.instance,
```

### Comparing `dagster-1.3.7/dagster/_core/executor/init.py` & `dagster-1.3.8/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/executor/multiprocess.py` & `dagster-1.3.8/dagster/_core/executor/multiprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import multiprocessing
 import os
 import sys
+from contextlib import ExitStack
 from multiprocessing.context import BaseContext as MultiprocessingBaseContext
 from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Mapping, Optional, Sequence
 
 from dagster import (
     _check as check,
 )
 from dagster._core.definitions.metadata import MetadataValue
@@ -16,24 +17,25 @@
     DagsterUnmetExecutorRequirementsError,
 )
 from dagster._core.events import DagsterEvent, EngineEventData
 from dagster._core.execution.api import create_execution_plan, execute_plan_iterator
 from dagster._core.execution.context.system import IStepContext, PlanOrchestrationContext
 from dagster._core.execution.context_creation_job import create_context_free_log_manager
 from dagster._core.execution.plan.active import ActiveExecution
+from dagster._core.execution.plan.instance_concurrency_context import InstanceConcurrencyContext
 from dagster._core.execution.plan.objects import StepFailureData
 from dagster._core.execution.plan.plan import ExecutionPlan
 from dagster._core.execution.plan.state import KnownExecutionState
 from dagster._core.execution.plan.step import ExecutionStep
 from dagster._core.execution.retries import RetryMode
 from dagster._core.executor.base import Executor
 from dagster._core.instance import DagsterInstance
 from dagster._utils import get_run_crash_explanation, start_termination_thread
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
-from dagster._utils.timing import format_duration, time_execution_scope
+from dagster._utils.timing import TimerResult, format_duration, time_execution_scope
 
 from .child_process_executor import (
     ChildProcessCommand,
     ChildProcessCrashException,
     ChildProcessEvent,
     ChildProcessSystemErrorEvent,
     execute_child_process_command,
@@ -182,154 +184,155 @@
                 pid=os.getpid()
             ),
             event_specific_data=EngineEventData.multiprocess(
                 os.getpid(), step_keys_to_execute=execution_plan.step_keys_to_execute
             ),
         )
 
-        with time_execution_scope() as timer_result:
-            with ActiveExecution(
-                execution_plan,
-                retry_mode=self.retries,
-                max_concurrent=limit,
-                tag_concurrency_limits=tag_concurrency_limits,
-            ) as active_execution:
-                active_iters: Dict[str, Iterator[Optional[DagsterEvent]]] = {}
-                errors: Dict[int, SerializableErrorInfo] = {}
-                term_events: Dict[str, Any] = {}
-                stopping: bool = False
-
-                while (not stopping and not active_execution.is_complete) or active_iters:
-                    if active_execution.check_for_interrupts():
-                        yield DagsterEvent.engine_event(
-                            plan_context,
-                            (
-                                "Multiprocess executor: received termination signal - "
-                                "forwarding to active child processes"
-                            ),
-                            EngineEventData.interrupted(list(term_events.keys())),
-                        )
-                        stopping = True
-                        active_execution.mark_interrupted()
-                        for key, event in term_events.items():
-                            event.set()
-
-                    while not stopping:
-                        steps = active_execution.get_steps_to_execute(
-                            limit=(limit - len(active_iters)),
-                        )
-
-                        if not steps:
-                            break
+        timer_result: Optional[TimerResult] = None
+        with ExitStack() as stack:
+            timer_result = stack.enter_context(time_execution_scope())
+            instance_concurrency_context = stack.enter_context(
+                InstanceConcurrencyContext(plan_context.instance, plan_context.run_id)
+            )
+            active_execution = stack.enter_context(
+                ActiveExecution(
+                    execution_plan,
+                    retry_mode=self.retries,
+                    max_concurrent=limit,
+                    tag_concurrency_limits=tag_concurrency_limits,
+                    instance_concurrency_context=instance_concurrency_context,
+                )
+            )
+            active_iters: Dict[str, Iterator[Optional[DagsterEvent]]] = {}
+            errors: Dict[int, SerializableErrorInfo] = {}
+            term_events: Dict[str, Any] = {}
+            stopping: bool = False
 
-                        for step in steps:
-                            step_context = plan_context.for_step(step)
-                            term_events[step.key] = multiproc_ctx.Event()
-                            active_iters[step.key] = execute_step_out_of_process(
-                                multiproc_ctx,
-                                job,
-                                step_context,
-                                step,
-                                errors,
-                                term_events,
-                                self.retries,
-                                active_execution.get_known_state(),
-                                execution_plan.repository_load_data,
-                            )
-
-                    # process active iterators
-                    empty_iters = []
-                    for key, step_iter in active_iters.items():
-                        try:
-                            event_or_none = next(step_iter)
-                            if event_or_none is None:
-                                continue
-                            else:
-                                yield event_or_none
-                                active_execution.handle_event(event_or_none)
-
-                        except ChildProcessCrashException as crash:
-                            serializable_error = serializable_error_info_from_exc_info(
-                                sys.exc_info()
-                            )
-                            step_context = plan_context.for_step(
-                                active_execution.get_step_by_key(key)
-                            )
-                            yield DagsterEvent.engine_event(
-                                step_context,
-                                get_run_crash_explanation(
-                                    prefix=f"Multiprocess executor: child process for step {key}",
-                                    exit_code=crash.exit_code,
-                                ),
-                                EngineEventData.engine_error(serializable_error),
-                            )
-                            step_failure_event = DagsterEvent.step_failure_event(
-                                step_context=plan_context.for_step(
-                                    active_execution.get_step_by_key(key)
-                                ),
-                                step_failure_data=StepFailureData(
-                                    error=serializable_error, user_failure_data=None
-                                ),
-                            )
-                            active_execution.handle_event(step_failure_event)
-                            yield step_failure_event
-                            empty_iters.append(key)
-                        except StopIteration:
-                            empty_iters.append(key)
-
-                    # clear and mark complete finished iterators
-                    for key in empty_iters:
-                        del active_iters[key]
-                        del term_events[key]
-                        active_execution.verify_complete(plan_context, key)
-
-                    # process skipped and abandoned steps
-                    yield from active_execution.plan_events_iterator(plan_context)
-
-                errs = {pid: err for pid, err in errors.items() if err}
-
-                # After termination starts, raise an interrupted exception once all subprocesses
-                # have finished cleaning up (and the only errors were from being interrupted)
-                if (
-                    stopping
-                    and (not active_iters)
-                    and all(
-                        [
-                            err_info.cls_name == "DagsterExecutionInterruptedError"
-                            for err_info in errs.values()
-                        ]
-                    )
-                ):
+            while (not stopping and not active_execution.is_complete) or active_iters:
+                if active_execution.check_for_interrupts():
                     yield DagsterEvent.engine_event(
                         plan_context,
-                        "Multiprocess executor: interrupted all active child processes",
-                        event_specific_data=EngineEventData(),
-                    )
-                    raise DagsterExecutionInterruptedError()
-                elif errs:
-                    raise DagsterSubprocessError(
-                        "During multiprocess execution errors occurred in child"
-                        " processes:\n{error_list}".format(
-                            error_list="\n".join(
-                                [
-                                    f"In process {pid}: {err.to_string()}"
-                                    for pid, err in errs.items()
-                                ]
-                            )
+                        (
+                            "Multiprocess executor: received termination signal - "
+                            "forwarding to active child processes"
                         ),
-                        subprocess_error_infos=list(errs.values()),
+                        EngineEventData.interrupted(list(term_events.keys())),
+                    )
+                    stopping = True
+                    active_execution.mark_interrupted()
+                    for key, event in term_events.items():
+                        event.set()
+
+                while not stopping:
+                    steps = active_execution.get_steps_to_execute(
+                        limit=(limit - len(active_iters)),
                     )
 
-        yield DagsterEvent.engine_event(
-            plan_context,
-            "Multiprocess executor: parent process exiting after {duration} (pid: {pid})".format(
-                duration=format_duration(timer_result.millis), pid=os.getpid()
-            ),
-            event_specific_data=EngineEventData.multiprocess(os.getpid()),
-        )
+                    if not steps:
+                        break
+
+                    for step in steps:
+                        step_context = plan_context.for_step(step)
+                        term_events[step.key] = multiproc_ctx.Event()
+                        active_iters[step.key] = execute_step_out_of_process(
+                            multiproc_ctx,
+                            job,
+                            step_context,
+                            step,
+                            errors,
+                            term_events,
+                            self.retries,
+                            active_execution.get_known_state(),
+                            execution_plan.repository_load_data,
+                        )
+
+                # process active iterators
+                empty_iters = []
+                for key, step_iter in active_iters.items():
+                    try:
+                        event_or_none = next(step_iter)
+                        if event_or_none is None:
+                            continue
+                        else:
+                            yield event_or_none
+                            active_execution.handle_event(event_or_none)
+
+                    except ChildProcessCrashException as crash:
+                        serializable_error = serializable_error_info_from_exc_info(sys.exc_info())
+                        step_context = plan_context.for_step(active_execution.get_step_by_key(key))
+                        yield DagsterEvent.engine_event(
+                            step_context,
+                            get_run_crash_explanation(
+                                prefix=f"Multiprocess executor: child process for step {key}",
+                                exit_code=crash.exit_code,
+                            ),
+                            EngineEventData.engine_error(serializable_error),
+                        )
+                        step_failure_event = DagsterEvent.step_failure_event(
+                            step_context=plan_context.for_step(
+                                active_execution.get_step_by_key(key)
+                            ),
+                            step_failure_data=StepFailureData(
+                                error=serializable_error, user_failure_data=None
+                            ),
+                        )
+                        active_execution.handle_event(step_failure_event)
+                        yield step_failure_event
+                        empty_iters.append(key)
+                    except StopIteration:
+                        empty_iters.append(key)
+
+                # clear and mark complete finished iterators
+                for key in empty_iters:
+                    del active_iters[key]
+                    del term_events[key]
+                    active_execution.verify_complete(plan_context, key)
+
+                # process skipped and abandoned steps
+                yield from active_execution.plan_events_iterator(plan_context)
+
+            errs = {pid: err for pid, err in errors.items() if err}
+
+            # After termination starts, raise an interrupted exception once all subprocesses
+            # have finished cleaning up (and the only errors were from being interrupted)
+            if (
+                stopping
+                and (not active_iters)
+                and all(
+                    [
+                        err_info.cls_name == "DagsterExecutionInterruptedError"
+                        for err_info in errs.values()
+                    ]
+                )
+            ):
+                yield DagsterEvent.engine_event(
+                    plan_context,
+                    "Multiprocess executor: interrupted all active child processes",
+                    event_specific_data=EngineEventData(),
+                )
+                raise DagsterExecutionInterruptedError()
+            elif errs:
+                raise DagsterSubprocessError(
+                    "During multiprocess execution errors occurred in child"
+                    " processes:\n{error_list}".format(
+                        error_list="\n".join(
+                            [f"In process {pid}: {err.to_string()}" for pid, err in errs.items()]
+                        )
+                    ),
+                    subprocess_error_infos=list(errs.values()),
+                )
+
+        if timer_result:
+            yield DagsterEvent.engine_event(
+                plan_context,
+                "Multiprocess executor: parent process exiting after {duration} (pid: {pid})"
+                .format(duration=format_duration(timer_result.millis), pid=os.getpid()),
+                event_specific_data=EngineEventData.multiprocess(os.getpid()),
+            )
 
 
 def execute_step_out_of_process(
     multiproc_ctx: MultiprocessingBaseContext,
     recon_job: ReconstructableJob,
     step_context: IStepContext,
     step: ExecutionStep,
```

### Comparing `dagster-1.3.7/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.3.8/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import pendulum
 
 import dagster._check as check
 from dagster._core.definitions.metadata import MetadataValue
 from dagster._core.events import DagsterEvent, DagsterEventType, EngineEventData
 from dagster._core.execution.context.system import PlanOrchestrationContext
 from dagster._core.execution.plan.active import ActiveExecution
+from dagster._core.execution.plan.instance_concurrency_context import InstanceConcurrencyContext
 from dagster._core.execution.plan.objects import StepFailureData
 from dagster._core.execution.plan.plan import ExecutionPlan
 from dagster._core.execution.plan.step import ExecutionStep
 from dagster._core.execution.retries import RetryMode
 from dagster._core.executor.step_delegating.step_handler.base import StepHandler, StepHandlerContext
 from dagster._grpc.types import ExecuteStepArgs
 from dagster._utils.error import serializable_error_info_from_exc_info
@@ -102,209 +103,218 @@
         self._event_cursor = -1
 
         DagsterEvent.engine_event(
             plan_context,
             f"Starting execution with step handler {self._step_handler.name}.",
             EngineEventData(),
         )
+        with InstanceConcurrencyContext(
+            plan_context.instance, plan_context.run_id
+        ) as instance_concurrency_context:
+            with ActiveExecution(
+                execution_plan,
+                retry_mode=self.retries,
+                max_concurrent=self._max_concurrent,
+                tag_concurrency_limits=self._tag_concurrency_limits,
+                instance_concurrency_context=instance_concurrency_context,
+            ) as active_execution:
+                running_steps: Dict[str, ExecutionStep] = {}
 
-        with ActiveExecution(
-            execution_plan,
-            retry_mode=self.retries,
-            max_concurrent=self._max_concurrent,
-            tag_concurrency_limits=self._tag_concurrency_limits,
-        ) as active_execution:
-            running_steps: Dict[str, ExecutionStep] = {}
-
-            if plan_context.resume_from_failure:
-                DagsterEvent.engine_event(
-                    plan_context,
-                    "Resuming execution from failure",
-                    EngineEventData(),
-                )
-
-                prior_events = self._pop_events(
-                    plan_context.instance,
-                    plan_context.run_id,
-                )
-                for dagster_event in prior_events:
-                    yield dagster_event
-
-                possibly_in_flight_steps = active_execution.rebuild_from_events(prior_events)
-                for step in possibly_in_flight_steps:
-                    step_handler_context = self._get_step_handler_context(
-                        plan_context, [step], active_execution
-                    )
-
+                if plan_context.resume_from_failure:
                     DagsterEvent.engine_event(
-                        step_handler_context.get_step_context(step.key),
-                        f"Checking on status of in-progress step {step.key} from previous run",
+                        plan_context,
+                        "Resuming execution from failure",
                         EngineEventData(),
                     )
 
-                    should_retry_step = False
-                    health_check = None
+                    prior_events = self._pop_events(
+                        plan_context.instance,
+                        plan_context.run_id,
+                    )
+                    for dagster_event in prior_events:
+                        yield dagster_event
+
+                    possibly_in_flight_steps = active_execution.rebuild_from_events(prior_events)
+                    for step in possibly_in_flight_steps:
+                        step_handler_context = self._get_step_handler_context(
+                            plan_context, [step], active_execution
+                        )
 
-                    try:
-                        health_check = self._step_handler.check_step_health(step_handler_context)
-                    except Exception:
-                        # For now we assume that an exception indicates that the step should be resumed.
-                        # This should probably be a separate should_resume_step method on the step handler.
                         DagsterEvent.engine_event(
                             step_handler_context.get_step_context(step.key),
-                            (
-                                f"Including {step.key} in the new run since it raised an error when"
-                                " checking whether it was running"
-                            ),
-                            EngineEventData(
-                                error=serializable_error_info_from_exc_info(sys.exc_info())
-                            ),
+                            f"Checking on status of in-progress step {step.key} from previous run",
+                            EngineEventData(),
                         )
-                        should_retry_step = True
-                    else:
-                        if not health_check.is_healthy:
+
+                        should_retry_step = False
+                        health_check = None
+
+                        try:
+                            health_check = self._step_handler.check_step_health(
+                                step_handler_context
+                            )
+                        except Exception:
+                            # For now we assume that an exception indicates that the step should be resumed.
+                            # This should probably be a separate should_resume_step method on the step handler.
                             DagsterEvent.engine_event(
                                 step_handler_context.get_step_context(step.key),
                                 (
-                                    f"Including step {step.key} in the new run since it is not"
-                                    f" currently running: {health_check.unhealthy_reason}"
+                                    f"Including {step.key} in the new run since it raised an error"
+                                    " when checking whether it was running"
+                                ),
+                                EngineEventData(
+                                    error=serializable_error_info_from_exc_info(sys.exc_info())
                                 ),
                             )
                             should_retry_step = True
-
-                    if should_retry_step:
-                        # health check failed, launch the step
-                        list(
-                            self._step_handler.launch_step(
-                                self._get_step_handler_context(
-                                    plan_context, [step], active_execution
+                        else:
+                            if not health_check.is_healthy:
+                                DagsterEvent.engine_event(
+                                    step_handler_context.get_step_context(step.key),
+                                    (
+                                        f"Including step {step.key} in the new run since it is not"
+                                        f" currently running: {health_check.unhealthy_reason}"
+                                    ),
                                 )
-                            )
-                        )
-
-                    running_steps[step.key] = step
-
-            last_check_step_health_time = pendulum.now("UTC")
+                                should_retry_step = True
 
-            # Order of events is important here. During an interation, we call handle_event, then get_steps_to_execute,
-            # then is_complete. get_steps_to_execute updates the state of ActiveExecution, and without it
-            # is_complete can return true when we're just between steps.
-            while not active_execution.is_complete:
-                if active_execution.check_for_interrupts():
-                    active_execution.mark_interrupted()
-                    if not plan_context.instance.run_will_resume(plan_context.run_id):
-                        DagsterEvent.engine_event(
-                            plan_context,
-                            "Executor received termination signal, forwarding to steps",
-                            EngineEventData.interrupted(list(running_steps.keys())),
-                        )
-                        for _, step in running_steps.items():
+                        if should_retry_step:
+                            # health check failed, launch the step
                             list(
-                                self._step_handler.terminate_step(
+                                self._step_handler.launch_step(
                                     self._get_step_handler_context(
                                         plan_context, [step], active_execution
                                     )
                                 )
                             )
-                    else:
-                        DagsterEvent.engine_event(
-                            plan_context,
-                            (
-                                "Executor received termination signal, not forwarding to steps"
-                                " because run will be resumed"
-                            ),
-                            EngineEventData(
-                                metadata={
-                                    "steps_in_flight": MetadataValue.text(str(running_steps.keys()))
-                                },
-                            ),
-                        )
 
-                    return
+                        running_steps[step.key] = step
 
-                for dagster_event in self._pop_events(
-                    plan_context.instance,
-                    plan_context.run_id,
-                ):
-                    yield dagster_event
-                    # STEP_SKIPPED events are only emitted by ActiveExecution, which already handles
-                    # and yields them.
-
-                    if dagster_event.is_step_skipped:
-                        assert isinstance(dagster_event.step_key, str)
-                        active_execution.verify_complete(plan_context, dagster_event.step_key)
-                    else:
-                        active_execution.handle_event(dagster_event)
-                        if (
-                            dagster_event.is_step_success
-                            or dagster_event.is_step_failure
-                            or dagster_event.is_resource_init_failure
-                            or dagster_event.is_step_up_for_retry
-                        ):
-                            assert isinstance(dagster_event.step_key, str)
-                            del running_steps[dagster_event.step_key]
+                last_check_step_health_time = pendulum.now("UTC")
 
-                            if not dagster_event.is_step_up_for_retry:
-                                active_execution.verify_complete(
-                                    plan_context, dagster_event.step_key
+                # Order of events is important here. During an interation, we call handle_event, then get_steps_to_execute,
+                # then is_complete. get_steps_to_execute updates the state of ActiveExecution, and without it
+                # is_complete can return true when we're just between steps.
+                while not active_execution.is_complete:
+                    if active_execution.check_for_interrupts():
+                        active_execution.mark_interrupted()
+                        if not plan_context.instance.run_will_resume(plan_context.run_id):
+                            DagsterEvent.engine_event(
+                                plan_context,
+                                "Executor received termination signal, forwarding to steps",
+                                EngineEventData.interrupted(list(running_steps.keys())),
+                            )
+                            for _, step in running_steps.items():
+                                list(
+                                    self._step_handler.terminate_step(
+                                        self._get_step_handler_context(
+                                            plan_context, [step], active_execution
+                                        )
+                                    )
                                 )
+                        else:
+                            DagsterEvent.engine_event(
+                                plan_context,
+                                (
+                                    "Executor received termination signal, not forwarding to steps"
+                                    " because run will be resumed"
+                                ),
+                                EngineEventData(
+                                    metadata={
+                                        "steps_in_flight": MetadataValue.text(
+                                            str(running_steps.keys())
+                                        )
+                                    },
+                                ),
+                            )
 
-                # process skips from failures or uncovered inputs
-                list(active_execution.plan_events_iterator(plan_context))
+                        return
 
-                curr_time = pendulum.now("UTC")
-                if (
-                    curr_time - last_check_step_health_time
-                ).total_seconds() >= self._check_step_health_interval_seconds:
-                    last_check_step_health_time = curr_time
-                    for _, step in running_steps.items():
-                        step_context = plan_context.for_step(step)
+                    for dagster_event in self._pop_events(
+                        plan_context.instance,
+                        plan_context.run_id,
+                    ):
+                        yield dagster_event
+                        # STEP_SKIPPED events are only emitted by ActiveExecution, which already handles
+                        # and yields them.
 
-                        try:
-                            health_check_result = self._step_handler.check_step_health(
-                                self._get_step_handler_context(
-                                    plan_context, [step], active_execution
+                        if dagster_event.is_step_skipped:
+                            assert isinstance(dagster_event.step_key, str)
+                            active_execution.verify_complete(plan_context, dagster_event.step_key)
+                        else:
+                            active_execution.handle_event(dagster_event)
+                            if (
+                                dagster_event.is_step_success
+                                or dagster_event.is_step_failure
+                                or dagster_event.is_resource_init_failure
+                                or dagster_event.is_step_up_for_retry
+                            ):
+                                assert isinstance(dagster_event.step_key, str)
+                                del running_steps[dagster_event.step_key]
+
+                                if not dagster_event.is_step_up_for_retry:
+                                    active_execution.verify_complete(
+                                        plan_context, dagster_event.step_key
+                                    )
+
+                    # process skips from failures or uncovered inputs
+                    list(active_execution.plan_events_iterator(plan_context))
+
+                    curr_time = pendulum.now("UTC")
+                    if (
+                        curr_time - last_check_step_health_time
+                    ).total_seconds() >= self._check_step_health_interval_seconds:
+                        last_check_step_health_time = curr_time
+                        for _, step in running_steps.items():
+                            step_context = plan_context.for_step(step)
+
+                            try:
+                                health_check_result = self._step_handler.check_step_health(
+                                    self._get_step_handler_context(
+                                        plan_context, [step], active_execution
+                                    )
                                 )
-                            )
-                            if not health_check_result.is_healthy:
+                                if not health_check_result.is_healthy:
+                                    DagsterEvent.step_failure_event(
+                                        step_context=step_context,
+                                        step_failure_data=StepFailureData(
+                                            error=None,
+                                            user_failure_data=None,
+                                        ),
+                                        message=(
+                                            f"Step {step.key} failed health check:"
+                                            f" {health_check_result.unhealthy_reason}"
+                                        ),
+                                    )
+                            except Exception:
+                                serializable_error = serializable_error_info_from_exc_info(
+                                    sys.exc_info()
+                                )
+                                # Log a step failure event if there was an error during the health
+                                # check
                                 DagsterEvent.step_failure_event(
-                                    step_context=step_context,
+                                    step_context=plan_context.for_step(step),
                                     step_failure_data=StepFailureData(
-                                        error=None,
+                                        error=serializable_error,
                                         user_failure_data=None,
                                     ),
-                                    message=(
-                                        f"Step {step.key} failed health check:"
-                                        f" {health_check_result.unhealthy_reason}"
-                                    ),
                                 )
-                        except Exception:
-                            serializable_error = serializable_error_info_from_exc_info(
-                                sys.exc_info()
-                            )
-                            # Log a step failure event if there was an error during the health
-                            # check
-                            DagsterEvent.step_failure_event(
-                                step_context=plan_context.for_step(step),
-                                step_failure_data=StepFailureData(
-                                    error=serializable_error,
-                                    user_failure_data=None,
-                                ),
-                            )
 
-                if self._max_concurrent is not None:
-                    max_steps_to_run = self._max_concurrent - len(running_steps)
-                    check.invariant(
-                        max_steps_to_run >= 0, "More steps are active than max_concurrent"
-                    )
-                else:
-                    max_steps_to_run = None  # disables limit
+                    if self._max_concurrent is not None:
+                        max_steps_to_run = self._max_concurrent - len(running_steps)
+                        check.invariant(
+                            max_steps_to_run >= 0, "More steps are active than max_concurrent"
+                        )
+                    else:
+                        max_steps_to_run = None  # disables limit
 
-                for step in active_execution.get_steps_to_execute(max_steps_to_run):
-                    running_steps[step.key] = step
-                    list(
-                        self._step_handler.launch_step(
-                            self._get_step_handler_context(plan_context, [step], active_execution)
+                    for step in active_execution.get_steps_to_execute(max_steps_to_run):
+                        running_steps[step.key] = step
+                        list(
+                            self._step_handler.launch_step(
+                                self._get_step_handler_context(
+                                    plan_context, [step], active_execution
+                                )
+                            )
                         )
-                    )
 
-                time.sleep(self._sleep_seconds)
+                    time.sleep(self._sleep_seconds)
```

### Comparing `dagster-1.3.7/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.3.8/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/host_representation/__init__.py` & `dagster-1.3.8/dagster/_core/host_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/host_representation/code_location.py` & `dagster-1.3.8/dagster/_core/host_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/host_representation/external.py` & `dagster-1.3.8/dagster/_core/host_representation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/host_representation/external_data.py` & `dagster-1.3.8/dagster/_core/host_representation/external_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/host_representation/grpc_server_registry.py` & `dagster-1.3.8/dagster/_core/host_representation/grpc_server_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,14 +144,20 @@
     ) -> TypeGuard[ManagedGrpcPythonEnvCodeLocationOrigin]:
         return isinstance(code_location_origin, ManagedGrpcPythonEnvCodeLocationOrigin)
 
     @property
     def supports_reload(self) -> bool:
         return True
 
+    def clear_all_grpc_endpoints(self):
+        # Free the map entry for all origins so that subsequent calls to _get_grpc_endpoint wil
+        # create a new process
+        with self._lock:
+            self._active_entries.clear()
+
     def reload_grpc_endpoint(
         self, code_location_origin: ManagedGrpcPythonEnvCodeLocationOrigin
     ) -> GrpcServerEndpoint:
         check.inst_param(code_location_origin, "code_location_origin", CodeLocationOrigin)
         with self._lock:
             origin_id = code_location_origin.get_id()
             if origin_id in self._active_entries:
```

### Comparing `dagster-1.3.7/dagster/_core/host_representation/grpc_server_state_subscriber.py` & `dagster-1.3.8/dagster/_core/host_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/host_representation/handle.py` & `dagster-1.3.8/dagster/_core/host_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/host_representation/historical.py` & `dagster-1.3.8/dagster/_core/host_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/host_representation/job_index.py` & `dagster-1.3.8/dagster/_core/host_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/host_representation/origin.py` & `dagster-1.3.8/dagster/_core/host_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/host_representation/represented.py` & `dagster-1.3.8/dagster/_core/host_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/instance/__init__.py` & `dagster-1.3.8/dagster/_core/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/instance/config.py` & `dagster-1.3.8/dagster/_core/instance/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,25 +333,27 @@
             {
                 "enabled": Field(Bool, is_required=False),
                 "start_timeout_seconds": Field(int, is_required=False),
                 "cancel_timeout_seconds": Field(int, is_required=False),
                 "max_resume_run_attempts": Field(int, is_required=False),
                 "poll_interval_seconds": Field(int, is_required=False),
                 "cancellation_thread_poll_interval_seconds": Field(int, is_required=False),
+                "free_slots_after_run_end_seconds": Field(int, is_required=False),
             },
         ),
         "run_retries": Field(
             {
                 "enabled": Field(bool, is_required=False, default_value=False),
                 "max_retries": Field(int, is_required=False, default_value=0),
             }
         ),
         "code_servers": Field(
             {
                 "local_startup_timeout": Field(int, is_required=False),
+                "reload_timeout": Field(int, is_required=False),
                 "wait_for_local_processes_on_shutdown": Field(bool, is_required=False),
             },
             is_required=False,
         ),
         "secrets": secrets_loader_config_schema(),
         "retention": retention_config_schema(),
         "sensors": sensors_daemon_config(),
```

### Comparing `dagster-1.3.7/dagster/_core/instance/ref.py` & `dagster-1.3.8/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/instance_for_test.py` & `dagster-1.3.8/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/launcher/base.py` & `dagster-1.3.8/dagster/_core/launcher/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
 
 class CheckRunHealthResult(NamedTuple):
     """Result of a check_run_worker_health call."""
 
     status: WorkerStatus
     msg: Optional[str] = None
+    transient: Optional[bool] = None
+    run_worker_id: Optional[str] = None  # Identifier for a particular run worker
 
     def __str__(self) -> str:
         return f"{self.status.value}: '{self.msg}'"
 
 
 class RunLauncher(ABC, MayHaveInstanceWeakref[T_DagsterInstance]):
     @abstractmethod
```

### Comparing `dagster-1.3.7/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.3.8/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.3.8/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/log_manager.py` & `dagster-1.3.8/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/nux.py` & `dagster-1.3.8/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/origin.py` & `dagster-1.3.8/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/run_coordinator/base.py` & `dagster-1.3.8/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.3.8/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.3.8/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/scheduler/__init__.py` & `dagster-1.3.8/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/scheduler/execution.py` & `dagster-1.3.8/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/scheduler/instigation.py` & `dagster-1.3.8/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/scheduler/scheduler.py` & `dagster-1.3.8/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/secrets/env_file.py` & `dagster-1.3.8/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/selector/subset_selector.py` & `dagster-1.3.8/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/snap/__init__.py` & `dagster-1.3.8/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/snap/dagster_types.py` & `dagster-1.3.8/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/snap/dep_snapshot.py` & `dagster-1.3.8/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.3.8/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/snap/job_snapshot.py` & `dagster-1.3.8/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/snap/mode.py` & `dagster-1.3.8/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/snap/node.py` & `dagster-1.3.8/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.3.8/dagster/_core/snap/snap_to_yaml.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,18 @@
 
 
 def default_values_from_type_snap(type_snap: ConfigTypeSnap, snapshot: ConfigSchemaSnapshot) -> Any:
     """Given a type snap and a snapshot, returns a dictionary of default values for the type
     snap, recursively assembling a default if the type snap does not have a default value
     explicitly set.
     """
-    defaults_by_field = {}
+    if not type_snap.fields:
+        return {}
 
+    defaults_by_field = {}
     for field_name in type_snap.field_names:
         field = type_snap.get_field(field_name)
 
         default_value_as_json = field.default_value_as_json_str
         field_snap = (
             snapshot.get_config_snap(field.type_key)
             if snapshot.has_config_snap(field.type_key)
```

### Comparing `dagster-1.3.7/dagster/_core/storage/DEVELOPING.md` & `dagster-1.3.8/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/README.md` & `dagster-1.3.8/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/env.py` & `dagster-1.3.8/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files 25% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 depends_on = None
 
 
 def upgrade():
     inspector = inspect(op.get_bind())
     has_tables = inspector.get_table_names()
 
+    if op.get_context().dialect.name == "sqlite":
+        return
+
     if "runs" in has_tables and "run_tags" in has_tables:
         op.drop_constraint("run_tags_run_id_fkey", table_name="run_tags", type_="foreignkey")
         op.create_foreign_key(
             "run_tags_run_id_fkey",
             source_table="run_tags",
             referent_table="runs",
             local_cols=["run_id"],
@@ -33,14 +36,17 @@
         )
 
 
 def downgrade():
     inspector = inspect(op.get_bind())
     has_tables = inspector.get_table_names()
 
+    if op.get_context().dialect.name == "sqlite":
+        return
+
     if "runs" in has_tables and "run_tags" in has_tables:
         op.drop_constraint("run_tags_run_id_fkey", table_name="run_tags", type_="foreignkey")
         op.create_foreign_key(
             "run_tags_run_id_fkey",
             source_table="run_tags",
             referent_table="runs",
             local_cols=["run_id"],
```

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.3.8/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/asset_value_loader.py` & `dagster-1.3.8/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/base_storage.py` & `dagster-1.3.8/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.3.8/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/captured_log_manager.py` & `dagster-1.3.8/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.3.8/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/compute_log_manager.py` & `dagster-1.3.8/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/config.py` & `dagster-1.3.8/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/dagster_run.py` & `dagster-1.3.8/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/db_io_manager.py` & `dagster-1.3.8/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/event_log/__init__.py` & `dagster-1.3.8/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/event_log/base.py` & `dagster-1.3.8/dagster/_core/storage/event_log/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     build_run_step_stats_from_events,
 )
 from dagster._core.instance import MayHaveInstanceWeakref, T_DagsterInstance
 from dagster._core.storage.dagster_run import DagsterRunStatsSnapshot
 from dagster._core.storage.sql import AlembicVersion
 from dagster._seven import json
 from dagster._utils import PrintFn
+from dagster._utils.concurrency import ConcurrencyClaimStatus, ConcurrencyKeyInfo
 
 if TYPE_CHECKING:
     from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
 
 
 class EventLogConnection(NamedTuple):
     records: Sequence[EventLogRecord]
@@ -407,7 +408,56 @@
     def alembic_version(self) -> Optional[AlembicVersion]:
         return None
 
     @property
     def is_run_sharded(self) -> bool:
         """Indicates that the EventLogStoarge is sharded."""
         return False
+
+    @property
+    def supports_global_concurrency_limits(self) -> bool:
+        """Indicates that the EventLogStorage supports global concurrency limits."""
+        return False
+
+    @abstractmethod
+    def set_concurrency_slots(self, concurrency_key: str, num: int) -> None:
+        """Allocate concurrency slots for the given concurrency key."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def get_concurrency_keys(self) -> Set[str]:
+        """Get the set of concurrency limited keys."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def get_concurrency_info(self, concurrency_key: str) -> ConcurrencyKeyInfo:
+        """Get concurrency info for key."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def claim_concurrency_slot(
+        self, concurrency_key: str, run_id: str, step_key: str, priority: Optional[int] = None
+    ) -> ConcurrencyClaimStatus:
+        """Claim concurrency slots for step."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def check_concurrency_claim(
+        self, concurrency_key: str, run_id: str, step_key: str
+    ) -> ConcurrencyClaimStatus:
+        """Claim concurrency slots for step."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def get_concurrency_run_ids(self) -> Set[str]:
+        """Get a list of run_ids that are occupying or waiting for a concurrency key slot."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def free_concurrency_slots_for_run(self, run_id: str) -> None:
+        """Frees concurrency slots for a given run."""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def free_concurrency_slot_for_step(self, run_id: str, step_key: str) -> None:
+        """Frees concurrency slots for a given run/step."""
+        raise NotImplementedError()
```

### Comparing `dagster-1.3.7/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.3.8/dagster/_core/storage/event_log/in_memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import uuid
 from collections import defaultdict
 from contextlib import contextmanager
 from typing import Callable, Optional
 
+import sqlalchemy as db
 from sqlalchemy.pool import NullPool
 
 from dagster._core.storage.event_log.base import EventLogCursor
 from dagster._core.storage.sql import create_engine, get_alembic_config, stamp_alembic_rev
 from dagster._core.storage.sqlite import create_in_memory_conn_string
 from dagster._serdes import ConfigurableClass
 from dagster._serdes.config_class import ConfigurableClassData
@@ -29,39 +30,40 @@
             poolclass=NullPool,
         )
         self._handlers = defaultdict(set)
         self._storage_id = 0  # mirror the storage id, to mimic watching cursors
 
         # hold one connection for life of instance, but vend new ones for specific calls
         self._held_conn = self._engine.connect()
+        with self._held_conn.begin():
+            SqlEventLogStorageMetadata.create_all(self._held_conn)
+            alembic_config = get_alembic_config(__file__, "sqlite/alembic/alembic.ini")
+            stamp_alembic_rev(alembic_config, self._held_conn)
 
-        SqlEventLogStorageMetadata.create_all(self._held_conn)
-        alembic_config = get_alembic_config(__file__, "sqlite/alembic/alembic.ini")
-        stamp_alembic_rev(alembic_config, self._held_conn)
         self.reindex_events()
         self.reindex_assets()
 
         if preload:
             for payload in preload:
                 for event in payload.event_list:
                     self.store_event(event)
 
     @contextmanager
-    def run_connection(self, run_id=None):
+    def _connect(self):
         with self._engine.connect() as conn:
-            conn.execute("PRAGMA journal_mode=WAL;")
-            conn.execute("PRAGMA foreign_keys=ON;")
-            yield conn
+            with conn.begin():
+                conn.execute(db.text("PRAGMA journal_mode=WAL;"))
+                conn.execute(db.text("PRAGMA foreign_keys=ON;"))
+                yield conn
+
+    def run_connection(self, run_id=None):
+        return self._connect()
 
-    @contextmanager
     def index_connection(self):
-        with self._engine.connect() as conn:
-            conn.execute("PRAGMA journal_mode=WAL;")
-            conn.execute("PRAGMA foreign_keys=ON;")
-            yield conn
+        return self._connect()
 
     def has_table(self, table_name: str) -> bool:
         with self._engine.connect() as conn:
             return bool(self._engine.dialect.has_table(conn, table_name))
 
     @property
     def inst_data(self):
@@ -96,10 +98,14 @@
         if handler in self._handlers[run_id]:
             self._handlers[run_id].remove(handler)
 
     @property
     def is_persistent(self) -> bool:
         return False
 
+    @property
+    def supports_global_concurrency_limits(self) -> bool:
+        return False
+
     def dispose(self):
         self._held_conn.close()
         self._engine.dispose()
```

### Comparing `dagster-1.3.7/dagster/_core/storage/event_log/migration.py` & `dagster-1.3.8/dagster/_core/storage/event_log/migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import NamedTuple
 
 import sqlalchemy as db
 from tqdm import tqdm
 
 from dagster._core.assets import AssetDetails
 from dagster._core.events.log import EventLogEntry
+from dagster._core.storage.sqlalchemy_compat import db_select
 from dagster._serdes.serdes import deserialize_value
 from dagster._utils import utc_datetime_from_timestamp
 
 SECONDARY_INDEX_ASSET_KEY = "asset_key_table"  # builds the asset key table from the event log
 ASSET_KEY_INDEX_COLS = "asset_key_index_columns"  # extracts index columns from the asset_keys table
 
 EVENT_LOG_DATA_MIGRATIONS = {
@@ -44,15 +45,15 @@
 
     from .schema import AssetKeyTable, SqlEventLogStorageTable
 
     if not isinstance(event_log_storage, SqlEventLogStorage):
         return
 
     query = (
-        db.select([SqlEventLogStorageTable.c.asset_key])
+        db_select([SqlEventLogStorageTable.c.asset_key])
         .where(SqlEventLogStorageTable.c.asset_key != None)  # noqa: E711
         .group_by(SqlEventLogStorageTable.c.asset_key)
     )
     with event_log_storage.index_connection() as conn:
         if print_fn:
             print_fn("Querying event logs.")
         to_insert = conn.execute(query).fetchall()
@@ -82,15 +83,15 @@
     if not isinstance(event_log_storage, SqlEventLogStorage):
         return
 
     with event_log_storage.index_connection() as conn:
         if print_fn:
             print_fn("Querying asset keys.")
         results = conn.execute(
-            db.select(
+            db_select(
                 [
                     AssetKeyTable.c.asset_key,
                     AssetKeyTable.c.asset_details,
                     AssetKeyTable.c.last_materialization,
                 ]
             )
         ).fetchall()
@@ -114,15 +115,15 @@
                 event_or_materialization = deserialize_value(last_materialization_str, NamedTuple)
 
                 if isinstance(event_or_materialization, EventLogEntry):
                     event = event_or_materialization
 
             if not event:
                 materialization_query = (
-                    db.select([SqlEventLogStorageTable.c.event])
+                    db_select([SqlEventLogStorageTable.c.event])
                     .where(
                         SqlEventLogStorageTable.c.asset_key == asset_key.to_string(),
                     )
                     .order_by(SqlEventLogStorageTable.c.timestamp.desc())
                     .limit(1)
                 )
                 materialization_row = conn.execute(materialization_query).fetchone()
@@ -160,15 +161,15 @@
                 )
 
 
 def sql_asset_event_generator(conn, cursor=None, batch_size=1000):
     from .schema import SqlEventLogStorageTable
 
     while True:
-        query = db.select([SqlEventLogStorageTable.c.id, SqlEventLogStorageTable.c.event]).where(
+        query = db_select([SqlEventLogStorageTable.c.id, SqlEventLogStorageTable.c.event]).where(
             SqlEventLogStorageTable.c.asset_key != None  # noqa: E711
         )
         if cursor:
             query = query.where(SqlEventLogStorageTable.c.id < cursor)
         query = query.order_by(SqlEventLogStorageTable.c.id.desc()).limit(batch_size)
         fetched = conn.execute(query).fetchall()
```

### Comparing `dagster-1.3.7/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.3.8/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/event_log/schema.py` & `dagster-1.3.8/dagster/_core/storage/event_log/schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,14 +76,46 @@
     SqlEventLogStorageMetadata,
     db.Column("id", db.Integer, primary_key=True, autoincrement=True),
     db.Column("partitions_def_name", db.Text, nullable=False),
     db.Column("partition", db.Text, nullable=False),
     db.Column("create_timestamp", db.DateTime, server_default=get_current_timestamp()),
 )
 
+ConcurrencySlotsTable = db.Table(
+    "concurrency_slots",
+    SqlEventLogStorageMetadata,
+    db.Column(
+        "id",
+        db.BigInteger().with_variant(sqlite.INTEGER(), "sqlite"),
+        primary_key=True,
+        autoincrement=True,
+    ),
+    db.Column("concurrency_key", db.Text, nullable=False),
+    db.Column("run_id", db.Text),
+    db.Column("step_key", db.Text),
+    db.Column("deleted", db.Boolean, nullable=False, default=False),
+    db.Column("create_timestamp", db.DateTime, server_default=get_current_timestamp()),
+)
+
+PendingStepsTable = db.Table(
+    "pending_steps",
+    SqlEventLogStorageMetadata,
+    db.Column(
+        "id",
+        db.BigInteger().with_variant(sqlite.INTEGER(), "sqlite"),
+        primary_key=True,
+        autoincrement=True,
+    ),
+    db.Column("concurrency_key", db.Text, nullable=False),
+    db.Column("run_id", db.Text),
+    db.Column("step_key", db.Text),
+    db.Column("priority", db.Integer),
+    db.Column("assigned_timestamp", db.DateTime),
+    db.Column("create_timestamp", db.DateTime, server_default=get_current_timestamp()),
+)
 
 db.Index(
     "idx_step_key",
     SqlEventLogStorageTable.c.step_key,
     mysql_length=32,
 )
 db.Index(
@@ -134,7 +166,15 @@
 db.Index(
     "idx_dynamic_partitions",
     DynamicPartitionsTable.c.partitions_def_name,
     DynamicPartitionsTable.c.partition,
     mysql_length={"partitions_def_name": 64, "partition": 64},
     unique=True,
 )
+db.Index(
+    "idx_pending_steps",
+    PendingStepsTable.c.concurrency_key,
+    PendingStepsTable.c.run_id,
+    PendingStepsTable.c.step_key,
+    mysql_length={"concurrency_key": 255, "run_id": 255, "step_key": 32},
+    unique=True,
+)
```

### Comparing `dagster-1.3.7/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.3.8/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.3.8/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 from collections import defaultdict
 from contextlib import contextmanager
 from typing import Any, Mapping, Optional
 
+import sqlalchemy as db
 from sqlalchemy.pool import NullPool
 from typing_extensions import Self
 from watchdog.events import PatternMatchingEventHandler
 from watchdog.observers import Observer
 
 import dagster._check as check
 from dagster._config import StringSource
@@ -84,31 +85,29 @@
         alembic_config = get_alembic_config(__file__)
 
         should_mark_indexes = False
         with engine.connect() as connection:
             db_revision, head_revision = check_alembic_revision(alembic_config, connection)
             if not (db_revision and head_revision):
                 SqlEventLogStorageMetadata.create_all(engine)
-                engine.execute("PRAGMA journal_mode=WAL;")
+                connection.execute(db.text("PRAGMA journal_mode=WAL;"))
                 stamp_alembic_rev(alembic_config, connection)
                 should_mark_indexes = True
 
         if should_mark_indexes:
             # mark all secondary indexes
             self.reindex_events()
             self.reindex_assets()
 
     @contextmanager
     def _connect(self):
         engine = create_engine(self._conn_string, poolclass=NullPool)
-        conn = engine.connect()
-        try:
-            yield conn
-        finally:
-            conn.close()
+        with engine.connect() as conn:
+            with conn.begin():
+                yield conn
 
     def run_connection(self, run_id: Optional[str]) -> SqlDbConnection:
         return self._connect()
 
     def index_connection(self):
         return self._connect()
 
@@ -142,14 +141,18 @@
             self._obs.start()
             self._obs.schedule(
                 ConsolidatedSqliteEventLogStorageWatchdog(self), self._base_dir, True
             )
 
         self._watchers[run_id][callback] = cursor
 
+    @property
+    def supports_global_concurrency_limits(self) -> bool:
+        return False
+
     def on_modified(self):
         keys = [
             (run_id, callback)
             for run_id, callback_dict in self._watchers.items()
             for callback, _ in callback_dict.items()
         ]
         for run_id, callback in keys:
```

### Comparing `dagster-1.3.7/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.3.8/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     AlembicVersion,
     check_alembic_revision,
     create_engine,
     get_alembic_config,
     run_alembic_upgrade,
     stamp_alembic_rev,
 )
+from dagster._core.storage.sqlalchemy_compat import db_select
 from dagster._core.storage.sqlite import create_db_conn_string
 from dagster._serdes import (
     ConfigurableClass,
     ConfigurableClassData,
 )
 from dagster._serdes.errors import DeserializationError
 from dagster._serdes.serdes import deserialize_value
@@ -164,15 +165,15 @@
         while True:
             try:
                 with engine.connect() as connection:
                     db_revision, head_revision = check_alembic_revision(alembic_config, connection)
 
                     if not (db_revision and head_revision):
                         SqlEventLogStorageMetadata.create_all(engine)
-                        connection.execute("PRAGMA journal_mode=WAL;")
+                        connection.execute(db.text("PRAGMA journal_mode=WAL;"))
                         stamp_alembic_rev(alembic_config, connection)
 
                 break
             except (db_exc.DatabaseError, sqlite3.DatabaseError, sqlite3.OperationalError) as exc:
                 # This is SQLite-specific handling for concurrency issues that can arise when
                 # multiple processes (e.g. the dagit process and user code process) contend with
                 # each other to init the db. When we hit the following errors, we know that another
@@ -208,20 +209,17 @@
             conn_string = self.conn_string_for_shard(shard)
             engine = create_engine(conn_string, poolclass=NullPool)
 
             if shard not in self._initialized_dbs:
                 self._initdb(engine)
                 self._initialized_dbs.add(shard)
 
-            conn = engine.connect()
-
-            try:
-                yield conn
-            finally:
-                conn.close()
+            with engine.connect() as conn:
+                with conn.begin():
+                    yield conn
             engine.dispose()
 
     def run_connection(self, run_id: Optional[str] = None) -> Any:
         return self._connect(run_id)  # type: ignore  # bad sig
 
     def index_connection(self) -> ContextManager[Connection]:
         return self._connect(INDEX_SHARD_NAME)
@@ -284,15 +282,15 @@
         if is_asset_query:
             # asset materializations, observations and materialization planned events
             # get mirrored into the index shard, so no custom run shard-aware cursor logic needed
             return super(SqliteEventLogStorage, self).get_event_records(
                 event_records_filter=event_records_filter, limit=limit, ascending=ascending
             )
 
-        query = db.select([SqlEventLogStorageTable.c.id, SqlEventLogStorageTable.c.event])
+        query = db_select([SqlEventLogStorageTable.c.id, SqlEventLogStorageTable.c.event])
         if event_records_filter.asset_key:
             asset_details = next(iter(self._get_assets_details([event_records_filter.asset_key])))
         else:
             asset_details = None
 
         if event_records_filter.after_cursor is not None and not isinstance(
             event_records_filter.after_cursor, RunShardedEventsCursor
@@ -422,14 +420,18 @@
         with self.index_connection() as conn:
             return check_alembic_revision(alembic_config, conn)
 
     @property
     def is_run_sharded(self) -> bool:
         return True
 
+    @property
+    def supports_global_concurrency_limits(self) -> bool:
+        return False
+
 
 class SqliteEventLogStorageWatchdog(PatternMatchingEventHandler):
     def __init__(
         self,
         event_log_storage: SqliteEventLogStorage,
         run_id: str,
         callback: EventHandlerFn,
```

### Comparing `dagster-1.3.7/dagster/_core/storage/file_manager.py` & `dagster-1.3.8/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/fs_io_manager.py` & `dagster-1.3.8/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/input_manager.py` & `dagster-1.3.8/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/io_manager.py` & `dagster-1.3.8/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/legacy_storage.py` & `dagster-1.3.8/dagster/_core/storage/legacy_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     _check as check,
 )
 from dagster._config.config_schema import UserConfigSchema
 from dagster._core.definitions.asset_reconciliation_sensor import AutoMaterializeAssetEvaluation
 from dagster._core.event_api import EventHandlerFn
 from dagster._serdes import ConfigurableClass, ConfigurableClassData
 from dagster._utils import PrintFn
+from dagster._utils.concurrency import ConcurrencyClaimStatus, ConcurrencyKeyInfo
 
 from .base_storage import DagsterStorage
 from .event_log.base import (
     AssetRecord,
     EventLogConnection,
     EventLogRecord,
     EventLogStorage,
@@ -541,14 +542,44 @@
         limit: Optional[int] = None,
         ascending: bool = True,
     ) -> EventLogConnection:
         return self._storage.event_log_storage.get_records_for_run(
             run_id, cursor, of_type, limit, ascending
         )
 
+    def set_concurrency_slots(self, concurrency_key: str, num: int) -> None:
+        return self._storage.event_log_storage.set_concurrency_slots(concurrency_key, num)
+
+    def get_concurrency_keys(self) -> Set[str]:
+        return self._storage.event_log_storage.get_concurrency_keys()
+
+    def get_concurrency_info(self, concurrency_key: str) -> ConcurrencyKeyInfo:
+        return self._storage.event_log_storage.get_concurrency_info(concurrency_key)
+
+    def claim_concurrency_slot(
+        self, concurrency_key: str, run_id: str, step_key: str, priority: Optional[int] = None
+    ) -> ConcurrencyClaimStatus:
+        return self._storage.event_log_storage.claim_concurrency_slot(
+            concurrency_key, run_id, step_key, priority
+        )
+
+    def check_concurrency_claim(self, concurrency_key: str, run_id: str, step_key: str):
+        return self._storage.event_log_storage.check_concurrency_claim(
+            concurrency_key, run_id, step_key
+        )
+
+    def get_concurrency_run_ids(self) -> Set[str]:
+        return self._storage.event_log_storage.get_concurrency_run_ids()
+
+    def free_concurrency_slots_for_run(self, run_id: str) -> None:
+        return self._storage.event_log_storage.free_concurrency_slots_for_run(run_id)
+
+    def free_concurrency_slot_for_step(self, run_id: str, step_key: str) -> None:
+        return self._storage.event_log_storage.free_concurrency_slot_for_step(run_id, step_key)
+
 
 class LegacyScheduleStorage(ScheduleStorage, ConfigurableClass):
     def __init__(self, storage: DagsterStorage, inst_data: Optional[ConfigurableClassData] = None):
         self._storage = check.inst_param(storage, "storage", DagsterStorage)
         self._inst_data = check.opt_inst_param(inst_data, "inst_data", ConfigurableClassData)
         super().__init__()
```

### Comparing `dagster-1.3.7/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.3.8/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/mem_io_manager.py` & `dagster-1.3.8/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.3.8/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/migration/utils.py` & `dagster-1.3.8/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.3.8/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/output_manager.py` & `dagster-1.3.8/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/partition_status_cache.py` & `dagster-1.3.8/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/root.py` & `dagster-1.3.8/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/root_input_manager.py` & `dagster-1.3.8/dagster/_core/storage/root_input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/runs/base.py` & `dagster-1.3.8/dagster/_core/storage/runs/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/runs/in_memory.py` & `dagster-1.3.8/dagster/_core/storage/runs/in_memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,38 +25,42 @@
             create_in_memory_conn_string(f"runs-{uuid.uuid4()}"),
             poolclass=NullPool,
         )
 
         # hold one connection for life of instance, but vend new ones for specific calls
         self._held_conn = self._engine.connect()
 
-        RunStorageSqlMetadata.create_all(self._held_conn)
-        alembic_config = get_alembic_config(__file__, "sqlite/alembic/alembic.ini")
-        stamp_alembic_rev(alembic_config, self._held_conn)
-        table_names = db.inspect(self._held_conn).get_table_names()
-        if "instance_info" not in table_names:
-            InstanceInfo.create(self._held_conn)
+        with self._held_conn.begin():
+            RunStorageSqlMetadata.create_all(self._held_conn)
+            alembic_config = get_alembic_config(__file__, "sqlite/alembic/alembic.ini")
+            stamp_alembic_rev(alembic_config, self._held_conn)
+
+            table_names = db.inspect(self._held_conn).get_table_names()
+
+            if "instance_info" not in table_names:
+                InstanceInfo.create(self._held_conn)
+
         self.migrate()
         self.optimize()
 
         if preload:
             for payload in preload:
                 self.add_job_snapshot(payload.job_snapshot, payload.dagster_run.job_snapshot_id)
                 self.add_execution_plan_snapshot(
                     payload.execution_plan_snapshot, payload.dagster_run.execution_plan_snapshot_id
                 )
                 self.add_run(payload.dagster_run)
 
     @contextmanager
     def connect(self) -> Iterator[Connection]:
         with self._engine.connect() as conn:
-            conn.execute("PRAGMA journal_mode=WAL;")
-            conn.execute("PRAGMA foreign_keys=ON;")
-
-            yield conn
+            with conn.begin():
+                conn.execute(db.text("PRAGMA journal_mode=WAL;"))
+                conn.execute(db.text("PRAGMA foreign_keys=ON;"))
+                yield conn
 
     def upgrade(self) -> None:
         pass
 
     def dispose(self) -> None:
         self._held_conn.close()
         self._engine.dispose()
```

### Comparing `dagster-1.3.7/dagster/_core/storage/runs/migration.py` & `dagster-1.3.8/dagster/_core/storage/runs/migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sqlalchemy as db
 import sqlalchemy.exc as db_exc
 from sqlalchemy.engine import Connection
 from tqdm import tqdm
 from typing_extensions import Final, TypeAlias
 
 import dagster._check as check
+from dagster._core.storage.sqlalchemy_compat import db_select
 from dagster._serdes import deserialize_value
 
 from ...execution.job_backfill import PartitionBackfill
 from ..dagster_run import DagsterRun, DagsterRunStatus, RunRecord
 from ..runs.base import RunStorage
 from ..runs.schema import BulkActionsTable, RunsTable, RunTagsTable
 from ..tags import PARTITION_NAME_TAG, PARTITION_SET_TAG, REPOSITORY_LABEL_TAG
@@ -161,20 +162,20 @@
     if not isinstance(run_storage, SqlRunStorage):
         return
 
     if print_fn:
         print_fn("Querying run storage.")
 
     subquery = (
-        db.select([RunTagsTable.c.run_id.label("tags_run_id")])
+        db_select([RunTagsTable.c.run_id.label("tags_run_id")])
         .where(RunTagsTable.c.key == REPOSITORY_LABEL_TAG)
         .alias("tag_subquery")
     )
     base_query = (
-        db.select([RunsTable.c.run_body, RunsTable.c.id])
+        db_select([RunsTable.c.run_body, RunsTable.c.id])
         .select_from(
             RunsTable.join(subquery, RunsTable.c.run_id == subquery.c.tags_run_id, isouter=True)
         )
         .where(subquery.c.tags_run_id.is_(None))
         .order_by(db.asc(RunsTable.c.id))
         .limit(CHUNK_SIZE)
     )
@@ -224,15 +225,15 @@
     if not isinstance(run_storage, SqlRunStorage):
         return
 
     if print_fn:
         print_fn("Querying run storage.")
 
     base_query = (
-        db.select([BulkActionsTable.c.body, BulkActionsTable.c.id])
+        db_select([BulkActionsTable.c.body, BulkActionsTable.c.id])
         .where(BulkActionsTable.c.action_type.is_(None))
         .order_by(db.asc(BulkActionsTable.c.id))
         .limit(CHUNK_SIZE)
     )
 
     cursor = None
     has_more = True
```

### Comparing `dagster-1.3.7/dagster/_core/storage/runs/schema.py` & `dagster-1.3.8/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.3.8/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,21 @@
 from dagster._core.host_representation.origin import ExternalJobOrigin
 from dagster._core.snap import (
     ExecutionPlanSnapshot,
     JobSnapshot,
     create_execution_plan_snapshot_id,
     create_job_snapshot_id,
 )
-from dagster._core.storage.sql import SqlAlchemyQuery, SqlAlchemyRow
+from dagster._core.storage.sql import SqlAlchemyQuery
+from dagster._core.storage.sqlalchemy_compat import (
+    db_fetch_mappings,
+    db_scalar_subquery,
+    db_select,
+    db_subquery,
+)
 from dagster._core.storage.tags import (
     PARTITION_NAME_TAG,
     PARTITION_SET_TAG,
     REPOSITORY_LABEL_TAG,
     ROOT_RUN_ID_TAG,
 )
 from dagster._daemon.types import DaemonHeartbeat
@@ -103,27 +109,22 @@
     def upgrade(self) -> None:
         """This method should perform any schema or data migrations necessary to bring an
         out-of-date instance of the storage up to date.
         """
 
     def fetchall(self, query: SqlAlchemyQuery) -> Sequence[Any]:
         with self.connect() as conn:
-            result_proxy = conn.execute(query)
-            res = result_proxy.fetchall()
-            result_proxy.close()
-
-        return res
+            return db_fetch_mappings(conn, query)
 
     def fetchone(self, query: SqlAlchemyQuery) -> Optional[Any]:
         with self.connect() as conn:
-            result_proxy = conn.execute(query)
-            row = result_proxy.fetchone()
-            result_proxy.close()
-
-        return row
+            if db.__version__.startswith("2."):
+                return conn.execute(query).mappings().first()
+            else:
+                return conn.execute(query).fetchone()
 
     def add_run(self, dagster_run: DagsterRun) -> DagsterRun:
         check.inst_param(dagster_run, "dagster_run", DagsterRun)
 
         if dagster_run.job_snapshot_id and not self.has_job_snapshot(dagster_run.job_snapshot_id):
             raise DagsterSnapshotDoesNotExist(
                 "Snapshot {ss_id} does not exist in run storage".format(
@@ -202,37 +203,37 @@
                     run_body=serialize_value(run.with_status(new_job_status)),
                     status=new_job_status.value,
                     update_timestamp=now,
                     **kwargs,
                 )
             )
 
-    def _row_to_run(self, row: SqlAlchemyRow) -> DagsterRun:
+    def _row_to_run(self, row: Dict) -> DagsterRun:
         run = deserialize_value(row["run_body"], DagsterRun)
         status = DagsterRunStatus(row["status"])
         # NOTE: the status column is more trustworthy than the status in the run body, since concurrent
         # writes (e.g.  handle_run_event and add_tags) can cause the status in the body to be out of
         # overriden with an old value.
         return run.with_status(status)
 
-    def _rows_to_runs(self, rows: Iterable[SqlAlchemyRow]) -> Sequence[DagsterRun]:
+    def _rows_to_runs(self, rows: Iterable[Dict]) -> Sequence[DagsterRun]:
         return list(map(self._row_to_run, rows))
 
     def _add_cursor_limit_to_query(
         self,
         query: SqlAlchemyQuery,
         cursor: Optional[str],
         limit: Optional[int],
         order_by: Optional[str],
         ascending: Optional[bool],
     ) -> SqlAlchemyQuery:
         """Helper function to deal with cursor/limit pagination args."""
         if cursor:
-            cursor_query = db.select([RunsTable.c.id]).where(RunsTable.c.run_id == cursor)
-            query = query.where(RunsTable.c.id < cursor_query)
+            cursor_query = db_select([RunsTable.c.id]).where(RunsTable.c.run_id == cursor)
+            query = query.where(RunsTable.c.id < db_scalar_subquery(cursor_query))
 
         if limit:
             query = query.limit(limit)
 
         sorting_column = getattr(RunsTable.c, order_by) if order_by else RunsTable.c.id
         direction = db.asc if ascending else db.desc
         query = query.order_by(direction(sorting_column))
@@ -270,15 +271,15 @@
             query = query.where(RunsTable.c.create_timestamp > filters.created_after)
 
         if filters.created_before:
             query = query.where(RunsTable.c.create_timestamp < filters.created_before)
 
         if filters.tags and self.supports_intersect:
             intersections = [
-                db.select([RunTagsTable.c.run_id]).where(
+                db_select([RunTagsTable.c.run_id]).where(
                     db.and_(
                         RunTagsTable.c.key == key,
                         (
                             RunTagsTable.c.value == value
                             if isinstance(value, str)
                             else RunTagsTable.c.value.in_(value)
                         ),
@@ -316,15 +317,15 @@
             return self._bucketed_runs_query(bucket_by, filters, columns, order_by, ascending)
 
         if filters.tags and not self.supports_intersect:
             table = self._apply_tags_table_joins(RunsTable, filters.tags)
         else:
             table = RunsTable
 
-        base_query = db.select([getattr(RunsTable.c, column) for column in columns]).select_from(
+        base_query = db_select([getattr(RunsTable.c, column) for column in columns]).select_from(
             table
         )
         base_query = self._add_filters_to_query(base_query, filters)
         return self._add_cursor_limit_to_query(base_query, cursor, limit, order_by, ascending)
 
     def _bucket_rank_column(
         self, bucket_by: Union[JobBucket, TagBucket], order_by: Optional[str], ascending: bool
@@ -356,15 +357,15 @@
         query_columns = [getattr(RunsTable.c, column) for column in columns] + [bucket_rank]
 
         if isinstance(bucket_by, JobBucket):
             if filters.tags and not self.supports_intersect:
                 table = self._apply_tags_table_joins(RunsTable, filters.tags)
             else:
                 table = RunsTable
-            base_query = db.select(query_columns).select_from(table)
+            base_query = db_select(query_columns).select_from(table)
             base_query = base_query.where(RunsTable.c.pipeline_name.in_(bucket_by.job_names))
             base_query = self._add_filters_to_query(base_query, filters)
 
         elif not filters.tags:
             # bucketing by tag, no tag filters
             if self.supports_intersect:
                 table = RunsTable.join(
@@ -377,65 +378,72 @@
                 )
             else:
                 table = self._apply_tags_table_joins(
                     RunsTable,
                     {bucket_by.tag_key: bucket_by.tag_values},
                 )
 
-            base_query = db.select(query_columns).select_from(table)
+            base_query = db_select(query_columns).select_from(table)
             base_query = self._add_filters_to_query(base_query, filters)
         else:
             # there are tag filters as well as tag buckets, so we have to apply the tag filters in
             # a separate join
             if self.supports_intersect:
-                filtered_query = db.select([RunsTable.c.run_id])
+                filtered_query = db_select([RunsTable.c.run_id])
             else:
-                filtered_query = db.select([RunsTable.c.run_id]).select_from(
+                filtered_query = db_select([RunsTable.c.run_id]).select_from(
                     self._apply_tags_table_joins(RunsTable, filters.tags)
                 )
 
-            filtered_query = self._add_filters_to_query(filtered_query, filters)
-            filtered_query = filtered_query.alias("filtered_query")
+            filtered_query = db_subquery(
+                self._add_filters_to_query(filtered_query, filters), "filtered_query"
+            )
             if self.supports_intersect:
                 table = RunsTable.join(
                     RunTagsTable,
                     db.and_(
                         RunsTable.c.run_id == RunTagsTable.c.run_id,
                         RunTagsTable.c.key == bucket_by.tag_key,
                         RunTagsTable.c.value.in_(bucket_by.tag_values),
                     ),
                 )
             else:
                 table = self._apply_tags_table_joins(
                     RunsTable, {bucket_by.tag_key: bucket_by.tag_values}
                 )
 
-            base_query = db.select(query_columns).select_from(
+            base_query = db_select(query_columns).select_from(
                 table.join(filtered_query, RunsTable.c.run_id == filtered_query.c.run_id)
             )
 
-        subquery = base_query.alias("subquery")
+        subquery = db_subquery(base_query, "runs_subquery")
 
         # select all the columns, but skip the bucket_rank column, which is only used for applying
         # the limit / order
         subquery_columns = [getattr(subquery.c, column) for column in columns]
-        query = db.select(subquery_columns).order_by(subquery.c.rank.asc())
+        query = db_select(subquery_columns).order_by(subquery.c.rank.asc())
         if bucket_by.bucket_limit:
             query = query.where(subquery.c.rank <= bucket_by.bucket_limit)
 
         return query
 
     def _apply_tags_table_joins(
         self,
         table: db.Table,
         tags: Mapping[str, Union[str, Sequence[str]]],
     ) -> db.Table:
         multi_join = len(tags) > 1
+        i = 0
         for key, value in tags.items():
-            tags_table = RunTagsTable.alias() if multi_join else RunTagsTable
+            i += 1
+            tags_table = (
+                db_subquery(db_select([RunTagsTable]), f"run_tags_subquery_{i}")
+                if multi_join
+                else RunTagsTable
+            )
             table = table.join(
                 tags_table,
                 db.and_(
                     RunsTable.c.run_id == tags_table.c.run_id,
                     tags_table.c.key == key,
                     (
                         tags_table.c.value == value
@@ -454,29 +462,24 @@
         bucket_by: Optional[Union[JobBucket, TagBucket]] = None,
     ) -> Sequence[DagsterRun]:
         query = self._runs_query(filters, cursor, limit, bucket_by=bucket_by)
         rows = self.fetchall(query)
         return self._rows_to_runs(rows)
 
     def get_runs_count(self, filters: Optional[RunsFilter] = None) -> int:
-        subquery = self._runs_query(filters=filters).alias("subquery")
-
-        # We use an alias here because Postgres requires subqueries to be
-        # aliased.
-        subquery = subquery.alias("subquery")
-
-        query = db.select([db.func.count()]).select_from(subquery)
-        rows = self.fetchall(query)
-        count = rows[0][0]
+        subquery = db_subquery(self._runs_query(filters=filters))
+        query = db_select([db.func.count().label("count")]).select_from(subquery)
+        row = self.fetchone(query)
+        count = row["count"] if row else 0
         return count
 
     def _get_run_by_id(self, run_id: str) -> Optional[DagsterRun]:
         check.str_param(run_id, "run_id")
 
-        query = db.select([RunsTable.c.run_body, RunsTable.c.status]).where(
+        query = db_select([RunsTable.c.run_body, RunsTable.c.status]).where(
             RunsTable.c.run_id == run_id
         )
         rows = self.fetchall(query)
         return self._row_to_run(rows[0]) if rows else None
 
     def get_run_records(
         self,
@@ -524,37 +527,33 @@
         self,
         tag_keys: Optional[Sequence[str]] = None,
         value_prefix: Optional[str] = None,
         limit: Optional[int] = None,
     ) -> Sequence[Tuple[str, Set[str]]]:
         result = defaultdict(set)
         query = (
-            db.select([RunTagsTable.c.key, RunTagsTable.c.value])
-            .distinct(RunTagsTable.c.key, RunTagsTable.c.value)
+            db_select([RunTagsTable.c.key, RunTagsTable.c.value])
+            .distinct()
             .order_by(RunTagsTable.c.key, RunTagsTable.c.value)
         )
         if tag_keys:
             query = query.where(RunTagsTable.c.key.in_(tag_keys))
         if value_prefix:
             query = query.where(RunTagsTable.c.value.startswith(value_prefix))
         if limit:
             query = query.limit(limit)
         rows = self.fetchall(query)
         for r in rows:
-            result[r[0]].add(r[1])
+            result[r["key"]].add(r["value"])
         return sorted(list([(k, v) for k, v in result.items()]), key=lambda x: x[0])
 
     def get_run_tag_keys(self) -> Sequence[str]:
-        query = (
-            db.select([RunTagsTable.c.key])
-            .distinct(RunTagsTable.c.key)
-            .order_by(RunTagsTable.c.key)
-        )
+        query = db_select([RunTagsTable.c.key]).distinct().order_by(RunTagsTable.c.key)
         rows = self.fetchall(query)
-        return sorted([r[0] for r in rows])
+        return sorted([r["key"] for r in rows])
 
     def add_run_tags(self, run_id: str, new_tags: Mapping[str, str]) -> None:
         check.str_param(run_id, "run_id")
         check.mapping_param(new_tags, "new_tags", key_type=str, value_type=str)
 
         run = self._get_run_by_id(run_id)
         if not run:
@@ -617,67 +616,66 @@
                 ),
                 invalid_run_id=root_run_id,
             )
 
         # root_run_id to run_id 1:1 mapping
         # https://github.com/dagster-io/dagster/issues/2495
         # Note: we currently use tags to persist the run group info
-        root_to_run = (
-            db.select(
+        root_to_run = db_subquery(
+            db_select(
                 [RunTagsTable.c.value.label("root_run_id"), RunTagsTable.c.run_id.label("run_id")]
-            )
-            .where(
+            ).where(
                 db.and_(RunTagsTable.c.key == ROOT_RUN_ID_TAG, RunTagsTable.c.value == root_run_id)
-            )
-            .alias("root_to_run")
+            ),
+            "root_to_run",
         )
         # get run group
-        run_group_query = (
-            db.select([RunsTable.c.run_body, RunsTable.c.status])
-            .select_from(
-                root_to_run.join(
-                    RunsTable,
-                    root_to_run.c.run_id == RunsTable.c.run_id,
-                    isouter=True,
-                )
+        run_group_query = db_select([RunsTable.c.run_body, RunsTable.c.status]).select_from(
+            root_to_run.join(
+                RunsTable,
+                root_to_run.c.run_id == RunsTable.c.run_id,
+                isouter=True,
             )
-            .alias("run_group")
         )
 
-        with self.connect() as conn:
-            res = conn.execute(run_group_query)
-            run_group = self._rows_to_runs(res)
+        res = self.fetchall(run_group_query)
+        run_group = self._rows_to_runs(res)
 
         return (root_run_id, [root_run, *run_group])
 
     def get_run_groups(
         self,
         filters: Optional[RunsFilter] = None,
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
     ) -> Mapping[str, RunGroupInfo]:
         # The runs that would be returned by calling RunStorage.get_runs with the same arguments
-        runs = self._runs_query(
-            filters=filters, cursor=cursor, limit=limit, columns=["run_body", "status", "run_id"]
-        ).alias("runs")
+        runs = db_subquery(
+            self._runs_query(
+                filters=filters,
+                cursor=cursor,
+                limit=limit,
+                columns=["run_body", "status", "run_id"],
+            ),
+            "runs",
+        )
 
         # Gets us the run_id and associated root_run_id for every run in storage that is a
         # descendant run of some root
         #
         # pseudosql:
         #   with all_descendant_runs as (
         #     select *
         #     from run_tags
         #     where key = @ROOT_RUN_ID_TAG
         #   )
 
-        all_descendant_runs = (
-            db.select([RunTagsTable])
-            .where(RunTagsTable.c.key == ROOT_RUN_ID_TAG)
-            .alias("all_descendant_runs")
+        all_descendant_runs = db_subquery(
+            db_select([RunTagsTable]).where(RunTagsTable.c.key == ROOT_RUN_ID_TAG),
+            "all_descendant_runs",
         )
 
         # Augment the runs in our query, for those runs that are the descendant of some root run,
         # with the root_run_id
         #
         # pseudosql:
         #
@@ -686,54 +684,54 @@
         #       runs.run_id as run_id,
         #       all_descendant_runs.value as root_run_id
         #     from runs
         #     left outer join all_descendant_runs
         #       on all_descendant_runs.run_id = runs.run_id
         #   )
 
-        runs_augmented = (
-            db.select(
+        runs_augmented = db_subquery(
+            db_select(
                 [
                     runs.c.run_id.label("run_id"),
                     all_descendant_runs.c.value.label("root_run_id"),
                 ]
-            )
-            .select_from(
+            ).select_from(
                 runs.join(
                     all_descendant_runs,
                     all_descendant_runs.c.run_id == RunsTable.c.run_id,
                     isouter=True,
                 )
-            )
-            .alias("runs_augmented")
+            ),
+            "runs_augmented",
         )
 
         # Get all the runs our query will return. This includes runs as well as their root runs.
         #
         # pseudosql:
         #
         #    with runs_and_root_runs as (
         #      select runs.run_id as run_id
         #      from runs, runs_augmented
         #      where
         #        runs.run_id = runs_augmented.run_id or
         #        runs.run_id = runs_augmented.root_run_id
         #    )
 
-        runs_and_root_runs = (
-            db.select([RunsTable.c.run_id.label("run_id")])
+        runs_and_root_runs = db_subquery(
+            db_select([RunsTable.c.run_id.label("run_id")])
+            .distinct()
             .select_from(runs_augmented)
             .where(
                 db.or_(
                     RunsTable.c.run_id == runs_augmented.c.run_id,
                     RunsTable.c.run_id == runs_augmented.c.root_run_id,
                 )
-            )
-            .distinct(RunsTable.c.run_id)
-        ).alias("runs_and_root_runs")
+            ),
+            "runs_and_root_runs",
+        )
 
         # We count the descendants of all of the runs in our query that are roots so that
         # we can accurately display when a root run has more descendants than are returned by this
         # query and afford a drill-down. This might be an unnecessary complication, but the
         # alternative isn't obvious -- we could go and fetch *all* the runs in any group that we're
         # going to return in this query, and then append those.
         #
@@ -744,15 +742,15 @@
         #    join runs_and_root_runs on runs.run_id = runs_and_root_runs.run_id
         #    left outer join all_descendant_runs
         #      on all_descendant_runs.value = runs_and_root_runs.run_id
         #    group by runs.run_body
         #    order by child_counts desc
 
         runs_and_root_runs_with_descendant_counts = (
-            db.select(
+            db_select(
                 [
                     RunsTable.c.run_body,
                     RunsTable.c.status,
                     db.func.count(all_descendant_runs.c.id).label("child_counts"),
                 ]
             )
             .select_from(
@@ -764,16 +762,15 @@
                     isouter=True,
                 )
             )
             .group_by(RunsTable.c.run_body, RunsTable.c.status)
             .order_by(db.desc(db.column("child_counts")))
         )
 
-        with self.connect() as conn:
-            res = conn.execute(runs_and_root_runs_with_descendant_counts).fetchall()
+        res = self.fetchall(runs_and_root_runs_with_descendant_counts)
 
         # Postprocess: descendant runs get aggregated with their roots
         root_run_id_to_group: Dict[str, List[DagsterRun]] = defaultdict(list)
         root_run_id_to_count: Dict[str, int] = defaultdict(int)
         for row in res:
             dagster_run = self._row_to_run(row)
             root_run_id = dagster_run.get_root_run_id()
@@ -852,45 +849,50 @@
 
         with self.connect() as conn:
             snapshot_insert = SnapshotsTable.insert().values(
                 snapshot_id=snapshot_id,
                 snapshot_body=zlib.compress(serialize_value(snapshot_obj).encode("utf-8")),
                 snapshot_type=snapshot_type.value,
             )
-            conn.execute(snapshot_insert)
+            try:
+                conn.execute(snapshot_insert)
+            except db_exc.IntegrityError:
+                # on_conflict_do_nothing equivalent
+                pass
+
             return snapshot_id
 
     def get_run_storage_id(self) -> str:
-        query = db.select([InstanceInfo.c.run_storage_id])
+        query = db_select([InstanceInfo.c.run_storage_id])
         row = self.fetchone(query)
         if not row:
             run_storage_id = str(uuid.uuid4())
             with self.connect() as conn:
                 conn.execute(InstanceInfo.insert().values(run_storage_id=run_storage_id))
             return run_storage_id
         else:
-            return row[0]
+            return row["run_storage_id"]
 
     def _has_snapshot_id(self, snapshot_id: str) -> bool:
-        query = db.select([SnapshotsTable.c.snapshot_id]).where(
+        query = db_select([SnapshotsTable.c.snapshot_id]).where(
             SnapshotsTable.c.snapshot_id == snapshot_id
         )
 
         row = self.fetchone(query)
 
         return bool(row)
 
     def _get_snapshot(self, snapshot_id: str) -> Optional[JobSnapshot]:
-        query = db.select([SnapshotsTable.c.snapshot_body]).where(
+        query = db_select([SnapshotsTable.c.snapshot_body]).where(
             SnapshotsTable.c.snapshot_id == snapshot_id
         )
 
         row = self.fetchone(query)
 
-        return defensively_unpack_execution_plan_snapshot_query(logging, row) if row else None  # type: ignore
+        return defensively_unpack_execution_plan_snapshot_query(logging, [row["snapshot_body"]]) if row else None  # type: ignore
 
     def get_run_partition_data(self, runs_filter: RunsFilter) -> Sequence[RunPartitionData]:
         if self.has_built_index(RUN_PARTITIONS) and self.has_run_stats_index_cols():
             query = self._runs_query(
                 filters=runs_filter,
                 columns=["run_id", "status", "start_time", "end_time", "partition"],
             )
@@ -979,21 +981,20 @@
         self._execute_data_migrations(REQUIRED_DATA_MIGRATIONS, print_fn, force_rebuild_all)
 
     def optimize(self, print_fn: Optional[PrintFn] = None, force_rebuild_all: bool = False) -> None:
         self._execute_data_migrations(OPTIONAL_DATA_MIGRATIONS, print_fn, force_rebuild_all)
 
     def has_built_index(self, migration_name: str) -> bool:
         query = (
-            db.select([1])
+            db_select([1])
             .where(SecondaryIndexMigrationTable.c.name == migration_name)
             .where(SecondaryIndexMigrationTable.c.migration_completed != None)  # noqa: E711
             .limit(1)
         )
-        with self.connect() as conn:
-            results = conn.execute(query).fetchall()
+        results = self.fetchall(query)
 
         return len(results) > 0
 
     def mark_index_built(self, migration_name: str) -> None:
         query = SecondaryIndexMigrationTable.insert().values(
             name=migration_name,
             migration_completed=datetime.now(),
@@ -1044,20 +1045,19 @@
                         timestamp=utc_datetime_from_timestamp(daemon_heartbeat.timestamp),
                         daemon_id=daemon_heartbeat.daemon_id,
                         body=serialize_value(daemon_heartbeat),
                     )
                 )
 
     def get_daemon_heartbeats(self) -> Mapping[str, DaemonHeartbeat]:
-        with self.connect() as conn:
-            rows = conn.execute(db.select([DaemonHeartbeatsTable.c.body]))
-            heartbeats = []
-            for row in rows:
-                heartbeats.append(deserialize_value(row.body, DaemonHeartbeat))
-            return {heartbeat.daemon_type: heartbeat for heartbeat in heartbeats}
+        rows = self.fetchall(db_select([DaemonHeartbeatsTable.c.body]))
+        heartbeats = []
+        for row in rows:
+            heartbeats.append(deserialize_value(row["body"], DaemonHeartbeat))
+        return {heartbeat.daemon_type: heartbeat for heartbeat in heartbeats}
 
     def wipe(self) -> None:
         """Clears the run storage."""
         with self.connect() as conn:
             # https://stackoverflow.com/a/54386260/324449
             conn.execute(RunsTable.delete())
             conn.execute(RunTagsTable.delete())
@@ -1073,33 +1073,33 @@
     def get_backfills(
         self,
         status: Optional[BulkActionStatus] = None,
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
     ) -> Sequence[PartitionBackfill]:
         check.opt_inst_param(status, "status", BulkActionStatus)
-        query = db.select([BulkActionsTable.c.body])
+        query = db_select([BulkActionsTable.c.body])
         if status:
             query = query.where(BulkActionsTable.c.status == status.value)
         if cursor:
-            cursor_query = db.select([BulkActionsTable.c.id]).where(
+            cursor_query = db_select([BulkActionsTable.c.id]).where(
                 BulkActionsTable.c.key == cursor
             )
             query = query.where(BulkActionsTable.c.id < cursor_query)
         if limit:
             query = query.limit(limit)
         query = query.order_by(BulkActionsTable.c.id.desc())
         rows = self.fetchall(query)
-        return [deserialize_value(row[0], PartitionBackfill) for row in rows]
+        return [deserialize_value(row["body"], PartitionBackfill) for row in rows]
 
     def get_backfill(self, backfill_id: str) -> Optional[PartitionBackfill]:
         check.str_param(backfill_id, "backfill_id")
-        query = db.select([BulkActionsTable.c.body]).where(BulkActionsTable.c.key == backfill_id)
+        query = db_select([BulkActionsTable.c.body]).where(BulkActionsTable.c.key == backfill_id)
         row = self.fetchone(query)
-        return deserialize_value(row[0], PartitionBackfill) if row else None
+        return deserialize_value(row["body"], PartitionBackfill) if row else None
 
     def add_backfill(self, partition_backfill: PartitionBackfill) -> None:
         check.inst_param(partition_backfill, "partition_backfill", PartitionBackfill)
         values: Dict[str, Any] = dict(
             key=partition_backfill.backfill_id,
             status=partition_backfill.status.value,
             timestamp=utc_datetime_from_timestamp(partition_backfill.backfill_timestamp),
@@ -1129,21 +1129,20 @@
                     body=serialize_value(partition_backfill),
                 )
             )
 
     def get_cursor_values(self, keys: Set[str]) -> Mapping[str, str]:
         check.set_param(keys, "keys", of_type=str)
 
-        with self.connect() as conn:
-            rows = conn.execute(
-                db.select([KeyValueStoreTable.c.key, KeyValueStoreTable.c.value]).where(
-                    KeyValueStoreTable.c.key.in_(keys)
-                ),
-            )
-            return {row.key: row.value for row in rows}
+        rows = self.fetchall(
+            db_select([KeyValueStoreTable.c.key, KeyValueStoreTable.c.value]).where(
+                KeyValueStoreTable.c.key.in_(keys)
+            ),
+        )
+        return {row["key"]: row["value"] for row in rows}
 
     def set_cursor_values(self, pairs: Mapping[str, str]) -> None:
         check.mapping_param(pairs, "pairs", key_type=str, value_type=str)
         db_values = [{"key": k, "value": v} for k, v in pairs.items()]
 
         with self.connect() as conn:
             try:
@@ -1174,19 +1173,18 @@
             )
 
 
 GET_PIPELINE_SNAPSHOT_QUERY_ID = "get-pipeline-snapshot"
 
 
 def defensively_unpack_execution_plan_snapshot_query(
-    logger: logging.Logger, row: SqlAlchemyRow
+    logger: logging.Logger, row: Sequence[Any]
 ) -> Optional[Union[ExecutionPlanSnapshot, JobSnapshot]]:
-    # no checking here because sqlalchemy returns a special
-    # row proxy and don't want to instance check on an internal
-    # implementation detail
+    # minimal checking here because sqlalchemy returns a different type based on what version of
+    # SqlAlchemy you are using
 
     def _warn(msg: str) -> None:
         logger.warning(f"get-pipeline-snapshot: {msg}")
 
     if not isinstance(row[0], bytes):
         _warn("First entry in row is not a binary type.")
         return None
```

### Comparing `dagster-1.3.7/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.3.8/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.3.8/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         alembic_config = get_alembic_config(__file__)
 
         should_mark_indexes = False
         with engine.connect() as connection:
             db_revision, head_revision = check_alembic_revision(alembic_config, connection)
             if not (db_revision and head_revision):
                 RunStorageSqlMetadata.create_all(engine)
-                connection.execute("PRAGMA journal_mode=WAL;")
+                connection.execute(db.text("PRAGMA journal_mode=WAL;"))
                 stamp_alembic_rev(alembic_config, connection)
                 should_mark_indexes = True
 
             table_names = db.inspect(engine).get_table_names()
             if "instance_info" not in table_names:
                 InstanceInfo.create(engine)
 
@@ -105,19 +105,17 @@
             run_storage.optimize()
 
         return run_storage
 
     @contextmanager
     def connect(self) -> Iterator[Connection]:
         engine = create_engine(self._conn_string, poolclass=NullPool)
-        conn = engine.connect()
-        try:
-            yield conn
-        finally:
-            conn.close()
+        with engine.connect() as conn:
+            with conn.begin():
+                yield conn
 
     def _alembic_upgrade(self, rev: str = "head") -> None:
         alembic_config = get_alembic_config(__file__)
         with self.connect() as conn:
             run_alembic_upgrade(alembic_config, conn, rev=rev)
 
     def _alembic_downgrade(self, rev: str = "head") -> None:
```

### Comparing `dagster-1.3.7/dagster/_core/storage/schedules/base.py` & `dagster-1.3.8/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/schedules/migration.py` & `dagster-1.3.8/dagster/_core/storage/schedules/migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Callable, Mapping, Optional
 
-import sqlalchemy as db
 import sqlalchemy.exc as db_exc
 from tqdm import tqdm
 
 from dagster._core.scheduler.instigation import InstigatorState
 from dagster._core.storage.schedules.base import ScheduleStorage
+from dagster._core.storage.sqlalchemy_compat import db_select
 from dagster._serdes import deserialize_value
 from dagster._utils import PrintFn
 
 from ..schedules.schema import InstigatorsTable, JobTable, JobTickTable
 
 SCHEDULE_JOBS_SELECTOR_ID = "schedule_jobs_selector_id"
 SCHEDULE_TICKS_SELECTOR_ID = "schedule_ticks_selector_id"
@@ -29,15 +29,15 @@
     it to the jobs table.
     """
     if print_fn:
         print_fn("Querying storage.")
 
     with storage.connect() as conn:  # type: ignore
         rows = conn.execute(
-            db.select(
+            db_select(
                 [
                     JobTable.c.id,
                     JobTable.c.job_body,
                     JobTable.c.create_timestamp,
                     JobTable.c.update_timestamp,
                 ]
             ).order_by(JobTable.c.id.asc())
```

### Comparing `dagster-1.3.7/dagster/_core/storage/schedules/schema.py` & `dagster-1.3.8/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.3.8/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     InstigatorState,
     InstigatorStatus,
     InstigatorTick,
     TickData,
     TickStatus,
 )
 from dagster._core.storage.sql import SqlAlchemyQuery, SqlAlchemyRow
+from dagster._core.storage.sqlalchemy_compat import db_fetch_mappings, db_select, db_subquery
 from dagster._serdes import serialize_value
 from dagster._serdes.serdes import deserialize_value
 from dagster._utils import PrintFn, utc_datetime_from_timestamp
 
 from .base import ScheduleStorage
 from .migration import (
     OPTIONAL_SCHEDULE_DATA_MIGRATIONS,
@@ -81,28 +82,28 @@
         repository_selector_id: Optional[str] = None,
         instigator_type: Optional[InstigatorType] = None,
         instigator_statuses: Optional[Set[InstigatorStatus]] = None,
     ) -> Sequence[InstigatorState]:
         check.opt_inst_param(instigator_type, "instigator_type", InstigatorType)
 
         if self.has_instigators_table() and self.has_built_index(SCHEDULE_JOBS_SELECTOR_ID):
-            query = db.select([InstigatorsTable.c.instigator_body]).select_from(InstigatorsTable)
+            query = db_select([InstigatorsTable.c.instigator_body]).select_from(InstigatorsTable)
             if repository_selector_id:
                 query = query.where(
                     InstigatorsTable.c.repository_selector_id == repository_selector_id
                 )
             if instigator_type:
                 query = query.where(InstigatorsTable.c.instigator_type == instigator_type.value)
             if instigator_statuses:
                 query = query.where(
                     InstigatorsTable.c.status.in_([status.value for status in instigator_statuses])
                 )
 
         else:
-            query = db.select([JobTable.c.job_body]).select_from(JobTable)
+            query = db_select([JobTable.c.job_body]).select_from(JobTable)
             if repository_origin_id:
                 query = query.where(JobTable.c.repository_origin_id == repository_origin_id)
             if instigator_type:
                 query = query.where(JobTable.c.job_type == instigator_type.value)
             if instigator_statuses:
                 query = query.where(
                     JobTable.c.status.in_([status.value for status in instigator_statuses])
@@ -113,33 +114,33 @@
 
     def get_instigator_state(self, origin_id: str, selector_id: str) -> Optional[InstigatorState]:
         check.str_param(origin_id, "origin_id")
         check.str_param(selector_id, "selector_id")
 
         if self.has_instigators_table() and self.has_built_index(SCHEDULE_JOBS_SELECTOR_ID):
             query = (
-                db.select([InstigatorsTable.c.instigator_body])
+                db_select([InstigatorsTable.c.instigator_body])
                 .select_from(InstigatorsTable)
                 .where(InstigatorsTable.c.selector_id == selector_id)
             )
         else:
             query = (
-                db.select([JobTable.c.job_body])
+                db_select([JobTable.c.job_body])
                 .select_from(JobTable)
                 .where(JobTable.c.job_origin_id == origin_id)
             )
 
         rows = self.execute(query)
         return self._deserialize_rows(rows[:1], InstigatorState)[0] if len(rows) else None
 
     def _has_instigator_state_by_selector(self, selector_id: str) -> bool:
         check.str_param(selector_id, "selector_id")
 
         query = (
-            db.select([JobTable.c.job_body])
+            db_select([JobTable.c.job_body])
             .select_from(JobTable)
             .where(JobTable.c.selector_id == selector_id)
         )
 
         rows = self.execute(query)
         return self._deserialize_rows(rows[:1])[0] if len(rows) else None  # type: ignore
 
@@ -237,15 +238,15 @@
                         InstigatorsTable.delete().where(
                             InstigatorsTable.c.selector_id == selector_id
                         )
                     )
 
     def _jobs_has_selector_state(self, conn: Connection, selector_id: str) -> bool:
         query = (
-            db.select([db.func.count()])
+            db_select([db.func.count()])
             .select_from(JobTable)
             .where(JobTable.c.selector_id == selector_id)
         )
         result = conn.execute(query)
         row = result.fetchone()
         result.close()
         return row[0] > 0  # type: ignore  # (possible none)
@@ -303,34 +304,33 @@
             db.func.rank()
             .over(
                 order_by=db.desc(JobTickTable.c.timestamp),
                 partition_by=JobTickTable.c.selector_id,
             )
             .label("rank")
         )
-        subquery = (
-            db.select(
+        subquery = db_subquery(
+            db_select(
                 [
                     JobTickTable.c.id,
                     JobTickTable.c.selector_id,
                     JobTickTable.c.tick_body,
                     bucket_rank_column,
                 ]
             )
             .select_from(JobTickTable)
             .where(JobTickTable.c.selector_id.in_(selector_ids))
-            .alias("subquery")
         )
         if statuses:
             subquery = subquery.where(
                 JobTickTable.c.status.in_([status.value for status in statuses])
             )
 
         query = (
-            db.select([subquery.c.id, subquery.c.selector_id, subquery.c.tick_body])
+            db_select([subquery.c.id, subquery.c.selector_id, subquery.c.tick_body])
             .order_by(subquery.c.rank.asc())
             .where(subquery.c.rank <= limit)
         )
 
         rows = self.execute(query)
         results = defaultdict(list)
         for row in rows:
@@ -352,15 +352,15 @@
         check.str_param(origin_id, "origin_id")
         check.opt_float_param(before, "before")
         check.opt_float_param(after, "after")
         check.opt_int_param(limit, "limit")
         check.opt_list_param(statuses, "statuses", of_type=TickStatus)
 
         base_query = (
-            db.select([JobTickTable.c.id, JobTickTable.c.tick_body])
+            db_select([JobTickTable.c.id, JobTickTable.c.tick_body])
             .select_from(JobTickTable)
             .order_by(JobTickTable.c.timestamp.desc())
         )
         if self.has_instigators_table():
             query = base_query.where(
                 db.or_(
                     JobTickTable.c.selector_id == selector_id,
@@ -489,30 +489,30 @@
             conn.execute(bulk_insert)
 
     def get_auto_materialize_asset_evaluations(
         self, asset_key: AssetKey, limit: int, cursor: Optional[int] = None
     ) -> Sequence[AutoMaterializeAssetEvaluationRecord]:
         with self.connect() as conn:
             query = (
-                db.select(
+                db_select(
                     [
                         AssetDaemonAssetEvaluationsTable.c.id,
                         AssetDaemonAssetEvaluationsTable.c.asset_evaluation_body,
                         AssetDaemonAssetEvaluationsTable.c.evaluation_id,
                         AssetDaemonAssetEvaluationsTable.c.create_timestamp,
                     ]
                 )
                 .where(AssetDaemonAssetEvaluationsTable.c.asset_key == asset_key.to_string())
                 .order_by(AssetDaemonAssetEvaluationsTable.c.evaluation_id.desc())
             ).limit(limit)
 
             if cursor:
                 query = query.where(AssetDaemonAssetEvaluationsTable.c.evaluation_id < cursor)
 
-            rows = conn.execute(query)
+            rows = db_fetch_mappings(conn, query)
             return [AutoMaterializeAssetEvaluationRecord.from_db_row(row) for row in rows]
 
     def wipe(self) -> None:
         """Clears the schedule storage."""
         with self.connect() as conn:
             # https://stackoverflow.com/a/54386260/324449
             conn.execute(JobTable.delete())
@@ -529,15 +529,15 @@
             return "secondary_indexes" in db.inspect(conn).get_table_names()
 
     def has_built_index(self, migration_name: str) -> bool:
         if not self.has_secondary_index_table():
             return False
 
         query = (
-            db.select([1])
+            db_select([1])
             .where(SecondaryIndexMigrationTable.c.name == migration_name)
             .where(SecondaryIndexMigrationTable.c.migration_completed != None)  # noqa: E711
             .limit(1)
         )
         with self.connect() as conn:
             results = conn.execute(query).fetchall()
```

### Comparing `dagster-1.3.7/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.3.8/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.3.8/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from contextlib import contextmanager
 from typing import Iterator, Optional
 
+import sqlalchemy as db
 from packaging.version import parse
 from sqlalchemy.engine import Connection
 from sqlalchemy.pool import NullPool
 
 from dagster import (
     StringSource,
     _check as check,
@@ -63,33 +64,31 @@
         alembic_config = get_alembic_config(__file__)
 
         should_migrate_data = False
         with engine.connect() as connection:
             db_revision, head_revision = check_alembic_revision(alembic_config, connection)
             if not (db_revision and head_revision):
                 ScheduleStorageSqlMetadata.create_all(engine)
-                connection.execute("PRAGMA journal_mode=WAL;")
+                connection.execute(db.text("PRAGMA journal_mode=WAL;"))
                 stamp_alembic_rev(alembic_config, connection)
                 should_migrate_data = True
 
         schedule_storage = cls(conn_string, inst_data)
         if should_migrate_data:
             schedule_storage.migrate()
             schedule_storage.optimize()
 
         return schedule_storage
 
     @contextmanager
     def connect(self) -> Iterator[Connection]:
         engine = create_engine(self._conn_string, poolclass=NullPool)
-        conn = engine.connect()
-        try:
-            yield conn
-        finally:
-            conn.close()
+        with engine.connect() as conn:
+            with conn.begin():
+                yield conn
 
     @property
     def supports_batch_queries(self) -> bool:
         if not super().supports_batch_queries:
             return False
 
         return super().supports_batch_queries and parse(get_sqlite_version()) >= parse(
```

### Comparing `dagster-1.3.7/dagster/_core/storage/sql.py` & `dagster-1.3.8/dagster/_core/storage/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from alembic.runtime.migration import MigrationContext
 from alembic.script import ScriptDirectory
 from sqlalchemy.engine import Connection
 from sqlalchemy.ext.compiler import compiles
 from typing_extensions import TypeAlias
 
 from dagster._utils import file_relative_path
-from dagster._utils.log import quieten
 
 create_engine = db.create_engine  # exported
 
 
 ALEMBIC_SCRIPTS_LOCATION = "dagster:_core/storage/alembic"
 
 # Stand-in for a typed query object, which is only available in sqlalchemy 2+
@@ -59,18 +58,16 @@
     downgrade(alembic_config, rev)
 
 
 # Ensure that at most one thread can be stamping alembic revisions at once
 _alembic_lock = threading.Lock()
 
 
-def stamp_alembic_rev(
-    alembic_config: Config, conn: Connection, rev: str = "head", quiet: bool = True
-) -> None:
-    with _alembic_lock, quieten(quiet):
+def stamp_alembic_rev(alembic_config: Config, conn: Connection, rev: str = "head") -> None:
+    with _alembic_lock:
         alembic_config.attributes["connection"] = conn
         stamp(alembic_config, rev)
 
 
 def check_alembic_revision(alembic_config: Config, conn: Connection) -> AlembicVersion:
     with _alembic_lock:
         migration_context = MigrationContext.configure(conn)
@@ -129,34 +126,33 @@
 
     In this scenario we need to create an Engine
     and associate a connection with the context.
 
     """
     from sqlite3 import DatabaseError
 
-    connectable = config.attributes.get("connection", None)
+    connection = config.attributes.get("connection", None)
 
-    if connectable is None:
+    if connection is None:
         raise Exception(
             "No connection set in alembic config. If you are trying to run this script from the "
             "command line, STOP and read the README."
         )
 
-    with connectable.connect() as connection:
-        try:
-            context.configure(connection=connection, target_metadata=target_metadata)
-
-            with context.begin_transaction():
-                context.run_migrations()
-
-        except DatabaseError as exc:
-            # This is to deal with concurrent execution -- if this table already exists thanks to a
-            # race with another process, we are fine and can continue.
-            if "table alembic_version already exists" not in str(exc):
-                raise
+    try:
+        context.configure(connection=connection, target_metadata=target_metadata)
+
+        with context.begin_transaction():
+            context.run_migrations()
+
+    except DatabaseError as exc:
+        # This is to deal with concurrent execution -- if this table already exists thanks to a
+        # race with another process, we are fine and can continue.
+        if "table alembic_version already exists" not in str(exc):
+            raise
 
 
 # SQLAlchemy types, compiler directives, etc. to avoid pre-0.11.0 migrations
 # as well as compiler directives to make cross-DB API semantics the same.
 
 # 1: make MySQL dates equivalent to PG or Sqlite dates
```

### Comparing `dagster-1.3.7/dagster/_core/storage/sqlite.py` & `dagster-1.3.8/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/sqlite_storage.py` & `dagster-1.3.8/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/tags.py` & `dagster-1.3.8/dagster/_core/storage/tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 USER_EDITABLE_SYSTEM_TAGS = [
     PRIORITY_TAG,
     MAX_RETRIES_TAG,
     RETRY_STRATEGY_TAG,
     MAX_RUNTIME_SECONDS_TAG,
 ]
 
+RUN_WORKER_ID_TAG = f"{HIDDEN_TAG_PREFIX}run_worker"
+GLOBAL_CONCURRENCY_TAG = f"{SYSTEM_TAG_PREFIX}concurrency_key"
+
 # In cloud, we tag runs with the email of the user who triggered the run
 # This is used to display the user in the UI
 USER_TAG = "user"
 
 
 class TagType(Enum):
     # Custom tag provided by a user
```

### Comparing `dagster-1.3.7/dagster/_core/storage/temp_file_manager.py` & `dagster-1.3.8/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/storage/upath_io_manager.py` & `dagster-1.3.8/dagster/_core/storage/upath_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/system_config/composite_descent.py` & `dagster-1.3.8/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/system_config/objects.py` & `dagster-1.3.8/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/telemetry.py` & `dagster-1.3.8/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/telemetry_upload.py` & `dagster-1.3.8/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/test_utils.py` & `dagster-1.3.8/dagster/_core/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from dagster._core.secrets import SecretsLoader
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus, RunsFilter
 from dagster._core.types.loadable_target_origin import LoadableTargetOrigin
 from dagster._core.workspace.context import WorkspaceProcessContext, WorkspaceRequestContext
 from dagster._core.workspace.load_target import WorkspaceLoadTarget
 from dagster._serdes import ConfigurableClass
 from dagster._serdes.config_class import ConfigurableClassData
-from dagster._seven.compat.pendulum import create_pendulum_time, mock_pendulum_timezone
+from dagster._seven.compat.pendulum import create_pendulum_time
 from dagster._utils import Counter, get_terminate_signal, traced, traced_counter
 from dagster._utils.log import configure_loggers
 
 # test utils from separate light weight file since are exported top level
 from .instance_for_test import (
     cleanup_test_instance as cleanup_test_instance,
     environ as environ,
@@ -463,28 +463,14 @@
 def get_crash_signals() -> Sequence[Signals]:
     return [get_terminate_signal()]
 
 
 _mocked_system_timezone: Dict[str, Optional[str]] = {"timezone": None}
 
 
-@contextmanager
-def mock_system_timezone(override_timezone: str) -> Iterator[None]:
-    with mock_pendulum_timezone(override_timezone):
-        try:
-            _mocked_system_timezone["timezone"] = override_timezone
-            yield
-        finally:
-            _mocked_system_timezone["timezone"] = None
-
-
-def get_mocked_system_timezone() -> Optional[str]:
-    return _mocked_system_timezone["timezone"]
-
-
 # Test utility for creating a test workspace for a function
 class InProcessTestWorkspaceLoadTarget(WorkspaceLoadTarget):
     def __init__(
         self, origin: Union[InProcessCodeLocationOrigin, Sequence[InProcessCodeLocationOrigin]]
     ):
         self._origins = cast(
             Sequence[InProcessCodeLocationOrigin],
```

### Comparing `dagster-1.3.7/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.3.8/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/types/config_schema.py` & `dagster-1.3.8/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/types/dagster_type.py` & `dagster-1.3.8/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/types/decorator.py` & `dagster-1.3.8/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/types/loadable_target_origin.py` & `dagster-1.3.8/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/types/primitive_mapping.py` & `dagster-1.3.8/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/types/python_dict.py` & `dagster-1.3.8/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/types/python_set.py` & `dagster-1.3.8/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/types/python_tuple.py` & `dagster-1.3.8/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/types/transform_typing.py` & `dagster-1.3.8/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/utility_ops.py` & `dagster-1.3.8/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/utils.py` & `dagster-1.3.8/dagster/_core/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 import os
 import random
 import string
 import uuid
 import warnings
 from collections import OrderedDict
-from typing import AbstractSet, Any, Iterable, Mapping, Sequence, Tuple, TypeVar, Union, cast
+from concurrent.futures import ThreadPoolExecutor
+from contextvars import copy_context
+from typing import (
+    AbstractSet,
+    Any,
+    Iterable,
+    Mapping,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import toposort as toposort_
 from typing_extensions import Final
 
 import dagster._check as check
 from dagster._utils import library_version_from_core_version, parse_package_version
 
@@ -106,7 +118,15 @@
         split = env_var_str.split("=", maxsplit=1)
         return (split[0], split[1])
     else:
         env_var_value = os.getenv(env_var_str)
         if env_var_value is None:
             raise Exception(f"Tried to load environment variable {env_var_str}, but it was not set")
         return (env_var_str, cast(str, env_var_value))
+
+
+class InheritContextThreadPoolExecutor(ThreadPoolExecutor):
+    """A ThreadPoolExecutor that copies over contextvars at submit time."""
+
+    def submit(self, fn, *args, **kwargs):
+        ctx = copy_context()
+        return super().submit(ctx.run, fn, *args, **kwargs)
```

### Comparing `dagster-1.3.7/dagster/_core/workspace/autodiscovery.py` & `dagster-1.3.8/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/workspace/config_schema.py` & `dagster-1.3.8/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/workspace/context.py` & `dagster-1.3.8/dagster/_core/workspace/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,14 +405,20 @@
         pass
 
     def shutdown_code_location(self, name: str) -> None:
         raise NotImplementedError
 
     @abstractmethod
     def reload_workspace(self) -> None:
+        """Reload the code in each code location."""
+        pass
+
+    @abstractmethod
+    def refresh_workspace(self) -> None:
+        """Refresh the snapshots for each code location, without reloading the underlying code."""
         pass
 
     @property
     @abstractmethod
     def instance(self) -> DagsterInstance:
         pass
 
@@ -458,14 +464,15 @@
         self._version = version
 
         # Guards changes to _location_entry_dict, _watch_thread_shutdown_events and _watch_threads
         self._lock = threading.Lock()
         self._watch_thread_shutdown_events: Dict[str, threading.Event] = {}
         self._watch_threads: Dict[str, threading.Thread] = {}
 
+        self._state_subscribers_lock = threading.Lock()
         self._state_subscriber_id_iter = count()
         self._state_subscribers: Dict[int, LocationStateSubscriber] = {}
         self.add_state_subscriber(LocationStateSubscriber(self._location_state_events_handler))
 
         if grpc_server_registry:
             self._grpc_server_registry: GrpcServerRegistry = check.inst_param(
                 grpc_server_registry, "grpc_server_registry", GrpcServerRegistry
@@ -496,20 +503,22 @@
 
     @property
     def _origins(self) -> Sequence[CodeLocationOrigin]:
         return self._workspace_load_target.create_origins() if self._workspace_load_target else []
 
     def add_state_subscriber(self, subscriber: LocationStateSubscriber) -> int:
         token = next(self._state_subscriber_id_iter)
-        self._state_subscribers[token] = subscriber
+        with self._state_subscribers_lock:
+            self._state_subscribers[token] = subscriber
         return token
 
     def rm_state_subscriber(self, token: int) -> None:
-        if token in self._state_subscribers:
-            del self._state_subscribers[token]
+        with self._state_subscribers_lock:
+            if token in self._state_subscribers:
+                del self._state_subscribers[token]
 
     @property
     def instance(self) -> DagsterInstance:
         return self._instance
 
     @property
     def read_only(self) -> bool:
@@ -524,16 +533,17 @@
 
     @property
     def version(self) -> str:
         return self._version
 
     def _send_state_event_to_subscribers(self, event: LocationStateChangeEvent) -> None:
         check.inst_param(event, "event", LocationStateChangeEvent)
-        for subscriber in self._state_subscribers.values():
-            subscriber.handle_event(event)
+        with self._state_subscribers_lock:
+            for subscriber in self._state_subscribers.values():
+                subscriber.handle_event(event)
 
     def _start_watch_thread(self, origin: GrpcServerCodeLocationOrigin) -> None:
         from dagster._grpc.server_watcher import create_grpc_watch_thread
 
         location_name = origin.location_name
         check.invariant(location_name not in self._watch_thread_shutdown_events)
         client = origin.create_client()
@@ -646,14 +656,21 @@
             # is referencing it
             self._location_entry_dict[name] = new
 
     def shutdown_code_location(self, name: str) -> None:
         with self._lock:
             self._location_entry_dict[name].origin.shutdown_server()
 
+    def refresh_workspace(self) -> None:
+        updated_locations = {
+            origin.location_name: self._load_location(origin, reload=False)
+            for origin in self._origins
+        }
+        self._update_workspace(updated_locations)
+
     def reload_workspace(self) -> None:
         updated_locations = {
             origin.location_name: self._load_location(origin, reload=True)
             for origin in self._origins
         }
         self._update_workspace(updated_locations)
```

### Comparing `dagster-1.3.7/dagster/_core/workspace/load.py` & `dagster-1.3.8/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/workspace/load_target.py` & `dagster-1.3.8/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_core/workspace/permissions.py` & `dagster-1.3.8/dagster/_core/workspace/permissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     RELOAD_REPOSITORY_LOCATION = "reload_repository_location"
     RELOAD_WORKSPACE = "reload_workspace"
     WIPE_ASSETS = "wipe_assets"
     LAUNCH_PARTITION_BACKFILL = "launch_partition_backfill"
     CANCEL_PARTITION_BACKFILL = "cancel_partition_backfill"
     EDIT_DYNAMIC_PARTITIONS = "edit_dynamic_partitions"
     TOGGLE_AUTO_MATERIALIZE = "toggle_auto_materialize"
+    EDIT_CONCURRENCY_LIMIT = "edit_concurrency_limit"
 
     def __str__(self) -> str:
         return str.__str__(self)
 
 
 VIEWER_PERMISSIONS: Dict[str, bool] = {
     Permissions.LAUNCH_PIPELINE_EXECUTION: False,
@@ -36,14 +37,15 @@
     Permissions.RELOAD_REPOSITORY_LOCATION: False,
     Permissions.RELOAD_WORKSPACE: False,
     Permissions.WIPE_ASSETS: False,
     Permissions.LAUNCH_PARTITION_BACKFILL: False,
     Permissions.CANCEL_PARTITION_BACKFILL: False,
     Permissions.EDIT_DYNAMIC_PARTITIONS: False,
     Permissions.TOGGLE_AUTO_MATERIALIZE: False,
+    Permissions.EDIT_CONCURRENCY_LIMIT: False,
 }
 
 EDITOR_PERMISSIONS: Dict[str, bool] = {
     Permissions.LAUNCH_PIPELINE_EXECUTION: True,
     Permissions.LAUNCH_PIPELINE_REEXECUTION: True,
     Permissions.START_SCHEDULE: True,
     Permissions.STOP_RUNNING_SCHEDULE: True,
@@ -54,14 +56,15 @@
     Permissions.RELOAD_REPOSITORY_LOCATION: True,
     Permissions.RELOAD_WORKSPACE: True,
     Permissions.WIPE_ASSETS: True,
     Permissions.LAUNCH_PARTITION_BACKFILL: True,
     Permissions.CANCEL_PARTITION_BACKFILL: True,
     Permissions.EDIT_DYNAMIC_PARTITIONS: True,
     Permissions.TOGGLE_AUTO_MATERIALIZE: True,
+    Permissions.EDIT_CONCURRENCY_LIMIT: True,
 }
 
 LOCATION_SCOPED_PERMISSIONS = {
     Permissions.LAUNCH_PIPELINE_EXECUTION,
     Permissions.LAUNCH_PIPELINE_REEXECUTION,
     Permissions.START_SCHEDULE,
     Permissions.STOP_RUNNING_SCHEDULE,
```

### Comparing `dagster-1.3.7/dagster/_core/workspace/workspace.py` & `dagster-1.3.8/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_daemon/__init__.py` & `dagster-1.3.8/dagster/_daemon/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,17 +23,18 @@
     SensorDaemon as SensorDaemon,
     get_default_daemon_logger as get_default_daemon_logger,
     get_telemetry_daemon_session_id as get_telemetry_daemon_session_id,
 )
 from .monitoring import (
     RESUME_RUN_LOG_MESSAGE as RESUME_RUN_LOG_MESSAGE,
     count_resume_run_attempts as count_resume_run_attempts,
-    execute_monitoring_iteration as execute_monitoring_iteration,
+    execute_concurrency_slots_iteration as execute_concurrency_slots_iteration,
+    execute_run_monitoring_iteration as execute_run_monitoring_iteration,
 )
-from .monitoring.monitoring_daemon import (
+from .monitoring.run_monitoring import (
     monitor_started_run as monitor_started_run,
     monitor_starting_run as monitor_starting_run,
 )
 from .run_coordinator.queued_run_coordinator_daemon import (
     QueuedRunCoordinatorDaemon as QueuedRunCoordinatorDaemon,
 )
 from .sensor import (
```

### Comparing `dagster-1.3.7/dagster/_daemon/asset_daemon.py` & `dagster-1.3.8/dagster/_daemon/asset_daemon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import dagster._check as check
 from dagster._core.definitions.asset_reconciliation_sensor import (
     AssetReconciliationCursor,
     reconcile,
 )
 from dagster._core.definitions.external_asset_graph import ExternalAssetGraph
 from dagster._core.definitions.selector import JobSubsetSelector
@@ -26,14 +28,27 @@
 
 def set_auto_materialize_paused(instance: DagsterInstance, paused: bool):
     instance.daemon_cursor_storage.set_cursor_values(
         {ASSET_DAEMON_PAUSED_KEY: "true" if paused else "false"}
     )
 
 
+def _get_raw_cursor(instance: DagsterInstance) -> Optional[str]:
+    return instance.daemon_cursor_storage.get_cursor_values({CURSOR_KEY}).get(CURSOR_KEY)
+
+
+def get_current_evaluation_id(instance: DagsterInstance) -> Optional[int]:
+    raw_cursor = _get_raw_cursor(instance)
+    return (
+        AssetReconciliationCursor.get_evaluation_id_from_serialized(raw_cursor)
+        if raw_cursor
+        else None
+    )
+
+
 class AssetDaemon(IntervalDaemon):
     def __init__(self, interval_seconds: int):
         super().__init__(interval_seconds=interval_seconds)
 
     @classmethod
     def daemon_type(cls) -> str:
         return "ASSET"
@@ -67,18 +82,15 @@
             if asset_graph.get_auto_materialize_policy(target_key) is not None
         }
 
         if not target_asset_keys:
             yield
             return
 
-        persisted_info = instance.daemon_cursor_storage.get_cursor_values(
-            {CURSOR_KEY, ASSET_DAEMON_PAUSED_KEY}
-        )
-        raw_cursor = persisted_info.get(CURSOR_KEY)
+        raw_cursor = _get_raw_cursor(instance)
         cursor = (
             AssetReconciliationCursor.from_serialized(raw_cursor, asset_graph)
             if raw_cursor
             else AssetReconciliationCursor.empty()
         )
 
         run_requests, new_cursor, evaluations = reconcile(
```

### Comparing `dagster-1.3.7/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.3.8/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.3.8/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_daemon/backfill.py` & `dagster-1.3.8/dagster/_daemon/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_daemon/cli/__init__.py` & `dagster-1.3.8/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_daemon/controller.py` & `dagster-1.3.8/dagster/_daemon/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 
 def create_daemon_grpc_server_registry(
     instance: DagsterInstance, code_server_log_level: str = "INFO"
 ) -> GrpcServerRegistry:
     return GrpcServerRegistry(
         instance_ref=instance.get_ref(),
-        reload_interval=DAEMON_GRPC_SERVER_RELOAD_INTERVAL,
+        reload_interval=0,  # refresh_workspace call handles the reload
         heartbeat_ttl=DAEMON_GRPC_SERVER_HEARTBEAT_TTL,
         startup_timeout=instance.code_server_process_startup_timeout,
         log_level=code_server_log_level,
         wait_for_processes_on_shutdown=instance.wait_for_local_code_server_processes_on_shutdown,
     )
 
 
@@ -106,37 +106,40 @@
         controller = stack.enter_context(
             DagsterDaemonController(
                 workspace_process_context,
                 daemons,
                 heartbeat_interval_seconds=heartbeat_interval_seconds,
                 heartbeat_tolerance_seconds=heartbeat_tolerance_seconds,
                 error_interval_seconds=error_interval_seconds,
+                grpc_server_registry=grpc_server_registry,
             )
         )
 
         yield controller
 
 
 class DagsterDaemonController(AbstractContextManager):
     _daemon_uuid: str
     _daemons: Dict[str, DagsterDaemon]
+    _grpc_server_registry: Optional[GrpcServerRegistry]
     _daemon_threads: Dict[str, threading.Thread]
     _workspace_process_context: IWorkspaceProcessContext
     _instance: DagsterInstance
     _heartbeat_interval_seconds: float
     _heartbeat_tolerance_seconds: float
     _daemon_shutdown_event: threading.Event
     _logger: logging.Logger
     _last_healthy_heartbeat_times: Dict[str, float]
     _start_time: datetime.datetime
 
     def __init__(
         self,
         workspace_process_context: IWorkspaceProcessContext,
         daemons: Sequence[DagsterDaemon],
+        grpc_server_registry: Optional[GrpcServerRegistry] = None,
         heartbeat_interval_seconds: float = DEFAULT_HEARTBEAT_INTERVAL_SECONDS,
         heartbeat_tolerance_seconds: float = DEFAULT_DAEMON_HEARTBEAT_TOLERANCE_SECONDS,
         error_interval_seconds: int = DEFAULT_DAEMON_ERROR_INTERVAL_SECONDS,
         handler: str = "default",
     ):
         self._daemon_uuid = str(uuid.uuid4())
 
@@ -151,14 +154,16 @@
             heartbeat_interval_seconds, "heartbeat_interval_seconds"
         )
 
         self._heartbeat_tolerance_seconds = check.numeric_param(
             heartbeat_tolerance_seconds, "heartbeat_tolerance_seconds"
         )
 
+        self._grpc_server_registry = grpc_server_registry
+
         if not self._daemons:
             raise Exception("No daemons configured on the DagsterInstance")
 
         self._daemon_shutdown_event = threading.Event()
 
         configure_loggers(handler=handler)
 
@@ -264,15 +269,17 @@
         while True:
             with raise_interrupts_as(KeyboardInterrupt):
                 time.sleep(THREAD_CHECK_INTERVAL)
                 self.check_daemon_threads()
 
                 # periodically refresh the shared workspace context
                 if (time.time() - last_workspace_update_time) > RELOAD_WORKSPACE_INTERVAL:
-                    self._workspace_process_context.reload_workspace()
+                    if self._grpc_server_registry:
+                        self._grpc_server_registry.clear_all_grpc_endpoints()
+                    self._workspace_process_context.refresh_workspace()
                     last_workspace_update_time = time.time()
 
                 if self._instance.daemon_skip_heartbeats_without_errors:
                     # If we're skipping heartbeats without errors, we just check the threads.
                     # If there's no errors, the daemons won't be writing heartbeats.
                     continue
```

### Comparing `dagster-1.3.7/dagster/_daemon/daemon.py` & `dagster-1.3.8/dagster/_daemon/daemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,18 @@
     DagsterInstance,
     _check as check,
 )
 from dagster._core.scheduler.scheduler import DagsterDaemonScheduler
 from dagster._core.telemetry import DAEMON_ALIVE, log_action
 from dagster._core.workspace.context import IWorkspaceProcessContext
 from dagster._daemon.backfill import execute_backfill_iteration
-from dagster._daemon.monitoring import execute_monitoring_iteration
+from dagster._daemon.monitoring import (
+    execute_concurrency_slots_iteration,
+    execute_run_monitoring_iteration,
+)
 from dagster._daemon.sensor import execute_sensor_iteration_loop
 from dagster._daemon.types import DaemonHeartbeat
 from dagster._scheduler.scheduler import execute_scheduler_iteration_loop
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 
 if TYPE_CHECKING:
     from pendulum.datetime import DateTime
@@ -291,8 +294,9 @@
     def daemon_type(cls) -> str:
         return "MONITORING"
 
     def run_iteration(
         self,
         workspace_process_context: IWorkspaceProcessContext,
     ) -> DaemonIterator:
-        yield from execute_monitoring_iteration(workspace_process_context, self._logger)
+        yield from execute_run_monitoring_iteration(workspace_process_context, self._logger)
+        yield from execute_concurrency_slots_iteration(workspace_process_context, self._logger)
```

### Comparing `dagster-1.3.7/dagster/_daemon/monitoring/monitoring_daemon.py` & `dagster-1.3.8/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
                 logger.info(msg)
                 instance.report_run_failed(run, msg)
                 # Return rather than immediately checking for a timeout, since we just failed
                 return
     check_run_timeout(instance, run_record, logger)
 
 
-def execute_monitoring_iteration(
+def execute_run_monitoring_iteration(
     workspace_process_context: IWorkspaceProcessContext,
     logger: logging.Logger,
     _debug_crash_flags: Optional[DebugCrashFlags] = None,
 ) -> Iterator[Optional[SerializableErrorInfo]]:
     instance = workspace_process_context.instance
 
     # TODO: consider limiting number of runs to fetch
```

### Comparing `dagster-1.3.7/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.3.8/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from dagster._core.storage.dagster_run import (
     IN_PROGRESS_RUN_STATUSES,
     DagsterRun,
     DagsterRunStatus,
     RunsFilter,
 )
 from dagster._core.storage.tags import PRIORITY_TAG
+from dagster._core.utils import InheritContextThreadPoolExecutor
 from dagster._core.workspace.context import IWorkspaceProcessContext
 from dagster._core.workspace.workspace import IWorkspace
 from dagster._daemon.daemon import DaemonIterator, IntervalDaemon
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.tags import TagConcurrencyLimitsCounter
 
 
@@ -44,15 +45,15 @@
         self._location_timeouts: Dict[str, float] = {}
         super().__init__(interval_seconds)
 
     def _get_executor(self, max_workers) -> ThreadPoolExecutor:
         if self._executor is None:
             # assumes max_workers wont change
             self._executor = self._exit_stack.enter_context(
-                ThreadPoolExecutor(
+                InheritContextThreadPoolExecutor(
                     max_workers=max_workers,
                     thread_name_prefix="run_dequeue_worker",
                 )
             )
         return self._executor
 
     def __exit__(self, _exception_type, _exception_value, _traceback):
```

### Comparing `dagster-1.3.7/dagster/_daemon/sensor.py` & `dagster-1.3.8/dagster/_daemon/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     SensorInstigatorData,
     TickData,
     TickStatus,
 )
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus, RunsFilter
 from dagster._core.storage.tags import RUN_KEY_TAG, SENSOR_NAME_TAG
 from dagster._core.telemetry import SENSOR_RUN_CREATED, hash_name, log_action
+from dagster._core.utils import InheritContextThreadPoolExecutor
 from dagster._core.workspace.context import IWorkspaceProcessContext
 from dagster._scheduler.stale import resolve_stale_or_missing_assets
 from dagster._utils import DebugCrashFlags, SingleInstigatorDebugCrashFlags
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.merger import merge_dicts
 
 if TYPE_CHECKING:
@@ -257,23 +258,23 @@
     sensor_tick_futures: Dict[str, Future] = {}
     submit_threadpool_executor = None
     threadpool_executor = None
     with ExitStack() as stack:
         settings = workspace_process_context.instance.get_settings("sensors")
         if settings.get("use_threads"):
             threadpool_executor = stack.enter_context(
-                ThreadPoolExecutor(
+                InheritContextThreadPoolExecutor(
                     max_workers=settings.get("num_workers"),
                     thread_name_prefix="sensor_daemon_worker",
                 )
             )
             num_submit_workers = settings.get("num_submit_workers")
             if num_submit_workers:
                 submit_threadpool_executor = stack.enter_context(
-                    ThreadPoolExecutor(
+                    InheritContextThreadPoolExecutor(
                         max_workers=settings.get("num_submit_workers"),
                         thread_name_prefix="sensor_submit_worker",
                     )
                 )
 
         last_verbose_time = None
         while True:
```

### Comparing `dagster-1.3.7/dagster/_daemon/types.py` & `dagster-1.3.8/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_daemon/workspace.py` & `dagster-1.3.8/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_generate/download.py` & `dagster-1.3.8/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_generate/generate.py` & `dagster-1.3.8/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.3.8/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.3.8/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.3.8/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/__init__.py` & `dagster-1.3.8/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/client.py` & `dagster-1.3.8/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/compile.py` & `dagster-1.3.8/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/impl.py` & `dagster-1.3.8/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/protos/api.proto` & `dagster-1.3.8/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/proxy_server.py` & `dagster-1.3.8/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/server.py` & `dagster-1.3.8/dagster/_grpc/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1068,31 +1068,26 @@
     container_image: Optional[str] = None,
     container_context: Optional[dict[str, Any]] = None,
 ):
     check.invariant((port or socket) and not (port and socket), "Set only port or socket")
     check.opt_inst_param(loadable_target_origin, "loadable_target_origin", LoadableTargetOrigin)
     check.opt_int_param(max_workers, "max_workers")
 
-    from dagster._core.test_utils import get_mocked_system_timezone
-
-    mocked_system_timezone = get_mocked_system_timezone()
-
     executable_path = loadable_target_origin.executable_path if loadable_target_origin else None
 
     subprocess_args = [
         *get_python_environment_entry_point(executable_path or sys.executable),
         *["api", "grpc"],
         *["--lazy-load-user-code"],
         *(["--port", str(port)] if port else []),
         *(["--socket", socket] if socket else []),
         *(["-n", str(max_workers)] if max_workers else []),
         *(["--heartbeat"] if heartbeat else []),
         *(["--heartbeat-timeout", str(heartbeat_timeout)] if heartbeat_timeout else []),
         *(["--fixed-server-id", fixed_server_id] if fixed_server_id else []),
-        *(["--override-system-timezone", mocked_system_timezone] if mocked_system_timezone else []),
         *(["--log-level", log_level]),
         # only use the Python environment if it has been explicitly set in the workspace,
         *(["--use-python-environment-entry-point"] if executable_path else []),
         *(["--inject-env-vars-from-instance"] if inject_env_vars_from_instance else []),
         *(["--instance-ref", serialize_value(instance_ref)] if instance_ref else []),
         *(["--location-name", location_name] if location_name else []),
         *(["--container-image", container_image] if container_image else []),
```

### Comparing `dagster-1.3.7/dagster/_grpc/server_watcher.py` & `dagster-1.3.8/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/types.py` & `dagster-1.3.8/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_grpc/utils.py` & `dagster-1.3.8/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_loggers/__init__.py` & `dagster-1.3.8/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_module_alias_map.py` & `dagster-1.3.8/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_scheduler/scheduler.py` & `dagster-1.3.8/dagster/_scheduler/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     TickData,
     TickStatus,
 )
 from dagster._core.scheduler.scheduler import DEFAULT_MAX_CATCHUP_RUNS, DagsterSchedulerError
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus, RunsFilter
 from dagster._core.storage.tags import RUN_KEY_TAG, SCHEDULED_EXECUTION_TIME_TAG
 from dagster._core.telemetry import SCHEDULED_RUN_CREATED, hash_name, log_action
+from dagster._core.utils import InheritContextThreadPoolExecutor
 from dagster._core.workspace.context import IWorkspaceProcessContext
 from dagster._scheduler.stale import resolve_stale_or_missing_assets
 from dagster._seven.compat.pendulum import to_timezone
 from dagster._utils import DebugCrashFlags, SingleInstigatorDebugCrashFlags
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.log import default_date_format_string
 from dagster._utils.merger import merge_dicts
@@ -128,23 +129,23 @@
     submit_threadpool_executor = None
     threadpool_executor = None
 
     with ExitStack() as stack:
         settings = workspace_process_context.instance.get_settings("schedules")
         if settings.get("use_threads"):
             threadpool_executor = stack.enter_context(
-                ThreadPoolExecutor(
+                InheritContextThreadPoolExecutor(
                     max_workers=settings.get("num_workers"),
                     thread_name_prefix="schedule_daemon_worker",
                 )
             )
             num_submit_workers = settings.get("num_submit_workers")
             if num_submit_workers:
                 submit_threadpool_executor = stack.enter_context(
-                    ThreadPoolExecutor(
+                    InheritContextThreadPoolExecutor(
                         max_workers=settings.get("num_submit_workers"),
                         thread_name_prefix="schedule_submit_worker",
                     )
                 )
 
         last_verbose_time = None
         while True:
```

### Comparing `dagster-1.3.7/dagster/_scheduler/stale.py` & `dagster-1.3.8/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_serdes/__init__.py` & `dagster-1.3.8/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_serdes/config_class.py` & `dagster-1.3.8/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_serdes/ipc.py` & `dagster-1.3.8/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_serdes/serdes.py` & `dagster-1.3.8/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_serdes/utils.py` & `dagster-1.3.8/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_seven/__init__.py` & `dagster-1.3.8/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_seven/abc.py` & `dagster-1.3.8/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_seven/compat/pendulum.py` & `dagster-1.3.8/dagster/_seven/compat/pendulum.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/__init__.py` & `dagster-1.3.8/dagster/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/alert.py` & `dagster-1.3.8/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/backcompat.py` & `dagster-1.3.8/dagster/_utils/backcompat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/backoff.py` & `dagster-1.3.8/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/cached_method.py` & `dagster-1.3.8/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/caching_instance_queryer.py` & `dagster-1.3.8/dagster/_utils/caching_instance_queryer.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 from dagster._core.definitions.asset_graph import AssetGraph
 from dagster._core.definitions.data_version import (
     DataVersion,
     extract_data_version_from_entry,
 )
 from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
+from dagster._core.definitions.partition import DynamicPartitionsDefinition
+from dagster._core.definitions.time_window_partitions import TimeWindowPartitionsDefinition
 from dagster._core.events import DagsterEventType
 from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
 from dagster._core.storage.dagster_run import (
     DagsterRun,
     RunRecord,
 )
 from dagster._core.storage.tags import PARTITION_NAME_TAG
@@ -576,20 +578,33 @@
         # always treat source assets as reconciled
         if asset_graph.is_source(asset_partition.asset_key):
             return True
 
         if not self.materialization_exists(asset_partition):
             return False
 
+        time_or_dynamic_partitioned = isinstance(
+            asset_graph.get_partitions_def(asset_partition.asset_key),
+            (TimeWindowPartitionsDefinition, DynamicPartitionsDefinition),
+        )
         for parent in asset_graph.get_parents_partitions(
             self,
             self._evaluation_time,
             asset_partition.asset_key,
             asset_partition.partition_key,
         ):
+            # when mapping from time or dynamic downstream to unpartitioned upstream, only check
+            # for existence of upstream materialization, do not worry about timestamps
+            if time_or_dynamic_partitioned and parent.partition_key is None:
+                return (
+                    # no materializations exist for source assets
+                    asset_graph.is_source(parent.asset_key)
+                    or self.materialization_exists(parent)
+                )
+
             if asset_graph.is_source(parent.asset_key):
                 if asset_graph.is_observable(
                     parent.asset_key
                 ) and self._new_version_of_source_exists_after_asset_partition(
                     observable_source_asset_key=parent.asset_key,
                     asset_partition=asset_partition,
                 ):
```

### Comparing `dagster-1.3.7/dagster/_utils/dagster_type.py` & `dagster-1.3.8/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/env.py` & `dagster-1.3.8/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/error.py` & `dagster-1.3.8/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/external.py` & `dagster-1.3.8/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/forked_pdb.py` & `dagster-1.3.8/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/hosted_user_process.py` & `dagster-1.3.8/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/indenting_printer.py` & `dagster-1.3.8/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/interrupts.py` & `dagster-1.3.8/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/log.py` & `dagster-1.3.8/dagster/_utils/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import copy
 import logging
 import sys
 import traceback
-from contextlib import contextmanager
 from typing import Mapping, NamedTuple, Optional
 
 import coloredlogs
-import pendulum
 
 import dagster._check as check
 import dagster._seven as seven
 from dagster._config import Enum, EnumValue
 from dagster._core.definitions.logger_definition import logger
 from dagster._core.utils import PYTHON_LOGGING_LEVELS_MAPPING, coerce_valid_log_level
 
@@ -202,44 +200,26 @@
     if hasattr(exception, "__traceback__"):
         tb = exception.__traceback__
     else:
         _exc_type, _exc_value, tb = sys.exc_info()
     return traceback.format_tb(tb)
 
 
-def _mockable_formatTime(record, datefmt=None):
-    """Uses pendulum.now to determine the logging time, causing pendulum
-    mocking to affect the logger timestamp in tests.
-    """
-    return pendulum.now().strftime(datefmt if datefmt else default_date_format_string())
-
-
 def default_format_string():
     return "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
 
 
 def default_date_format_string():
     return "%Y-%m-%d %H:%M:%S %z"
 
 
 def define_default_formatter():
     return logging.Formatter(default_format_string(), default_date_format_string())
 
 
-@contextmanager
-def quieten(quiet=True, level=logging.WARNING):
-    if quiet:
-        logging.disable(level)
-    try:
-        yield
-    finally:
-        if quiet:
-            logging.disable(logging.NOTSET)
-
-
 def configure_loggers(handler="default", log_level="INFO"):
     LOGGING_CONFIG = {
         "version": 1,
         "disable_existing_loggers": False,
         "formatters": {
             "colored": {
                 "()": coloredlogs.ColoredFormatter,
@@ -270,18 +250,14 @@
                 "level": "INFO",
             },
         },
     }
 
     logging.config.dictConfig(LOGGING_CONFIG)
 
-    if handler == "default":
-        for name in ["dagster", "dagit"]:
-            logging.getLogger(name).handlers[0].formatter.formatTime = _mockable_formatTime
-
 
 def create_console_logger(name, level):
     klass = logging.getLoggerClass()
     handler = klass(name, level=level)
     coloredlogs.install(
         logger=handler,
         level=level,
```

### Comparing `dagster-1.3.7/dagster/_utils/merger.py` & `dagster-1.3.8/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/net.py` & `dagster-1.3.8/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/schedules.py` & `dagster-1.3.8/dagster/_utils/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/tags.py` & `dagster-1.3.8/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/temp_file.py` & `dagster-1.3.8/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/test/__init__.py` & `dagster-1.3.8/dagster/_utils/test/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # top-level include is dangerous in terms of incurring circular deps
 from dagster import (
     DagsterInvariantViolationError,
     DependencyDefinition,
     NodeInvocation,
     _check as check,
 )
+from dagster._config import Field, StringSource
+from dagster._config.config_schema import UserConfigSchema
 from dagster._core.definitions import (
     GraphDefinition,
     InputMapping,
     JobDefinition,
     OpDefinition,
     OutputMapping,
 )
@@ -33,16 +35,20 @@
     create_log_manager,
     create_plan_data,
 )
 from dagster._core.execution.execute_in_process_result import ExecuteInProcessResult
 from dagster._core.instance import DagsterInstance
 from dagster._core.scheduler import Scheduler
 from dagster._core.storage.dagster_run import DagsterRun
+from dagster._core.storage.event_log.sqlite.sqlite_event_log import SqliteEventLogStorage
+from dagster._core.storage.sqlite_storage import SqliteStorageConfig
 from dagster._core.utility_ops import create_stub_op
 from dagster._serdes import ConfigurableClass
+from dagster._serdes.config_class import ConfigurableClassData
+from dagster._utils.concurrency import ConcurrencyClaimStatus
 
 # re-export
 from ..temp_file import (
     get_temp_dir as get_temp_dir,
     get_temp_file_handle as get_temp_file_handle,
     get_temp_file_handle_with_data as get_temp_file_handle_with_data,
     get_temp_file_name as get_temp_file_name,
@@ -272,7 +278,57 @@
 
     def get_logs_path(self, _instance: DagsterInstance, schedule_origin_id: str) -> str:
         check.str_param(schedule_origin_id, "schedule_origin_id")
         return os.path.join(self._artifacts_dir, "logs", schedule_origin_id, "scheduler.log")
 
     def wipe(self, instance: DagsterInstance) -> None:
         pass
+
+
+class TestStorageConfig(SqliteStorageConfig):
+    # interval to sleep between claim checks
+    sleep_interval: int
+
+
+class ConcurrencyEnabledSqliteTestEventLogStorage(SqliteEventLogStorage, ConfigurableClass):
+    """Sqlite is sorta supported for concurrency, as long as the rate of concurrent writes is tolerably
+    low.  Officially, we should not support, but in the spirit of getting code coverage in the core
+    dagster package, let's mark it as that.
+    """
+
+    __test__ = False
+
+    def __init__(
+        self,
+        base_dir: str,
+        sleep_interval: Optional[float] = None,
+        inst_data: Optional[ConfigurableClassData] = None,
+    ):
+        self._sleep_interval = sleep_interval
+        self._check_calls = defaultdict(int)
+        super().__init__(base_dir, inst_data)
+
+    @classmethod
+    def config_type(cls) -> UserConfigSchema:
+        return {"base_dir": StringSource, "sleep_interval": Field(float, is_required=False)}
+
+    @classmethod
+    def from_config_value(
+        cls, inst_data: Optional[ConfigurableClassData], config_value: TestStorageConfig
+    ) -> "ConcurrencyEnabledSqliteTestEventLogStorage":
+        return ConcurrencyEnabledSqliteTestEventLogStorage(inst_data=inst_data, **config_value)
+
+    @property
+    def supports_global_concurrency_limits(self) -> bool:
+        return True
+
+    def get_check_calls(self, step_key: str) -> int:
+        return self._check_calls[step_key]
+
+    def check_concurrency_claim(
+        self, concurrency_key: str, run_id: str, step_key: str
+    ) -> ConcurrencyClaimStatus:
+        self._check_calls[step_key] += 1
+        claim_status = super().check_concurrency_claim(concurrency_key, run_id, step_key)
+        if not self._sleep_interval:
+            return claim_status
+        return claim_status.with_sleep_interval(float(self._sleep_interval))
```

### Comparing `dagster-1.3.7/dagster/_utils/test/mysql_instance.py` & `dagster-1.3.8/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/test/postgres_instance.py` & `dagster-1.3.8/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/test/schedule_storage.py` & `dagster-1.3.8/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/timing.py` & `dagster-1.3.8/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/typing_api.py` & `dagster-1.3.8/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster/_utils/yaml_utils.py` & `dagster-1.3.8/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.3.7/dagster.egg-info/PKG-INFO` & `dagster-1.3.8/dagster.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.3.7
+Version: 1.3.8
 Summary: The data orchestration platform built for productivity.
 Author: Elementl
 Author-email: hello@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Changelog, https://github.com/dagster-io/dagster/releases
```

### Comparing `dagster-1.3.7/dagster.egg-info/SOURCES.txt` & `dagster-1.3.8/dagster.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,15 @@
 dagster/_core/execution/plan/compute.py
 dagster/_core/execution/plan/compute_generator.py
 dagster/_core/execution/plan/execute_plan.py
 dagster/_core/execution/plan/execute_step.py
 dagster/_core/execution/plan/external_step.py
 dagster/_core/execution/plan/handle.py
 dagster/_core/execution/plan/inputs.py
+dagster/_core/execution/plan/instance_concurrency_context.py
 dagster/_core/execution/plan/local_external_step_main.py
 dagster/_core/execution/plan/objects.py
 dagster/_core/execution/plan/outputs.py
 dagster/_core/execution/plan/plan.py
 dagster/_core/execution/plan/resume_retry.py
 dagster/_core/execution/plan/state.py
 dagster/_core/execution/plan/step.py
@@ -305,14 +306,15 @@
 dagster/_core/storage/memoizable_io_manager.py
 dagster/_core/storage/noop_compute_log_manager.py
 dagster/_core/storage/output_manager.py
 dagster/_core/storage/partition_status_cache.py
 dagster/_core/storage/root.py
 dagster/_core/storage/root_input_manager.py
 dagster/_core/storage/sql.py
+dagster/_core/storage/sqlalchemy_compat.py
 dagster/_core/storage/sqlite.py
 dagster/_core/storage/sqlite_storage.py
 dagster/_core/storage/tags.py
 dagster/_core/storage/temp_file_manager.py
 dagster/_core/storage/upath_io_manager.py
 dagster/_core/storage/alembic/README.md
 dagster/_core/storage/alembic/env.py
@@ -390,14 +392,15 @@
 dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
 dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
 dagster/_core/storage/alembic/versions/035_add_run_job_index.py
 dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
 dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
 dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
 dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
 dagster/_core/storage/alembic/versions/__init__.py
 dagster/_core/storage/branching/__init__.py
 dagster/_core/storage/branching/branching_io_manager.py
 dagster/_core/storage/event_log/__init__.py
 dagster/_core/storage/event_log/base.py
 dagster/_core/storage/event_log/in_memory.py
 dagster/_core/storage/event_log/migration.py
@@ -459,15 +462,16 @@
 dagster/_daemon/types.py
 dagster/_daemon/workspace.py
 dagster/_daemon/auto_run_reexecution/__init__.py
 dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
 dagster/_daemon/auto_run_reexecution/event_log_consumer.py
 dagster/_daemon/cli/__init__.py
 dagster/_daemon/monitoring/__init__.py
-dagster/_daemon/monitoring/monitoring_daemon.py
+dagster/_daemon/monitoring/concurrency.py
+dagster/_daemon/monitoring/run_monitoring.py
 dagster/_daemon/run_coordinator/__init__.py
 dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
 dagster/_experimental/__init__.py
 dagster/_generate/__init__.py
 dagster/_generate/download.py
 dagster/_generate/generate.py
 dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
@@ -519,14 +523,15 @@
 dagster/_seven/compat/pendulum.py
 dagster/_utils/__init__.py
 dagster/_utils/alert.py
 dagster/_utils/backcompat.py
 dagster/_utils/backoff.py
 dagster/_utils/cached_method.py
 dagster/_utils/caching_instance_queryer.py
+dagster/_utils/concurrency.py
 dagster/_utils/dagster_type.py
 dagster/_utils/env.py
 dagster/_utils/error.py
 dagster/_utils/external.py
 dagster/_utils/forked_pdb.py
 dagster/_utils/hosted_user_process.py
 dagster/_utils/indenting_printer.py
```

### Comparing `dagster-1.3.7/dagster.egg-info/requires.txt` & `dagster-1.3.8/dagster.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 pytz
 requests
 setuptools
 tabulate
 tomli
 tqdm
 typing_extensions>=4.4.0
-sqlalchemy<2.0.0,>=1.0
+sqlalchemy>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 universal_pathlib
 pydantic!=1.10.7
 
 [:platform_system == "Windows"]
```

### Comparing `dagster-1.3.7/setup.py` & `dagster-1.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         "pytz",
         "requests",
         "setuptools",
         "tabulate",
         "tomli",
         "tqdm",
         "typing_extensions>=4.4.0",
-        "sqlalchemy>=1.0,<2.0.0",
+        "sqlalchemy>=1.0",
         "toposort>=1.0",
         "watchdog>=0.8.3",
         'psutil >= 1.0; platform_system=="Windows"',
         # https://github.com/mhammond/pywin32/issues/1439
         'pywin32 != 226; platform_system=="Windows"',
         "docstring-parser",
         "universal_pathlib",
```

