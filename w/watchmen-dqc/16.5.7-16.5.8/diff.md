# Comparing `tmp/watchmen_dqc-16.5.7.tar.gz` & `tmp/watchmen_dqc-16.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_dqc-16.5.7.tar", max compression
+gzip compressed data, was "watchmen_dqc-16.5.8.tar", max compression
```

## Comparing `watchmen_dqc-16.5.7.tar` & `watchmen_dqc-16.5.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1061 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/LICENSE
--rw-r--r--   0        0        0     1097 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/__init__.py
--rw-r--r--   0        0        0       36 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/boot/__init__.py
--rw-r--r--   0        0        0      129 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/boot/boot.py
--rw-r--r--   0        0        0      257 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/common/__init__.py
--rw-r--r--   0        0        0       37 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/common/exception.py
--rw-r--r--   0        0        0     1517 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/common/settings.py
--rw-r--r--   0        0        0      140 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/__init__.py
--rw-r--r--   0        0        0     5070 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/monitor_data_service.py
--rw-r--r--   0        0        0      293 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/__init__.py
--rw-r--r--   0        0        0     3538 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/data_service_utils.py
--rw-r--r--   0        0        0     1346 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/date_range.py
--rw-r--r--   0        0        0      460 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/disabled_rules.py
--rw-r--r--   0        0        0      797 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/enum_service.py
--rw-r--r--   0        0        0     1325 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_aggregate_value_not_in_range.py
--rw-r--r--   0        0        0     1173 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_and_another.py
--rw-r--r--   0        0        0      675 2023-06-07 11:34:15.611986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_avg_not_in_range.py
--rw-r--r--   0        0        0     1104 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_common_value_not_in_range.py
--rw-r--r--   0        0        0     1063 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_common_value_over_coverage.py
--rw-r--r--   0        0        0     1034 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_empty_over_coverage.py
--rw-r--r--   0        0        0      809 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_is_blank.py
--rw-r--r--   0        0        0      809 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_is_empty.py
--rw-r--r--   0        0        0      697 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_match_regexp.py
--rw-r--r--   0        0        0      675 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_max_not_in_range.py
--rw-r--r--   0        0        0      935 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_median_not_in_range.py
--rw-r--r--   0        0        0      675 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_min_not_in_range.py
--rw-r--r--   0        0        0     1052 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_mismatch_enum.py
--rw-r--r--   0        0        0      701 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_mismatch_regexp.py
--rw-r--r--   0        0        0     6291 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_mismatch_type.py
--rw-r--r--   0        0        0     1345 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_not_in_range.py
--rw-r--r--   0        0        0      945 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_quantile_not_in_range.py
--rw-r--r--   0        0        0      951 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_stdev_not_in_range.py
--rw-r--r--   0        0        0     1152 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_string_length_mismatch.py
--rw-r--r--   0        0        0     1587 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_string_length_not_in_range.py
--rw-r--r--   0        0        0     1237 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_use_regexp.py
--rw-r--r--   0        0        0      855 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_value_assert.py
--rw-r--r--   0        0        0     2923 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/retrieve_all_data_rules.py
--rw-r--r--   0        0        0     1448 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/retrieve_data_rules_utils.py
--rw-r--r--   0        0        0     3443 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/retrieve_distinct_data_rules.py
--rw-r--r--   0        0        0     1758 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/rows_count_mismatch_with_another.py
--rw-r--r--   0        0        0      609 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/rows_no_change.py
--rw-r--r--   0        0        0      571 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/rows_not_exists.py
--rw-r--r--   0        0        0     4498 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/rules_controller.py
--rw-r--r--   0        0        0     2828 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/trigger_pipeline.py
--rw-r--r--   0        0        0      789 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/types.py
--rw-r--r--   0        0        0      361 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/value_range.py
--rw-r--r--   0        0        0    10093 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rules_runner.py
--rw-r--r--   0        0        0       55 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/topic_profile/__init__.py
--rw-r--r--   0        0        0     4044 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/topic_profile/topic_profile_service.py
--rw-r--r--   0        0        0      136 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/util/__init__.py
--rw-r--r--   0        0        0     2482 2023-06-07 11:34:15.615986 watchmen_dqc-16.5.7/src/watchmen_dqc/util/data_frame.py
--rw-r--r--   0        0        0     1180 1970-01-01 00:00:00.000000 watchmen_dqc-16.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/LICENSE
+-rw-r--r--   0        0        0     1097 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/__init__.py
+-rw-r--r--   0        0        0       36 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/boot/__init__.py
+-rw-r--r--   0        0        0      129 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/boot/boot.py
+-rw-r--r--   0        0        0      257 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/common/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/common/exception.py
+-rw-r--r--   0        0        0     1517 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/common/settings.py
+-rw-r--r--   0        0        0      140 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/__init__.py
+-rw-r--r--   0        0        0     5070 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/monitor_data_service.py
+-rw-r--r--   0        0        0      293 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/__init__.py
+-rw-r--r--   0        0        0     3538 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/data_service_utils.py
+-rw-r--r--   0        0        0     1346 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/date_range.py
+-rw-r--r--   0        0        0      460 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/disabled_rules.py
+-rw-r--r--   0        0        0      797 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/enum_service.py
+-rw-r--r--   0        0        0     1325 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_aggregate_value_not_in_range.py
+-rw-r--r--   0        0        0     1173 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_and_another.py
+-rw-r--r--   0        0        0      675 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_avg_not_in_range.py
+-rw-r--r--   0        0        0     1104 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_common_value_not_in_range.py
+-rw-r--r--   0        0        0     1063 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_common_value_over_coverage.py
+-rw-r--r--   0        0        0     1034 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_empty_over_coverage.py
+-rw-r--r--   0        0        0      809 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_is_blank.py
+-rw-r--r--   0        0        0      809 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_is_empty.py
+-rw-r--r--   0        0        0      697 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_match_regexp.py
+-rw-r--r--   0        0        0      675 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_max_not_in_range.py
+-rw-r--r--   0        0        0      935 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_median_not_in_range.py
+-rw-r--r--   0        0        0      675 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_min_not_in_range.py
+-rw-r--r--   0        0        0     1052 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_mismatch_enum.py
+-rw-r--r--   0        0        0      701 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_mismatch_regexp.py
+-rw-r--r--   0        0        0     6291 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_mismatch_type.py
+-rw-r--r--   0        0        0     1345 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_not_in_range.py
+-rw-r--r--   0        0        0      945 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_quantile_not_in_range.py
+-rw-r--r--   0        0        0      951 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_stdev_not_in_range.py
+-rw-r--r--   0        0        0     1152 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_string_length_mismatch.py
+-rw-r--r--   0        0        0     1587 2023-06-08 03:33:39.191630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_string_length_not_in_range.py
+-rw-r--r--   0        0        0     1237 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_use_regexp.py
+-rw-r--r--   0        0        0      855 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_value_assert.py
+-rw-r--r--   0        0        0     2923 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/retrieve_all_data_rules.py
+-rw-r--r--   0        0        0     1448 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/retrieve_data_rules_utils.py
+-rw-r--r--   0        0        0     3443 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/retrieve_distinct_data_rules.py
+-rw-r--r--   0        0        0     1758 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/rows_count_mismatch_with_another.py
+-rw-r--r--   0        0        0      609 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/rows_no_change.py
+-rw-r--r--   0        0        0      571 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/rows_not_exists.py
+-rw-r--r--   0        0        0     4498 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/rules_controller.py
+-rw-r--r--   0        0        0     2828 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/trigger_pipeline.py
+-rw-r--r--   0        0        0      789 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/types.py
+-rw-r--r--   0        0        0      361 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/value_range.py
+-rw-r--r--   0        0        0    10093 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rules_runner.py
+-rw-r--r--   0        0        0       55 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/topic_profile/__init__.py
+-rw-r--r--   0        0        0     4044 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/topic_profile/topic_profile_service.py
+-rw-r--r--   0        0        0      136 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/util/__init__.py
+-rw-r--r--   0        0        0     2482 2023-06-08 03:33:39.195630 watchmen_dqc-16.5.8/src/watchmen_dqc/util/data_frame.py
+-rw-r--r--   0        0        0     1180 1970-01-01 00:00:00.000000 watchmen_dqc-16.5.8/PKG-INFO
```

### Comparing `watchmen_dqc-16.5.7/LICENSE` & `watchmen_dqc-16.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/pyproject.toml` & `watchmen_dqc-16.5.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "watchmen-dqc"
-version = "16.5.7"
+version = "16.5.8"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_dqc", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "~1.4.2"
 pandas-profiling = "^3.1.0"
 APScheduler = "^3.9.1"
-watchmen-meta = "16.5.7"
-watchmen-data-kernel = "16.5.7"
-watchmen-pipeline-kernel = "16.5.7"
-watchmen-storage-mysql = { version = "16.5.7", optional = true }
-watchmen-storage-oracle = { version = "16.5.7", optional = true }
-watchmen-storage-mongodb = { version = "16.5.7", optional = true }
-watchmen-storage-mssql = { version = "16.5.7", optional = true }
-watchmen-storage-postgresql = { version = "16.5.7", optional = true }
+watchmen-meta = "16.5.8"
+watchmen-data-kernel = "16.5.8"
+watchmen-pipeline-kernel = "16.5.8"
+watchmen-storage-mysql = { version = "16.5.8", optional = true }
+watchmen-storage-oracle = { version = "16.5.8", optional = true }
+watchmen-storage-mongodb = { version = "16.5.8", optional = true }
+watchmen-storage-mssql = { version = "16.5.8", optional = true }
+watchmen-storage-postgresql = { version = "16.5.8", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/common/settings.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/monitor_data_service.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/monitor_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/data_service_utils.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/data_service_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/date_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/date_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/enum_service.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/enum_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_aggregate_value_not_in_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_aggregate_value_not_in_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_and_another.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_and_another.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_avg_not_in_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_avg_not_in_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_common_value_not_in_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_common_value_not_in_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_common_value_over_coverage.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_common_value_over_coverage.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_empty_over_coverage.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_empty_over_coverage.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_is_blank.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_is_blank.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_is_empty.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_is_empty.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_match_regexp.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_match_regexp.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_max_not_in_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_max_not_in_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_median_not_in_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_median_not_in_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_min_not_in_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_min_not_in_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_mismatch_enum.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_mismatch_enum.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_mismatch_regexp.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_mismatch_regexp.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_mismatch_type.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_mismatch_type.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_not_in_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_not_in_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_quantile_not_in_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_quantile_not_in_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_stdev_not_in_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_stdev_not_in_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_string_length_mismatch.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_string_length_mismatch.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_string_length_not_in_range.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_string_length_not_in_range.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_use_regexp.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_use_regexp.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/factor_value_assert.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/factor_value_assert.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/retrieve_all_data_rules.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/retrieve_all_data_rules.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/retrieve_data_rules_utils.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/retrieve_data_rules_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/retrieve_distinct_data_rules.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/retrieve_distinct_data_rules.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/rows_count_mismatch_with_another.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/rows_count_mismatch_with_another.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/rows_no_change.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/rows_no_change.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/rows_not_exists.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/rows_not_exists.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/rules_controller.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/rules_controller.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/trigger_pipeline.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/trigger_pipeline.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rule/types.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rule/types.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/monitor/rules_runner.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/monitor/rules_runner.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/topic_profile/topic_profile_service.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/topic_profile/topic_profile_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/src/watchmen_dqc/util/data_frame.py` & `watchmen_dqc-16.5.8/src/watchmen_dqc/util/data_frame.py`

 * *Files identical despite different names*

### Comparing `watchmen_dqc-16.5.7/PKG-INFO` & `watchmen_dqc-16.5.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-dqc
-Version: 16.5.7
+Version: 16.5.8
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: postgresql
 Requires-Dist: APScheduler (>=3.9.1,<4.0.0)
 Requires-Dist: pandas (>=1.4.2,<1.5.0)
 Requires-Dist: pandas-profiling (>=3.1.0,<4.0.0)
-Requires-Dist: watchmen-data-kernel (==16.5.7)
-Requires-Dist: watchmen-meta (==16.5.7)
-Requires-Dist: watchmen-pipeline-kernel (==16.5.7)
-Requires-Dist: watchmen-storage-mongodb (==16.5.7) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.7) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.7) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.7) ; extra == "oracle"
-Requires-Dist: watchmen-storage-postgresql (==16.5.7) ; extra == "postgresql"
+Requires-Dist: watchmen-data-kernel (==16.5.8)
+Requires-Dist: watchmen-meta (==16.5.8)
+Requires-Dist: watchmen-pipeline-kernel (==16.5.8)
+Requires-Dist: watchmen-storage-mongodb (==16.5.8) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.8) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.8) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.8) ; extra == "oracle"
+Requires-Dist: watchmen-storage-postgresql (==16.5.8) ; extra == "postgresql"
```

