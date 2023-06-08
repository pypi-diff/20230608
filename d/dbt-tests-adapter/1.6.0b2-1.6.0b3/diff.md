# Comparing `tmp/dbt-tests-adapter-1.6.0b2.tar.gz` & `tmp/dbt-tests-adapter-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-tests-adapter-1.6.0b2.tar", last modified: Thu May 25 15:44:09 2023, max compression
+gzip compressed data, was "dbt-tests-adapter-1.6.0b3.tar", last modified: Thu Jun  8 20:55:15 2023, max compression
```

## Comparing `dbt-tests-adapter-1.6.0b2.tar` & `dbt-tests-adapter-1.6.0b3.tar`

### file list

```diff
@@ -1,157 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.080701 dbt-tests-adapter-1.6.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-25 15:44:09.080701 dbt-tests-adapter-1.6.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.060700 dbt-tests-adapter-1.6.0b2/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.060700 dbt-tests-adapter-1.6.0b2/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.064700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.064700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/aliases/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/aliases/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/aliases/test_aliases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.064700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/expected_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_adapter_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_docs_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_incremental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_singular_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_snapshot_check_cols.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_snapshot_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_table_materialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_validate_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.064700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/caching/
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/caching/test_caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.064700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/column_types/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/column_types/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/column_types/test_column_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.064700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/concurrency/
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/concurrency/test_concurrency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/constraints/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/constraints/test_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/dbt_debug/
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/ephemeral/
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/ephemeral/test_ephemeral.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/base_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/test_incremental_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/test_invalid_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/test_model_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/test_seed_grants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/test_snapshot_grants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/hooks/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/hooks/test_model_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/hooks/test_run_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/test_incremental_predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    17492 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/test_incremental_unique_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/persist_docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/persist_docs/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/persist_docs/test_persist_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/python_model/test_python_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/python_model/test_spark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/query_comment/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/query_comment/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/query_comment/test_query_comment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/relations/
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/relations/test_changing_relation_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.068700 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_copy/
--rw-r--r--   0 runner    (1001) docker     (123)    19865 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_copy/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_copy/test_simple_copy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.072701 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_seed/
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_seed/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    78093 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_seed/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_seed/test_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_seed/test_seed_type_override.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.072701 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_snapshot/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_snapshot/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_snapshot/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_snapshot/test_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.072701 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/store_test_failures_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/store_test_failures_tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.076701 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/base_array_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/base_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.080701 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_bigint.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_int.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_any_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_array_append.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_array_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_array_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_bool_or.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_date_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_dateadd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_datediff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_except.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_last_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_length.py
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_listagg.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_null_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_right.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_safe_cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_split_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_any_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_array_append.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_array_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_array_construct.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_bool_or.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_cast_bool_to_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_current_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_date_trunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_dateadd.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_datediff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_escape_single_quotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_except.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_intersect.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_last_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_listagg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_null_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_right.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_safe_cast.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_split_part.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_string_literal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_timestamps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 15:44:09.080701 dbt-tests-adapter-1.6.0b2/dbt_tests_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-25 15:44:09.000000 dbt-tests-adapter-1.6.0b2/dbt_tests_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-25 15:44:09.000000 dbt-tests-adapter-1.6.0b2/dbt_tests_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:44:09.000000 dbt-tests-adapter-1.6.0b2/dbt_tests_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 15:44:09.000000 dbt-tests-adapter-1.6.0b2/dbt_tests_adapter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-25 15:44:09.000000 dbt-tests-adapter-1.6.0b2/dbt_tests_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 15:44:09.000000 dbt-tests-adapter-1.6.0b2/dbt_tests_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 15:44:09.080701 dbt-tests-adapter-1.6.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-25 15:43:54.000000 dbt-tests-adapter-1.6.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.285822 dbt-tests-adapter-1.6.0b3/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.285822 dbt-tests-adapter-1.6.0b3/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/aliases/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/aliases/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/aliases/test_aliases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/expected_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_adapter_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_docs_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_singular_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_snapshot_check_cols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_snapshot_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_table_materialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_validate_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/caching/
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/caching/test_caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/column_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/column_types/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/column_types/test_column_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.289821 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/concurrency/test_concurrency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/constraints/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/constraints/test_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/dbt_debug/
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/dbt_debug/test_dbt_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/ephemeral/
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/ephemeral/test_ephemeral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/base_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_incremental_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_invalid_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_model_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_seed_grants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_snapshot_grants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/test_model_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/test_run_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17492 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_unique_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/materialized_view/
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/materialized_view/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/materialized_view/on_configuration_change.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/persist_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/persist_docs/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/persist_docs/test_persist_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/python_model/test_python_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/python_model/test_spark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/query_comment/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/query_comment/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/query_comment/test_query_comment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.293822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/relations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/relations/test_changing_relation_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.297822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/
+-rw-r--r--   0 runner    (1001) docker     (123)    19865 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/test_copy_uppercase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/test_simple_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.297822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78093 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/test_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/test_seed_type_override.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.297822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8638 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/test_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.297822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/store_test_failures_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/store_test_failures_tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/base_array_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/base_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/base_data_type_macro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_int.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_any_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_array_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_array_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_array_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_bool_or.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_date_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_dateadd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_datediff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_equals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_escape_single_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_except.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_last_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_listagg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_null_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_safe_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_split_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_any_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_append.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_bool_or.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_cast_bool_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_concat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_current_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_date_trunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_dateadd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_datediff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_equals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_escape_single_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_except.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_intersect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_last_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_listagg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_null_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_right.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_safe_cast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_split_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_timestamps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 20:55:15.000000 dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:55:15.305822 dbt-tests-adapter-1.6.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-08 20:55:01.000000 dbt-tests-adapter-1.6.0b3/setup.py
```

### Comparing `dbt-tests-adapter-1.6.0b2/PKG-INFO` & `dbt-tests-adapter-1.6.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-tests-adapter
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: The dbt adapter tests for adapter plugins
 Home-page: https://github.com/dbt-labs/dbt-core/tree/main/tests/adapter
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt-core/fa1ea14ddfb1d5ae319d5141844910dd53ab2834/etc/dbt-core.svg" alt="dbt logo" width="750"/>
 </p>
 
 # dbt-tests-adapter
```

### Comparing `dbt-tests-adapter-1.6.0b2/README.md` & `dbt-tests-adapter-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/aliases/fixtures.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/aliases/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/aliases/test_aliases.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/aliases/test_aliases.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/expected_catalog.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/expected_catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/files.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/files.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_adapter_methods.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_adapter_methods.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_base.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_base.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_docs_generate.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_docs_generate.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_empty.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_empty.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_ephemeral.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_generic_tests.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_incremental.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_incremental.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_singular_tests.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_singular_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_singular_tests_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_snapshot_check_cols.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_snapshot_check_cols.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_snapshot_timestamp.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_snapshot_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/basic/test_table_materialization.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/basic/test_table_materialization.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/caching/test_caching.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/caching/test_caching.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/column_types/fixtures.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/column_types/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/column_types/test_column_types.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/column_types/test_column_types.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/concurrency/test_concurrency.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/concurrency/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/constraints/test_constraints.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/constraints/test_constraints.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,22 @@
     my_model_view_wrong_order_sql,
     my_model_view_wrong_name_sql,
     my_model_incremental_wrong_order_sql,
     my_model_incremental_wrong_name_sql,
     my_model_with_nulls_sql,
     my_model_incremental_with_nulls_sql,
     model_schema_yml,
+    model_fk_constraint_schema_yml,
     constrained_model_schema_yml,
+    foreign_key_model_sql,
+    my_model_wrong_order_depends_on_fk_sql,
+    my_model_incremental_wrong_order_depends_on_fk_sql,
+    my_model_contract_sql_header_sql,
+    my_model_incremental_contract_sql_header_sql,
+    model_contract_header_schema_yml,
 )
 
 
 class BaseConstraintsColumnsEqual:
     """
     dbt should catch these mismatches during its "preflight" checks.
     """
@@ -157,33 +164,41 @@
             assert contract_actual_config.enforced is True
 
 
 def _normalize_whitespace(input: str) -> str:
     return re.sub(r"\s+", " ", input).lower().strip()
 
 
+def _find_and_replace(sql, find, replace):
+    sql_tokens = sql.split(" ")
+    for idx in [n for n, x in enumerate(sql_tokens) if find in x]:
+        sql_tokens[idx] = replace
+    return " ".join(sql_tokens)
+
+
 class BaseConstraintsRuntimeDdlEnforcement:
     """
     These constraints pass muster for dbt's preflight checks. Make sure they're
     passed into the DDL statement. If they don't match up with the underlying data,
     the data platform should raise an error at runtime.
     """
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model.sql": my_model_wrong_order_sql,
-            "constraints_schema.yml": model_schema_yml,
+            "my_model.sql": my_model_wrong_order_depends_on_fk_sql,
+            "foreign_key_model.sql": foreign_key_model_sql,
+            "constraints_schema.yml": model_fk_constraint_schema_yml,
         }
 
     @pytest.fixture(scope="class")
     def expected_sql(self):
         return """
 create table <model_identifier> (
-    id integer not null primary key check (id > 0),
+    id integer not null primary key check ((id > 0)) check (id >= 1) references <foreign_key_model_identifier> (id) unique,
     color text,
     date_day text
 ) ;
 insert into <model_identifier> (
     id ,
     color ,
     date_day
@@ -191,35 +206,46 @@
 (
     select
        id,
        color,
        date_day
        from
     (
+        -- depends_on: <foreign_key_model_identifier>
         select
             'blue' as color,
             1 as id,
             '2019-01-01' as date_day
     ) as model_subq
 );
 """
 
     def test__constraints_ddl(self, project, expected_sql):
-        results = run_dbt(["run", "-s", "my_model"])
-        assert len(results) == 1
+        unformatted_constraint_schema_yml = read_file("models", "constraints_schema.yml")
+        write_file(
+            unformatted_constraint_schema_yml.format(schema=project.test_schema),
+            "models",
+            "constraints_schema.yml",
+        )
+
+        results = run_dbt(["run", "-s", "+my_model"])
+        # assert at least my_model was run - additional upstreams may or may not be provided to the test setup via models fixture
+        assert len(results) >= 1
 
         # grab the sql and replace the model identifier to make it generic for all adapters
         # the name is not what we're testing here anyways and varies based on materialization
         # TODO: consider refactoring this to introspect logs instead
         generated_sql = read_file("target", "run", "test", "models", "my_model.sql")
         generated_sql_modified = _normalize_whitespace(generated_sql)
-        generated_sql_list = generated_sql_modified.split(" ")
-        for idx in [n for n, x in enumerate(generated_sql_list) if "my_model" in x]:
-            generated_sql_list[idx] = "<model_identifier>"
-        generated_sql_generic = " ".join(generated_sql_list)
+        generated_sql_generic = _find_and_replace(
+            generated_sql_modified, "my_model", "<model_identifier>"
+        )
+        generated_sql_generic = _find_and_replace(
+            generated_sql_generic, "foreign_key_model", "<foreign_key_model_identifier>"
+        )
 
         expected_sql_check = _normalize_whitespace(expected_sql)
 
         assert expected_sql_check == generated_sql_generic
 
 
 class BaseConstraintsRollback:
@@ -306,16 +332,17 @@
         }
 
 
 class BaseIncrementalConstraintsRuntimeDdlEnforcement(BaseConstraintsRuntimeDdlEnforcement):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model.sql": my_model_incremental_wrong_order_sql,
-            "constraints_schema.yml": model_schema_yml,
+            "my_model.sql": my_model_incremental_wrong_order_depends_on_fk_sql,
+            "foreign_key_model.sql": foreign_key_model_sql,
+            "constraints_schema.yml": model_fk_constraint_schema_yml,
         }
 
 
 class BaseIncrementalConstraintsRollback(BaseConstraintsRollback):
     @pytest.fixture(scope="class")
     def models(self):
         return {
@@ -354,66 +381,119 @@
     pass
 
 
 class TestIncrementalConstraintsRollback(BaseIncrementalConstraintsRollback):
     pass
 
 
+class BaseContractSqlHeader:
+    """Tests a contracted model with a sql header dependency."""
+
+    def test__contract_sql_header(self, project):
+        run_dbt(["run", "-s", "my_model_contract_sql_header"])
+
+        manifest = get_manifest(project.project_root)
+        model_id = "model.test.my_model_contract_sql_header"
+        model_config = manifest.nodes[model_id].config
+
+        assert model_config.contract.enforced
+
+
+class BaseTableContractSqlHeader(BaseContractSqlHeader):
+    @pytest.fixture(scope="class")
+    def models(self):
+        return {
+            "my_model_contract_sql_header.sql": my_model_contract_sql_header_sql,
+            "constraints_schema.yml": model_contract_header_schema_yml,
+        }
+
+
+class BaseIncrementalContractSqlHeader(BaseContractSqlHeader):
+    @pytest.fixture(scope="class")
+    def models(self):
+        return {
+            "my_model_contract_sql_header.sql": my_model_incremental_contract_sql_header_sql,
+            "constraints_schema.yml": model_contract_header_schema_yml,
+        }
+
+
+class TestTableContractSqlHeader(BaseTableContractSqlHeader):
+    pass
+
+
+class TestIncrementalContractSqlHeader(BaseIncrementalContractSqlHeader):
+    pass
+
+
 class BaseModelConstraintsRuntimeEnforcement:
     """
     These model-level constraints pass muster for dbt's preflight checks. Make sure they're
     passed into the DDL statement. If they don't match up with the underlying data,
     the data platform should raise an error at runtime.
     """
 
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "my_model.sql": my_model_sql,
+            "my_model.sql": my_model_wrong_order_depends_on_fk_sql,
+            "foreign_key_model.sql": foreign_key_model_sql,
             "constraints_schema.yml": constrained_model_schema_yml,
         }
 
     @pytest.fixture(scope="class")
     def expected_sql(self):
         return """
 create table <model_identifier> (
     id integer not null,
     color text,
     date_day text,
-    check (id > 0),
+    check ((id > 0)),
+    check (id >= 1),
     primary key (id),
-    constraint strange_uniqueness_requirement unique (color, date_day)
+    constraint strange_uniqueness_requirement unique (color, date_day),
+    foreign key (id) references <foreign_key_model_identifier> (id)
 ) ;
 insert into <model_identifier> (
     id ,
     color ,
     date_day
 )
 (
     select
        id,
        color,
        date_day
        from
     (
+        -- depends_on: <foreign_key_model_identifier>
         select
-            1 as id,
             'blue' as color,
+            1 as id,
             '2019-01-01' as date_day
     ) as model_subq
 );
 """
 
     def test__model_constraints_ddl(self, project, expected_sql):
-        results = run_dbt(["run", "-s", "my_model"])
-        assert len(results) == 1
+        unformatted_constraint_schema_yml = read_file("models", "constraints_schema.yml")
+        write_file(
+            unformatted_constraint_schema_yml.format(schema=project.test_schema),
+            "models",
+            "constraints_schema.yml",
+        )
+
+        results = run_dbt(["run", "-s", "+my_model"])
+        # assert at least my_model was run - additional upstreams may or may not be provided to the test setup via models fixture
+        assert len(results) >= 1
         generated_sql = read_file("target", "run", "test", "models", "my_model.sql")
-        generated_sql_list = _normalize_whitespace(generated_sql).split(" ")
-        generated_sql_list = [
-            "<model_identifier>" if "my_model" in s else s for s in generated_sql_list
-        ]
-        generated_sql_generic = " ".join(generated_sql_list)
+        generated_sql_modified = _normalize_whitespace(generated_sql)
+        generated_sql_generic = _find_and_replace(
+            generated_sql_modified, "my_model", "<model_identifier>"
+        )
+        generated_sql_generic = _find_and_replace(
+            generated_sql_generic, "foreign_key_model", "<foreign_key_model_identifier>"
+        )
         assert _normalize_whitespace(expected_sql) == generated_sql_generic
 
 
 class TestModelConstraintsRuntimeEnforcement(BaseModelConstraintsRuntimeEnforcement):
     pass
```

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/dbt_debug/test_dbt_debug.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/dbt_debug/test_dbt_debug.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 import os
 import re
 import yaml
 
 from dbt.cli.exceptions import DbtUsageException
-from dbt.tests.util import run_dbt
+from dbt.tests.util import run_dbt, run_dbt_and_capture
 
 MODELS__MODEL_SQL = """
 seled 1 as id
 """
 
 
 class BaseDebug:
@@ -47,14 +47,32 @@
 
 
 class TestDebugPostgres(BaseDebug):
     def test_ok(self, project):
         run_dbt(["debug"])
         assert "ERROR" not in self.capsys.readouterr().out
 
+    def test_connection_flag(self, project):
+        """Testing that the --connection flag works as expected, including that output is not lost"""
+        _, out = run_dbt_and_capture(["debug", "--connection"])
+        assert "Skipping steps before connection verification" in out
+
+        _, out = run_dbt_and_capture(
+            ["debug", "--connection", "--target", "NONE"], expect_pass=False
+        )
+        assert "1 check failed" in out
+        assert "The profile 'test' does not have a target named 'NONE'." in out
+
+        _, out = run_dbt_and_capture(
+            ["debug", "--connection", "--profiles-dir", "NONE"], expect_pass=False
+        )
+        assert "Using profiles dir at NONE"
+        assert "1 check failed" in out
+        assert "dbt looked for a profiles.yml file in NONE" in out
+
     def test_nopass(self, project):
         run_dbt(["debug", "--target", "nopass"], expect_pass=False)
         self.assertGotValue(re.compile(r"\s+profiles\.yml file"), "ERROR invalid")
 
     def test_wronguser(self, project):
         run_dbt(["debug", "--target", "wronguser"], expect_pass=False)
         self.assertGotValue(re.compile(r"\s+Connection test"), "ERROR")
@@ -96,7 +114,14 @@
         project_config = {"invalid-key": "not a valid key in this project"}
         os.makedirs("custom", exist_ok=True)
         with open("custom/dbt_project.yml", "w") as f:
             yaml.safe_dump(project_config, f, default_flow_style=True)
         run_dbt(["debug", "--project-dir", "custom"], expect_pass=False)
         splitout = self.capsys.readouterr().out.split("\n")
         self.check_project(splitout)
+
+    def test_profile_not_found(self, project):
+        _, out = run_dbt_and_capture(
+            ["debug", "--connection", "--profile", "NONE"], expect_pass=False
+        )
+        assert "Profile loading failed for the following reason" in out
+        assert "Could not find profile named 'NONE'" in out
```

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/ephemeral/test_ephemeral.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/ephemeral/test_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/base_grants.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/base_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/test_incremental_grants.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_incremental_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/test_invalid_grants.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_invalid_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/test_model_grants.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_model_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/test_seed_grants.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_seed_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/grants/test_snapshot_grants.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/grants/test_snapshot_grants.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/hooks/fixtures.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/hooks/test_model_hooks.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/test_model_hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/hooks/test_run_hooks.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/hooks/test_run_hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/fixtures.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_on_schema_change.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/test_incremental_predicates.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_predicates.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/incremental/test_incremental_unique_id.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/incremental/test_incremental_unique_id.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/persist_docs/fixtures.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/persist_docs/fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 _DOCS__MY_FUN_DOCS = """
 {% docs my_fun_doc %}
 name Column description "with double quotes"
 and with 'single  quotes' as welll as other;
 '''abc123'''
 reserved -- characters
+80% of statistics are made up on the spot
 --
 /* comment */
 Some $lbl$ labeled $lbl$ and $$ unlabeled $$ dollar-quoting
 
 {% enddocs %}
 """
 
@@ -63,68 +64,74 @@
 models:
   - name: table_model
     description: |
       Table model description "with double quotes"
       and with 'single  quotes' as welll as other;
       '''abc123'''
       reserved -- characters
+      80% of statistics are made up on the spot
       --
       /* comment */
       Some $lbl$ labeled $lbl$ and $$ unlabeled $$ dollar-quoting
     columns:
       - name: id
         description: |
           id Column description "with double quotes"
           and with 'single  quotes' as welll as other;
           '''abc123'''
           reserved -- characters
+          80% of statistics are made up on the spot
           --
           /* comment */
           Some $lbl$ labeled $lbl$ and $$ unlabeled $$ dollar-quoting
       - name: name
         description: |
           Some stuff here and then a call to
           {{ doc('my_fun_doc')}}
   - name: view_model
     description: |
       View model description "with double quotes"
       and with 'single  quotes' as welll as other;
       '''abc123'''
       reserved -- characters
+      80% of statistics are made up on the spot
       --
       /* comment */
       Some $lbl$ labeled $lbl$ and $$ unlabeled $$ dollar-quoting
     columns:
       - name: id
         description: |
           id Column description "with double quotes"
           and with 'single  quotes' as welll as other;
           '''abc123'''
           reserved -- characters
+          80% of statistics are made up on the spot
           --
           /* comment */
           Some $lbl$ labeled $lbl$ and $$ unlabeled $$ dollar-quoting
 
 seeds:
   - name: seed
     description: |
       Seed model description "with double quotes"
       and with 'single  quotes' as welll as other;
       '''abc123'''
       reserved -- characters
+      80% of statistics are made up on the spot
       --
       /* comment */
       Some $lbl$ labeled $lbl$ and $$ unlabeled $$ dollar-quoting
     columns:
       - name: id
         description: |
           id Column description "with double quotes"
           and with 'single  quotes' as welll as other;
           '''abc123'''
           reserved -- characters
+          80% of statistics are made up on the spot
           --
           /* comment */
           Some $lbl$ labeled $lbl$ and $$ unlabeled $$ dollar-quoting
       - name: name
         description: |
           Some stuff here and then a call to
           {{ doc('my_fun_doc')}}
```

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/persist_docs/test_persist_docs.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/persist_docs/test_persist_docs.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/python_model/test_python_model.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/python_model/test_python_model.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/python_model/test_spark.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/python_model/test_spark.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/query_comment/fixtures.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/query_comment/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/query_comment/test_query_comment.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/query_comment/test_query_comment.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/relations/test_changing_relation_type.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/relations/test_changing_relation_type.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_copy/fixtures.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_copy/test_copy_uppercase.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/test_copy_uppercase.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_copy/test_simple_copy.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_copy/test_simple_copy.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_seed/fixtures.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_seed/seeds.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_seed/test_seed.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/test_seed.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_seed/test_seed_type_override.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_seed/test_seed_type_override.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_snapshot/common.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/common.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_snapshot/seeds.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_snapshot/snapshots.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/simple_snapshot/test_snapshot.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/simple_snapshot/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/store_test_failures_tests/fixtures.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/store_test_failures_tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/store_test_failures_tests/test_store_test_failures.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/base_array_utils.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/base_array_utils.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/base_utils.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/base_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 import pytest
 from dbt.tests.util import run_dbt
 
 macros__equals_sql = """
-{% macro equals(actual, expected) %}
-{# -- actual is not distinct from expected #}
-(({{ actual }} = {{ expected }}) or ({{ actual }} is null and {{ expected }} is null))
+{% macro equals(expr1, expr2) -%}
+case when (({{ expr1 }} = {{ expr2 }}) or ({{ expr1 }} is null and {{ expr2 }} is null))
+    then 0
+    else 1
+end = 0
 {% endmacro %}
 """
 
 macros__test_assert_equal_sql = """
 {% test assert_equal(model, actual, expected) %}
 select * from {{ model }}
 where not {{ equals(actual, expected) }}
 {% endtest %}
 """
 
+macros__replace_empty_sql = """
+{% macro replace_empty(expr) -%}
+case
+    when {{ expr }} = 'EMPTY' then ''
+    else {{ expr }}
+end
+{% endmacro %}
+"""
+
 
 class BaseUtils:
     # setup
     @pytest.fixture(scope="class")
     def macros(self):
         return {
             "equals.sql": macros__equals_sql,
             "test_assert_equal.sql": macros__test_assert_equal_sql,
+            "replace_empty.sql": macros__replace_empty_sql,
         }
 
     # make it possible to dynamically update the macro call with a namespace
     # (e.g.) 'dateadd', 'dbt.dateadd', 'dbt_utils.dateadd'
     def macro_namespace(self):
         return ""
```

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/base_data_type_macro.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/base_data_type_macro.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_bigint.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_bigint.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_boolean.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_boolean.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_float.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_float.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_int.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_int.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_numeric.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_numeric.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_string.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_string.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/data_types/test_type_timestamp.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/data_types/test_type_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_any_value.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_any_value.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_array_concat.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_array_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_bool_or.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_bool_or.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_date_trunc.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_date_trunc.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_dateadd.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_dateadd.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_datediff.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_datediff.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_escape_single_quotes.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_escape_single_quotes.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_except.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_except.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_hash.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_hash.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 # hash
 
+# https://github.com/dbt-labs/dbt-core/issues/4725
 seeds__data_hash_csv = """input_1,output
 ab,187ef4436122d1cc2f40dc2b92f0eba0
 a,0cc175b9c0f1b6a831c399e269772661
 1,c4ca4238a0b923820dcc509a6f75849b
-,d41d8cd98f00b204e9800998ecf8427e
+EMPTY,d41d8cd98f00b204e9800998ecf8427e
 """
 
 
 models__test_hash_sql = """
-with data as (
+with seed_data as (
 
     select * from {{ ref('data_hash') }}
 
+),
+
+data as (
+
+    select
+        {{ replace_empty('input_1') }} as input_1,
+        {{ replace_empty('output') }} as output
+    from seed_data
+
 )
 
 select
     {{ hash('input_1') }} as actual,
     output as expected
 
 from data
```

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_intersect.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_last_day.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_last_day.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_listagg.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_listagg.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_null_compare.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_null_compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     null as expected
 """
 
 
 MODELS__TEST_MIXED_NULL_COMPARE_YML = """
 version: 2
 models:
-  - name: test_null_compare
+  - name: test_mixed_null_compare
     tests:
       - assert_equal:
           actual: actual
           expected: expected
 """
```

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_position.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_position.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_replace.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_replace.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_right.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_right.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_split_part.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_split_part.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/fixture_string_literal.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/fixture_string_literal.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_any_value.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_any_value.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_array_append.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_append.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_array_concat.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_array_construct.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_array_construct.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_bool_or.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_bool_or.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_cast_bool_to_text.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_cast_bool_to_text.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_concat.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_concat.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_current_timestamp.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_current_timestamp.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_date_trunc.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_date_trunc.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_dateadd.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_dateadd.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_datediff.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_datediff.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_escape_single_quotes.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_escape_single_quotes.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_except.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_except.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_hash.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_hash.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_intersect.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_intersect.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_last_day.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_last_day.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_length.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_length.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_listagg.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_listagg.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_null_compare.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_null_compare.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 from dbt.tests.util import run_dbt
 
 
 class BaseMixedNullCompare(BaseUtils):
     @pytest.fixture(scope="class")
     def models(self):
         return {
-            "test_mixed_null_compare.yml": MODELS__TEST_MIXED_NULL_COMPARE_SQL,
-            "test_mixed_null_compare.sql": MODELS__TEST_MIXED_NULL_COMPARE_YML,
+            "test_mixed_null_compare.yml": MODELS__TEST_MIXED_NULL_COMPARE_YML,
+            "test_mixed_null_compare.sql": MODELS__TEST_MIXED_NULL_COMPARE_SQL,
         }
 
     def test_build_assert_equal(self, project):
         run_dbt()
         run_dbt(["test"], expect_pass=False)
 
 
@@ -28,13 +28,13 @@
     def models(self):
         return {
             "test_null_compare.yml": MODELS__TEST_NULL_COMPARE_YML,
             "test_null_compare.sql": MODELS__TEST_NULL_COMPARE_SQL,
         }
 
 
-class TestMixedNullCompare(BaseNullCompare):
+class TestMixedNullCompare(BaseMixedNullCompare):
     pass
 
 
 class TestNullCompare(BaseNullCompare):
     pass
```

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_position.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_position.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_replace.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_replace.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_right.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_right.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_safe_cast.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_safe_cast.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_split_part.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_split_part.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_string_literal.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_string_literal.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt/tests/adapter/utils/test_timestamps.py` & `dbt-tests-adapter-1.6.0b3/dbt/tests/adapter/utils/test_timestamps.py`

 * *Files identical despite different names*

### Comparing `dbt-tests-adapter-1.6.0b2/dbt_tests_adapter.egg-info/PKG-INFO` & `dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-tests-adapter
-Version: 1.6.0b2
+Version: 1.6.0b3
 Summary: The dbt adapter tests for adapter plugins
 Home-page: https://github.com/dbt-labs/dbt-core/tree/main/tests/adapter
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt-core/fa1ea14ddfb1d5ae319d5141844910dd53ab2834/etc/dbt-core.svg" alt="dbt logo" width="750"/>
 </p>
 
 # dbt-tests-adapter
```

### Comparing `dbt-tests-adapter-1.6.0b2/dbt_tests_adapter.egg-info/SOURCES.txt` & `dbt-tests-adapter-1.6.0b3/dbt_tests_adapter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 dbt/tests/adapter/hooks/test_model_hooks.py
 dbt/tests/adapter/hooks/test_run_hooks.py
 dbt/tests/adapter/incremental/fixtures.py
 dbt/tests/adapter/incremental/test_incremental_merge_exclude_columns.py
 dbt/tests/adapter/incremental/test_incremental_on_schema_change.py
 dbt/tests/adapter/incremental/test_incremental_predicates.py
 dbt/tests/adapter/incremental/test_incremental_unique_id.py
+dbt/tests/adapter/materialized_view/base.py
+dbt/tests/adapter/materialized_view/on_configuration_change.py
 dbt/tests/adapter/persist_docs/fixtures.py
 dbt/tests/adapter/persist_docs/test_persist_docs.py
 dbt/tests/adapter/python_model/test_python_model.py
 dbt/tests/adapter/python_model/test_spark.py
 dbt/tests/adapter/query_comment/fixtures.py
 dbt/tests/adapter/query_comment/test_query_comment.py
 dbt/tests/adapter/relations/test_changing_relation_type.py
@@ -69,14 +71,15 @@
 dbt/tests/adapter/utils/fixture_array_construct.py
 dbt/tests/adapter/utils/fixture_bool_or.py
 dbt/tests/adapter/utils/fixture_cast_bool_to_text.py
 dbt/tests/adapter/utils/fixture_concat.py
 dbt/tests/adapter/utils/fixture_date_trunc.py
 dbt/tests/adapter/utils/fixture_dateadd.py
 dbt/tests/adapter/utils/fixture_datediff.py
+dbt/tests/adapter/utils/fixture_equals.py
 dbt/tests/adapter/utils/fixture_escape_single_quotes.py
 dbt/tests/adapter/utils/fixture_except.py
 dbt/tests/adapter/utils/fixture_hash.py
 dbt/tests/adapter/utils/fixture_intersect.py
 dbt/tests/adapter/utils/fixture_last_day.py
 dbt/tests/adapter/utils/fixture_length.py
 dbt/tests/adapter/utils/fixture_listagg.py
@@ -94,14 +97,15 @@
 dbt/tests/adapter/utils/test_bool_or.py
 dbt/tests/adapter/utils/test_cast_bool_to_text.py
 dbt/tests/adapter/utils/test_concat.py
 dbt/tests/adapter/utils/test_current_timestamp.py
 dbt/tests/adapter/utils/test_date_trunc.py
 dbt/tests/adapter/utils/test_dateadd.py
 dbt/tests/adapter/utils/test_datediff.py
+dbt/tests/adapter/utils/test_equals.py
 dbt/tests/adapter/utils/test_escape_single_quotes.py
 dbt/tests/adapter/utils/test_except.py
 dbt/tests/adapter/utils/test_hash.py
 dbt/tests/adapter/utils/test_intersect.py
 dbt/tests/adapter/utils/test_last_day.py
 dbt/tests/adapter/utils/test_length.py
 dbt/tests/adapter/utils/test_listagg.py
```

### Comparing `dbt-tests-adapter-1.6.0b2/setup.py` & `dbt-tests-adapter-1.6.0b3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 import os
 import sys
 
-if sys.version_info < (3, 7):
+if sys.version_info < (3, 8):
     print("Error: dbt does not support this version of Python.")
-    print("Please upgrade to Python 3.7 or higher.")
+    print("Please upgrade to Python 3.8 or higher.")
     sys.exit(1)
 
 
 from setuptools import setup
 
 try:
     from setuptools import find_namespace_packages
@@ -16,15 +16,15 @@
     # the user has a downlevel version of setuptools.
     print("Error: dbt requires setuptools v40.1.0 or higher.")
     print('Please upgrade setuptools with "pip install --upgrade setuptools" ' "and try again")
     sys.exit(1)
 
 
 package_name = "dbt-tests-adapter"
-package_version = "1.6.0b2"
+package_version = "1.6.0b3"
 description = """The dbt adapter tests for adapter plugins"""
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 setup(
@@ -44,13 +44,14 @@
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

