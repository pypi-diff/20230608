# Comparing `tmp/vdk-core-0.3.765384785.tar.gz` & `tmp/vdk-core-0.3.893910391.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-core-0.3.765384785.tar", last modified: Thu Feb  2 13:10:30 2023, max compression
+gzip compressed data, was "dist/vdk-core-0.3.893910391.tar", last modified: Thu Jun  8 13:45:30 2023, max compression
```

## Comparing `vdk-core-0.3.765384785.tar` & `vdk-core-0.3.893910391.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2460 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1542 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      435 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/api/
--rw-rw-rw-   0 root         (0) root         (0)     2556 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/api/data_job.py
--rw-rw-rw-   0 root         (0) root         (0)    17317 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/api/job_input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/api/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     6710 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/api/plugin/connection_hook_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     7779 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/api/plugin/core_hook_spec.py
--rw-rw-rw-   0 root         (0) root         (0)     2581 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/api/plugin/hook_markers.py
--rw-rw-rw-   0 root         (0) root         (0)    25723 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/api/plugin/plugin_input.py
--rw-rw-rw-   0 root         (0) root         (0)     4052 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/api/plugin/plugin_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3956 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/api/plugin/plugin_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/
--rw-rw-rw-   0 root         (0) root         (0)     5714 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/builtin_hook_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/config/
--rw-rw-rw-   0 root         (0) root         (0)     5107 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/config/config_help.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/config/job_config.py
--rw-rw-rw-   0 root         (0) root         (0)    11174 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/config/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9338 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/config/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/
--rw-rw-rw-   0 root         (0) root         (0)     3118 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/connection_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/connection_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4656 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py
--rw-rw-rw-   0 root         (0) root         (0)     2311 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/execution_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/impl/
--rw-rw-rw-   0 root         (0) root         (0)     6459 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/impl/router.py
--rw-rw-rw-   0 root         (0) root         (0)     1667 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py
--rw-rw-rw-   0 root         (0) root         (0)    10051 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py
--rw-rw-rw-   0 root         (0) root         (0)    10043 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/managed_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/pep249/
--rw-rw-rw-   0 root         (0) root         (0)     2953 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     2269 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py
--rw-rw-rw-   0 root         (0) root         (0)     3975 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/debug/
--rw-rw-rw-   0 root         (0) root         (0)     5741 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/debug/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/
--rw-rw-rw-   0 root         (0) root         (0)    29367 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     4064 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)    13242 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py
--rw-rw-rw-   0 root         (0) root         (0)     4626 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1844 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/internal_hookspecs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/
--rw-rw-rw-   0 root         (0) root         (0)      892 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3697 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2357 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/properties_config.py
--rw-rw-rw-   0 root         (0) root         (0)     8203 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/properties_router.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/notification/
--rw-rw-rw-   0 root         (0) root         (0)     4649 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/notification/notification.py
--rw-rw-rw-   0 root         (0) root         (0)    10651 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/notification/notification_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7980 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/notification/notification_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/
--rw-rw-rw-   0 root         (0) root         (0)     6220 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/cli_run.py
--rw-rw-rw-   0 root         (0) root         (0)    13568 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/execution_environment.py
--rw-rw-rw-   0 root         (0) root         (0)     5510 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/execution_results.py
--rw-rw-rw-   0 root         (0) root         (0)      872 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/execution_state.py
--rw-rw-rw-   0 root         (0) root         (0)     2674 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/execution_tracking.py
--rw-rw-rw-   0 root         (0) root         (0)     7125 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/file_based_step.py
--rw-rw-rw-   0 root         (0) root         (0)     3906 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/job_context.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/job_input.py
--rw-rw-rw-   0 root         (0) root         (0)     4851 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/run_status.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py
--rw-rw-rw-   0 root         (0) root         (0)     7954 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/standalone_data_job.py
--rw-rw-rw-   0 root         (0) root         (0)     1280 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3801 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/templates/template_impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/termination_message/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/termination_message/file_util.py
--rw-rw-rw-   0 root         (0) root         (0)     3115 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/termination_message/writer.py
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/version/
--rw-rw-rw-   0 root         (0) root         (0)     2652 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/version/new_version_check.py
--rw-rw-rw-   0 root         (0) root         (0)     4968 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     2759 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/version/version.py
--rw-rw-rw-   0 root         (0) root         (0)     6466 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/cli_entry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/core/
--rw-rw-rw-   0 root         (0) root         (0)     9593 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2350 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/core/context.py
--rw-rw-rw-   0 root         (0) root         (0)    21232 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/core/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     5352 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/core/statestore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     5195 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/plugin/plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/plugin/plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk/internal/util/
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/util/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-02-02 13:10:13.000000 vdk-core-0.3.765384785/src/vdk/internal/util/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2023-02-02 13:10:29.000000 vdk-core-0.3.765384785/src/vdk/internal/vdk_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2460 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4333 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk_core.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk_core.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-02-02 13:10:30.000000 vdk-core-0.3.765384785/src/vdk_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-02-02 13:10:29.000000 vdk-core-0.3.765384785/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/api/data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)    18539 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/api/job_input.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/api/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     6715 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/api/plugin/connection_hook_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     7784 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/api/plugin/core_hook_spec.py
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/api/plugin/hook_markers.py
+-rw-rw-rw-   0 root         (0) root         (0)    25728 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/api/plugin/plugin_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     4057 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/api/plugin/plugin_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3961 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/api/plugin/plugin_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)     5894 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/builtin_hook_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/config/
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/config/config_help.py
+-rw-rw-rw-   0 root         (0) root         (0)     4020 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/config/job_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/config/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    10141 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/config/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/
+-rw-rw-rw-   0 root         (0) root         (0)     3123 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/connection_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/connection_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4661 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/execution_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/impl/
+-rw-rw-rw-   0 root         (0) root         (0)     6464 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/impl/router.py
+-rw-rw-rw-   0 root         (0) root         (0)     1672 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10048 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/managed_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/pep249/
+-rw-rw-rw-   0 root         (0) root         (0)     2958 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3980 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/debug/
+-rw-rw-rw-   0 root         (0) root         (0)     5746 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/debug/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/
+-rw-rw-rw-   0 root         (0) root         (0)    29371 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4069 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13247 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/internal_hookspecs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3700 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/properties_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     8208 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/properties_router.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/notification/
+-rw-rw-rw-   0 root         (0) root         (0)     4654 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/notification/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)    10656 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/notification/notification_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7985 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/notification/notification_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/
+-rw-rw-rw-   0 root         (0) root         (0)     6225 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/cli_run.py
+-rw-rw-rw-   0 root         (0) root         (0)    13573 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1752 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/execution_environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     5515 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/execution_results.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/execution_state.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/execution_tracking.py
+-rw-rw-rw-   0 root         (0) root         (0)     7130 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/file_based_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     3911 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/job_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7082 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/job_input.py
+-rw-rw-rw-   0 root         (0) root         (0)     4856 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/run_status.py
+-rw-rw-rw-   0 root         (0) root         (0)     1366 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7959 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/standalone_data_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3806 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/templates/template_impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/termination_message/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/termination_message/file_util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3119 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/termination_message/writer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/version/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/version/new_version_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     4973 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2764 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/version/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6471 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/cli_entry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/core/
+-rw-rw-rw-   0 root         (0) root         (0)     9586 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2355 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/core/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    21237 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/core/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5683 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/core/statestore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     5200 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/plugin/plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/plugin/plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk/internal/util/
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/util/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2598 2023-06-08 13:45:07.000000 vdk-core-0.3.893910391/src/vdk/internal/util/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-06-08 13:45:28.000000 vdk-core-0.3.893910391/src/vdk/internal/vdk_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2460 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4333 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk_core.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk_core.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-08 13:45:30.000000 vdk-core-0.3.893910391/src/vdk_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-08 13:45:28.000000 vdk-core-0.3.893910391/version.txt
```

### Comparing `vdk-core-0.3.765384785/PKG-INFO` & `vdk-core-0.3.893910391/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-core
-Version: 0.3.765384785
+Version: 0.3.893910391
 Summary: Versatile Data Kit SDK Core
 Home-page: https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Author: VMware Inc.
 Author-email: taurus@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/projects/vdk-core/README.md
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Platform: any
```

### Comparing `vdk-core-0.3.765384785/README.md` & `vdk-core-0.3.893910391/README.md`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.765384785/setup.cfg` & `vdk-core-0.3.893910391/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-core-0.3.765384785/src/vdk/api/data_job.py` & `vdk-core-0.3.893910391/src/vdk/api/data_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import pathlib
 from abc import abstractmethod
 
 from vdk.api.job_input import IJobInput
```

### Comparing `vdk-core-0.3.765384785/src/vdk/api/job_input.py` & `vdk-core-0.3.893910391/src/vdk/api/job_input.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 from abc import ABCMeta
 from abc import abstractmethod
 from typing import Any
 from typing import List
 from typing import Optional
@@ -376,7 +376,29 @@
             the template will continue executing normally.
 
             This is to be used when users want
             customizable behaviour of data jobs/templates, where execution could be skipped. E.g. if a data job
             depends on processing data from a source which has indicated no new entries since last run, then we can skip
             the execution.
         """
+
+    @abstractmethod
+    def get_temporary_write_directory(self) -> pathlib.Path:
+        """
+        :return:
+            Returns a path pointing to a writable directory for
+            data job executions in the cloud. This is needed because
+            different cloud deployments may restrict access to the file
+            system in a cloud execution. In this way data job users can make
+            sure the returned folder will allow read/write access.
+            Files written to this directory are temporary and there is no
+            guarantee that a file created during a local data job execution will
+            be present in a subsequent local execution. Therefore precautions
+            must be taken when developing locally since temporary files created
+            might not have been deleted by the OS. Files created during
+            cloud executions are deleted when the data job completes. Users can
+            assume that the temp directory is empty on subsequent cloud
+            executions. Default returned folder (non cloud executions) is
+            tempfile.gettempdir() therefore the default temporary directory is
+            managed by the underlying OS.
+        """
+        pass
```

### Comparing `vdk-core-0.3.765384785/src/vdk/api/plugin/connection_hook_spec.py` & `vdk-core-0.3.893910391/src/vdk/api/plugin/connection_hook_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import Container
 from typing import Optional
 
 from vdk.api.plugin.hook_markers import hookspec
 from vdk.internal.builtin_plugins.connection.decoration_cursor import DecorationCursor
 from vdk.internal.builtin_plugins.connection.execution_cursor import (
```

### Comparing `vdk-core-0.3.765384785/src/vdk/api/plugin/core_hook_spec.py` & `vdk-core-0.3.893910391/src/vdk/api/plugin/core_hook_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import List
 from typing import Optional
 
 import click
 from vdk.api.plugin.hook_markers import hookspec
 from vdk.api.plugin.plugin_registry import IPluginRegistry
```

### Comparing `vdk-core-0.3.765384785/src/vdk/api/plugin/hook_markers.py` & `vdk-core-0.3.893910391/src/vdk/api/plugin/hook_markers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pluggy
 
 """
 The plugin project name. It is used in auto-discovery of the hooks and plugins.
 If external module needs to recognize as a plugin module they need to specify this as an entry point.
 """
```

### Comparing `vdk-core-0.3.765384785/src/vdk/api/plugin/plugin_input.py` & `vdk-core-0.3.893910391/src/vdk/api/plugin/plugin_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 from abc import ABC
 from abc import ABCMeta
 from abc import abstractmethod
 from typing import Any
 from typing import Callable
```

### Comparing `vdk-core-0.3.765384785/src/vdk/api/plugin/plugin_registry.py` & `vdk-core-0.3.893910391/src/vdk/api/plugin/plugin_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from abc import ABCMeta
 from abc import abstractmethod
 from typing import List
 from typing import Tuple
 
 import pluggy
```

### Comparing `vdk-core-0.3.765384785/src/vdk/api/plugin/plugin_utils.py` & `vdk-core-0.3.893910391/src/vdk/api/plugin/plugin_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Dict
 
 import click
 from vdk.internal.core import errors
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/builtin_hook_impl.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/builtin_hook_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import time
 import uuid
 from datetime import datetime
 from typing import List
 
@@ -93,14 +93,18 @@
         )
         context.state.set(CommonStoreKeys.OP_ID, op_id)
         context.state.set(CommonStoreKeys.EXECUTION_ID, execution_id)
         context.state.set(CommonStoreKeys.ATTEMPT_ID, attempt_id)
 
         context.state.set(CommonStoreKeys.VDK_VERSION, vdk_build_info.RELEASE_VERSION)
         context.state.set(CommonStoreKeys.START_TIME, datetime.utcnow())
+        context.state.set(
+            CommonStoreKeys.TEMPORARY_WRITE_DIRECTORY,
+            context.configuration.get_value(vdk_config.TEMPORARY_WRITE_DIRECTORY),
+        )
 
 
 @hookimpl
 def vdk_start(plugin_registry: PluginRegistry, command_line_args: List) -> None:
     """
     Load all default (builtin) vdk plugins
     """
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/config/config_help.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/config/config_help.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import re
 from collections import OrderedDict
 from textwrap import wrap
 from typing import cast
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/config/job_config.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/config/job_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import configparser
 import pathlib
 from enum import Enum
 from typing import Any
 from typing import Dict
 from typing import List
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/config/log_config.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/config/log_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import re
 import socket
 import types
 from sys import modules
 from typing import cast
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/config/vdk_config.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/config/vdk_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import os
 import pathlib
+import tempfile
 from os import getenv
 from typing import Optional
 
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.internal.builtin_plugins.config.job_config import JobConfig
 from vdk.internal.builtin_plugins.config.job_config import JobConfigKeys
 from vdk.internal.core.config import ConfigurationBuilder
@@ -19,14 +20,15 @@
 LOG_CONFIG = "LOG_CONFIG"
 LOG_LEVEL_VDK = "LOG_LEVEL_VDK"
 LOG_LEVEL_MODULE = "LOG_LEVEL_MODULE"
 WORKING_DIR = "WORKING_DIR"
 ATTEMPT_ID = "ATTEMPT_ID"
 EXECUTION_ID = "EXECUTION_ID"
 OP_ID = "OP_ID"
+TEMPORARY_WRITE_DIRECTORY = "TEMPORARY_WRITE_DIRECTORY"
 
 log = logging.getLogger(__name__)
 
 
 class CoreConfigDefinitionPlugin:
     """
     Define the core configuration.
@@ -109,14 +111,27 @@
             True,
             "An identifier to be associated with the current VDK execution attempt."
             "If left empty it will be auto-generated. "
             "An instance of a running Data Job deployment is called an execution. "
             "Data Job execution can run a Data Job one or more times."
             "Each distinct run would a single attempt.",
         )
+        config_builder.add(
+            TEMPORARY_WRITE_DIRECTORY,
+            tempfile.gettempdir(),
+            True,
+            "Temporary data job write directory, to be used if job needs to"
+            " write temporary files to local storage during job execution"
+            " (since writing to any directory might be restricted on a"
+            " deployment basis). Default value is tempfile.gettempdir()."
+            " Deletion of temporary files in the default directory is managed"
+            " by the underlying OS the data job executes on. There is"
+            " no guarantee that files created during a local data job execution"
+            " will  be present or absent for the next execution.",
+        )
 
 
 class EnvironmentVarsConfigPlugin:
     """
     Configuration loaded from environment variables.
     """
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/connection_hooks.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/connection_hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import Any
 from typing import cast
 
 from vdk.api.plugin.connection_hook_spec import ConnectionHookSpec
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.api.plugin.plugin_registry import IPluginRegistry
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/connection_plugin.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/connection_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.internal.builtin_plugins.connection.decoration_cursor import DecorationCursor
 from vdk.internal.builtin_plugins.connection.decoration_cursor import ManagedOperation
 from vdk.internal.builtin_plugins.connection.recovery_cursor import RecoveryCursor
 from vdk.internal.builtin_plugins.run.job_context import JobContext
 from vdk.internal.core.context import CoreContext
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/decoration_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import Container
 from typing import Optional
 from typing import Tuple
 
 from vdk.internal.builtin_plugins.connection.pep249.interfaces import PEP249Cursor
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/execution_cursor.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/execution_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Any
 
 from vdk.internal.builtin_plugins.connection.decoration_cursor import ManagedOperation
 from vdk.internal.builtin_plugins.connection.pep249.interfaces import PEP249Cursor
 from vdk.internal.builtin_plugins.connection.proxy_cursor import ProxyCursor
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/impl/router.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/impl/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Callable
 from typing import Dict
 from typing import Union
 
 from vdk.api.plugin.plugin_input import IManagedConnectionRegistry
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/impl/wrapped_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Any
 from typing import Callable
 
 from vdk.internal.builtin_plugins.connection.connection_hooks import (
     ConnectionHookSpecFactory,
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/managed_connection_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import types
 from abc import abstractmethod
 from types import TracebackType
 from typing import Any
 from typing import cast
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/managed_cursor.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/managed_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import types
 from datetime import timedelta
 from timeit import default_timer as timer
 from typing import Any
 from typing import cast
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/pep249/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 
 
 class PEP249Connection:
     """
     Interface and protocol for PEP 249 compatible connection
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/proxy_cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import types
 from typing import Any
 
 from vdk.internal.builtin_plugins.connection.pep249.interfaces import PEP249Cursor
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/connection/recovery_cursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from vdk.internal.builtin_plugins.connection.decoration_cursor import DecorationCursor
 from vdk.internal.builtin_plugins.connection.decoration_cursor import ManagedOperation
 from vdk.internal.builtin_plugins.connection.pep249.interfaces import PEP249Cursor
 
 
 class RecoveryCursor(PEP249Cursor):
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/debug/debug.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/debug/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import os
 import sys
 from dataclasses import dataclass
 from typing import Any
 from typing import cast
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/ingester_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import logging
 import queue
 import sys
 import threading
 from collections import defaultdict
@@ -556,15 +556,14 @@
         self.close_now()
 
     def close_now(self):
         """
         Close immediately. The method will not wait for the active queue items to get processed.
         """
         if self._closed.get_and_increment() == 0:
-
             if self._exception_on_failure:
                 self.__handle_results()
 
             log.info(
                 "Ingester statistics: \n\t\t"
                 f"Successful uploads: {self._success_count}\n\t\t"
                 f"Failed uploads: {self._fail_count}\n\t\t"
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from vdk.internal.core.config import Configuration
 from vdk.internal.core.config import ConfigurationBuilder
 
 INGESTER_NUMBER_OF_WORKER_THREADS = "INGESTER_NUMBER_OF_WORKER_THREADS"
 INGESTER_PAYLOAD_SIZE_BYTES_THRESHOLD = "INGESTER_PAYLOAD_SIZE_BYTES_THRESHOLD"
 INGESTER_OBJECTS_QUEUE_SIZE = "INGESTER_OBJECTS_QUEUE_SIZE"
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/ingester_configuration_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.internal.builtin_plugins.ingestion import ingester_configuration
 from vdk.internal.builtin_plugins.run.job_context import JobContext
 from vdk.internal.core.config import ConfigurationBuilder
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/ingester_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/ingestion/ingester_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 Ingestion Utilities
 """
 import datetime
 import itertools
 import logging
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/internal_hookspecs.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/internal_hookspecs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import List
 
 import click
 from vdk.api.plugin.hook_markers import hookspec
 from vdk.api.plugin.plugin_registry import IPluginRegistry
 from vdk.internal.core.context import CoreContext
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/base_properties_impl.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import List
 from typing import Type
 
 
 def check_valid_property(k: str, v: str, supported_types: List[Type] = []) -> None:
     """
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/cached_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from vdk.api.job_input import IProperties
 
 
 class CachedPropertiesWrapper(IProperties):
     """
     Wraps any IProperties so that get_* calls are cached until set_* is called
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/datajobs_service_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from copy import deepcopy
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
@@ -88,15 +88,15 @@
                         what_happened=f"A write pre-processor of properties client {client} had failed.",
                         why_it_happened=f"User Error occurred. Exception was: {e}",
                         consequences="PROPERTIES_WRITE_PREPROCESS_SEQUENCE was interrupted, and "
                         "properties won't be written by the PROPERTIES_DEFAULT_TYPE client.",
                         countermeasures=f"Handle the exception raised.",
                     )
 
-        for (k, v) in list(properties.items()):
+        for k, v in list(properties.items()):
             check_valid_property(
                 k, v, DataJobsServiceProperties.__VALID_TYPES
             )  # throws
 
         self._properties_service_client.write_properties(
             self._job_name, self._team_name, properties
         )
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/inmemproperties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from copy import deepcopy
 from typing import Dict
 
 from vdk.api.plugin.plugin_input import IPropertiesServiceClient
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/properties_api_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.internal.builtin_plugins.job_properties import properties_config
 from vdk.internal.builtin_plugins.job_properties.inmemproperties import (
     InMemPropertiesServiceClient,
 )
 from vdk.internal.builtin_plugins.run.job_context import JobContext
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/properties_config.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/properties_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import List
 
 from vdk.internal.core.config import Configuration
 from vdk.internal.core.config import ConfigurationBuilder
 from vdk.internal.util.utils import parse_config_sequence
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/properties_router.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/properties_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Any
 
 from vdk.api.job_input import IProperties
 from vdk.api.plugin.plugin_input import IPropertiesFactory
 from vdk.api.plugin.plugin_input import IPropertiesRegistry
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/job_properties/propertiesnotavailable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import Callable
 
 from vdk.api.job_input import IProperties
 
 
 class PropertiesNotAvailable(IProperties):
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/notification/notification.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/notification/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import List
 
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.internal.builtin_plugins.config.job_config import JobConfigKeys
 from vdk.internal.builtin_plugins.config.vdk_config import LOG_CONFIG
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/notification/notification_base.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/notification/notification_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import smtplib
 import time
 from abc import ABC
 from abc import abstractmethod
 from email.mime.text import MIMEText
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/notification/notification_configuration.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/notification/notification_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import List
 
 from vdk.internal.builtin_plugins.config.job_config import JobConfigKeys
 from vdk.internal.core.config import Configuration
 from vdk.internal.core.config import ConfigurationBuilder
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/cli_run.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/cli_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import logging
 import math
 import os
 import pathlib
 from typing import cast
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/data_job.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/data_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import logging
 import pathlib
 from dataclasses import dataclass
 from datetime import datetime
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/execution_environment.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/execution_environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import functools
 import getpass
 import logging
 import platform
 import socket
 import sys
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/execution_results.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/execution_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import logging
 import pprint
 import sys
 from dataclasses import dataclass
 from datetime import datetime
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/execution_state.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/execution_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from typing import List
 from typing import Optional
 
 from vdk.internal.builtin_plugins.run.execution_results import ExecutionResult
 from vdk.internal.core.statestore import StoreKey
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/execution_tracking.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/execution_tracking.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pluggy
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.api.plugin.plugin_registry import HookCallResult
 from vdk.internal.builtin_plugins.config import vdk_config
 from vdk.internal.builtin_plugins.run.execution_results import ExecutionResult
 from vdk.internal.builtin_plugins.run.execution_results import StepResult
@@ -15,15 +15,14 @@
 class ExecutionTrackingPlugin:
     """
     We are going to track data job executions in this plugin and update the statestore of the execution.
     """
 
     @hookimpl
     def initialize_job(self, context: JobContext):
-
         state = context.core_context.state
         configuration = context.core_context.configuration
 
         state.set(ExecutionStateStoreKeys.JOB_NAME, context.name)
         state.set(
             ExecutionStateStoreKeys.JOB_GIT_HASH,
             configuration.get_value(vdk_config.JOB_GITHASH),
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/file_based_step.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/file_based_step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import imp
 import inspect
 import logging
 import pathlib
 import sys
 from typing import Callable
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/job_context.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/job_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import pathlib
 from dataclasses import dataclass
 from typing import cast
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/job_input.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/job_input.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import pathlib
 import textwrap
 from typing import List
 from typing import Optional
 
@@ -182,7 +182,11 @@
             ),
             countermeasures=(
                 "Revise job/template code and determine need for skipping. "
                 + "If cancellation behaviour no longer desired, refactor the job/template code."
             ),
         )
         raise SkipRemainingStepsException(error_message)
+
+    def get_temporary_write_directory(self) -> pathlib.Path:
+        path_string = self.__statestore.get(CommonStoreKeys.TEMPORARY_WRITE_DIRECTORY)
+        return pathlib.Path(path_string)
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/job_input_error_classifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """This module contains the logic that
 decides who is to blame, between Platform (SRE) Team and VDK Users,
 when an exception occurs while executing a Data Job step.
 """
 import logging
 import os
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/sql_argument_substitutor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 from typing import Dict
 
 log = logging.getLogger(__name__)
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/standalone_data_job.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/standalone_data_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import logging
 import pathlib
 import sys
 from pathlib import Path
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/run/step.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/run/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import logging
 import pathlib
 from abc import ABC
 from dataclasses import dataclass
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/templates/template_impl.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/templates/template_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import pathlib
 from typing import Dict
 from typing import Optional
 
 from vdk.api.job_input import ITemplate
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/termination_message/file_util.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/termination_message/file_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 
 log = logging.getLogger(__name__)
 
 
 class WriteToFileAction:
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/termination_message/writer.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/termination_message/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import json
 import logging
 
 from vdk.api.plugin.hook_markers import hookimpl
 from vdk.internal.builtin_plugins.config.vdk_config import LOG_CONFIG
 from vdk.internal.builtin_plugins.termination_message import (
@@ -71,15 +71,14 @@
         except Exception as e:
             log.exception(f"Failed to write termination message. See exception: {e}")
 
     @staticmethod
     def _execute_termination_action(
         file_util, error_overall, user_error, execution_skipped
     ):
-
         termination_message = {"vdk_version": get_version()}
 
         if execution_skipped:
             status = "Skipped"
         elif not error_overall:
             status = "Success"
         elif user_error:
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/termination_message/writer_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from vdk.internal.core.config import Configuration
 from vdk.internal.core.config import ConfigurationBuilder
 
 TERMINATION_MESSAGE_WRITER_ENABLED = "TERMINATION_MESSAGE_WRITER_ENABLED"
 TERMINATION_MESSAGE_WRITER_OUTPUT_FILE = "TERMINATION_MESSAGE_WRITER_OUTPUT_FILE"
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/version/new_version_check.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/version/new_version_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 The code is adapted from: https://github.com/vuolter/autoupgrade
 """
 import http.client
 import logging
 import re
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/version/new_version_check_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import textwrap
 from enum import Enum
 from typing import List
 
 import click
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/builtin_plugins/version/version.py` & `vdk-core-0.3.893910391/src/vdk/internal/builtin_plugins/version/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import os
 
 import click
 from pkg_resources import DistributionNotFound
 from pkg_resources import get_distribution
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/cli_entry.py` & `vdk-core-0.3.893910391/src/vdk/internal/cli_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import sys
 from typing import cast
 from typing import List
 
 import click
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/core/config.py` & `vdk-core-0.3.893910391/src/vdk/internal/core/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 import logging
 from collections import OrderedDict
 from dataclasses import dataclass
 from dataclasses import field
@@ -22,15 +22,15 @@
 ) -> ConfigValue:
     """
     Allows for configurations to be converted to the type of their default value.
 
     E.g. IMPALA_PORT is converted to int, because it's default value is int.
     """
     if default_value is not None:
-        if type(default_value) == type(True) and type(v) != type(True):
+        if type(default_value) == bool and type(v) != bool:
             allowed_values = ["true", "false", "1", "0", "yes", "no", "y", "n"]
             if str(v).lower() not in allowed_values:
                 msg = (
                     f"Provided configuration "
                     f'"{key}={v}" is invalid. Allowed values for {key} are {allowed_values}'
                 )
                 raise VdkConfigurationError(msg)
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/core/context.py` & `vdk-core-0.3.893910391/src/vdk/internal/core/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from dataclasses import dataclass
 from typing import List
 
 from vdk.api.plugin.plugin_registry import IPluginRegistry
 from vdk.internal.core.config import Configuration
 from vdk.internal.core.statestore import ImmutableStoreKey
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/core/errors.py` & `vdk-core-0.3.893910391/src/vdk/internal/core/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 errors -- Exception handling implementations
 
 errors is a module that handles all errors.
 It defines classes and methods for handling exceptions, and ensuring that there are two types of exceptions:
  - infrastructure-related: should be handled by Platform team.
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/core/statestore.py` & `vdk-core-0.3.893910391/src/vdk/internal/core/statestore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 from __future__ import annotations
 
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any
 from typing import cast
@@ -65,14 +65,23 @@
     END_TIME: StoreKey[datetime] = StoreKey[datetime]("vdk.end_time")
 
     """
     Build information about the CLI:
     """
     VDK_VERSION: StoreKey[str] = ImmutableStoreKey[str]("vdk.vdk_version")
 
+    """
+    Write data job directory, to be used if job needs to write files to local
+    storage during cloud execution (since writing to any directory might be
+    restricted on a deployment basis:
+    """
+    TEMPORARY_WRITE_DIRECTORY: StoreKey[str] = ImmutableStoreKey[str](
+        "vdk.temporary_write_directory"
+    )
+
 
 class StateStore:
     """
     StateStore is a type-safe heterogeneous mapping that allows keys and value types to be defined to keep state of app.
 
     It is meant to keeps state of the current CLI execution.
     Contains data like opId, executionID, start time, end time, steps executed, etc.
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/plugin/plugin.py` & `vdk-core-0.3.893910391/src/vdk/internal/plugin/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import logging
 import os
 from typing import List
 from typing import Tuple
 
 from vdk.api.plugin import hook_markers
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/util/decorators.py` & `vdk-core-0.3.893910391/src/vdk/internal/util/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import functools
 import logging
 from contextlib import contextmanager
 from typing import TypeVar
 
 log = logging.getLogger(__name__)
```

### Comparing `vdk-core-0.3.765384785/src/vdk/internal/util/utils.py` & `vdk-core-0.3.893910391/src/vdk/internal/util/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021 VMware, Inc.
+# Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import inspect
 from logging import Logger
 from typing import Any
 from typing import List
 from typing import Optional
```

### Comparing `vdk-core-0.3.765384785/src/vdk_core.egg-info/PKG-INFO` & `vdk-core-0.3.893910391/src/vdk_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-core
-Version: 0.3.765384785
+Version: 0.3.893910391
 Summary: Versatile Data Kit SDK Core
 Home-page: https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Author: VMware Inc.
 Author-email: taurus@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/projects/vdk-core/README.md
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-core
 Platform: any
```

### Comparing `vdk-core-0.3.765384785/src/vdk_core.egg-info/SOURCES.txt` & `vdk-core-0.3.893910391/src/vdk_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

