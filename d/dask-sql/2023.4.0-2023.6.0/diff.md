# Comparing `tmp/dask_sql-2023.4.0.tar.gz` & `tmp/dask_sql-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask_sql-2023.4.0.tar", last modified: Thu Apr  6 14:40:06 2023, max compression
+gzip compressed data, was "dask_sql-2023.6.0.tar", last modified: Thu Jun  8 16:19:57 2023, max compression
```

## Comparing `dask_sql-2023.4.0.tar` & `dask_sql-2023.6.0.tar`

### file list

```diff
@@ -1,181 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.719195 dask_sql-2023.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-06 14:40:06.719195 dask_sql-2023.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.699195 dask_sql-2023.4.0/dask_planner/
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/.classpath
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.699195 dask_sql-2023.4.0/dask_planner/.settings/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/.settings/org.eclipse.core.resources.prefs
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/.settings/org.eclipse.jdt.apt.core.prefs
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/.settings/org.eclipse.jdt.core.prefs
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/.settings/org.eclipse.m2e.core.prefs
--rw-r--r--   0 runner    (1001) docker     (123)    59398 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/Cargo.lock
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.699195 dask_sql-2023.4.0/dask_planner/src/
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/dialect.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (123)    32752 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/expression.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)    54776 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/parser.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.703195 dask_sql-2023.4.0/dask_planner/src/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/column.rs
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/exceptions.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/function.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.707195 dask_sql-2023.4.0/dask_planner/src/sql/logical/
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/aggregate.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/alter_schema.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/alter_table.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/analyze_table.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/create_catalog_schema.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/create_experiment.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/create_memory_table.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/create_model.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/create_table.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/describe_model.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/drop_model.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/drop_schema.rs
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/drop_table.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/empty_relation.rs
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/explain.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/export_model.rs
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/filter.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/join.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/limit.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/predict_model.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/projection.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/repartition_by.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/show_columns.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/show_models.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/show_schemas.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/show_tables.rs
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/sort.rs
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/subquery_alias.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/table_scan.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/use_schema.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical/window.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/logical.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.707195 dask_sql-2023.4.0/dask_planner/src/sql/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)    22403 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/optimizer/filter_columns_post_join.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/optimizer/join_reorder.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/optimizer.rs
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/parser_utils.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/schema.rs
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/statement.rs
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/table.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.707195 dask_sql-2023.4.0/dask_planner/src/sql/types/
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/types/rel_data_type.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/types/rel_data_type_field.rs
--rw-r--r--   0 runner    (1001) docker     (123)    15196 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql/types.rs
--rw-r--r--   0 runner    (1001) docker     (123)    31438 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/src/sql.rs
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_planner/update-dependencies.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.719195 dask_sql-2023.4.0/dask_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-06 14:40:06.719195 dask_sql-2023.4.0/dask_sql/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    36295 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/datacontainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.711195 dask_sql-2023.4.0/dask_sql/input_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/input_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/input_utils/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/input_utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/input_utils/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/input_utils/hive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/input_utils/intake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/input_utils/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/input_utils/pandaslike.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/input_utils/sqlalchemy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.711195 dask_sql-2023.4.0/dask_sql/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/integrations/fugue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/integrations/ipython.py
--rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/mappings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.711195 dask_sql-2023.4.0/dask_sql/physical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.711195 dask_sql-2023.4.0/dask_sql/physical/rel/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.715195 dask_sql-2023.4.0/dask_sql/physical/rel/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/alter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/analyze_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/create_catalog_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/create_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/create_memory_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/create_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/create_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/describe_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/distributeby.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/drop_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/drop_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/drop_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/export_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/predict_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/show_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/show_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/show_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/show_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/use_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    28191 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/custom/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.715195 dask_sql-2023.4.0/dask_sql/physical/rel/logical/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21656 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/cross_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/join.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/subquery_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/table_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/union.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/values.py
--rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rel/logical/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.715195 dask_sql-2023.4.0/dask_sql/physical/rex/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rex/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.715195 dask_sql-2023.4.0/dask_sql/physical/rex/core/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rex/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rex/core/alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    35329 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rex/core/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rex/core/input_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rex/core/literal.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/rex/core/subquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.719195 dask_sql-2023.4.0/dask_sql/physical/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13012 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/utils/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/utils/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/utils/ml_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/physical/utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.719195 dask_sql-2023.4.0/dask_sql/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/server/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/server/presto_jdbc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/server/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/sql-schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/sql.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/dask_sql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:40:06.707195 dask_sql-2023.4.0/dask_sql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-06 14:40:06.000000 dask_sql-2023.4.0/dask_sql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-04-06 14:40:06.000000 dask_sql-2023.4.0/dask_sql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:40:06.000000 dask_sql-2023.4.0/dask_sql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-06 14:40:06.000000 dask_sql-2023.4.0/dask_sql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:40:06.000000 dask_sql-2023.4.0/dask_sql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-06 14:40:06.000000 dask_sql-2023.4.0/dask_sql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-06 14:40:06.000000 dask_sql-2023.4.0/dask_sql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-06 14:40:06.719195 dask_sql-2023.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83601 2023-04-06 14:39:11.000000 dask_sql-2023.4.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.155178 dask_sql-2023.6.0/dask_planner/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.155178 dask_sql-2023.6.0/dask_planner/.cargo/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.cargo/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.classpath
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.155178 dask_sql-2023.6.0/dask_planner/.settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.settings/org.eclipse.core.resources.prefs
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.settings/org.eclipse.jdt.apt.core.prefs
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.settings/org.eclipse.jdt.core.prefs
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/.settings/org.eclipse.m2e.core.prefs
+-rw-r--r--   0 runner    (1001) docker     (123)   101603 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/Cargo.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.155178 dask_sql-2023.6.0/dask_planner/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/dialect.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    36601 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/expression.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    54871 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/parser.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.155178 dask_sql-2023.6.0/dask_planner/src/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/column.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/exceptions.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/function.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.159178 dask_sql-2023.6.0/dask_planner/src/sql/logical/
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/aggregate.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/alter_schema.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/alter_table.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/analyze_table.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/create_catalog_schema.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/create_experiment.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/create_memory_table.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/create_model.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/create_table.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/describe_model.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_model.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_schema.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_table.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/empty_relation.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/explain.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/export_model.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/filter.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/join.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/limit.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/predict_model.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/projection.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/repartition_by.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/show_columns.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/show_models.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/show_schemas.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/show_tables.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/sort.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/subquery_alias.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/table_scan.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/use_schema.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical/window.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    17170 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/logical.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.159178 dask_sql-2023.6.0/dask_planner/src/sql/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/optimizer/join_reorder.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/optimizer.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/parser_utils.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/schema.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/statement.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/table.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.159178 dask_sql-2023.6.0/dask_planner/src/sql/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/types/rel_data_type.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/types/rel_data_type_field.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql/types.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    32505 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/src/sql.rs
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_planner/update-dependencies.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/dask_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/dask_sql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36798 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/datacontainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.163178 dask_sql-2023.6.0/dask_sql/input_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/hive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/pandaslike.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/input_utils/sqlalchemy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.163178 dask_sql-2023.6.0/dask_sql/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/integrations/fugue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/integrations/ipython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12400 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/mappings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.163178 dask_sql-2023.6.0/dask_sql/physical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.163178 dask_sql-2023.6.0/dask_sql/physical/rel/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.167178 dask_sql-2023.6.0/dask_sql/physical/rel/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/alter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/analyze_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_catalog_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_memory_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/describe_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/distributeby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/export_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/predict_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/use_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28036 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/custom/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.167178 dask_sql-2023.6.0/dask_sql/physical/rel/logical/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21656 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/cross_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13610 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/subquery_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/table_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rel/logical/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.167178 dask_sql-2023.6.0/dask_sql/physical/rex/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.167178 dask_sql-2023.6.0/dask_sql/physical/rex/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36009 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/input_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7821 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/literal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/rex/core/subquery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/dask_sql/physical/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/ml_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/physical/utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/dask_sql/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/server/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/server/presto_jdbc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/server/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/sql-schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/sql.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/dask_sql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:57.163178 dask_sql-2023.6.0/dask_sql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 16:19:57.000000 dask_sql-2023.6.0/dask_sql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-08 16:19:57.171178 dask_sql-2023.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83601 2023-06-08 16:19:08.000000 dask_sql-2023.6.0/versioneer.py
```

### Comparing `dask_sql-2023.4.0/LICENSE.txt` & `dask_sql-2023.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/PKG-INFO` & `dask_sql-2023.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask_sql
-Version: 2023.4.0
+Version: 2023.6.0
 Summary: SQL query layer for Dask
 Home-page: https://github.com/dask-contrib/dask-sql/
 Maintainer: Nils Braun
 Maintainer-email: nilslennartbraun@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -30,15 +30,15 @@
 if you need it.
 
 * **Combine the power of Python and SQL**: load your data with Python, transform it with SQL, enhance it with Python and query it with SQL - or the other way round.
   With `dask-sql` you can mix the well known Python dataframe API of `pandas` and `Dask` with common SQL operations, to
   process your data in exactly the way that is easiest for you.
 * **Infinite Scaling**: using the power of the great `Dask` ecosystem, your computations can scale as you need it - from your laptop to your super cluster - without changing any line of SQL code. From k8s to cloud deployments, from batch systems to YARN - if `Dask` [supports it](https://docs.dask.org/en/latest/setup.html), so will `dask-sql`.
 * **Your data - your queries**: Use Python user-defined functions (UDFs) in SQL without any performance drawback and extend your SQL queries with the large number of Python libraries, e.g. machine learning, different complicated input formats, complex statistics.
-* **Easy to install and maintain**: `dask-sql` is just a pip/conda install away (or a docker run if you prefer). No need for complicated cluster setups - `dask-sql` will run out of the box on your machine and can be easily connected to your computing cluster.
+* **Easy to install and maintain**: `dask-sql` is just a pip/conda install away (or a docker run if you prefer).
 * **Use SQL from wherever you like**: `dask-sql` integrates with your jupyter notebook, your normal Python module or can be used as a standalone SQL server from any BI tool. It even integrates natively with [Apache Hue](https://gethue.com/).
 * **GPU Support**: `dask-sql` supports running SQL queries on CUDA-enabled GPUs by utilizing [RAPIDS](https://rapids.ai) libraries like [`cuDF`](https://github.com/rapidsai/cudf), enabling accelerated compute for SQL.
 
 Read more in the [documentation](https://dask-sql.readthedocs.io/en/latest/).
 
 <div align="center">
     <img src="./.github/animation.gif" alt="dask-sql GIF">
```

### Comparing `dask_sql-2023.4.0/README.md` & `dask_sql-2023.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 if you need it.
 
 * **Combine the power of Python and SQL**: load your data with Python, transform it with SQL, enhance it with Python and query it with SQL - or the other way round.
   With `dask-sql` you can mix the well known Python dataframe API of `pandas` and `Dask` with common SQL operations, to
   process your data in exactly the way that is easiest for you.
 * **Infinite Scaling**: using the power of the great `Dask` ecosystem, your computations can scale as you need it - from your laptop to your super cluster - without changing any line of SQL code. From k8s to cloud deployments, from batch systems to YARN - if `Dask` [supports it](https://docs.dask.org/en/latest/setup.html), so will `dask-sql`.
 * **Your data - your queries**: Use Python user-defined functions (UDFs) in SQL without any performance drawback and extend your SQL queries with the large number of Python libraries, e.g. machine learning, different complicated input formats, complex statistics.
-* **Easy to install and maintain**: `dask-sql` is just a pip/conda install away (or a docker run if you prefer). No need for complicated cluster setups - `dask-sql` will run out of the box on your machine and can be easily connected to your computing cluster.
+* **Easy to install and maintain**: `dask-sql` is just a pip/conda install away (or a docker run if you prefer).
 * **Use SQL from wherever you like**: `dask-sql` integrates with your jupyter notebook, your normal Python module or can be used as a standalone SQL server from any BI tool. It even integrates natively with [Apache Hue](https://gethue.com/).
 * **GPU Support**: `dask-sql` supports running SQL queries on CUDA-enabled GPUs by utilizing [RAPIDS](https://rapids.ai) libraries like [`cuDF`](https://github.com/rapidsai/cudf), enabling accelerated compute for SQL.
 
 Read more in the [documentation](https://dask-sql.readthedocs.io/en/latest/).
 
 <div align="center">
     <img src="./.github/animation.gif" alt="dask-sql GIF">
```

### Comparing `dask_sql-2023.4.0/dask_planner/.classpath` & `dask_sql-2023.6.0/dask_planner/.classpath`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_planner/.gitignore` & `dask_sql-2023.6.0/dask_planner/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_planner/Cargo.lock` & `dask_sql-2023.6.0/dask_planner/Cargo.lock`

 * *Files 24% similar despite different names*

```diff
@@ -5,31 +5,37 @@
 [[package]]
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
+name = "adler32"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aae1277d39aeec15cb388266ecc24b11c80469deae6067e17a1a7aa9e5c1f234"
+
+[[package]]
 name = "ahash"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
  "cfg-if",
  "const-random",
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "alloc-no-stdlib"
 version = "2.0.4"
@@ -51,14 +57,47 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "anyhow"
+version = "1.0.71"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+
+[[package]]
+name = "apache-avro"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8cf4144857f9e4d7dd6cc4ba4c78efd2a46bad682b029bd0d91e76a021af1b2a"
+dependencies = [
+ "byteorder",
+ "crc32fast",
+ "digest",
+ "lazy_static",
+ "libflate",
+ "log",
+ "num-bigint",
+ "quad-rand",
+ "rand",
+ "regex",
+ "serde",
+ "serde_json",
+ "snap",
+ "strum",
+ "strum_macros",
+ "thiserror",
+ "typed-builder",
+ "uuid",
+ "zerocopy",
+]
+
+[[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
 name = "arrayref"
@@ -70,17 +109,17 @@
 name = "arrayvec"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
 
 [[package]]
 name = "arrow"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87d948f553cf556656eb89265700258e1032d26fec9b7920cd20319336e06afd"
+checksum = "990dfa1a9328504aa135820da1c95066537b69ad94c04881b785f64328e0fa6b"
 dependencies = [
  "ahash",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-csv",
@@ -88,79 +127,81 @@
  "arrow-ipc",
  "arrow-json",
  "arrow-ord",
  "arrow-row",
  "arrow-schema",
  "arrow-select",
  "arrow-string",
- "comfy-table",
+ "pyo3",
 ]
 
 [[package]]
 name = "arrow-arith"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf30d4ebc3df9dfd8bd26883aa30687d4ddcfd7b2443e62bd7c8fedf153b8e45"
+checksum = "f2b2e52de0ab54173f9b08232b7184c26af82ee7ab4ac77c83396633c90199fa"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-array"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9fe66ec388d882a61fff3eb613b5266af133aa08a3318e5e493daf0f5c1696cb"
+checksum = "e10849b60c17dbabb334be1f4ef7550701aa58082b71335ce1ed586601b2f423"
 dependencies = [
  "ahash",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
+ "chrono-tz",
  "half",
  "hashbrown 0.13.2",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4ef967dadbccd4586ec8d7aab27d7033ecb5dfae8a605c839613039eac227bda"
+checksum = "b0746ae991b186be39933147117f8339eb1c4bbbea1c8ad37e7bf5851a1a06ba"
 dependencies = [
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-cast"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "491a7979ea9e76dc218f532896e2d245fde5235e2e6420ce80d27cf6395dda84"
+checksum = "b88897802515d7b193e38b27ddd9d9e43923d410a9e46307582d756959ee9595"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "chrono",
+ "comfy-table",
  "lexical-core",
  "num",
 ]
 
 [[package]]
 name = "arrow-csv"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b1d4fc91078dbe843c2c50d90f8119c96e8dfac2f78d30f7a8cb9397399c61d"
+checksum = "1c8220d9741fc37961262710ceebd8451a5b393de57c464f0267ffdda1775c0a"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -169,43 +210,43 @@
  "lazy_static",
  "lexical-core",
  "regex",
 ]
 
 [[package]]
 name = "arrow-data"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee0c0e3c5d3b80be8f267f4b2af714c08cad630569be01a8379cfe27b4866495"
+checksum = "533f937efa1aaad9dc86f6a0e382c2fa736a4943e2090c946138079bdf060cef"
 dependencies = [
  "arrow-buffer",
  "arrow-schema",
  "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-ipc"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0a3ca7eb8d23c83fe40805cbafec70a6a31df72de47355545ff34c850f715403"
+checksum = "18b75296ff01833f602552dff26a423fc213db8e5049b540ca4a00b1c957e41c"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "flatbuffers",
 ]
 
 [[package]]
 name = "arrow-json"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf65aff76d2e340d827d5cab14759e7dd90891a288347e2202e4ee28453d9bed"
+checksum = "e501d3de4d612c90677594896ca6c0fa075665a7ff980dc4189bb531c17e19f6"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-schema",
  "chrono",
@@ -214,73 +255,77 @@
  "lexical-core",
  "num",
  "serde_json",
 ]
 
 [[package]]
 name = "arrow-ord"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "074a5a55c37ae4750af4811c8861c0378d8ab2ff6c262622ad24efae6e0b73b3"
+checksum = "33d2671eb3793f9410230ac3efb0e6d36307be8a2dac5fad58ac9abde8e9f01e"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
+ "half",
  "num",
 ]
 
 [[package]]
 name = "arrow-row"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e064ac4e64960ebfbe35f218f5e7d9dc9803b59c2e56f611da28ce6d008f839e"
+checksum = "fc11fa039338cebbf4e29cf709c8ac1d6a65c7540063d4a25f991ab255ca85c8"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half",
  "hashbrown 0.13.2",
 ]
 
 [[package]]
 name = "arrow-schema"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ead3f373b9173af52f2fdefcb5a7dd89f453fbc40056f574a8aeb23382a4ef81"
+checksum = "d04f17f7b86ded0b5baf98fe6123391c4343e031acc3ccc5fa604cc180bff220"
+dependencies = [
+ "bitflags 2.2.1",
+]
 
 [[package]]
 name = "arrow-select"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "646b4f15b5a77c970059e748aeb1539705c68cd397ecf0f0264c4ef3737d35f3"
+checksum = "163e35de698098ff5f5f672ada9dc1f82533f10407c7a11e2cd09f3bcf31d18a"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "num",
 ]
 
 [[package]]
 name = "arrow-string"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8b8bf150caaeca03f39f1a91069701387d93f7cfd256d27f423ac8496d99a51"
+checksum = "bfdfbed1b10209f0dc68e6aa4c43dc76079af65880965c7c3b73f641f23d4aba"
 dependencies = [
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "arrow-select",
  "regex",
- "regex-syntax",
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "async-compression"
 version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "942c7cd7ae39e91bde4820d74132e9862e62c2f386c3aa90ccf55949f5bad63a"
@@ -289,25 +334,38 @@
  "flate2",
  "futures-core",
  "futures-io",
  "memchr",
  "pin-project-lite",
  "tokio",
  "xz2",
+ "zstd 0.11.2+zstd.1.5.2",
+ "zstd-safe 5.0.2+zstd.1.5.2",
+]
+
+[[package]]
+name = "async-recursion"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0e97ce7de6cf12de5d7226c73f5ba9811622f4db3a5b91b55c53e987e5f91cba"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
@@ -321,14 +379,20 @@
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "24a6904aef64d73cf10ab17ebace7befb918b82164785cb89907993be7f83813"
+
+[[package]]
 name = "blake2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "46502ad458c9a52b69d4d4d32775c788b7a1b85e8bc9d482d92250fc0e3f8efe"
 dependencies = [
  "digest",
 ]
@@ -374,18 +438,39 @@
 checksum = "4b6561fd3f895a11e8f72af2cb7d22e08366bebc2b6b57f7744c4bda27034744"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
+name = "bstr"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c3d4260bcc2e8fc9df1eac4919a720effeb63a3f0952f5bf4944adfa18897f09"
+dependencies = [
+ "memchr",
+ "once_cell",
+ "regex-automata",
+ "serde",
+]
+
+[[package]]
+name = "btoi"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9dd6407f73a9b8b6162d8a2ef999fe6afd7cc15902ebf42c5cd296addf17e0ad"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
@@ -434,20 +519,52 @@
 [[package]]
 name = "chrono"
 version = "0.4.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
 dependencies = [
  "iana-time-zone",
+ "js-sys",
  "num-integer",
  "num-traits",
+ "serde",
+ "time 0.1.45",
+ "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
+name = "chrono-tz"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf9cc2b23599e6d7479755f3594285efb3f74a1bdca7a7374948bc831e23a552"
+dependencies = [
+ "chrono",
+ "chrono-tz-build",
+ "phf",
+]
+
+[[package]]
+name = "chrono-tz-build"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d9998fb9f7e9b2111641485bf8beb32f92945f97f92a3d061f744cfef335f751"
+dependencies = [
+ "parse-zoneinfo",
+ "phf",
+ "phf_codegen",
+]
+
+[[package]]
+name = "clru"
+version = "0.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b8191fa7302e03607ff0e237d4246cc043ff5b3cb9409d995172ba3bea16b807"
+
+[[package]]
 name = "codespan-reporting"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
 dependencies = [
  "termcolor",
  "unicode-width",
@@ -490,23 +607,23 @@
 name = "constant_time_eq"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "13418e745008f7349ec7e449155f419a61b92b58a99cc3616942b926825ec76b"
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -573,15 +690,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
@@ -590,15 +707,15 @@
 name = "cxxbridge-macro"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.11",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "dashmap"
 version = "5.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
@@ -611,222 +728,323 @@
 ]
 
 [[package]]
 name = "dask_planner"
 version = "0.1.0"
 dependencies = [
  "async-trait",
- "datafusion",
- "datafusion-common",
- "datafusion-expr",
- "datafusion-optimizer",
- "datafusion-sql",
+ "datafusion-python",
  "env_logger",
  "log",
- "mimalloc",
- "parking_lot",
  "pyo3",
+ "pyo3-build-config 0.19.0",
  "pyo3-log",
- "rand",
- "tokio",
- "uuid",
 ]
 
 [[package]]
 name = "datafusion"
-version = "18.0.0"
+version = "22.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd805bdf93d3137b37fd9966042df0c84ddfca0df5a8d32eaacb16cf6ab0d93d"
+checksum = "9bdb93fee4f30368f1f71bfd5cd28882ec9fab0183db7924827b76129d33227c"
 dependencies = [
  "ahash",
+ "apache-avro",
  "arrow",
  "async-compression",
  "async-trait",
  "bytes",
  "bzip2",
  "chrono",
  "dashmap",
  "datafusion-common",
+ "datafusion-execution",
  "datafusion-expr",
  "datafusion-optimizer",
  "datafusion-physical-expr",
  "datafusion-row",
  "datafusion-sql",
  "flate2",
  "futures",
  "glob",
  "hashbrown 0.13.2",
  "indexmap",
  "itertools",
  "lazy_static",
  "log",
+ "num-traits",
  "num_cpus",
  "object_store",
  "parking_lot",
  "parquet",
- "paste",
  "percent-encoding",
  "pin-project-lite",
  "rand",
  "smallvec",
  "sqlparser",
  "tempfile",
  "tokio",
  "tokio-stream",
  "tokio-util",
  "url",
  "uuid",
  "xz2",
+ "zstd 0.12.3+zstd.1.5.2",
 ]
 
 [[package]]
 name = "datafusion-common"
-version = "18.0.0"
+version = "22.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08c58d6714427f52f9815d19debab7adab5bac5b4d2a99d51c250e606acb6cf5"
+checksum = "e82401ce129e601d406012b6d718f8978ba84c386e1c342fa155877120d68824"
 dependencies = [
+ "apache-avro",
  "arrow",
+ "arrow-array",
  "chrono",
  "num_cpus",
  "object_store",
  "parquet",
+ "pyo3",
  "sqlparser",
 ]
 
 [[package]]
+name = "datafusion-execution"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b08b2078aed21a27239cd93f3015e492a58b0d50ebeeaf8d2236cf108ef583ce"
+dependencies = [
+ "dashmap",
+ "datafusion-common",
+ "datafusion-expr",
+ "hashbrown 0.13.2",
+ "log",
+ "object_store",
+ "parking_lot",
+ "rand",
+ "tempfile",
+ "url",
+]
+
+[[package]]
 name = "datafusion-expr"
-version = "18.0.0"
+version = "22.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a32ee054230dd9a57d0bed587406869c4a7814d90154616aff2cb9991c1756f"
+checksum = "16b5b977ce9695fb4c67614266ec57f384fc11e9a9f9b3e6d0e62b9c5a9f2c1f"
 dependencies = [
  "ahash",
  "arrow",
  "datafusion-common",
- "log",
  "sqlparser",
 ]
 
 [[package]]
 name = "datafusion-optimizer"
-version = "18.0.0"
+version = "22.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6de4d144924de29a835feeff8313a81fdc2c7190111301508e09ea59a80edbbc"
+checksum = "a0b2bb9e73ed778d1bc5af63a270f0154bf6eab5099c77668a6362296888e46b"
 dependencies = [
  "arrow",
  "async-trait",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-physical-expr",
  "hashbrown 0.13.2",
+ "itertools",
  "log",
- "regex-syntax",
+ "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "datafusion-physical-expr"
-version = "18.0.0"
+version = "22.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "943e42356f0f6f5ac37ceacd412de9c4d7d8eba1e81b6f724f88699540c7f070"
+checksum = "80cd8ea5ab0a07b1b2a3e17d5909f1b1035bd129ffeeb5c66842a32e682f8f79"
 dependencies = [
  "ahash",
  "arrow",
+ "arrow-array",
  "arrow-buffer",
  "arrow-schema",
  "blake2",
  "blake3",
  "chrono",
  "datafusion-common",
  "datafusion-expr",
  "datafusion-row",
  "half",
  "hashbrown 0.13.2",
  "indexmap",
  "itertools",
  "lazy_static",
  "md-5",
- "num-traits",
  "paste",
+ "petgraph",
  "rand",
  "regex",
  "sha2",
  "unicode-segmentation",
  "uuid",
 ]
 
 [[package]]
+name = "datafusion-python"
+version = "22.0.0"
+source = "git+https://github.com/apache/arrow-datafusion-python.git?rev=9493638#94936380e58a266f5dd5de6b70a06d3aa36fbe22"
+dependencies = [
+ "async-trait",
+ "datafusion",
+ "datafusion-common",
+ "datafusion-expr",
+ "datafusion-optimizer",
+ "datafusion-sql",
+ "datafusion-substrait",
+ "futures",
+ "mimalloc",
+ "object_store",
+ "parking_lot",
+ "pyo3",
+ "pyo3-build-config 0.18.3",
+ "rand",
+ "regex-syntax 0.6.29",
+ "syn 2.0.15",
+ "tokio",
+ "url",
+ "uuid",
+]
+
+[[package]]
 name = "datafusion-row"
-version = "18.0.0"
+version = "22.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a506f5924f8af54e0806a995da0897f8c2b548d492793e045a3896d88d6714a"
+checksum = "2a95d6badab19fd6e9195fdc5209ac0a7e5ce9bcdedc67767b9ffc1b4e645760"
 dependencies = [
  "arrow",
  "datafusion-common",
  "paste",
  "rand",
 ]
 
 [[package]]
 name = "datafusion-sql"
-version = "18.0.0"
+version = "22.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a3d12047a5847f9667f4e2aa8fa2e7d5a6e1094b8e3546d58de492152a50dc7"
+checksum = "37a78f8fc67123c4357e63bc0c87622a2a663d26f074958d749a633d0ecde90f"
 dependencies = [
+ "arrow",
  "arrow-schema",
  "datafusion-common",
  "datafusion-expr",
  "log",
  "sqlparser",
 ]
 
 [[package]]
+name = "datafusion-substrait"
+version = "22.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae6ed64a2005f0d78f2b1b3ec3f8148183f4523d5d364e5367115f8d8a82b7df"
+dependencies = [
+ "async-recursion",
+ "chrono",
+ "datafusion",
+ "itertools",
+ "object_store",
+ "prost",
+ "substrait",
+ "tokio",
+]
+
+[[package]]
 name = "digest"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
 dependencies = [
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
+name = "dirs"
+version = "4.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
+dependencies = [
+ "dirs-sys",
+]
+
+[[package]]
+name = "dirs-sys"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
+dependencies = [
+ "libc",
+ "redox_users",
+ "winapi",
+]
+
+[[package]]
 name = "doc-comment"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
 
 [[package]]
+name = "dunce"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56ce8c6da7551ec6c462cbaf3bfbc75131ebbfa1c944aeaa9dab51ca1c5f0c3b"
+
+[[package]]
+name = "dyn-clone"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
+
+[[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
+name = "encoding_rs"
+version = "0.8.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "env_logger"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85cdab6a89accf66733ad5a1693a4dcced6aeff64602b634530dd73c1f3ee9f0"
 dependencies = [
  "humantime",
  "is-terminal",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
 name = "errno"
-version = "0.2.8"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
@@ -841,118 +1059,142 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
+name = "filetime"
+version = "0.2.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "redox_syscall 0.2.16",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "fixedbitset"
+version = "0.4.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
+
+[[package]]
 name = "flatbuffers"
 version = "23.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77f5399c2c9c50ae9418e522842ad362f61ee48b346ac106807bd355a8a7c619"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "rustc_version",
 ]
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
+name = "fnv"
+version = "1.0.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
+
+[[package]]
 name = "form_urlencoded"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "futures"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "531ac96c6ff5fd7c62263c5e3c67a603af4fcaee2e1a0ae5565ba3a11e69e549"
+checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "164713a5a0dcc3e7b4b1ed7d3b433cabc18025386f9339346e8daf15963cf7ac"
+checksum = "955518d47e09b25bbebc7a18df10b81f0c766eaf4c4f1cccef2fca5f2a4fb5f2"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86d7a0c1aa76363dac491de0ee99faf6941128376f1cf96f07db7603b7de69dd"
+checksum = "4bca583b7e26f571124fe5b7561d49cb2868d79116cfa0eefce955557c6fee8c"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1997dd9df74cdac935c76252744c1ed5794fac083242ea4fe77ef3ed60ba0f83"
+checksum = "ccecee823288125bd88b4d7f565c9e58e41858e47ab72e8ea2d64e93624386e0"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d422fa3cbe3b40dca574ab087abb5bc98258ea57eea3fd6f1fa7162c778b91"
+checksum = "4fff74096e71ed47f8e023204cfd0aa1289cd54ae5430a9523be060cdb849964"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3eb14ed937631bd8b8b8977f2c198443447a8355b6e3ca599f38c975e5a963b6"
+checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ec93083a4aecafb2a80a885c9de1f0ccae9dbd32c2bb54b0c3a65690e0b8d2f2"
+checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
 
 [[package]]
 name = "futures-task"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd65540d33b37b16542a0438c12e6aeead10d4ac5d05bd3f805b8f35ab592879"
+checksum = "76d3d132be6c0e6aa1534069c705a74a5997a356c0dc2f86a47765e5617c5b65"
 
 [[package]]
 name = "futures-util"
-version = "0.3.27"
+version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ef6b17e481503ec85211fed8f39d1970f128935ca1f814cd32ac4a6842e84ab"
+checksum = "26b01e40b772d54cf6c6d721c1d1abd0647a0106a12ecaa1c186273392a69533"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -970,30 +1212,589 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "libc",
- "wasi",
+ "wasi 0.11.0+wasi-snapshot-preview1",
+]
+
+[[package]]
+name = "gix"
+version = "0.43.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c256ea71cc1967faaefdaad15f334146b7c806f12460dcafd3afed845c8c78dd"
+dependencies = [
+ "gix-actor",
+ "gix-attributes",
+ "gix-config",
+ "gix-credentials",
+ "gix-date",
+ "gix-diff",
+ "gix-discover",
+ "gix-features 0.28.1",
+ "gix-glob",
+ "gix-hash 0.10.4",
+ "gix-hashtable",
+ "gix-index",
+ "gix-lock",
+ "gix-mailmap",
+ "gix-object",
+ "gix-odb",
+ "gix-pack",
+ "gix-path",
+ "gix-prompt",
+ "gix-ref",
+ "gix-refspec",
+ "gix-revision",
+ "gix-sec",
+ "gix-tempfile",
+ "gix-traverse",
+ "gix-url",
+ "gix-validate",
+ "gix-worktree",
+ "log",
+ "once_cell",
+ "signal-hook",
+ "smallvec",
+ "thiserror",
+ "unicode-normalization",
+]
+
+[[package]]
+name = "gix-actor"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc22b0cdc52237667c301dd7cdc6ead8f8f73c9f824e9942c8ebd6b764f6c0bf"
+dependencies = [
+ "bstr",
+ "btoi",
+ "gix-date",
+ "itoa",
+ "nom",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-attributes"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2231a25934a240d0a4b6f4478401c73ee81d8be52de0293eedbc172334abf3e1"
+dependencies = [
+ "bstr",
+ "gix-features 0.28.1",
+ "gix-glob",
+ "gix-path",
+ "gix-quote",
+ "thiserror",
+ "unicode-bom",
+]
+
+[[package]]
+name = "gix-bitmap"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55a95f4942360766c3880bdb2b4b57f1ef73b190fc424755e7fdf480430af618"
+dependencies = [
+ "thiserror",
+]
+
+[[package]]
+name = "gix-chunk"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0d39583cab06464b8bf73b3f1707458270f0e7383cb24c3c9c1a16e6f792978"
+dependencies = [
+ "thiserror",
+]
+
+[[package]]
+name = "gix-command"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2c6f75c1e0f924de39e750880a6e21307194bb1ab773efe3c7d2d787277f8ab"
+dependencies = [
+ "bstr",
+]
+
+[[package]]
+name = "gix-config"
+version = "0.20.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7fbad5ce54a8fc997acc50febd89ec80fa6e97cb7f8d0654cb229936407489d8"
+dependencies = [
+ "bstr",
+ "gix-config-value",
+ "gix-features 0.28.1",
+ "gix-glob",
+ "gix-path",
+ "gix-ref",
+ "gix-sec",
+ "log",
+ "memchr",
+ "nom",
+ "once_cell",
+ "smallvec",
+ "thiserror",
+ "unicode-bom",
+]
+
+[[package]]
+name = "gix-config-value"
+version = "0.10.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d09154c0c8677e4da0ec35e896f56ee3e338e741b9599fae06075edd83a4081c"
+dependencies = [
+ "bitflags 1.3.2",
+ "bstr",
+ "gix-path",
+ "libc",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-credentials"
+version = "0.12.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "750b684197374518ea057e0a0594713e07683faa0a3f43c0f93d97f64130ad8d"
+dependencies = [
+ "bstr",
+ "gix-command",
+ "gix-config-value",
+ "gix-path",
+ "gix-prompt",
+ "gix-sec",
+ "gix-url",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-date"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b96271912ce39822501616f177dea7218784e6c63be90d5f36322ff3a722aae2"
+dependencies = [
+ "bstr",
+ "itoa",
+ "thiserror",
+ "time 0.3.20",
+]
+
+[[package]]
+name = "gix-diff"
+version = "0.28.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "103a0fa79b0d438f5ecb662502f052e530ace4fe1fe8e1c83c0c6da76d728e67"
+dependencies = [
+ "gix-hash 0.10.4",
+ "gix-object",
+ "imara-diff",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-discover"
+version = "0.16.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6eba8ba458cb8f4a6c33409b0fe650b1258655175a7ffd1d24fafd3ed31d880b"
+dependencies = [
+ "bstr",
+ "dunce",
+ "gix-hash 0.10.4",
+ "gix-path",
+ "gix-ref",
+ "gix-sec",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-features"
+version = "0.28.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0b76f9a80f6dd7be66442ae86e1f534effad9546676a392acc95e269d0c21c22"
+dependencies = [
+ "crc32fast",
+ "flate2",
+ "gix-hash 0.10.4",
+ "libc",
+ "once_cell",
+ "prodash",
+ "sha1_smol",
+ "thiserror",
+ "walkdir",
+]
+
+[[package]]
+name = "gix-features"
+version = "0.29.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cf69b0f5c701cc3ae22d3204b671907668f6437ca88862d355eaf9bc47a4f897"
+dependencies = [
+ "gix-hash 0.11.1",
+ "libc",
+]
+
+[[package]]
+name = "gix-fs"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9b37a1832f691fdc09910bd267f9a2e413737c1f9ec68c6e31f9e802616278a9"
+dependencies = [
+ "gix-features 0.29.0",
+]
+
+[[package]]
+name = "gix-glob"
+version = "0.5.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93e43efd776bc543f46f0fd0ca3d920c37af71a764a16f2aebd89765e9ff2993"
+dependencies = [
+ "bitflags 1.3.2",
+ "bstr",
+]
+
+[[package]]
+name = "gix-hash"
+version = "0.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2a258595457bc192d1f1c59d0d168a1e34e2be9b97a614e14995416185de41a7"
+dependencies = [
+ "hex",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-hash"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "078eec3ac2808cc03f0bddd2704cb661da5c5dc33b41a9d7947b141d499c7c42"
+dependencies = [
+ "hex",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-hashtable"
+version = "0.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e4e55e40dfd694884f0eb78796c5bddcf2f8b295dace47039099dd7e76534973"
+dependencies = [
+ "gix-hash 0.10.4",
+ "hashbrown 0.13.2",
+ "parking_lot",
+]
+
+[[package]]
+name = "gix-index"
+version = "0.15.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "717ab601ece7921f59fe86849dbe27d44a46ebb883b5885732c4f30df4996177"
+dependencies = [
+ "bitflags 1.3.2",
+ "bstr",
+ "btoi",
+ "filetime",
+ "gix-bitmap",
+ "gix-features 0.28.1",
+ "gix-hash 0.10.4",
+ "gix-lock",
+ "gix-object",
+ "gix-traverse",
+ "itoa",
+ "memmap2",
+ "smallvec",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-lock"
+version = "5.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c693d7f05730fa74a7c467150adc7cea393518410c65f0672f80226b8111555"
+dependencies = [
+ "gix-tempfile",
+ "gix-utils",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-mailmap"
+version = "0.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b66aea5e52875cd4915f4957a6f4b75831a36981e2ec3f5fad9e370e444fe1a"
+dependencies = [
+ "bstr",
+ "gix-actor",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-object"
+version = "0.28.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8df068db9180ee935fbb70504848369e270bdcb576b05c0faa8b9fd3b86fc017"
+dependencies = [
+ "bstr",
+ "btoi",
+ "gix-actor",
+ "gix-features 0.28.1",
+ "gix-hash 0.10.4",
+ "gix-validate",
+ "hex",
+ "itoa",
+ "nom",
+ "smallvec",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-odb"
+version = "0.43.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e83af2e3e36005bfe010927f0dff41fb5acc3e3d89c6f1174135b3a34086bda2"
+dependencies = [
+ "arc-swap",
+ "gix-features 0.28.1",
+ "gix-hash 0.10.4",
+ "gix-object",
+ "gix-pack",
+ "gix-path",
+ "gix-quote",
+ "parking_lot",
+ "tempfile",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-pack"
+version = "0.33.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9401911c7fe032ad7b31c6a6b5be59cb283d1d6c999417a8215056efe6d635f3"
+dependencies = [
+ "clru",
+ "gix-chunk",
+ "gix-diff",
+ "gix-features 0.28.1",
+ "gix-hash 0.10.4",
+ "gix-hashtable",
+ "gix-object",
+ "gix-path",
+ "gix-tempfile",
+ "gix-traverse",
+ "memmap2",
+ "parking_lot",
+ "smallvec",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-path"
+version = "0.7.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32370dce200bb951df013e03dff35b4233fc7a89458642b047629b91734a7e19"
+dependencies = [
+ "bstr",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-prompt"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0f3034d4d935aef2c7bf719aaa54b88c520e82413118d886ae880a31d5bdee57"
+dependencies = [
+ "gix-command",
+ "gix-config-value",
+ "nix",
+ "parking_lot",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-quote"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a282f5a8d9ee0b09ec47390ac727350c48f2f5c76d803cd8da6b3e7ad56e0bcb"
+dependencies = [
+ "bstr",
+ "btoi",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-ref"
+version = "0.27.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e4e909396ed3b176823991ccc391c276ae2a015e54edaafa3566d35123cfac9d"
+dependencies = [
+ "gix-actor",
+ "gix-features 0.28.1",
+ "gix-hash 0.10.4",
+ "gix-lock",
+ "gix-object",
+ "gix-path",
+ "gix-tempfile",
+ "gix-validate",
+ "memmap2",
+ "nom",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-refspec"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aba332462bda2e8efeae4302b39a6ed01ad56ef772fd5b7ef197cf2798294d65"
+dependencies = [
+ "bstr",
+ "gix-hash 0.10.4",
+ "gix-revision",
+ "gix-validate",
+ "smallvec",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-revision"
+version = "0.12.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c6f6ff53f888858afc24bf12628446a14279ceec148df6194481f306f553ad2"
+dependencies = [
+ "bstr",
+ "gix-date",
+ "gix-hash 0.10.4",
+ "gix-hashtable",
+ "gix-object",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-sec"
+version = "0.6.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e8ffa5bf0772f9b01de501c035b6b084cf9b8bb07dec41e3afc6a17336a65f47"
+dependencies = [
+ "bitflags 1.3.2",
+ "dirs",
+ "gix-path",
+ "libc",
+ "windows 0.43.0",
+]
+
+[[package]]
+name = "gix-tempfile"
+version = "5.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d71a0d32f34e71e86586124225caefd78dabc605d0486de580d717653addf182"
+dependencies = [
+ "gix-fs",
+ "libc",
+ "once_cell",
+ "parking_lot",
+ "signal-hook",
+ "signal-hook-registry",
+ "tempfile",
+]
+
+[[package]]
+name = "gix-traverse"
+version = "0.24.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dd9a4a07bb22168dc79c60e1a6a41919d198187ca83d8a5940ad8d7122a45df3"
+dependencies = [
+ "gix-hash 0.10.4",
+ "gix-hashtable",
+ "gix-object",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-url"
+version = "0.16.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6a22b4b32ad14d68f7b7fb6458fa58d44b01797d94c1b8f4db2d9c7b3c366b5"
+dependencies = [
+ "bstr",
+ "gix-features 0.28.1",
+ "gix-path",
+ "home",
+ "thiserror",
+ "url",
+]
+
+[[package]]
+name = "gix-utils"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c10b69beac219acb8df673187a1f07dde2d74092f974fb3f9eb385aeb667c909"
+dependencies = [
+ "fastrand",
+]
+
+[[package]]
+name = "gix-validate"
+version = "0.7.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7bd629d3680773e1785e585d76fd4295b740b559cad9141517300d99a0c8c049"
+dependencies = [
+ "bstr",
+ "thiserror",
+]
+
+[[package]]
+name = "gix-worktree"
+version = "0.15.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "54ec9a000b4f24af706c3cc680c7cda235656cbe3216336522f5692773b8a301"
+dependencies = [
+ "bstr",
+ "gix-attributes",
+ "gix-features 0.28.1",
+ "gix-glob",
+ "gix-hash 0.10.4",
+ "gix-index",
+ "gix-object",
+ "gix-path",
+ "io-close",
+ "thiserror",
 ]
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
+name = "h2"
+version = "0.3.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "17f8a914c2987b688368b5138aa05321db91f4090cf26118185672ad588bce21"
+dependencies = [
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "futures-util",
+ "http",
+ "indexmap",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
 name = "half"
 version = "2.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02b4af3693f1b705df946e9fe5631932443781d0aabb423b62fcd4d73f6d2fd0"
 dependencies = [
  "crunchy",
  "num-traits",
@@ -1032,31 +1833,117 @@
 [[package]]
 name = "hermit-abi"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
+name = "hex"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
+
+[[package]]
+name = "home"
+version = "0.5.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5444c27eef6923071f7ebcc33e3444508466a76f7a2b93da00ed6e19f30c1ddb"
+dependencies = [
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "http"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd6effc99afb63425aff9b05836f029929e345a6148a14b7ecd5ab67af944482"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
+name = "http-body"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+dependencies = [
+ "bytes",
+ "http",
+ "pin-project-lite",
+]
+
+[[package]]
+name = "httparse"
+version = "1.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
+
+[[package]]
+name = "httpdate"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c4a1e36c821dbe04574f602848a19f742f4fb3c98d40449f11bcad18d6b17421"
+
+[[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
+name = "hyper"
+version = "0.14.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ab302d72a6f11a3b910431ff93aae7e773078c769f0a3ef15fb9ec692ed147d4"
+dependencies = [
+ "bytes",
+ "futures-channel",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "httparse",
+ "httpdate",
+ "itoa",
+ "pin-project-lite",
+ "socket2",
+ "tokio",
+ "tower-service",
+ "tracing",
+ "want",
+]
+
+[[package]]
+name = "hyper-rustls"
+version = "0.23.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1788965e61b367cd03a62950836d5cd41560c3577d90e40e0819373194d1661c"
+dependencies = [
+ "http",
+ "hyper",
+ "rustls",
+ "tokio",
+ "tokio-rustls",
+]
+
+[[package]]
 name = "iana-time-zone"
-version = "0.1.54"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c17cc76786e99f8d2f055c11159e7f0091c42474dcc3189fbab96072e873e6d"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "windows",
+ "windows 0.48.0",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
@@ -1072,14 +1959,24 @@
 checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
+name = "imara-diff"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e98c1d0ad70fc91b8b9654b1f33db55e59579d3b3de2bffdced0fdb810570cb8"
+dependencies = [
+ "ahash",
+ "hashbrown 0.12.3",
+]
+
+[[package]]
 name = "indexmap"
 version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown 0.12.3",
@@ -1103,34 +2000,50 @@
 [[package]]
 name = "integer-encoding"
 version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8bb03732005da905c88227371639bf1ad885cc712789c011c31c5fb3ab3ccf02"
 
 [[package]]
+name = "io-close"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9cadcf447f06744f8ce713d2d6239bb5bde2c357a452397a9ed90c625da390bc"
+dependencies = [
+ "libc",
+ "winapi",
+]
+
+[[package]]
 name = "io-lifetimes"
-version = "1.0.9"
+version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09270fd4fa1111bc614ed2246c7ef56239a3063d5be0d1ec3b589c505d400aeb"
+checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "ipnet"
+version = "2.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "12b6ee2129af8d4fb011108c73d99a1b83a85977f23b82460c0ae2e25bb4b57f"
+
+[[package]]
 name = "is-terminal"
-version = "0.4.5"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8687c819457e979cc940d09cb16e42a1bf70aa6b60a549de6d3a62a0ee90c69e"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
  "io-lifetimes",
  "rustix",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
@@ -1230,29 +2143,49 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.142"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+
+[[package]]
+name = "libflate"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "97822bf791bd4d5b403713886a5fbe8bf49520fe78e323b0dc480ca1a03e50b0"
+dependencies = [
+ "adler32",
+ "crc32fast",
+ "libflate_lz77",
+]
+
+[[package]]
+name = "libflate_lz77"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "a52d3a8bfc85f250440e4424db7d857e241a3aebbbe301f3eb606ab15c39acbf"
+dependencies = [
+ "rle-decode-fast",
+]
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
 [[package]]
 name = "libmimalloc-sys"
-version = "0.1.32"
+version = "0.1.33"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43a558e3d911bc3c7bfc8c78bc580b404d6e51c1cefbf656e176a94b49b0df40"
+checksum = "f4ac0e912c8ef1b735e92369695618dc5b1819f5a7bf3f167301a3ba1cea515e"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "link-cplusplus"
@@ -1261,17 +2194,17 @@
 checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.1.4"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
+checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -1331,41 +2264,102 @@
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
+name = "memmap2"
+version = "0.5.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "memoffset"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
-version = "0.1.36"
+version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d88dad3f985ec267a3fcb7a1726f5cb1a7e8cad8b646e70a84f967210df23da"
+checksum = "4e2894987a3459f3ffb755608bd82188f8ed00d0ae077f1edea29c068d639d98"
 dependencies = [
  "libmimalloc-sys",
 ]
 
 [[package]]
+name = "mime"
+version = "0.3.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
+
+[[package]]
+name = "minimal-lexical"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
+
+[[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
+name = "mio"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+dependencies = [
+ "libc",
+ "log",
+ "wasi 0.11.0+wasi-snapshot-preview1",
+ "windows-sys 0.45.0",
+]
+
+[[package]]
+name = "multimap"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
+
+[[package]]
+name = "nix"
+version = "0.26.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfdda3d196821d6af13126e40375cdf7da646a96114af134d5f417a9a1dc8e1a"
+dependencies = [
+ "bitflags 1.3.2",
+ "cfg-if",
+ "libc",
+ "static_assertions",
+]
+
+[[package]]
+name = "nom"
+version = "7.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
+dependencies = [
+ "memchr",
+ "minimal-lexical",
+]
+
+[[package]]
 name = "num"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43db66d1170d347f9a065114077f7dccb00c1b9478c89384490a3425279a4606"
 dependencies = [
  "num-bigint",
  "num-complex",
@@ -1445,26 +2439,43 @@
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
  "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
+name = "num_threads"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "object_store"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1ea8f683b4f89a64181393742c041520a1a87e9775e6b4c0dd5a3281af05fc6"
+checksum = "ec9cd6ca25e796a49fa242876d1c4de36a24a6da5258e9f0bc062dbf5e81c53b"
 dependencies = [
  "async-trait",
+ "base64",
  "bytes",
  "chrono",
  "futures",
  "itertools",
  "parking_lot",
  "percent-encoding",
+ "quick-xml",
+ "rand",
+ "reqwest",
+ "ring",
+ "rustls-pemfile",
+ "serde",
+ "serde_json",
  "snafu",
  "tokio",
  "tracing",
  "url",
  "walkdir",
 ]
 
@@ -1497,24 +2508,24 @@
 name = "parking_lot_core"
 version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "parquet"
-version = "32.0.0"
+version = "36.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23b3d4917209e17e1da5fb07d276da237a42465f0def2b8d5fa5ce0e85855b4c"
+checksum = "321a15f8332645759f29875b07f8233d16ed8ec1b3582223de81625a9f8506b7"
 dependencies = [
  "ahash",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-data",
  "arrow-ipc",
@@ -1532,15 +2543,24 @@
  "num-bigint",
  "paste",
  "seq-macro",
  "snap",
  "thrift",
  "tokio",
  "twox-hash",
- "zstd",
+ "zstd 0.12.3+zstd.1.5.2",
+]
+
+[[package]]
+name = "parse-zoneinfo"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c705f256449c60da65e11ff6626e0c16a0a0b96aaa348de61376b249bc340f41"
+dependencies = [
+ "regex",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f746c4065a8fa3fe23974dd82f15431cc8d40779821001404d10d2e79ca7d79"
@@ -1548,124 +2568,266 @@
 [[package]]
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
+name = "petgraph"
+version = "0.6.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4dd7d28ee937e54fe3080c91faa1c3a46c06de6252988a7f4592ba2310ef22a4"
+dependencies = [
+ "fixedbitset",
+ "indexmap",
+]
+
+[[package]]
+name = "phf"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
+dependencies = [
+ "phf_shared",
+]
+
+[[package]]
+name = "phf_codegen"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a56ac890c5e3ca598bbdeaa99964edb5b0258a583a9eb6ef4e89fc85d9224770"
+dependencies = [
+ "phf_generator",
+ "phf_shared",
+]
+
+[[package]]
+name = "phf_generator"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1181c94580fa345f50f19d738aaa39c0ed30a600d95cb2d3e23f94266f14fbf"
+dependencies = [
+ "phf_shared",
+ "rand",
+]
+
+[[package]]
+name = "phf_shared"
+version = "0.11.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e1fb5f6f826b772a8d4c0394209441e7d37cbbb967ae9c7e0e8134365c9ee676"
+dependencies = [
+ "siphasher",
+]
+
+[[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
+name = "prettyplease"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1ceca8aaf45b5c46ec7ed39fff75f57290368c1846d33d24a122ca81416ab058"
+dependencies = [
+ "proc-macro2",
+ "syn 2.0.15",
+]
+
+[[package]]
 name = "proc-macro-hack"
 version = "0.5.20+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.54"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e472a104799c74b514a57226160104aa483546de37e839ec50e3c2e41dd87534"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
+name = "prodash"
+version = "23.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9516b775656bc3e8985e19cd4b8c0c0de045095074e453d2c0a513b5f978392d"
+
+[[package]]
+name = "prost"
+version = "0.11.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0b82eaa1d779e9a4bc1c3217db8ffbeabaae1dca241bf70183242128d48681cd"
+dependencies = [
+ "bytes",
+ "prost-derive",
+]
+
+[[package]]
+name = "prost-build"
+version = "0.11.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "119533552c9a7ffacc21e099c24a0ac8bb19c2a2a3f363de84cd9b844feab270"
+dependencies = [
+ "bytes",
+ "heck",
+ "itertools",
+ "lazy_static",
+ "log",
+ "multimap",
+ "petgraph",
+ "prost",
+ "prost-types",
+ "regex",
+ "tempfile",
+ "which",
+]
+
+[[package]]
+name = "prost-derive"
+version = "0.11.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e5d2d8d10f3c6ded6da8b05b5fb3b8a5082514344d56c9f871412d29b4e075b4"
+dependencies = [
+ "anyhow",
+ "itertools",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "prost-types"
+version = "0.11.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "213622a1460818959ac1181aaeb2dc9c7f63df720db7d788b3e24eacd1983e13"
+dependencies = [
+ "prost",
+]
+
+[[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
- "pyo3-build-config",
+ "pyo3-build-config 0.18.3",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
+dependencies = [
+ "once_cell",
+ "target-lexicon",
+]
+
+[[package]]
+name = "pyo3-build-config"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
- "pyo3-build-config",
+ "pyo3-build-config 0.18.3",
 ]
 
 [[package]]
 name = "pyo3-log"
-version = "0.8.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9c8b57fe71fb5dcf38970ebedc2b1531cf1c14b1b9b4c560a182a57e115575c"
+checksum = "c94ff6535a6bae58d7d0b85e60d4c53f7f84d0d0aa35d6a28c3f3e70bfe51444"
 dependencies = [
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "quad-rand"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "658fa1faf7a4cc5f057c9ee5ef560f717ad9d8dc66d975267f709624d6e1ab88"
+
+[[package]]
+name = "quick-xml"
+version = "0.28.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ce5e73202a820a31f8a0ee32ada5e21029c81fd9e3ebf668a40832e4219d9d1"
+dependencies = [
+ "memchr",
+ "serde",
+]
+
+[[package]]
 name = "quote"
 version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
@@ -1702,55 +2864,180 @@
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
+]
+
+[[package]]
+name = "redox_syscall"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+dependencies = [
+ "bitflags 1.3.2",
+]
+
+[[package]]
+name = "redox_users"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b033d837a7cf162d7993aded9304e30a83213c648b6e389db233191f891e5c2b"
+dependencies = [
+ "getrandom",
+ "redox_syscall 0.2.16",
+ "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.1",
 ]
 
 [[package]]
+name = "regex-automata"
+version = "0.1.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
+
+[[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
+name = "regex-syntax"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+
+[[package]]
+name = "regress"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d995d590bd8ec096d1893f414bf3f5e8b0ee4c9eed9a5642b9766ef2c8e2e8e9"
+dependencies = [
+ "hashbrown 0.13.2",
+ "memchr",
+]
+
+[[package]]
+name = "reqwest"
+version = "0.11.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "13293b639a097af28fc8a90f22add145a9c954e49d77da06263d58cf44d5fb91"
+dependencies = [
+ "base64",
+ "bytes",
+ "encoding_rs",
+ "futures-core",
+ "futures-util",
+ "h2",
+ "http",
+ "http-body",
+ "hyper",
+ "hyper-rustls",
+ "ipnet",
+ "js-sys",
+ "log",
+ "mime",
+ "once_cell",
+ "percent-encoding",
+ "pin-project-lite",
+ "rustls",
+ "rustls-pemfile",
+ "serde",
+ "serde_json",
+ "serde_urlencoded",
+ "tokio",
+ "tokio-rustls",
+ "tokio-util",
+ "tower-service",
+ "url",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "wasm-streams",
+ "web-sys",
+ "webpki-roots",
+ "winreg",
+]
+
+[[package]]
+name = "ring"
+version = "0.16.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3053cf52e236a3ed746dfc745aa9cacf1b791d846bdaf412f60a8d7d6e17c8fc"
+dependencies = [
+ "cc",
+ "libc",
+ "once_cell",
+ "spin",
+ "untrusted",
+ "web-sys",
+ "winapi",
+]
+
+[[package]]
+name = "rle-decode-fast"
+version = "1.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3582f63211428f83597b51b2ddb88e2a91a9d52d12831f9d08f5e624e8977422"
+
+[[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.36.11"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db4165c9963ab29e422d6c26fbc1d37f15bace6b2810221f9d925023480fcf0e"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
+name = "rustls"
+version = "0.20.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fff78fc74d175294f4e83b28343315ffcfb114b156f0185e9741cb5570f50e2f"
+dependencies = [
+ "log",
+ "ring",
+ "sct",
+ "webpki",
+]
+
+[[package]]
+name = "rustls-pemfile"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
+dependencies = [
+ "base64",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
@@ -1767,66 +3054,192 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
+name = "schemars"
+version = "0.8.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "02c613288622e5f0c3fdc5dbd4db1c5fbe752746b1d1a56a0630b78fd00de44f"
+dependencies = [
+ "dyn-clone",
+ "schemars_derive",
+ "serde",
+ "serde_json",
+]
+
+[[package]]
+name = "schemars_derive"
+version = "0.8.12"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "109da1e6b197438deb6db99952990c7f959572794b80ff93707d55a232545e7c"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "serde_derive_internals",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "scratch"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
 
 [[package]]
+name = "sct"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
+dependencies = [
+ "ring",
+ "untrusted",
+]
+
+[[package]]
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "seq-macro"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6b44e8fc93a14e66336d230954dda83d18b4605ccace8fe09bc7514a71ad0bc"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+dependencies = [
+ "serde_derive",
+]
+
+[[package]]
+name = "serde_derive"
+version = "1.0.160"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
+
+[[package]]
+name = "serde_derive_internals"
+version = "0.26.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
+dependencies = [
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
+name = "serde_tokenstream"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "797ba1d80299b264f3aac68ab5d12e5825a561749db4df7cd7c8083900c5d4e9"
+dependencies = [
+ "proc-macro2",
+ "serde",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "serde_urlencoded"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
 dependencies = [
+ "form_urlencoded",
+ "itoa",
+ "ryu",
+ "serde",
+]
+
+[[package]]
+name = "serde_yaml"
+version = "0.9.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d9d684e3ec7de3bf5466b32bd75303ac16f0736426e5a4e0d6e489559ce1249c"
+dependencies = [
+ "indexmap",
  "itoa",
  "ryu",
  "serde",
+ "unsafe-libyaml",
 ]
 
 [[package]]
+name = "sha1_smol"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ae1a47186c03a32177042e55dbc5fd5aee900b8e0069a8d70fba96a9375cd012"
+
+[[package]]
 name = "sha2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
+name = "signal-hook"
+version = "0.3.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "732768f1176d21d09e076c23a93123d40bba92d50c4058da34d45c8de8e682b9"
+dependencies = [
+ "libc",
+ "signal-hook-registry",
+]
+
+[[package]]
+name = "signal-hook-registry"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+dependencies = [
+ "libc",
+]
+
+[[package]]
+name = "siphasher"
+version = "0.3.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7bd3e3206899af3f8b12af284fafc038cc1dc2b41d1b89dd17297221c5d225de"
+
+[[package]]
 name = "slab"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
@@ -1862,18 +3275,34 @@
 [[package]]
 name = "snap"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5e9f0ab6ef7eb7353d9119c170a436d1bf248eea575ac42d19d12f4e34130831"
 
 [[package]]
+name = "socket2"
+version = "0.4.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "64a4a911eed85daf18834cfaa86a79b7d266ff93ff5ba14005426219480ed662"
+dependencies = [
+ "libc",
+ "winapi",
+]
+
+[[package]]
+name = "spin"
+version = "0.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6e63cff320ae2c57904679ba7cb63280a3dc4613885beafb148ee7bf9aa9042d"
+
+[[package]]
 name = "sqlparser"
-version = "0.30.0"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db67dc6ef36edb658196c3fef0464a80b53dbbc194a904e81f9bd4190f9ecc5b"
+checksum = "0366f270dbabb5cc2e4c88427dc4c08bba144f81e32fbd459a013f26a4d16aa0"
 dependencies = [
  "log",
  "sqlparser_derive",
 ]
 
 [[package]]
 name = "sqlparser_derive"
@@ -1908,14 +3337,36 @@
  "proc-macro2",
  "quote",
  "rustversion",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "substrait"
+version = "0.7.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e3ae64fb7ad0670c7d6d53d57b1b91beb2212afc30e164cc8edb02d6b2cff32a"
+dependencies = [
+ "gix",
+ "heck",
+ "prettyplease",
+ "prost",
+ "prost-build",
+ "prost-types",
+ "schemars",
+ "semver",
+ "serde",
+ "serde_json",
+ "serde_yaml",
+ "syn 2.0.15",
+ "typify",
+ "walkdir",
+]
+
+[[package]]
 name = "subtle"
 version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
 
 [[package]]
 name = "syn"
@@ -1926,63 +3377,123 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.11"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21e3787bb71465627110e7d87ed4faaa36c1f61042ee67badb9e2ef173accc40"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.6"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
-version = "3.4.0"
+version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
+checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall",
+ "redox_syscall 0.3.5",
  "rustix",
- "windows-sys 0.42.0",
+ "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
+name = "thiserror"
+version = "1.0.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
+dependencies = [
+ "thiserror-impl",
+]
+
+[[package]]
+name = "thiserror-impl"
+version = "1.0.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.15",
+]
+
+[[package]]
 name = "thrift"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e54bc85fc7faa8bc175c4bab5b92ba8d9a3ce893d0e9f42cc455c8ab16a9e09"
 dependencies = [
  "byteorder",
  "integer-encoding",
  "ordered-float",
 ]
 
 [[package]]
+name = "time"
+version = "0.1.45"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
+dependencies = [
+ "libc",
+ "wasi 0.10.0+wasi-snapshot-preview1",
+ "winapi",
+]
+
+[[package]]
+name = "time"
+version = "0.3.20"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+dependencies = [
+ "itoa",
+ "libc",
+ "num_threads",
+ "serde",
+ "time-core",
+ "time-macros",
+]
+
+[[package]]
+name = "time-core"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+
+[[package]]
+name = "time-macros"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+dependencies = [
+ "time-core",
+]
+
+[[package]]
 name = "tiny-keccak"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c9d3793400a45f954c52e73d068316d76b6f4e36977e3fcebb13a2721e80237"
 dependencies = [
  "crunchy",
 ]
@@ -2000,117 +3511,205 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.27.0"
+version = "1.28.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
+checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
 dependencies = [
  "autocfg",
  "bytes",
+ "libc",
+ "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
+ "socket2",
  "tokio-macros",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
-version = "2.0.0"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "61a573bdc87985e9d6ddeed1b3d864e8a302c847e40d647746df2f1de209d1ce"
+checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.11",
+ "syn 2.0.15",
+]
+
+[[package]]
+name = "tokio-rustls"
+version = "0.23.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c43ee83903113e03984cb9e5cebe6c04a5116269e900e3ddba8f068a62adda59"
+dependencies = [
+ "rustls",
+ "tokio",
+ "webpki",
 ]
 
 [[package]]
 name = "tokio-stream"
-version = "0.1.12"
+version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8fb52b74f05dbf495a8fba459fdc331812b96aa086d9eb78101fa0d4569c3313"
+checksum = "397c988d37662c7dda6d2208364a706264bf3d6138b11d436cbac0ad38832842"
 dependencies = [
  "futures-core",
  "pin-project-lite",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.7"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
+ "tracing",
 ]
 
 [[package]]
+name = "tower-service"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
+
+[[package]]
 name = "tracing"
 version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
  "cfg-if",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
+name = "try-lock"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+
+[[package]]
 name = "twox-hash"
 version = "1.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
 dependencies = [
  "cfg-if",
  "static_assertions",
 ]
 
 [[package]]
+name = "typed-builder"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "89851716b67b937e393b3daa8423e67ddfc4bbbf1654bcf05488e95e0828db0c"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
+name = "typify"
+version = "0.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "30bfde96849e25d7feef1bbf652e9cfc51deb63203fdc07b115b8bc3bcfe20b9"
+dependencies = [
+ "typify-impl",
+ "typify-macro",
+]
+
+[[package]]
+name = "typify-impl"
+version = "0.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95d27d749378ceab6ec22188ed7ad102205c89ddb92ab662371c850ffc71aa1a"
+dependencies = [
+ "heck",
+ "log",
+ "proc-macro2",
+ "quote",
+ "regress",
+ "schemars",
+ "serde_json",
+ "syn 1.0.109",
+ "thiserror",
+ "unicode-ident",
+]
+
+[[package]]
+name = "typify-macro"
+version = "0.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "35db6fc2bd9220ecdac6eeb88158824b83610de3dda0c6d0f2142b49efd858b0"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "schemars",
+ "serde",
+ "serde_json",
+ "serde_tokenstream",
+ "syn 1.0.109",
+ "typify-impl",
+]
+
+[[package]]
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
+name = "unicode-bom"
+version = "1.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "63ec69f541d875b783ca40184d655f2927c95f0bffd486faa83cd3ac3529ec32"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
 
 [[package]]
 name = "unicode-normalization"
@@ -2136,31 +3735,44 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "unsafe-libyaml"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1865806a559042e51ab5414598446a5871b561d21b6764f2eabb0dd481d880a6"
+
+[[package]]
+name = "untrusted"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a156c684c91ea7d62626509bce3cb4e1d9ed5c4d978f7b4352658f96a4c26b4a"
+
+[[package]]
 name = "url"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.0"
+version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1674845326ee10d37ca60470760d4288a6f80f304007d92e5c53bab78c9cfd79"
+checksum = "4dad5567ad0cf5b760e5665964bec1b47dfd077ba8a2544b513f3556d3d239a2"
 dependencies = [
  "getrandom",
+ "serde",
 ]
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
@@ -2172,14 +3784,30 @@
 checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
+name = "want"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
+dependencies = [
+ "log",
+ "try-lock",
+]
+
+[[package]]
+name = "wasi"
+version = "0.10.0+wasi-snapshot-preview1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a143597ca7c7793eff794def352d41792a93c481eb1042423ff7ff72ba2c31f"
+
+[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
@@ -2203,14 +3831,26 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
+name = "wasm-bindgen-futures"
+version = "0.4.34"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+dependencies = [
+ "cfg-if",
+ "js-sys",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
@@ -2232,14 +3872,67 @@
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
 
 [[package]]
+name = "wasm-streams"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6bbae3363c08332cadccd13b67db371814cd214c2524020932f0804b8cf7c078"
+dependencies = [
+ "futures-util",
+ "js-sys",
+ "wasm-bindgen",
+ "wasm-bindgen-futures",
+ "web-sys",
+]
+
+[[package]]
+name = "web-sys"
+version = "0.3.61"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "webpki"
+version = "0.22.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f095d78192e208183081cc07bc5515ef55216397af48b873e5edcd72637fa1bd"
+dependencies = [
+ "ring",
+ "untrusted",
+]
+
+[[package]]
+name = "webpki-roots"
+version = "0.22.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6c71e40d7d2c34a5106301fb632274ca37242cd0c9d3e64dbece371a40a2d87"
+dependencies = [
+ "webpki",
+]
+
+[[package]]
+name = "which"
+version = "4.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2441c784c52b289a054b7201fc93253e288f094e2f4be9058343127c4226a269"
+dependencies = [
+ "either",
+ "libc",
+ "once_cell",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -2264,133 +3957,248 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
-version = "0.46.0"
+version = "0.43.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
+checksum = "04662ed0e3e5630dfa9b26e4cb823b817f1a9addda855d973a9458c236556244"
 dependencies = [
- "windows-targets",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
+name = "winreg"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80d0f4e272c85def139476380b12f9ac60926689dd2e01d4923222f40580869d"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
 name = "xz2"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "388c44dc09d76f1536602ead6d325eb532f5c122f17782bd57fb47baeeb767e2"
 dependencies = [
  "lzma-sys",
 ]
 
 [[package]]
+name = "zerocopy"
+version = "0.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "332f188cc1bcf1fe1064b8c58d150f497e697f49774aa846f2dc949d9a25f236"
+dependencies = [
+ "byteorder",
+ "zerocopy-derive",
+]
+
+[[package]]
+name = "zerocopy-derive"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6505e6815af7de1746a08f69c69606bb45695a17149517680f3b2149713b19a3"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "zstd"
+version = "0.11.2+zstd.1.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "20cc960326ece64f010d2d2107537f26dc589a6573a316bd5b1dba685fa5fde4"
+dependencies = [
+ "zstd-safe 5.0.2+zstd.1.5.2",
+]
+
+[[package]]
 name = "zstd"
 version = "0.12.3+zstd.1.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
 dependencies = [
- "zstd-safe",
+ "zstd-safe 6.0.5+zstd.1.5.4",
+]
+
+[[package]]
+name = "zstd-safe"
+version = "5.0.2+zstd.1.5.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1d2a5585e04f9eea4b2a3d1eca508c4dee9592a89ef6f450c11719da0726f4db"
+dependencies = [
+ "libc",
+ "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.4+zstd.1.5.4"
+version = "6.0.5+zstd.1.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7afb4b54b8910cf5447638cb54bf4e8a65cbedd783af98b98c62ffe91f185543"
+checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.7+zstd.1.5.4"
+version = "2.0.8+zstd.1.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94509c3ba2fe55294d752b79842c530ccfab760192521df74a081a78d2b3c7f5"
+checksum = "5556e6ee25d32df2586c098bbfa278803692a20d0ab9565e049480d52707ec8c"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
 ]
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/dialect.rs` & `dask_sql-2023.6.0/dask_planner/src/dialect.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use core::{iter::Peekable, str::Chars};
 
-use datafusion_sql::sqlparser::{
+use datafusion_python::datafusion_sql::sqlparser::{
     ast::{Expr, Function, FunctionArg, FunctionArgExpr, Ident, ObjectName, Value},
     dialect::Dialect,
     keywords::Keyword,
     parser::{Parser, ParserError},
     tokenizer::Token,
 };
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/error.rs` & `dask_sql-2023.6.0/dask_planner/src/error.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 use std::fmt::{Display, Formatter};
 
-use datafusion_common::DataFusionError;
-use datafusion_sql::sqlparser::{parser::ParserError, tokenizer::TokenizerError};
+use datafusion_python::{
+    datafusion_common::DataFusionError,
+    datafusion_sql::sqlparser::{parser::ParserError, tokenizer::TokenizerError},
+};
 use pyo3::PyErr;
 
 pub type Result<T> = std::result::Result<T, DaskPlannerError>;
 
 #[derive(Debug)]
 pub enum DaskPlannerError {
     DataFusionError(DataFusionError),
     ParserError(ParserError),
     TokenizerError(TokenizerError),
     Internal(String),
+    InvalidIOFilter(String),
 }
 
 impl Display for DaskPlannerError {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         match self {
             Self::DataFusionError(e) => write!(f, "DataFusion Error: {e}"),
             Self::ParserError(e) => write!(f, "SQL Parser Error: {e}"),
             Self::TokenizerError(e) => write!(f, "SQL Tokenizer Error: {e}"),
             Self::Internal(e) => write!(f, "Internal Error: {e}"),
+            Self::InvalidIOFilter(e) => write!(f, "Invalid pyarrow filter: {e} encountered. Defaulting to Dask CPU/GPU bound task operation"),
         }
     }
 }
 
 impl From<TokenizerError> for DaskPlannerError {
     fn from(err: TokenizerError) -> Self {
         Self::TokenizerError(err)
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/expression.rs` & `dask_sql-2023.6.0/dask_planner/src/expression.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-use std::{convert::From, sync::Arc};
+use std::{borrow::Cow, convert::From, sync::Arc};
 
-use datafusion::arrow::datatypes::DataType;
-use datafusion_common::{Column, DFField, DFSchema, ScalarValue};
-use datafusion_expr::{
-    expr::{AggregateFunction, BinaryExpr, Cast, Sort, TryCast, WindowFunction},
-    lit,
-    utils::exprlist_to_fields,
-    Between,
-    BuiltinScalarFunction,
-    Case,
-    Expr,
-    GetIndexedField,
-    Like,
-    LogicalPlan,
-    Operator,
+use datafusion_python::{
+    datafusion::arrow::datatypes::DataType,
+    datafusion_common::{Column, DFField, DFSchema, ScalarValue},
+    datafusion_expr::{
+        expr::{AggregateFunction, BinaryExpr, Cast, Sort, TryCast, WindowFunction},
+        lit,
+        utils::exprlist_to_fields,
+        Between,
+        BuiltinScalarFunction,
+        Case,
+        Expr,
+        GetIndexedField,
+        Like,
+        LogicalPlan,
+        Operator,
+    },
+    datafusion_sql::TableReference,
 };
 use pyo3::prelude::*;
 
 use crate::{
     error::{DaskPlannerError, Result},
     sql::{
         exceptions::{py_runtime_err, py_type_err},
@@ -117,14 +120,15 @@
             | Expr::GroupingSet(..)
             | Expr::IsTrue(..)
             | Expr::IsFalse(..)
             | Expr::IsUnknown(_)
             | Expr::IsNotTrue(..)
             | Expr::IsNotFalse(..)
             | Expr::Placeholder { .. }
+            | Expr::OuterReferenceColumn(_, _)
             | Expr::IsNotUnknown(_) => RexType::Call,
             Expr::ScalarSubquery(..) => RexType::ScalarSubquery,
         }
     }
 }
 
 macro_rules! extract_scalar_value {
@@ -180,21 +184,50 @@
                     schema.merge(plan.schema().as_ref());
                 }
                 let name = get_expr_name(&self.expr).map_err(py_runtime_err)?;
                 schema
                     .index_of_column(&Column::from_qualified_name(name.clone()))
                     .or_else(|_| {
                         // Handles cases when from_qualified_name doesn't format the Column correctly.
-                        // Here, we split the name string and grab the relation/table names
-                        let split_name: Vec<&str> = name.split('.').collect();
-                        let relation = &split_name.first();
-                        let table = &split_name.get(1);
+                        // "name" will always contain the name of the column. Anything in addition to
+                        // that will be separated by a '.' and should be further referenced.
+                        let parts = name.split('.').collect::<Vec<&str>>();
+                        let tbl_reference = match parts.len() {
+                            // Single element means name contains just the column name so no TableReference
+                            1 => None,
+                            // Tablename.column_name
+                            2 => Some(
+                                TableReference::Bare {
+                                    table: Cow::Borrowed(parts[0]),
+                                }
+                                .to_owned_reference(),
+                            ),
+                            // Schema_name.table_name.column_name
+                            3 => Some(
+                                TableReference::Partial {
+                                    schema: Cow::Borrowed(parts[0]),
+                                    table: Cow::Borrowed(parts[1]),
+                                }
+                                .to_owned_reference(),
+                            ),
+                            // catalog_name.schema_name.table_name.column_name
+                            4 => Some(
+                                TableReference::Full {
+                                    catalog: Cow::Borrowed(parts[0]),
+                                    schema: Cow::Borrowed(parts[1]),
+                                    table: Cow::Borrowed(parts[2]),
+                                }
+                                .to_owned_reference(),
+                            ),
+                            _ => None,
+                        };
+
                         let col = Column {
-                            relation: Some(relation.unwrap().to_string()),
-                            name: table.unwrap().to_string(),
+                            relation: tbl_reference.clone(),
+                            name: parts[parts.len() - 1].to_string(),
                         };
                         schema.index_of_column(&col).map_err(py_runtime_err)
                     })
             }
             _ => Err(py_runtime_err(
                 "We need a valid LogicalPlan instance to get the Expr's index in the schema",
             )),
@@ -221,14 +254,15 @@
             | Expr::InSubquery { .. }
             | Expr::ScalarUDF { .. }
             | Expr::AggregateUDF { .. }
             | Expr::Exists { .. }
             | Expr::ScalarSubquery(..)
             | Expr::QualifiedWildcard { .. }
             | Expr::Not(..)
+            | Expr::OuterReferenceColumn(_, _)
             | Expr::GroupingSet(..) => self.expr.variant_name(),
             Expr::ScalarVariable(..)
             | Expr::IsNotNull(..)
             | Expr::Negative(..)
             | Expr::GetIndexedField { .. }
             | Expr::IsNull(..)
             | Expr::IsTrue(_)
@@ -315,22 +349,32 @@
                 expr,
                 when_then_expr,
                 else_expr,
             }) => {
                 let mut operands: Vec<PyExpr> = Vec::new();
 
                 if let Some(e) = expr {
-                    operands.push(PyExpr::from(*e.clone(), self.input_plan.clone()));
+                    for (when, then) in when_then_expr {
+                        operands.push(PyExpr::from(
+                            Expr::BinaryExpr(BinaryExpr::new(
+                                Box::new(*e.clone()),
+                                Operator::Eq,
+                                Box::new(*when.clone()),
+                            )),
+                            self.input_plan.clone(),
+                        ));
+                        operands.push(PyExpr::from(*then.clone(), self.input_plan.clone()));
+                    }
+                } else {
+                    for (when, then) in when_then_expr {
+                        operands.push(PyExpr::from(*when.clone(), self.input_plan.clone()));
+                        operands.push(PyExpr::from(*then.clone(), self.input_plan.clone()));
+                    }
                 };
 
-                for (when, then) in when_then_expr {
-                    operands.push(PyExpr::from(*when.clone(), self.input_plan.clone()));
-                    operands.push(PyExpr::from(*then.clone(), self.input_plan.clone()));
-                }
-
                 if let Some(e) = else_expr {
                     operands.push(PyExpr::from(*e.clone(), self.input_plan.clone()));
                 };
 
                 Ok(operands)
             }
             Expr::InList { expr, list, .. } => {
@@ -367,14 +411,15 @@
                 PyExpr::from(*expr.clone(), self.input_plan.clone()),
                 PyExpr::from(*low.clone(), self.input_plan.clone()),
                 PyExpr::from(*high.clone(), self.input_plan.clone()),
             ]),
 
             // Currently un-support/implemented Expr types for Rex Call operations
             Expr::GroupingSet(..)
+            | Expr::OuterReferenceColumn(_, _)
             | Expr::Wildcard
             | Expr::QualifiedWildcard { .. }
             | Expr::ScalarSubquery(..)
             | Expr::Placeholder { .. }
             | Expr::Exists { .. } => Err(py_runtime_err(format!(
                 "Unimplemented Expr type: {}",
                 self.expr
@@ -561,14 +606,37 @@
                     "Catch all triggered in get_type; {:?}",
                     &self.expr
                 )))
             }
         }))
     }
 
+    /// Gets the precision/scale represented by the Expression's decimal datatype
+    #[pyo3(name = "getPrecisionScale")]
+    pub fn get_precision_scale(&self) -> PyResult<(u8, i8)> {
+        Ok(match &self.expr {
+            Expr::Cast(Cast { expr: _, data_type }) => match data_type {
+                DataType::Decimal128(precision, scale) | DataType::Decimal256(precision, scale) => {
+                    (*precision, *scale)
+                }
+                _ => {
+                    return Err(py_type_err(format!(
+                        "Catch all triggered for Cast in get_precision_scale; {data_type:?}"
+                    )))
+                }
+            },
+            _ => {
+                return Err(py_type_err(format!(
+                    "Catch all triggered in get_precision_scale; {:?}",
+                    &self.expr
+                )))
+            }
+        })
+    }
+
     #[pyo3(name = "getFilterExpr")]
     pub fn get_filter_expr(&self) -> PyResult<Option<PyExpr>> {
         // TODO refactor to avoid duplication
         match &self.expr {
             Expr::Alias(expr, _) => match expr.as_ref() {
                 Expr::AggregateFunction(AggregateFunction { filter, .. })
                 | Expr::AggregateUDF { filter, .. } => match filter {
@@ -699,14 +767,29 @@
                 Ok(Some((days, ms)))
             }
             ScalarValue::IntervalDayTime(None) => Ok(None),
             other => Err(unexpected_literal_value(other)),
         }
     }
 
+    #[pyo3(name = "getIntervalMonthDayNanoValue")]
+    pub fn interval_month_day_nano_value(&self) -> PyResult<Option<(i32, i32, i64)>> {
+        match self.get_scalar_value()? {
+            ScalarValue::IntervalMonthDayNano(Some(iv)) => {
+                let interval = *iv as u128;
+                let months = (interval >> 32) as i32;
+                let days = (interval >> 64) as i32;
+                let ns = interval as i64;
+                Ok(Some((months, days, ns)))
+            }
+            ScalarValue::IntervalMonthDayNano(None) => Ok(None),
+            other => Err(unexpected_literal_value(other)),
+        }
+    }
+
     #[pyo3(name = "isNegated")]
     pub fn is_negated(&self) -> PyResult<bool> {
         match &self.expr {
             Expr::Between(Between { negated, .. })
             | Expr::Exists { negated, .. }
             | Expr::InList { negated, .. }
             | Expr::InSubquery { negated, .. } => Ok(*negated),
@@ -813,16 +896,18 @@
             Ok(fields[0].clone())
         }
     }
 }
 
 #[cfg(test)]
 mod test {
-    use datafusion_common::{Column, ScalarValue};
-    use datafusion_expr::Expr;
+    use datafusion_python::{
+        datafusion_common::{Column, ScalarValue},
+        datafusion_expr::Expr,
+    };
 
     use crate::{error::Result, expression::PyExpr};
 
     #[test]
     fn get_value_u32() -> Result<()> {
         test_get_value(ScalarValue::UInt32(None))?;
         test_get_value(ScalarValue::UInt32(Some(123)))
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/lib.rs` & `dask_sql-2023.6.0/dask_planner/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 use log::debug;
-use mimalloc::MiMalloc;
 use pyo3::prelude::*;
 
 mod dialect;
 mod error;
 mod expression;
 mod parser;
 mod sql;
 
-#[global_allocator]
-static GLOBAL: MiMalloc = MiMalloc;
-
 /// Low-level DataFusion internal package.
 ///
 /// The higher-level public API is defined in pure python files under the
 /// dask_planner directory.
 #[pymodule]
 #[pyo3(name = "rust")]
 fn rust(py: Python, m: &PyModule) -> PyResult<()> {
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/parser.rs` & `dask_sql-2023.6.0/dask_planner/src/parser.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 //! SQL Parser
 //!
 //! Declares a SQL parser based on sqlparser that handles custom formats that we need.
 
 use std::collections::VecDeque;
 
-use datafusion_sql::sqlparser::{
+use datafusion_python::datafusion_sql::sqlparser::{
     ast::{Expr, Ident, SelectItem, Statement as SQLStatement, UnaryOperator, Value},
     dialect::{keywords::Keyword, Dialect},
     parser::{Parser, ParserError},
     tokenizer::{Token, TokenWithLocation, Tokenizer},
 };
 use pyo3::prelude::*;
 
@@ -1091,15 +1091,16 @@
                             self.parser.prev_token();
                             self.parser.prev_token();
                         }
 
                         // True if TABLE and False if VIEW
                         if is_table {
                             Ok(DaskStatement::Statement(Box::from(
-                                self.parser.parse_create_table(or_replace, false, None)?,
+                                self.parser
+                                    .parse_create_table(or_replace, false, None, false)?,
                             )))
                         } else {
                             self.parser.prev_token();
                             Ok(DaskStatement::Statement(Box::from(
                                 self.parser.parse_create_view(or_replace)?,
                             )))
                         }
@@ -1138,15 +1139,16 @@
                     // Go back three tokens if IF NOT EXISTS was consumed
                     self.parser.prev_token();
                     self.parser.prev_token();
                     self.parser.prev_token();
                 }
                 // use the native parser
                 Ok(DaskStatement::Statement(Box::from(
-                    self.parser.parse_create_table(or_replace, false, None)?,
+                    self.parser
+                        .parse_create_table(or_replace, false, None, false)?,
                 )))
             }
         }
     }
 
     /// Parse Dask-SQL EXPORT MODEL statement
     fn parse_export_model(&mut self) -> Result<DaskStatement, ParserError> {
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/column.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/column.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_common::Column;
+use datafusion_python::datafusion_common::Column;
 use pyo3::prelude::*;
 
 #[pyclass(name = "Column", module = "dask_planner", subclass)]
 #[derive(Debug, Clone)]
 pub struct PyColumn {
     /// Original Column instance
     pub(crate) column: Column,
@@ -20,15 +20,15 @@
     }
 }
 
 #[pymethods]
 impl PyColumn {
     #[pyo3(name = "getRelation")]
     pub fn relation(&self) -> String {
-        self.column.relation.clone().unwrap()
+        self.column.relation.clone().unwrap().to_string()
     }
 
     #[pyo3(name = "getName")]
     pub fn name(&self) -> String {
         self.column.name.clone()
     }
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/exceptions.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/exceptions.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/function.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/function.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use std::collections::HashMap;
 
-use datafusion::arrow::datatypes::DataType;
+use datafusion_python::datafusion::arrow::datatypes::DataType;
 use pyo3::prelude::*;
 
 use super::types::PyDataType;
 
 #[pyclass(name = "DaskFunction", module = "dask_planner", subclass)]
 #[derive(Debug, Clone)]
 pub struct DaskFunction {
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/aggregate.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/aggregate.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_expr::{
+use datafusion_python::datafusion_expr::{
     expr::AggregateFunction,
     logical_plan::{Aggregate, Distinct},
     Expr,
     LogicalPlan,
 };
 use pyo3::prelude::*;
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/alter_schema.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_schema.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,45 @@
-use std::{any::Any, fmt, sync::Arc};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
 
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{
-    logical_plan::{Extension, UserDefinedLogicalNode},
-    Expr,
-    LogicalPlan,
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan},
 };
 use fmt::Debug;
 use pyo3::prelude::*;
 
 use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
-pub struct AlterSchemaPlanNode {
+#[derive(Clone, PartialEq)]
+pub struct DropSchemaPlanNode {
     pub schema: DFSchemaRef,
-    pub old_schema_name: String,
-    pub new_schema_name: String,
+    pub schema_name: String,
+    pub if_exists: bool,
 }
 
-impl Debug for AlterSchemaPlanNode {
+impl Debug for DropSchemaPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
-impl UserDefinedLogicalNode for AlterSchemaPlanNode {
+impl Hash for DropSchemaPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.schema_name.hash(state);
+        self.if_exists.hash(state);
+    }
+}
+
+impl UserDefinedLogicalNode for DropSchemaPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
     }
@@ -36,73 +47,80 @@
     fn schema(&self) -> &DFSchemaRef {
         &self.schema
     }
 
     fn expressions(&self) -> Vec<Expr> {
         // there is no need to expose any expressions here since DataFusion would
         // not be able to do anything with expressions that are specific to
-        // ALTER SCHEMA {table_name}
+        // DROP SCHEMA
         vec![]
     }
 
     fn fmt_for_explain(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        write!(
-            f,
-            "Alter Schema: old_schema_name: {:?}, new_schema_name: {:?}",
-            self.old_schema_name, self.new_schema_name
-        )
+        write!(f, "DropSchema: schema_name={}", self.schema_name)
     }
 
     fn from_template(
         &self,
         _exprs: &[Expr],
         _inputs: &[LogicalPlan],
     ) -> Arc<dyn UserDefinedLogicalNode> {
-        Arc::new(AlterSchemaPlanNode {
+        Arc::new(DropSchemaPlanNode {
             schema: Arc::new(DFSchema::empty()),
-            old_schema_name: self.old_schema_name.clone(),
-            new_schema_name: self.new_schema_name.clone(),
+            schema_name: self.schema_name.clone(),
+            if_exists: self.if_exists,
         })
     }
+
+    fn name(&self) -> &str {
+        "DropSchema"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
-#[pyclass(name = "AlterSchema", module = "dask_planner", subclass)]
-pub struct PyAlterSchema {
-    pub(crate) alter_schema: AlterSchemaPlanNode,
+#[pyclass(name = "DropSchema", module = "dask_planner", subclass)]
+pub struct PyDropSchema {
+    pub(crate) drop_schema: DropSchemaPlanNode,
 }
 
 #[pymethods]
-impl PyAlterSchema {
-    #[pyo3(name = "getOldSchemaName")]
-    fn get_old_schema_name(&self) -> PyResult<String> {
-        Ok(self.alter_schema.old_schema_name.clone())
+impl PyDropSchema {
+    #[pyo3(name = "getSchemaName")]
+    fn get_schema_name(&self) -> PyResult<String> {
+        Ok(self.drop_schema.schema_name.clone())
     }
 
-    #[pyo3(name = "getNewSchemaName")]
-    fn get_new_schema_name(&self) -> PyResult<String> {
-        Ok(self.alter_schema.new_schema_name.clone())
+    #[pyo3(name = "getIfExists")]
+    fn get_if_exists(&self) -> PyResult<bool> {
+        Ok(self.drop_schema.if_exists)
     }
 }
 
-impl TryFrom<logical::LogicalPlan> for PyAlterSchema {
+impl TryFrom<logical::LogicalPlan> for PyDropSchema {
     type Error = PyErr;
 
     fn try_from(logical_plan: logical::LogicalPlan) -> Result<Self, Self::Error> {
         match logical_plan {
-            LogicalPlan::Extension(Extension { node })
-                if node
-                    .as_any()
-                    .downcast_ref::<AlterSchemaPlanNode>()
-                    .is_some() =>
-            {
-                let ext = node
-                    .as_any()
-                    .downcast_ref::<AlterSchemaPlanNode>()
-                    .expect("AlterSchemaPlanNode");
-                Ok(PyAlterSchema {
-                    alter_schema: ext.clone(),
-                })
+            logical::LogicalPlan::Extension(extension) => {
+                if let Some(ext) = extension.node.as_any().downcast_ref::<DropSchemaPlanNode>() {
+                    Ok(PyDropSchema {
+                        drop_schema: ext.clone(),
+                    })
+                } else {
+                    Err(py_type_err("unexpected plan"))
+                }
             }
             _ => Err(py_type_err("unexpected plan")),
         }
     }
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/alter_table.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/export_model.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,50 @@
-use std::{any::Any, fmt, sync::Arc};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
 
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{
-    logical_plan::{Extension, UserDefinedLogicalNode},
-    Expr,
-    LogicalPlan,
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan},
 };
 use fmt::Debug;
 use pyo3::prelude::*;
 
-use crate::sql::{exceptions::py_type_err, logical};
+use crate::{
+    parser::PySqlArg,
+    sql::{exceptions::py_type_err, logical},
+};
 
-#[derive(Clone)]
-pub struct AlterTablePlanNode {
+#[derive(Clone, PartialEq)]
+pub struct ExportModelPlanNode {
     pub schema: DFSchemaRef,
-    pub old_table_name: String,
-    pub new_table_name: String,
     pub schema_name: Option<String>,
-    pub if_exists: bool,
+    pub model_name: String,
+    pub with_options: Vec<(String, PySqlArg)>,
 }
 
-impl Debug for AlterTablePlanNode {
+impl Debug for ExportModelPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
-impl UserDefinedLogicalNode for AlterTablePlanNode {
+impl Hash for ExportModelPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.schema_name.hash(state);
+        self.model_name.hash(state);
+        // self.with_options.hash(state);
+    }
+}
+
+impl UserDefinedLogicalNode for ExportModelPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
     }
@@ -38,82 +52,91 @@
     fn schema(&self) -> &DFSchemaRef {
         &self.schema
     }
 
     fn expressions(&self) -> Vec<Expr> {
         // there is no need to expose any expressions here since DataFusion would
         // not be able to do anything with expressions that are specific to
-        // ALTER TABLE {table_name}
+        // EXPORT MODEL
         vec![]
     }
 
     fn fmt_for_explain(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        write!(
-            f,
-            "Alter Table: old_table_name: {:?}, new_table_name: {:?}, schema_name: {:?}",
-            self.old_table_name, self.new_table_name, self.schema_name
-        )
+        write!(f, "ExportModel: model_name={}", self.model_name)
     }
 
     fn from_template(
         &self,
         _exprs: &[Expr],
-        _inputs: &[LogicalPlan],
+        inputs: &[LogicalPlan],
     ) -> Arc<dyn UserDefinedLogicalNode> {
-        Arc::new(AlterTablePlanNode {
+        assert_eq!(inputs.len(), 0, "input size inconsistent");
+        Arc::new(ExportModelPlanNode {
             schema: Arc::new(DFSchema::empty()),
-            old_table_name: self.old_table_name.clone(),
-            new_table_name: self.new_table_name.clone(),
             schema_name: self.schema_name.clone(),
-            if_exists: self.if_exists,
+            model_name: self.model_name.clone(),
+            with_options: self.with_options.clone(),
         })
     }
+
+    fn name(&self) -> &str {
+        "ExportModel"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
-#[pyclass(name = "AlterTable", module = "dask_planner", subclass)]
-pub struct PyAlterTable {
-    pub(crate) alter_table: AlterTablePlanNode,
+#[pyclass(name = "ExportModel", module = "dask_planner", subclass)]
+pub struct PyExportModel {
+    pub(crate) export_model: ExportModelPlanNode,
 }
 
 #[pymethods]
-impl PyAlterTable {
-    #[pyo3(name = "getOldTableName")]
-    fn get_old_table_name(&self) -> PyResult<String> {
-        Ok(self.alter_table.old_table_name.clone())
-    }
-
-    #[pyo3(name = "getNewTableName")]
-    fn get_new_table_name(&self) -> PyResult<String> {
-        Ok(self.alter_table.new_table_name.clone())
+impl PyExportModel {
+    #[pyo3(name = "getModelName")]
+    fn get_model_name(&self) -> PyResult<String> {
+        Ok(self.export_model.model_name.clone())
     }
 
     #[pyo3(name = "getSchemaName")]
     fn get_schema_name(&self) -> PyResult<Option<String>> {
-        Ok(self.alter_table.schema_name.clone())
+        Ok(self.export_model.schema_name.clone())
     }
 
-    #[pyo3(name = "getIfExists")]
-    fn get_if_exists(&self) -> PyResult<bool> {
-        Ok(self.alter_table.if_exists)
+    #[pyo3(name = "getSQLWithOptions")]
+    fn sql_with_options(&self) -> PyResult<Vec<(String, PySqlArg)>> {
+        Ok(self.export_model.with_options.clone())
     }
 }
 
-impl TryFrom<logical::LogicalPlan> for PyAlterTable {
+impl TryFrom<logical::LogicalPlan> for PyExportModel {
     type Error = PyErr;
 
     fn try_from(logical_plan: logical::LogicalPlan) -> Result<Self, Self::Error> {
         match logical_plan {
-            LogicalPlan::Extension(Extension { node })
-                if node.as_any().downcast_ref::<AlterTablePlanNode>().is_some() =>
-            {
-                let ext = node
+            logical::LogicalPlan::Extension(extension) => {
+                if let Some(ext) = extension
+                    .node
                     .as_any()
-                    .downcast_ref::<AlterTablePlanNode>()
-                    .expect("AlterTablePlanNode");
-                Ok(PyAlterTable {
-                    alter_table: ext.clone(),
-                })
+                    .downcast_ref::<ExportModelPlanNode>()
+                {
+                    Ok(PyExportModel {
+                        export_model: ext.clone(),
+                    })
+                } else {
+                    Err(py_type_err("unexpected plan"))
+                }
             }
             _ => Err(py_type_err("unexpected plan")),
         }
     }
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/analyze_table.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/analyze_table.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,50 @@
-use std::{any::Any, fmt, sync::Arc};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
 
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{
-    logical_plan::{Extension, UserDefinedLogicalNode},
-    Expr,
-    LogicalPlan,
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{
+        logical_plan::{Extension, UserDefinedLogicalNode},
+        Expr,
+        LogicalPlan,
+    },
 };
 use fmt::Debug;
 use pyo3::prelude::*;
 
 use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
+#[derive(Clone, PartialEq)]
 pub struct AnalyzeTablePlanNode {
     pub schema: DFSchemaRef,
     pub table_name: String,
     pub schema_name: Option<String>,
     pub columns: Vec<String>,
 }
 
 impl Debug for AnalyzeTablePlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
+impl Hash for AnalyzeTablePlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.table_name.hash(state);
+        self.schema_name.hash(state);
+        self.columns.hash(state);
+    }
+}
+
 impl UserDefinedLogicalNode for AnalyzeTablePlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
@@ -61,14 +77,30 @@
         Arc::new(AnalyzeTablePlanNode {
             schema: Arc::new(DFSchema::empty()),
             table_name: self.table_name.clone(),
             schema_name: self.schema_name.clone(),
             columns: self.columns.clone(),
         })
     }
+
+    fn name(&self) -> &str {
+        "AnalyzeTable"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
 #[pyclass(name = "AnalyzeTable", module = "dask_planner", subclass)]
 pub struct PyAnalyzeTable {
     pub(crate) analyze_table: AnalyzeTablePlanNode,
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/create_catalog_schema.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/create_catalog_schema.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,46 @@
-use std::{any::Any, fmt, sync::Arc};
-
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
+
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan},
+};
 use fmt::Debug;
 use pyo3::prelude::*;
 
 use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
+#[derive(Clone, PartialEq)]
 pub struct CreateCatalogSchemaPlanNode {
     pub schema: DFSchemaRef,
     pub schema_name: String,
     pub if_not_exists: bool,
     pub or_replace: bool,
 }
 
 impl Debug for CreateCatalogSchemaPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
+impl Hash for CreateCatalogSchemaPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.schema_name.hash(state);
+        self.if_not_exists.hash(state);
+        self.or_replace.hash(state);
+    }
+}
+
 impl UserDefinedLogicalNode for CreateCatalogSchemaPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
@@ -57,14 +73,30 @@
         Arc::new(CreateCatalogSchemaPlanNode {
             schema: Arc::new(DFSchema::empty()),
             schema_name: self.schema_name.clone(),
             if_not_exists: self.if_not_exists,
             or_replace: self.or_replace,
         })
     }
+
+    fn name(&self) -> &str {
+        "CreateCatalogSchema"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
 #[pyclass(name = "CreateCatalogSchema", module = "dask_planner", subclass)]
 pub struct PyCreateCatalogSchema {
     pub(crate) create_catalog_schema: CreateCatalogSchemaPlanNode,
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/create_experiment.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/alter_schema.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,136 +1,139 @@
-use std::{any::Any, fmt, sync::Arc};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
 
-use datafusion_common::DFSchemaRef;
-use datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan};
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{
+        logical_plan::{Extension, UserDefinedLogicalNode},
+        Expr,
+        LogicalPlan,
+    },
+};
 use fmt::Debug;
 use pyo3::prelude::*;
 
-use crate::{
-    parser::PySqlArg,
-    sql::{exceptions::py_type_err, logical},
-};
+use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
-pub struct CreateExperimentPlanNode {
-    pub schema_name: Option<String>,
-    pub experiment_name: String,
-    pub input: LogicalPlan,
-    pub if_not_exists: bool,
-    pub or_replace: bool,
-    pub with_options: Vec<(String, PySqlArg)>,
+#[derive(Clone, PartialEq)]
+pub struct AlterSchemaPlanNode {
+    pub schema: DFSchemaRef,
+    pub old_schema_name: String,
+    pub new_schema_name: String,
 }
 
-impl Debug for CreateExperimentPlanNode {
+impl Debug for AlterSchemaPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
-impl UserDefinedLogicalNode for CreateExperimentPlanNode {
+impl Hash for AlterSchemaPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.old_schema_name.hash(state);
+        self.new_schema_name.hash(state);
+    }
+}
+
+impl UserDefinedLogicalNode for AlterSchemaPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
-        vec![&self.input]
+        vec![]
     }
 
     fn schema(&self) -> &DFSchemaRef {
-        self.input.schema()
+        &self.schema
     }
 
     fn expressions(&self) -> Vec<Expr> {
         // there is no need to expose any expressions here since DataFusion would
         // not be able to do anything with expressions that are specific to
-        // CREATE EXPERIMENT
+        // ALTER SCHEMA {table_name}
         vec![]
     }
 
     fn fmt_for_explain(&self, f: &mut fmt::Formatter) -> fmt::Result {
         write!(
             f,
-            "CreateExperiment: experiment_name={}",
-            self.experiment_name
+            "Alter Schema: old_schema_name: {:?}, new_schema_name: {:?}",
+            self.old_schema_name, self.new_schema_name
         )
     }
 
     fn from_template(
         &self,
         _exprs: &[Expr],
-        inputs: &[LogicalPlan],
+        _inputs: &[LogicalPlan],
     ) -> Arc<dyn UserDefinedLogicalNode> {
-        assert_eq!(inputs.len(), 1, "input size inconsistent");
-        Arc::new(CreateExperimentPlanNode {
-            schema_name: self.schema_name.clone(),
-            experiment_name: self.experiment_name.clone(),
-            input: inputs[0].clone(),
-            if_not_exists: self.if_not_exists,
-            or_replace: self.or_replace,
-            with_options: self.with_options.clone(),
+        Arc::new(AlterSchemaPlanNode {
+            schema: Arc::new(DFSchema::empty()),
+            old_schema_name: self.old_schema_name.clone(),
+            new_schema_name: self.new_schema_name.clone(),
         })
     }
-}
 
-#[pyclass(name = "CreateExperiment", module = "dask_planner", subclass)]
-pub struct PyCreateExperiment {
-    pub(crate) create_experiment: CreateExperimentPlanNode,
-}
-
-#[pymethods]
-impl PyCreateExperiment {
-    /// Creating an experiment requires that a subquery be passed to the CREATE EXPERIMENT
-    /// statement to be used to gather the dataset which should be used for the
-    /// experiment. This function returns that portion of the statement.
-    #[pyo3(name = "getSelectQuery")]
-    fn get_select_query(&self) -> PyResult<logical::PyLogicalPlan> {
-        Ok(self.create_experiment.input.clone().into())
+    fn name(&self) -> &str {
+        "AlterSchema"
     }
 
-    #[pyo3(name = "getSchemaName")]
-    fn get_schema_name(&self) -> PyResult<Option<String>> {
-        Ok(self.create_experiment.schema_name.clone())
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
     }
 
-    #[pyo3(name = "getExperimentName")]
-    fn get_experiment_name(&self) -> PyResult<String> {
-        Ok(self.create_experiment.experiment_name.clone())
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
     }
+}
 
-    #[pyo3(name = "getIfNotExists")]
-    fn get_if_not_exists(&self) -> PyResult<bool> {
-        Ok(self.create_experiment.if_not_exists)
-    }
+#[pyclass(name = "AlterSchema", module = "dask_planner", subclass)]
+pub struct PyAlterSchema {
+    pub(crate) alter_schema: AlterSchemaPlanNode,
+}
 
-    #[pyo3(name = "getOrReplace")]
-    pub fn get_or_replace(&self) -> PyResult<bool> {
-        Ok(self.create_experiment.or_replace)
+#[pymethods]
+impl PyAlterSchema {
+    #[pyo3(name = "getOldSchemaName")]
+    fn get_old_schema_name(&self) -> PyResult<String> {
+        Ok(self.alter_schema.old_schema_name.clone())
     }
 
-    #[pyo3(name = "getSQLWithOptions")]
-    fn sql_with_options(&self) -> PyResult<Vec<(String, PySqlArg)>> {
-        Ok(self.create_experiment.with_options.clone())
+    #[pyo3(name = "getNewSchemaName")]
+    fn get_new_schema_name(&self) -> PyResult<String> {
+        Ok(self.alter_schema.new_schema_name.clone())
     }
 }
 
-impl TryFrom<logical::LogicalPlan> for PyCreateExperiment {
+impl TryFrom<logical::LogicalPlan> for PyAlterSchema {
     type Error = PyErr;
 
     fn try_from(logical_plan: logical::LogicalPlan) -> Result<Self, Self::Error> {
         match logical_plan {
-            logical::LogicalPlan::Extension(extension) => {
-                if let Some(ext) = extension
-                    .node
+            LogicalPlan::Extension(Extension { node })
+                if node
+                    .as_any()
+                    .downcast_ref::<AlterSchemaPlanNode>()
+                    .is_some() =>
+            {
+                let ext = node
                     .as_any()
-                    .downcast_ref::<CreateExperimentPlanNode>()
-                {
-                    Ok(PyCreateExperiment {
-                        create_experiment: ext.clone(),
-                    })
-                } else {
-                    Err(py_type_err("unexpected plan"))
-                }
+                    .downcast_ref::<AlterSchemaPlanNode>()
+                    .expect("AlterSchemaPlanNode");
+                Ok(PyAlterSchema {
+                    alter_schema: ext.clone(),
+                })
             }
             _ => Err(py_type_err("unexpected plan")),
         }
     }
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/create_memory_table.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/create_memory_table.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_expr::{
+use datafusion_python::datafusion_expr::{
     logical_plan::{CreateMemoryTable, CreateView},
     LogicalPlan,
 };
 use pyo3::prelude::*;
 
 use crate::sql::{exceptions::py_type_err, logical::PyLogicalPlan};
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/create_model.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/create_model.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-use std::{any::Any, fmt, sync::Arc};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
 
-use datafusion_common::DFSchemaRef;
-use datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan};
+use datafusion_python::{
+    datafusion_common::DFSchemaRef,
+    datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan},
+};
 use fmt::Debug;
 use pyo3::prelude::*;
 
 use crate::{
     parser::PySqlArg,
     sql::{exceptions::py_type_err, logical},
 };
 
-#[derive(Clone)]
+#[derive(Clone, PartialEq)]
 pub struct CreateModelPlanNode {
     pub schema_name: Option<String>,
     pub model_name: String,
     pub input: LogicalPlan,
     pub if_not_exists: bool,
     pub or_replace: bool,
     pub with_options: Vec<(String, PySqlArg)>,
@@ -22,14 +29,25 @@
 
 impl Debug for CreateModelPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
+impl Hash for CreateModelPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema_name.hash(state);
+        self.model_name.hash(state);
+        self.input.hash(state);
+        self.if_not_exists.hash(state);
+        self.or_replace.hash(state);
+        // self.with_options.hash(state);
+    }
+}
+
 impl UserDefinedLogicalNode for CreateModelPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![&self.input]
@@ -61,14 +79,30 @@
             model_name: self.model_name.clone(),
             input: inputs[0].clone(),
             if_not_exists: self.if_not_exists,
             or_replace: self.or_replace,
             with_options: self.with_options.clone(),
         })
     }
+
+    fn name(&self) -> &str {
+        "CreateModel"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
 #[pyclass(name = "CreateModel", module = "dask_planner", subclass)]
 pub struct PyCreateModel {
     pub(crate) create_model: CreateModelPlanNode,
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/create_table.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/create_table.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,27 @@
-use std::{any::Any, fmt, sync::Arc};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
 
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan};
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan},
+};
 use fmt::Debug;
 use pyo3::prelude::*;
 
 use crate::{
     parser::PySqlArg,
     sql::{exceptions::py_type_err, logical},
 };
 
-#[derive(Clone)]
+#[derive(Clone, PartialEq)]
 pub struct CreateTablePlanNode {
     pub schema: DFSchemaRef,
     pub schema_name: Option<String>, // "something" in `something.table_name`
     pub table_name: String,
     pub if_not_exists: bool,
     pub or_replace: bool,
     pub with_options: Vec<(String, PySqlArg)>,
@@ -22,14 +29,25 @@
 
 impl Debug for CreateTablePlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
+impl Hash for CreateTablePlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.schema_name.hash(state);
+        self.table_name.hash(state);
+        self.if_not_exists.hash(state);
+        self.or_replace.hash(state);
+        // self.with_options.hash(state);
+    }
+}
+
 impl UserDefinedLogicalNode for CreateTablePlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
@@ -60,14 +78,30 @@
             schema_name: self.schema_name.clone(),
             table_name: self.table_name.clone(),
             if_not_exists: self.if_not_exists,
             or_replace: self.or_replace,
             with_options: self.with_options.clone(),
         })
     }
+
+    fn name(&self) -> &str {
+        "CreateTable"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
 #[pyclass(name = "CreateTable", module = "dask_planner", subclass)]
 pub struct PyCreateTable {
     pub(crate) create_table: CreateTablePlanNode,
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/describe_model.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/describe_model.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,44 @@
-use std::{any::Any, fmt, sync::Arc};
-
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
+
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan},
+};
 use fmt::Debug;
 use pyo3::prelude::*;
 
 use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
+#[derive(Clone, PartialEq)]
 pub struct DescribeModelPlanNode {
     pub schema: DFSchemaRef,
     pub schema_name: Option<String>,
     pub model_name: String,
 }
 
 impl Debug for DescribeModelPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
+impl Hash for DescribeModelPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.schema_name.hash(state);
+        self.model_name.hash(state);
+    }
+}
+
 impl UserDefinedLogicalNode for DescribeModelPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
@@ -52,14 +67,30 @@
         assert_eq!(inputs.len(), 0, "input size inconsistent");
         Arc::new(DescribeModelPlanNode {
             schema: Arc::new(DFSchema::empty()),
             schema_name: self.schema_name.clone(),
             model_name: self.model_name.clone(),
         })
     }
+
+    fn name(&self) -> &str {
+        "DescribeModel"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
 #[pyclass(name = "DescribeModel", module = "dask_planner", subclass)]
 pub struct PyDescribeModel {
     pub(crate) describe_model: DescribeModelPlanNode,
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/drop_model.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/show_models.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,43 @@
-use std::{any::Any, fmt, sync::Arc};
-
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
+
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan},
+};
 use fmt::Debug;
 use pyo3::prelude::*;
 
-use crate::sql::{exceptions::py_type_err, logical};
+use crate::sql::logical::py_type_err;
 
-#[derive(Clone)]
-pub struct DropModelPlanNode {
-    pub schema_name: Option<String>,
-    pub model_name: String,
-    pub if_exists: bool,
+#[derive(Clone, PartialEq)]
+pub struct ShowModelsPlanNode {
     pub schema: DFSchemaRef,
+    pub schema_name: Option<String>,
 }
 
-impl Debug for DropModelPlanNode {
+impl Debug for ShowModelsPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
-impl UserDefinedLogicalNode for DropModelPlanNode {
+impl Hash for ShowModelsPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.schema_name.hash(state);
+    }
+}
+
+impl UserDefinedLogicalNode for ShowModelsPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
     }
@@ -33,69 +45,72 @@
     fn schema(&self) -> &DFSchemaRef {
         &self.schema
     }
 
     fn expressions(&self) -> Vec<Expr> {
         // there is no need to expose any expressions here since DataFusion would
         // not be able to do anything with expressions that are specific to
-        // DROP MODEL
+        // SHOW MODELS
         vec![]
     }
 
     fn fmt_for_explain(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        write!(f, "DropModel: model_name={}", self.model_name)
+        write!(f, "ShowModels")
     }
 
     fn from_template(
         &self,
         _exprs: &[Expr],
-        inputs: &[LogicalPlan],
+        _inputs: &[LogicalPlan],
     ) -> Arc<dyn UserDefinedLogicalNode> {
-        assert_eq!(inputs.len(), 0, "input size inconsistent");
-        Arc::new(DropModelPlanNode {
-            schema_name: self.schema_name.clone(),
-            model_name: self.model_name.clone(),
-            if_exists: self.if_exists,
+        Arc::new(ShowModelsPlanNode {
             schema: Arc::new(DFSchema::empty()),
+            schema_name: self.schema_name.clone(),
         })
     }
+
+    fn name(&self) -> &str {
+        "ShowModels"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
-#[pyclass(name = "DropModel", module = "dask_planner", subclass)]
-pub struct PyDropModel {
-    pub(crate) drop_model: DropModelPlanNode,
+#[pyclass(name = "ShowModels", module = "dask_planner", subclass)]
+pub struct PyShowModels {
+    pub(crate) show_models: ShowModelsPlanNode,
 }
 
 #[pymethods]
-impl PyDropModel {
+impl PyShowModels {
     #[pyo3(name = "getSchemaName")]
     fn get_schema_name(&self) -> PyResult<Option<String>> {
-        Ok(self.drop_model.schema_name.clone())
-    }
-
-    #[pyo3(name = "getModelName")]
-    fn get_model_name(&self) -> PyResult<String> {
-        Ok(self.drop_model.model_name.clone())
-    }
-
-    #[pyo3(name = "getIfExists")]
-    pub fn get_if_exists(&self) -> PyResult<bool> {
-        Ok(self.drop_model.if_exists)
+        Ok(self.show_models.schema_name.clone())
     }
 }
 
-impl TryFrom<logical::LogicalPlan> for PyDropModel {
+impl TryFrom<LogicalPlan> for PyShowModels {
     type Error = PyErr;
 
-    fn try_from(logical_plan: logical::LogicalPlan) -> Result<Self, Self::Error> {
+    fn try_from(logical_plan: LogicalPlan) -> Result<Self, Self::Error> {
         match logical_plan {
-            logical::LogicalPlan::Extension(extension) => {
-                if let Some(ext) = extension.node.as_any().downcast_ref::<DropModelPlanNode>() {
-                    Ok(PyDropModel {
-                        drop_model: ext.clone(),
+            LogicalPlan::Extension(extension) => {
+                if let Some(ext) = extension.node.as_any().downcast_ref::<ShowModelsPlanNode>() {
+                    Ok(PyShowModels {
+                        show_models: ext.clone(),
                     })
                 } else {
                     Err(py_type_err("unexpected plan"))
                 }
             }
             _ => Err(py_type_err("unexpected plan")),
         }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/drop_schema.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/use_schema.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,43 @@
-use std::{any::Any, fmt, sync::Arc};
-
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
+
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan},
+};
 use fmt::Debug;
 use pyo3::prelude::*;
 
 use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
-pub struct DropSchemaPlanNode {
+#[derive(Clone, PartialEq)]
+pub struct UseSchemaPlanNode {
     pub schema: DFSchemaRef,
     pub schema_name: String,
-    pub if_exists: bool,
 }
 
-impl Debug for DropSchemaPlanNode {
+impl Debug for UseSchemaPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
-impl UserDefinedLogicalNode for DropSchemaPlanNode {
+impl Hash for UseSchemaPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.schema_name.hash(state);
+    }
+}
+
+impl UserDefinedLogicalNode for UseSchemaPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
     }
@@ -32,62 +45,72 @@
     fn schema(&self) -> &DFSchemaRef {
         &self.schema
     }
 
     fn expressions(&self) -> Vec<Expr> {
         // there is no need to expose any expressions here since DataFusion would
         // not be able to do anything with expressions that are specific to
-        // DROP SCHEMA
+        // USE SCHEMA
         vec![]
     }
 
     fn fmt_for_explain(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        write!(f, "DropSchema: schema_name={}", self.schema_name)
+        write!(f, "UseSchema: schema_name={}", self.schema_name)
     }
 
     fn from_template(
         &self,
         _exprs: &[Expr],
         _inputs: &[LogicalPlan],
     ) -> Arc<dyn UserDefinedLogicalNode> {
-        Arc::new(DropSchemaPlanNode {
+        Arc::new(UseSchemaPlanNode {
             schema: Arc::new(DFSchema::empty()),
             schema_name: self.schema_name.clone(),
-            if_exists: self.if_exists,
         })
     }
+
+    fn name(&self) -> &str {
+        "UseSchema"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
-#[pyclass(name = "DropSchema", module = "dask_planner", subclass)]
-pub struct PyDropSchema {
-    pub(crate) drop_schema: DropSchemaPlanNode,
+#[pyclass(name = "UseSchema", module = "dask_planner", subclass)]
+pub struct PyUseSchema {
+    pub(crate) use_schema: UseSchemaPlanNode,
 }
 
 #[pymethods]
-impl PyDropSchema {
+impl PyUseSchema {
     #[pyo3(name = "getSchemaName")]
     fn get_schema_name(&self) -> PyResult<String> {
-        Ok(self.drop_schema.schema_name.clone())
-    }
-
-    #[pyo3(name = "getIfExists")]
-    fn get_if_exists(&self) -> PyResult<bool> {
-        Ok(self.drop_schema.if_exists)
+        Ok(self.use_schema.schema_name.clone())
     }
 }
 
-impl TryFrom<logical::LogicalPlan> for PyDropSchema {
+impl TryFrom<logical::LogicalPlan> for PyUseSchema {
     type Error = PyErr;
 
     fn try_from(logical_plan: logical::LogicalPlan) -> Result<Self, Self::Error> {
         match logical_plan {
             logical::LogicalPlan::Extension(extension) => {
-                if let Some(ext) = extension.node.as_any().downcast_ref::<DropSchemaPlanNode>() {
-                    Ok(PyDropSchema {
-                        drop_schema: ext.clone(),
+                if let Some(ext) = extension.node.as_any().downcast_ref::<UseSchemaPlanNode>() {
+                    Ok(PyUseSchema {
+                        use_schema: ext.clone(),
                     })
                 } else {
                     Err(py_type_err("unexpected plan"))
                 }
             }
             _ => Err(py_type_err("unexpected plan")),
         }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/drop_table.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_table.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_expr::logical_plan::{DropTable, LogicalPlan};
+use datafusion_python::datafusion_expr::logical_plan::{DropTable, LogicalPlan};
 use pyo3::prelude::*;
 
 use crate::sql::exceptions::py_type_err;
 
 #[pyclass(name = "DropTable", module = "dask_planner", subclass)]
 #[derive(Clone)]
 pub struct PyDropTable {
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/empty_relation.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/empty_relation.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_expr::logical_plan::{EmptyRelation, LogicalPlan};
+use datafusion_python::datafusion_expr::logical_plan::{EmptyRelation, LogicalPlan};
 use pyo3::prelude::*;
 
 use crate::sql::exceptions::py_type_err;
 
 #[pyclass(name = "EmptyRelation", module = "dask_planner", subclass)]
 #[derive(Clone)]
 pub struct PyEmptyRelation {
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/explain.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/explain.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_expr::{logical_plan::Explain, LogicalPlan};
+use datafusion_python::datafusion_expr::{logical_plan::Explain, LogicalPlan};
 use pyo3::prelude::*;
 
 use crate::sql::exceptions::py_type_err;
 
 #[pyclass(name = "Explain", module = "dask_planner", subclass)]
 #[derive(Clone)]
 pub struct PyExplain {
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/export_model.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/predict_model.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,108 +1,134 @@
-use std::{any::Any, fmt, sync::Arc};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
 
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan};
+use datafusion_python::{
+    datafusion_common::DFSchemaRef,
+    datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan},
+};
 use fmt::Debug;
 use pyo3::prelude::*;
 
-use crate::{
-    parser::PySqlArg,
-    sql::{exceptions::py_type_err, logical},
-};
+use super::PyLogicalPlan;
+use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
-pub struct ExportModelPlanNode {
-    pub schema: DFSchemaRef,
-    pub schema_name: Option<String>,
+#[derive(Clone, PartialEq)]
+pub struct PredictModelPlanNode {
+    pub schema_name: Option<String>, // "something" in `something.model_name`
     pub model_name: String,
-    pub with_options: Vec<(String, PySqlArg)>,
+    pub input: LogicalPlan,
 }
 
-impl Debug for ExportModelPlanNode {
+impl Debug for PredictModelPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
-impl UserDefinedLogicalNode for ExportModelPlanNode {
+impl Hash for PredictModelPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema_name.hash(state);
+        self.model_name.hash(state);
+        self.input.hash(state);
+    }
+}
+
+impl UserDefinedLogicalNode for PredictModelPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
-        vec![]
+        vec![&self.input]
     }
 
     fn schema(&self) -> &DFSchemaRef {
-        &self.schema
+        self.input.schema()
     }
 
     fn expressions(&self) -> Vec<Expr> {
         // there is no need to expose any expressions here since DataFusion would
         // not be able to do anything with expressions that are specific to
-        // EXPORT MODEL
+        // PREDICT TABLE
         vec![]
     }
 
     fn fmt_for_explain(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        write!(f, "ExportModel: model_name={}", self.model_name)
+        write!(f, "PredictModel: model_name={}", self.model_name)
     }
 
     fn from_template(
         &self,
         _exprs: &[Expr],
         inputs: &[LogicalPlan],
     ) -> Arc<dyn UserDefinedLogicalNode> {
-        assert_eq!(inputs.len(), 0, "input size inconsistent");
-        Arc::new(ExportModelPlanNode {
-            schema: Arc::new(DFSchema::empty()),
+        Arc::new(PredictModelPlanNode {
             schema_name: self.schema_name.clone(),
             model_name: self.model_name.clone(),
-            with_options: self.with_options.clone(),
+            input: inputs[0].clone(),
         })
     }
+
+    fn name(&self) -> &str {
+        "PredictModel"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
-#[pyclass(name = "ExportModel", module = "dask_planner", subclass)]
-pub struct PyExportModel {
-    pub(crate) export_model: ExportModelPlanNode,
+#[pyclass(name = "PredictModel", module = "dask_planner", subclass)]
+pub struct PyPredictModel {
+    pub(crate) predict_model: PredictModelPlanNode,
 }
 
 #[pymethods]
-impl PyExportModel {
-    #[pyo3(name = "getModelName")]
-    fn get_model_name(&self) -> PyResult<String> {
-        Ok(self.export_model.model_name.clone())
-    }
-
+impl PyPredictModel {
     #[pyo3(name = "getSchemaName")]
     fn get_schema_name(&self) -> PyResult<Option<String>> {
-        Ok(self.export_model.schema_name.clone())
+        Ok(self.predict_model.schema_name.clone())
+    }
+
+    #[pyo3(name = "getModelName")]
+    fn get_model_name(&self) -> PyResult<String> {
+        Ok(self.predict_model.model_name.clone())
     }
 
-    #[pyo3(name = "getSQLWithOptions")]
-    fn sql_with_options(&self) -> PyResult<Vec<(String, PySqlArg)>> {
-        Ok(self.export_model.with_options.clone())
+    #[pyo3(name = "getSelect")]
+    fn get_select(&self) -> PyResult<PyLogicalPlan> {
+        Ok(PyLogicalPlan::from(self.predict_model.input.clone()))
     }
 }
 
-impl TryFrom<logical::LogicalPlan> for PyExportModel {
+impl TryFrom<logical::LogicalPlan> for PyPredictModel {
     type Error = PyErr;
 
     fn try_from(logical_plan: logical::LogicalPlan) -> Result<Self, Self::Error> {
         match logical_plan {
             logical::LogicalPlan::Extension(extension) => {
                 if let Some(ext) = extension
                     .node
                     .as_any()
-                    .downcast_ref::<ExportModelPlanNode>()
+                    .downcast_ref::<PredictModelPlanNode>()
                 {
-                    Ok(PyExportModel {
-                        export_model: ext.clone(),
+                    Ok(PyPredictModel {
+                        predict_model: ext.clone(),
                     })
                 } else {
                     Err(py_type_err("unexpected plan"))
                 }
             }
             _ => Err(py_type_err("unexpected plan")),
         }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/filter.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/filter.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_expr::{logical_plan::Filter, LogicalPlan};
+use datafusion_python::datafusion_expr::{logical_plan::Filter, LogicalPlan};
 use pyo3::prelude::*;
 
 use crate::{expression::PyExpr, sql::exceptions::py_type_err};
 
 #[pyclass(name = "Filter", module = "dask_planner", subclass)]
 #[derive(Clone)]
 pub struct PyFilter {
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/join.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/join.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-use datafusion_common::Column;
-use datafusion_expr::{
-    and,
-    logical_plan::{Join, JoinType, LogicalPlan},
-    BinaryExpr,
-    Expr,
-    Operator,
+use datafusion_python::{
+    datafusion_common::Column,
+    datafusion_expr::{
+        and,
+        logical_plan::{Join, JoinType, LogicalPlan},
+        BinaryExpr,
+        Expr,
+        Operator,
+    },
 };
 use pyo3::prelude::*;
 
 use crate::{
     expression::PyExpr,
     sql::{column, exceptions::py_type_err},
 };
@@ -66,38 +68,36 @@
         } else {
             Ok(None)
         }
     }
 
     #[pyo3(name = "getJoinConditions")]
     pub fn join_conditions(&mut self) -> PyResult<Vec<(column::PyColumn, column::PyColumn)>> {
-        let lhs_table_name: String = match &*self.join.left {
-            LogicalPlan::TableScan(scan) => scan.table_name.clone(),
-            _ => {
-                return Err(py_type_err(
-                    "lhs Expected TableScan but something else was received!",
-                ))
-            }
-        };
-
-        let rhs_table_name: String = match &*self.join.right {
-            LogicalPlan::TableScan(scan) => scan.table_name.clone(),
-            _ => {
-                return Err(py_type_err(
-                    "rhs Expected TableScan but something else was received!",
-                ))
-            }
-        };
+        // let lhs_table_name = match &*self.join.left {
+        //     LogicalPlan::TableScan(scan) => scan.table_name.clone(),
+        //     _ => {
+        //         return Err(py_type_err(
+        //             "lhs Expected TableScan but something else was received!",
+        //         ))
+        //     }
+        // };
+
+        // let rhs_table_name = match &*self.join.right {
+        //     LogicalPlan::TableScan(scan) => scan.table_name.clone(),
+        //     _ => {
+        //         return Err(py_type_err(
+        //             "rhs Expected TableScan but something else was received!",
+        //         ))
+        //     }
+        // };
 
         let mut join_conditions: Vec<(column::PyColumn, column::PyColumn)> = Vec::new();
         for (lhs, rhs) in self.join.on.clone() {
             match (lhs, rhs) {
-                (Expr::Column(mut lhs), Expr::Column(mut rhs)) => {
-                    lhs.relation = Some(lhs_table_name.clone());
-                    rhs.relation = Some(rhs_table_name.clone());
+                (Expr::Column(lhs), Expr::Column(rhs)) => {
                     join_conditions.push((lhs.into(), rhs.into()));
                 }
                 _ => return Err(py_type_err("unsupported join condition")),
             }
         }
         Ok(join_conditions)
     }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/limit.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/limit.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-use datafusion_common::ScalarValue;
-use datafusion_expr::{logical_plan::Limit, Expr, LogicalPlan};
+use datafusion_python::{
+    datafusion_common::ScalarValue,
+    datafusion_expr::{logical_plan::Limit, Expr, LogicalPlan},
+};
 use pyo3::prelude::*;
 
 use crate::{expression::PyExpr, sql::exceptions::py_type_err};
 
 #[pyclass(name = "Limit", module = "dask_planner", subclass)]
 #[derive(Clone)]
 pub struct PyLimit {
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/projection.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/projection.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_expr::{logical_plan::Projection, Expr, LogicalPlan};
+use datafusion_python::datafusion_expr::{logical_plan::Projection, Expr, LogicalPlan};
 use pyo3::prelude::*;
 
 use crate::{expression::PyExpr, sql::exceptions::py_type_err};
 
 #[pyclass(name = "Projection", module = "dask_planner", subclass)]
 #[derive(Clone)]
 pub struct PyProjection {
@@ -30,16 +30,24 @@
     #[pyo3(name = "getNamedProjects")]
     fn named_projects(&mut self) -> PyResult<Vec<(String, PyExpr)>> {
         let mut named: Vec<(String, PyExpr)> = Vec::new();
         for expression in self.projection.expr.clone() {
             let py_expr: PyExpr =
                 PyExpr::from(expression, Some(vec![self.projection.input.clone()]));
             for expr in self.projected_expressions(&py_expr) {
-                if let Ok(name) = expr._column_name(&self.projection.input) {
-                    named.push((name, expr.clone()));
+                match expr.expr {
+                    Expr::Alias(ex, name) => named.push((
+                        name.to_string(),
+                        PyExpr::from(*ex, Some(vec![self.projection.input.clone()])),
+                    )),
+                    _ => {
+                        if let Ok(name) = expr._column_name(&self.projection.input) {
+                            named.push((name, expr.clone()));
+                        }
+                    }
                 }
             }
         }
         Ok(named)
     }
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/repartition_by.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/repartition_by.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_expr::{
+use datafusion_python::datafusion_expr::{
     logical_plan::{Partitioning, Repartition},
     Expr,
     LogicalPlan,
 };
 use pyo3::prelude::*;
 
 use crate::{
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/show_columns.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/show_columns.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,48 @@
-use std::{any::Any, fmt, sync::Arc};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
 
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{
-    logical_plan::{Extension, UserDefinedLogicalNode},
-    Expr,
-    LogicalPlan,
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{
+        logical_plan::{Extension, UserDefinedLogicalNode},
+        Expr,
+        LogicalPlan,
+    },
 };
 use fmt::Debug;
 use pyo3::prelude::*;
 
 use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
+#[derive(Clone, PartialEq)]
 pub struct ShowColumnsPlanNode {
     pub schema: DFSchemaRef,
     pub table_name: String,
     pub schema_name: Option<String>,
 }
 
 impl Debug for ShowColumnsPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
+impl Hash for ShowColumnsPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.table_name.hash(state);
+        self.schema_name.hash(state);
+    }
+}
+
 impl UserDefinedLogicalNode for ShowColumnsPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
@@ -55,14 +70,30 @@
     ) -> Arc<dyn UserDefinedLogicalNode> {
         Arc::new(ShowColumnsPlanNode {
             schema: Arc::new(DFSchema::empty()),
             table_name: self.table_name.clone(),
             schema_name: self.schema_name.clone(),
         })
     }
+
+    fn name(&self) -> &str {
+        "ShowColumns"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
 #[pyclass(name = "ShowColumns", module = "dask_planner", subclass)]
 pub struct PyShowColumns {
     pub(crate) show_columns: ShowColumnsPlanNode,
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/show_models.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/drop_model.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,47 @@
-use std::{any::Any, fmt, sync::Arc};
-
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
+
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{logical_plan::UserDefinedLogicalNode, Expr, LogicalPlan},
+};
 use fmt::Debug;
 use pyo3::prelude::*;
 
-use crate::sql::logical::py_type_err;
+use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
-pub struct ShowModelsPlanNode {
-    pub schema: DFSchemaRef,
+#[derive(Clone, PartialEq)]
+pub struct DropModelPlanNode {
     pub schema_name: Option<String>,
+    pub model_name: String,
+    pub if_exists: bool,
+    pub schema: DFSchemaRef,
 }
 
-impl Debug for ShowModelsPlanNode {
+impl Debug for DropModelPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
-impl UserDefinedLogicalNode for ShowModelsPlanNode {
+impl Hash for DropModelPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema_name.hash(state);
+        self.model_name.hash(state);
+        self.if_exists.hash(state);
+        self.schema.hash(state);
+    }
+}
+
+impl UserDefinedLogicalNode for DropModelPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
     }
@@ -31,56 +49,85 @@
     fn schema(&self) -> &DFSchemaRef {
         &self.schema
     }
 
     fn expressions(&self) -> Vec<Expr> {
         // there is no need to expose any expressions here since DataFusion would
         // not be able to do anything with expressions that are specific to
-        // SHOW MODELS
+        // DROP MODEL
         vec![]
     }
 
     fn fmt_for_explain(&self, f: &mut fmt::Formatter) -> fmt::Result {
-        write!(f, "ShowModels")
+        write!(f, "DropModel: model_name={}", self.model_name)
     }
 
     fn from_template(
         &self,
         _exprs: &[Expr],
-        _inputs: &[LogicalPlan],
+        inputs: &[LogicalPlan],
     ) -> Arc<dyn UserDefinedLogicalNode> {
-        Arc::new(ShowModelsPlanNode {
-            schema: Arc::new(DFSchema::empty()),
+        assert_eq!(inputs.len(), 0, "input size inconsistent");
+        Arc::new(DropModelPlanNode {
             schema_name: self.schema_name.clone(),
+            model_name: self.model_name.clone(),
+            if_exists: self.if_exists,
+            schema: Arc::new(DFSchema::empty()),
         })
     }
+
+    fn name(&self) -> &str {
+        "DropModel"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
-#[pyclass(name = "ShowModels", module = "dask_planner", subclass)]
-pub struct PyShowModels {
-    pub(crate) show_models: ShowModelsPlanNode,
+#[pyclass(name = "DropModel", module = "dask_planner", subclass)]
+pub struct PyDropModel {
+    pub(crate) drop_model: DropModelPlanNode,
 }
 
 #[pymethods]
-impl PyShowModels {
+impl PyDropModel {
     #[pyo3(name = "getSchemaName")]
     fn get_schema_name(&self) -> PyResult<Option<String>> {
-        Ok(self.show_models.schema_name.clone())
+        Ok(self.drop_model.schema_name.clone())
+    }
+
+    #[pyo3(name = "getModelName")]
+    fn get_model_name(&self) -> PyResult<String> {
+        Ok(self.drop_model.model_name.clone())
+    }
+
+    #[pyo3(name = "getIfExists")]
+    pub fn get_if_exists(&self) -> PyResult<bool> {
+        Ok(self.drop_model.if_exists)
     }
 }
 
-impl TryFrom<LogicalPlan> for PyShowModels {
+impl TryFrom<logical::LogicalPlan> for PyDropModel {
     type Error = PyErr;
 
-    fn try_from(logical_plan: LogicalPlan) -> Result<Self, Self::Error> {
+    fn try_from(logical_plan: logical::LogicalPlan) -> Result<Self, Self::Error> {
         match logical_plan {
-            LogicalPlan::Extension(extension) => {
-                if let Some(ext) = extension.node.as_any().downcast_ref::<ShowModelsPlanNode>() {
-                    Ok(PyShowModels {
-                        show_models: ext.clone(),
+            logical::LogicalPlan::Extension(extension) => {
+                if let Some(ext) = extension.node.as_any().downcast_ref::<DropModelPlanNode>() {
+                    Ok(PyDropModel {
+                        drop_model: ext.clone(),
                     })
                 } else {
                     Err(py_type_err("unexpected plan"))
                 }
             }
             _ => Err(py_type_err("unexpected plan")),
         }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/show_schemas.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/show_schemas.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,47 @@
-use std::{any::Any, fmt, sync::Arc};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
 
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{
-    logical_plan::{Extension, UserDefinedLogicalNode},
-    Expr,
-    LogicalPlan,
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{
+        logical_plan::{Extension, UserDefinedLogicalNode},
+        Expr,
+        LogicalPlan,
+    },
 };
 use fmt::Debug;
 use pyo3::prelude::*;
 
 use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
+#[derive(Clone, PartialEq)]
 pub struct ShowSchemasPlanNode {
     pub schema: DFSchemaRef,
     pub catalog_name: Option<String>,
     pub like: Option<String>,
 }
 
 impl Debug for ShowSchemasPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
+impl Hash for ShowSchemasPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.like.hash(state);
+    }
+}
+
 impl UserDefinedLogicalNode for ShowSchemasPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
@@ -55,14 +69,30 @@
     ) -> Arc<dyn UserDefinedLogicalNode> {
         Arc::new(ShowSchemasPlanNode {
             schema: Arc::new(DFSchema::empty()),
             catalog_name: self.catalog_name.clone(),
             like: self.like.clone(),
         })
     }
+
+    fn name(&self) -> &str {
+        "ShowSchema"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
 #[pyclass(name = "ShowSchema", module = "dask_planner", subclass)]
 pub struct PyShowSchema {
     pub(crate) show_schema: ShowSchemasPlanNode,
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/show_tables.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/show_tables.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,47 @@
-use std::{any::Any, fmt, sync::Arc};
+use std::{
+    any::Any,
+    fmt,
+    hash::{Hash, Hasher},
+    sync::Arc,
+};
 
-use datafusion_common::{DFSchema, DFSchemaRef};
-use datafusion_expr::{
-    logical_plan::{Extension, UserDefinedLogicalNode},
-    Expr,
-    LogicalPlan,
+use datafusion_python::{
+    datafusion_common::{DFSchema, DFSchemaRef},
+    datafusion_expr::{
+        logical_plan::{Extension, UserDefinedLogicalNode},
+        Expr,
+        LogicalPlan,
+    },
 };
 use fmt::Debug;
 use pyo3::prelude::*;
 
 use crate::sql::{exceptions::py_type_err, logical};
 
-#[derive(Clone)]
+#[derive(Clone, PartialEq)]
 pub struct ShowTablesPlanNode {
     pub schema: DFSchemaRef,
     pub catalog_name: Option<String>,
     pub schema_name: Option<String>,
 }
 
 impl Debug for ShowTablesPlanNode {
     fn fmt(&self, f: &mut fmt::Formatter) -> fmt::Result {
         self.fmt_for_explain(f)
     }
 }
 
+impl Hash for ShowTablesPlanNode {
+    fn hash<H: Hasher>(&self, state: &mut H) {
+        self.schema.hash(state);
+        self.schema_name.hash(state);
+    }
+}
+
 impl UserDefinedLogicalNode for ShowTablesPlanNode {
     fn as_any(&self) -> &dyn Any {
         self
     }
 
     fn inputs(&self) -> Vec<&LogicalPlan> {
         vec![]
@@ -59,14 +73,30 @@
     ) -> Arc<dyn UserDefinedLogicalNode> {
         Arc::new(ShowTablesPlanNode {
             schema: Arc::new(DFSchema::empty()),
             catalog_name: self.catalog_name.clone(),
             schema_name: self.schema_name.clone(),
         })
     }
+
+    fn name(&self) -> &str {
+        "ShowTables"
+    }
+
+    fn dyn_hash(&self, state: &mut dyn Hasher) {
+        let mut s = state;
+        self.hash(&mut s);
+    }
+
+    fn dyn_eq(&self, other: &dyn UserDefinedLogicalNode) -> bool {
+        match other.as_any().downcast_ref::<Self>() {
+            Some(o) => self == o,
+            None => false,
+        }
+    }
 }
 
 #[pyclass(name = "ShowTables", module = "dask_planner", subclass)]
 pub struct PyShowTables {
     pub(crate) show_tables: ShowTablesPlanNode,
 }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/sort.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/sort.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_expr::{logical_plan::Sort, LogicalPlan};
+use datafusion_python::datafusion_expr::{logical_plan::Sort, LogicalPlan};
 use pyo3::prelude::*;
 
 use crate::{
     expression::{py_expr_list, PyExpr},
     sql::exceptions::py_type_err,
 };
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/subquery_alias.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/subquery_alias.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_expr::{logical_plan::SubqueryAlias, LogicalPlan};
+use datafusion_python::datafusion_expr::{logical_plan::SubqueryAlias, LogicalPlan};
 use pyo3::prelude::*;
 
 use crate::sql::exceptions::py_type_err;
 
 #[pyclass(name = "SubqueryAlias", module = "dask_planner", subclass)]
 #[derive(Clone)]
 pub struct PySubqueryAlias {
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical/window.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical/window.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-use datafusion_common::ScalarValue;
-use datafusion_expr::{
-    expr::WindowFunction,
-    logical_plan::Window,
-    Expr,
-    LogicalPlan,
-    WindowFrame,
-    WindowFrameBound,
+use datafusion_python::{
+    datafusion_common::ScalarValue,
+    datafusion_expr::{
+        expr::WindowFunction,
+        logical_plan::Window,
+        Expr,
+        LogicalPlan,
+        WindowFrame,
+        WindowFrameBound,
+    },
 };
 use pyo3::prelude::*;
 
 use crate::{
     error::DaskPlannerError,
     expression::{py_expr_list, PyExpr},
     sql::exceptions::py_type_err,
@@ -167,14 +169,24 @@
     pub fn get_offset(&self) -> PyResult<Option<u64>> {
         match &self.frame_bound {
             WindowFrameBound::Preceding(val) | WindowFrameBound::Following(val) => match val {
                 x if x.is_null() => Ok(None),
                 ScalarValue::UInt64(v) => Ok(*v),
                 // The cast below is only safe because window bounds cannot be negative
                 ScalarValue::Int64(v) => Ok(v.map(|n| n as u64)),
+                ScalarValue::Utf8(v) => {
+                    let s = v.clone().unwrap();
+                    match s.parse::<u64>() {
+                        Ok(s) => Ok(Some(s)),
+                        Err(_e) => Err(DaskPlannerError::Internal(format!(
+                            "Unable to parse u64 from Utf8 value '{s}'"
+                        ))
+                        .into()),
+                    }
+                }
                 ref x => Err(DaskPlannerError::Internal(format!(
                     "Unexpected window frame bound: {x}"
                 ))
                 .into()),
             },
             WindowFrameBound::CurrentRow => Ok(None),
         }
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/logical.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/logical.rs`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 pub mod show_tables;
 pub mod sort;
 pub mod subquery_alias;
 pub mod table_scan;
 pub mod use_schema;
 pub mod window;
 
-use datafusion_common::{DFSchemaRef, DataFusionError};
-use datafusion_expr::LogicalPlan;
+use datafusion_python::{
+    datafusion_common::{DFSchemaRef, DataFusionError},
+    datafusion_expr::LogicalPlan,
+};
 use pyo3::prelude::*;
 
 use self::{
     alter_schema::AlterSchemaPlanNode,
     alter_table::AlterTablePlanNode,
     analyze_table::AnalyzeTablePlanNode,
     create_catalog_schema::CreateCatalogSchemaPlanNode,
@@ -321,15 +323,15 @@
             LogicalPlan::Explain(_explain) => "Explain",
             LogicalPlan::Analyze(_analyze) => "Analyze",
             LogicalPlan::Subquery(_sub_query) => "Subquery",
             LogicalPlan::SubqueryAlias(_sqalias) => "SubqueryAlias",
             LogicalPlan::CreateCatalogSchema(_create) => "CreateCatalogSchema",
             LogicalPlan::CreateCatalog(_create_catalog) => "CreateCatalog",
             LogicalPlan::CreateView(_create_view) => "CreateView",
-            LogicalPlan::SetVariable(_) => "SetVariable",
+            LogicalPlan::Statement(_) => "Statement",
             // Further examine and return the name that is a possible Dask-SQL Extension type
             LogicalPlan::Extension(extension) => {
                 let node = extension.node.as_any();
                 if node.downcast_ref::<CreateModelPlanNode>().is_some() {
                     "CreateModel"
                 } else if node.downcast_ref::<CreateExperimentPlanNode>().is_some() {
                     "CreateExperiment"
@@ -421,14 +423,15 @@
                 let schema = self.original_plan.schema();
                 let rel_fields: Vec<RelDataTypeField> = schema
                     .fields()
                     .iter()
                     .map(|f| RelDataTypeField::from(f, schema.as_ref()))
                     .collect::<Result<Vec<_>>>()
                     .map_err(py_type_err)?;
+
                 Ok(RelDataType::new(false, rel_fields))
             }
         }
     }
 }
 
 impl From<PyLogicalPlan> for LogicalPlan {
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/optimizer/join_reorder.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/optimizer/join_reorder.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 //! Join reordering based on the paper "Improving Join Reordering for Large Scale Distributed Computing"
 //! https://ieeexplore.ieee.org/document/9378281
 
 use std::collections::HashSet;
 
-use datafusion_common::{Column, Result};
-use datafusion_expr::{Expr, Join, JoinType, LogicalPlan, LogicalPlanBuilder};
-use datafusion_optimizer::{utils, utils::split_conjunction, OptimizerConfig, OptimizerRule};
+use datafusion_python::{
+    datafusion_common::{Column, Result},
+    datafusion_expr::{Expr, Join, JoinType, LogicalPlan, LogicalPlanBuilder},
+    datafusion_optimizer::{utils, utils::split_conjunction, OptimizerConfig, OptimizerRule},
+};
 use log::warn;
 
 use crate::sql::table::DaskTableSource;
 
 pub struct JoinReorder {
     /// Maximum number of fact tables to allow in a join
     max_fact_tables: usize,
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/optimizer.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/optimizer.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,88 @@
 use std::sync::Arc;
 
-use datafusion_common::DataFusionError;
-use datafusion_expr::LogicalPlan;
-use datafusion_optimizer::{
-    common_subexpr_eliminate::CommonSubexprEliminate,
-    decorrelate_where_exists::DecorrelateWhereExists,
-    decorrelate_where_in::DecorrelateWhereIn,
-    eliminate_cross_join::EliminateCrossJoin,
-    eliminate_limit::EliminateLimit,
-    eliminate_outer_join::EliminateOuterJoin,
-    filter_null_join_keys::FilterNullJoinKeys,
-    inline_table_scan::InlineTableScan,
-    optimizer::{Optimizer, OptimizerRule},
-    push_down_filter::PushDownFilter,
-    push_down_limit::PushDownLimit,
-    push_down_projection::PushDownProjection,
-    rewrite_disjunctive_predicate::RewriteDisjunctivePredicate,
-    scalar_subquery_to_join::ScalarSubqueryToJoin,
-    simplify_expressions::SimplifyExpressions,
-    type_coercion::TypeCoercion,
-    unwrap_cast_in_comparison::UnwrapCastInComparison,
-    OptimizerContext,
+use datafusion_python::{
+    datafusion_common::DataFusionError,
+    datafusion_expr::LogicalPlan,
+    datafusion_optimizer::{
+        decorrelate_where_exists::DecorrelateWhereExists,
+        decorrelate_where_in::DecorrelateWhereIn,
+        eliminate_cross_join::EliminateCrossJoin,
+        eliminate_limit::EliminateLimit,
+        eliminate_outer_join::EliminateOuterJoin,
+        eliminate_project::EliminateProjection,
+        filter_null_join_keys::FilterNullJoinKeys,
+        optimizer::{Optimizer, OptimizerRule},
+        push_down_filter::PushDownFilter,
+        push_down_limit::PushDownLimit,
+        push_down_projection::PushDownProjection,
+        rewrite_disjunctive_predicate::RewriteDisjunctivePredicate,
+        scalar_subquery_to_join::ScalarSubqueryToJoin,
+        simplify_expressions::SimplifyExpressions,
+        unwrap_cast_in_comparison::UnwrapCastInComparison,
+        OptimizerContext,
+    },
 };
 use log::{debug, trace};
 
-mod filter_columns_post_join;
-
 mod join_reorder;
 use join_reorder::JoinReorder;
 
 /// Houses the optimization logic for Dask-SQL. This optimization controls the optimizations
 /// and their ordering in regards to their impact on the underlying `LogicalPlan` instance
 pub struct DaskSqlOptimizer {
     optimizer: Optimizer,
 }
 
 impl DaskSqlOptimizer {
     /// Creates a new instance of the DaskSqlOptimizer with all the DataFusion desired
     /// optimizers as well as any custom `OptimizerRule` trait impls that might be desired.
     pub fn new() -> Self {
         debug!("Creating new instance of DaskSqlOptimizer");
+
         let rules: Vec<Arc<dyn OptimizerRule + Sync + Send>> = vec![
-            Arc::new(InlineTableScan::new()),
-            Arc::new(TypeCoercion::new()),
             Arc::new(SimplifyExpressions::new()),
             Arc::new(UnwrapCastInComparison::new()),
+            // Arc::new(ReplaceDistinctWithAggregate::new()),
             Arc::new(DecorrelateWhereExists::new()),
             Arc::new(DecorrelateWhereIn::new()),
             Arc::new(ScalarSubqueryToJoin::new()),
+            //Arc::new(ExtractEquijoinPredicate::new()),
+
             // simplify expressions does not simplify expressions in subqueries, so we
             // run it again after running the optimizations that potentially converted
             // subqueries to joins
             Arc::new(SimplifyExpressions::new()),
+            // Arc::new(MergeProjection::new()),
+            Arc::new(RewriteDisjunctivePredicate::new()),
+            // Arc::new(EliminateDuplicatedExpr::new()),
+
             // TODO: need to handle EmptyRelation for GPU cases
             // Arc::new(EliminateFilter::new()),
             Arc::new(EliminateCrossJoin::new()),
-            Arc::new(CommonSubexprEliminate::new()),
+            // Arc::new(CommonSubexprEliminate::new()),
             Arc::new(EliminateLimit::new()),
-            Arc::new(RewriteDisjunctivePredicate::new()),
+            // Arc::new(PropagateEmptyRelation::new()),
             Arc::new(FilterNullJoinKeys::default()),
             Arc::new(EliminateOuterJoin::new()),
-            Arc::new(PushDownFilter::new()),
+            // Filters can't be pushed down past Limits, we should do PushDownFilter after PushDownLimit
             Arc::new(PushDownLimit::new()),
+            Arc::new(PushDownFilter::new()),
+            // Arc::new(SingleDistinctToGroupBy::new()),
             // Dask-SQL specific optimizations
-            // Arc::new(FilterColumnsPostJoin::new()),
             Arc::new(JoinReorder::default()),
             // The previous optimizations added expressions and projections,
             // that might benefit from the following rules
             Arc::new(SimplifyExpressions::new()),
             Arc::new(UnwrapCastInComparison::new()),
-            Arc::new(CommonSubexprEliminate::new()),
+            // Arc::new(CommonSubexprEliminate::new()),
             Arc::new(PushDownProjection::new()),
+            Arc::new(EliminateProjection::new()),
+            // PushDownProjection can pushdown Projections through Limits, do PushDownLimit again.
+            Arc::new(PushDownLimit::new()),
         ];
 
         Self {
             optimizer: Optimizer::with_rules(rules),
         }
     }
 
@@ -94,21 +102,23 @@
     }
 }
 
 #[cfg(test)]
 mod tests {
     use std::{any::Any, collections::HashMap, sync::Arc};
 
-    use datafusion::arrow::datatypes::{DataType, Field, Schema, SchemaRef};
-    use datafusion_common::{config::ConfigOptions, DataFusionError, Result};
-    use datafusion_expr::{AggregateUDF, LogicalPlan, ScalarUDF, TableSource};
-    use datafusion_sql::{
-        planner::{ContextProvider, SqlToRel},
-        sqlparser::{ast::Statement, parser::Parser},
-        TableReference,
+    use datafusion_python::{
+        datafusion::arrow::datatypes::{DataType, Field, Schema, SchemaRef},
+        datafusion_common::{config::ConfigOptions, DataFusionError, Result},
+        datafusion_expr::{AggregateUDF, LogicalPlan, ScalarUDF, TableSource},
+        datafusion_sql::{
+            planner::{ContextProvider, SqlToRel},
+            sqlparser::{ast::Statement, parser::Parser},
+            TableReference,
+        },
     };
 
     use crate::{dialect::DaskDialect, sql::optimizer::DaskSqlOptimizer};
 
     #[test]
     fn subquery_filter_with_cast() -> Result<()> {
         // regression test for https://github.com/apache/arrow-datafusion/issues/3760
@@ -122,16 +132,17 @@
         let expected = r#"Projection: test.col_int32
   Filter: CAST(test.col_int32 AS Float64) > __scalar_sq_1.__value
     CrossJoin:
       TableScan: test projection=[col_int32]
       SubqueryAlias: __scalar_sq_1
         Projection: AVG(test.col_int32) AS __value
           Aggregate: groupBy=[[]], aggr=[[AVG(test.col_int32)]]
-            Filter: test.col_utf8 >= Utf8("2002-05-08") AND test.col_utf8 <= Utf8("2002-05-13")
-              TableScan: test projection=[col_int32, col_utf8]"#;
+            Projection: test.col_int32
+              Filter: test.col_utf8 >= Utf8("2002-05-08") AND test.col_utf8 <= Utf8("2002-05-13")
+                TableScan: test projection=[col_int32, col_utf8]"#;
         assert_eq!(expected, format!("{:?}", plan));
         Ok(())
     }
 
     fn test_sql(sql: &str) -> Result<LogicalPlan> {
         // parse the SQL
         let dialect = DaskDialect {};
@@ -164,15 +175,15 @@
         fn options(&self) -> &ConfigOptions {
             &self.options
         }
 
         fn get_table_provider(
             &self,
             name: TableReference,
-        ) -> datafusion_common::Result<Arc<dyn TableSource>> {
+        ) -> datafusion_python::datafusion_common::Result<Arc<dyn TableSource>> {
             let table_name = name.table();
             if table_name.starts_with("test") {
                 let schema = Schema::new_with_metadata(
                     vec![
                         Field::new("col_int32", DataType::Int32, true),
                         Field::new("col_uint32", DataType::UInt32, true),
                         Field::new("col_utf8", DataType::Utf8, true),
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/parser_utils.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/parser_utils.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use datafusion_sql::sqlparser::{ast::ObjectName, parser::ParserError};
+use datafusion_python::datafusion_sql::sqlparser::{ast::ObjectName, parser::ParserError};
 
 pub struct DaskParserUtils;
 
 impl DaskParserUtils {
     /// Retrieves the schema and object name from a `ObjectName` instance
     pub fn elements_from_object_name(
         obj_name: &ObjectName,
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/schema.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/schema.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/statement.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/statement.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/table.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/table.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 use std::{any::Any, sync::Arc};
 
 use async_trait::async_trait;
-use datafusion::arrow::datatypes::{DataType, Field, SchemaRef};
-use datafusion_common::DFField;
-use datafusion_expr::{Expr, LogicalPlan, TableProviderFilterPushDown, TableSource};
-use datafusion_optimizer::utils::split_conjunction;
-use datafusion_sql::TableReference;
+use datafusion_python::{
+    datafusion::arrow::datatypes::{DataType, Field, SchemaRef},
+    datafusion_common::DFField,
+    datafusion_expr::{Expr, LogicalPlan, TableProviderFilterPushDown, TableSource},
+    datafusion_optimizer::utils::split_conjunction,
+    datafusion_sql::TableReference,
+};
 use pyo3::prelude::*;
 
 use super::logical::{create_table::CreateTablePlanNode, predict_model::PredictModelPlanNode};
 use crate::{
     error::DaskPlannerError,
     sql::{
         logical,
@@ -65,15 +67,15 @@
     fn schema(&self) -> SchemaRef {
         self.schema.clone()
     }
 
     fn supports_filter_pushdown(
         &self,
         filter: &Expr,
-    ) -> datafusion_common::Result<TableProviderFilterPushDown> {
+    ) -> datafusion_python::datafusion_common::Result<TableProviderFilterPushDown> {
         let filters = split_conjunction(filter);
         if filters.iter().all(|f| is_supported_push_down_expr(f)) {
             // Push down filters to the tablescan operation if all are supported
             Ok(TableProviderFilterPushDown::Exact)
         } else if filters.iter().any(|f| is_supported_push_down_expr(f)) {
             // Partially apply the filter in the TableScan but retain
             // the Filter operator in the plan as well
@@ -158,15 +160,15 @@
         let mut qualified_name = match &self.schema_name {
             Some(schema_name) => vec![schema_name.clone()],
             None => vec![],
         };
 
         match plan.original_plan {
             LogicalPlan::TableScan(table_scan) => {
-                qualified_name.push(table_scan.table_name);
+                qualified_name.push(table_scan.table_name.to_string());
             }
             _ => {
                 qualified_name.push(self.table_name.clone());
             }
         }
 
         qualified_name
@@ -203,15 +205,15 @@
                     DaskTypeMap::from(
                         SqlTypeName::from_arrow(data_type)?,
                         data_type.clone().into(),
                     ),
                 ));
             }
 
-            let table_ref: TableReference = table_scan.table_name.as_str().into();
+            let table_ref: TableReference = table_scan.table_name.clone();
             let (schema, tbl) = match table_ref {
                 TableReference::Bare { table } => ("".to_string(), table),
                 TableReference::Partial { schema, table } => (schema.to_string(), table),
                 TableReference::Full {
                     catalog: _,
                     schema,
                     table,
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/types/rel_data_type.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/types/rel_data_type.rs`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/types/rel_data_type_field.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/types/rel_data_type_field.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 use std::fmt;
 
-use datafusion_common::{DFField, DFSchema};
+use datafusion_python::{
+    datafusion_common::{DFField, DFSchema},
+    datafusion_sql::TableReference,
+};
 use pyo3::prelude::*;
 
 use crate::{
     error::Result,
     sql::types::{DaskTypeMap, SqlTypeName},
 };
 
@@ -17,26 +20,25 @@
     data_type: DaskTypeMap,
     index: usize,
 }
 
 // Functions that should not be presented to Python are placed here
 impl RelDataTypeField {
     pub fn from(field: &DFField, schema: &DFSchema) -> Result<RelDataTypeField> {
-        let qualifier: Option<&str> = match field.qualifier() {
-            Some(qualifier) => Some(qualifier),
-            None => None,
-        };
+        let qualifier: Option<&TableReference> = field.qualifier();
         Ok(RelDataTypeField {
             qualifier: qualifier.map(|qualifier| qualifier.to_string()),
             name: field.name().clone(),
             data_type: DaskTypeMap {
                 sql_type: SqlTypeName::from_arrow(field.data_type())?,
                 data_type: field.data_type().clone().into(),
             },
-            index: schema.index_of_column_by_name(qualifier, field.name())?,
+            index: schema
+                .index_of_column_by_name(qualifier, field.name())?
+                .unwrap(),
         })
     }
 }
 
 #[pymethods]
 impl RelDataTypeField {
     #[new]
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql/types.rs` & `dask_sql-2023.6.0/dask_planner/src/sql/types.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 pub mod rel_data_type;
 pub mod rel_data_type_field;
 
-use datafusion::arrow::datatypes::{DataType, IntervalUnit, TimeUnit};
-use datafusion_sql::sqlparser::{ast::DataType as SQLType, parser::Parser, tokenizer::Tokenizer};
+use datafusion_python::{
+    datafusion::arrow::datatypes::{DataType, IntervalUnit, TimeUnit},
+    datafusion_sql::sqlparser::{ast::DataType as SQLType, parser::Parser, tokenizer::Tokenizer},
+};
 use pyo3::{prelude::*, types::PyDict};
 
-use crate::{dialect::DaskDialect, error::DaskPlannerError};
+use crate::{dialect::DaskDialect, error::DaskPlannerError, sql::exceptions::py_type_err};
 
 #[derive(Debug, Clone, PartialEq, Eq, Hash, PartialOrd, Ord)]
 #[pyclass(name = "RexType", module = "datafusion")]
 pub enum RexType {
     Alias,
     Literal,
     Call,
@@ -107,14 +109,37 @@
                         (unit, tz)
                     }
                     // Default to Nanosecond and None for tz which is common if not present
                     None => (TimeUnit::Nanosecond, None),
                 };
                 DataType::Timestamp(unit, tz)
             }
+            SqlTypeName::DECIMAL => {
+                let (precision, scale) = match py_kwargs {
+                    Some(dict) => {
+                        let precision: u8 = match dict.get_item("precision") {
+                            Some(e) => {
+                                let res: PyResult<u8> = e.extract();
+                                res.unwrap()
+                            }
+                            None => 38,
+                        };
+                        let scale: i8 = match dict.get_item("scale") {
+                            Some(e) => {
+                                let res: PyResult<i8> = e.extract();
+                                res.unwrap()
+                            }
+                            None => 0,
+                        };
+                        (precision, scale)
+                    }
+                    None => (38, 10),
+                };
+                DataType::Decimal128(precision, scale)
+            }
             _ => sql_type.to_arrow()?,
         };
 
         Ok(DaskTypeMap {
             sql_type,
             data_type: d_type.into(),
         })
@@ -137,14 +162,33 @@
 
 #[derive(Debug, Clone, PartialEq, Eq, Hash, PartialOrd, Ord)]
 #[pyclass(name = "PyDataType", module = "datafusion", subclass)]
 pub struct PyDataType {
     data_type: DataType,
 }
 
+#[pymethods]
+impl PyDataType {
+    /// Gets the precision/scale represented by the PyDataType's decimal datatype
+    #[pyo3(name = "getPrecisionScale")]
+    pub fn get_precision_scale(&self) -> PyResult<(u8, i8)> {
+        Ok(match &self.data_type {
+            DataType::Decimal128(precision, scale) | DataType::Decimal256(precision, scale) => {
+                (*precision, *scale)
+            }
+            _ => {
+                return Err(py_type_err(format!(
+                    "Catch all triggered in get_precision_scale, {:?}",
+                    &self.data_type
+                )))
+            }
+        })
+    }
+}
+
 impl From<PyDataType> for DataType {
     fn from(data_type: PyDataType) -> DataType {
         data_type.data_type
     }
 }
 
 impl From<DataType> for PyDataType {
@@ -185,14 +229,15 @@
     INTERVAL_DAY_SECOND,
     INTERVAL_HOUR,
     INTERVAL_HOUR_MINUTE,
     INTERVAL_HOUR_SECOND,
     INTERVAL_MINUTE,
     INTERVAL_MINUTE_SECOND,
     INTERVAL_MONTH,
+    INTERVAL_MONTH_DAY_NANOSECOND,
     INTERVAL_SECOND,
     INTERVAL_YEAR,
     INTERVAL_YEAR_MONTH,
     MAP,
     MULTISET,
     NULL,
     OTHER,
@@ -253,15 +298,15 @@
                 None => Ok(SqlTypeName::TIMESTAMP),
             },
             DataType::Date32 => Ok(SqlTypeName::DATE),
             DataType::Date64 => Ok(SqlTypeName::DATE),
             DataType::Interval(unit) => match unit {
                 IntervalUnit::DayTime => Ok(SqlTypeName::INTERVAL_DAY),
                 IntervalUnit::YearMonth => Ok(SqlTypeName::INTERVAL_YEAR_MONTH),
-                IntervalUnit::MonthDayNano => Ok(SqlTypeName::INTERVAL_MONTH),
+                IntervalUnit::MonthDayNano => Ok(SqlTypeName::INTERVAL_MONTH_DAY_NANOSECOND),
             },
             DataType::Binary => Ok(SqlTypeName::BINARY),
             DataType::FixedSizeBinary(_size) => Ok(SqlTypeName::VARBINARY),
             DataType::Utf8 => Ok(SqlTypeName::CHAR),
             DataType::LargeUtf8 => Ok(SqlTypeName::VARCHAR),
             DataType::Struct(_fields) => Ok(SqlTypeName::STRUCTURED),
             DataType::Decimal128(_precision, _scale) => Ok(SqlTypeName::DECIMAL),
```

### Comparing `dask_sql-2023.4.0/dask_planner/src/sql.rs` & `dask_sql-2023.6.0/dask_planner/src/sql.rs`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,42 @@
 pub mod schema;
 pub mod statement;
 pub mod table;
 pub mod types;
 
 use std::{collections::HashMap, sync::Arc};
 
-use datafusion::arrow::datatypes::{DataType, Field, Schema, TimeUnit};
-use datafusion_common::{config::ConfigOptions, DFSchema, DataFusionError};
-use datafusion_expr::{
-    logical_plan::Extension,
-    AccumulatorFunctionImplementation,
-    AggregateUDF,
-    LogicalPlan,
-    PlanVisitor,
-    ReturnTypeFunction,
-    ScalarFunctionImplementation,
-    ScalarUDF,
-    Signature,
-    StateTypeFunction,
-    TableSource,
-    TypeSignature,
-    Volatility,
-};
-use datafusion_sql::{
-    parser::Statement as DFStatement,
-    planner::{ContextProvider, SqlToRel},
-    ResolvedTableReference,
-    TableReference,
+use datafusion_python::{
+    datafusion::arrow::datatypes::{DataType, Field, Schema, TimeUnit},
+    datafusion_common::{
+        config::ConfigOptions,
+        tree_node::{TreeNode, TreeNodeVisitor, VisitRecursion},
+        DFSchema,
+        DataFusionError,
+    },
+    datafusion_expr::{
+        logical_plan::Extension,
+        AccumulatorFunctionImplementation,
+        AggregateUDF,
+        LogicalPlan,
+        ReturnTypeFunction,
+        ScalarFunctionImplementation,
+        ScalarUDF,
+        Signature,
+        StateTypeFunction,
+        TableSource,
+        TypeSignature,
+        Volatility,
+    },
+    datafusion_sql::{
+        parser::Statement as DFStatement,
+        planner::{ContextProvider, SqlToRel},
+        ResolvedTableReference,
+        TableReference,
+    },
 };
 use log::{debug, warn};
 use pyo3::prelude::*;
 
 use self::logical::{
     create_catalog_schema::CreateCatalogSchemaPlanNode,
     drop_schema::DropSchemaPlanNode,
@@ -70,17 +76,17 @@
 /// DaskSQLContext is main interface used for interacting with DataFusion to
 /// parse SQL queries, build logical plans, and optimize logical plans.
 ///
 /// The following example demonstrates how to generate an optimized LogicalPlan
 /// from SQL using DaskSQLContext.
 ///
 /// ```
-/// use datafusion::prelude::*;
+/// use datafusion_python::datafusion::prelude::*;
 ///
-/// # use datafusion_common::Result;
+/// # use datafusion_python::datafusion_common::Result;
 /// # #[tokio::main]
 /// # async fn main() -> Result<()> {
 /// let mut ctx = DaskSQLContext::new();
 /// let parsed_sql = ctx.parse_sql("SELECT COUNT(*) FROM test_table");
 /// let nonOptimizedRelAlgebra = ctx.logical_relational_algebra(parsed_sql);
 /// let optmizedRelAlg = ctx.optimizeRelationalAlgebra(nonOptimizedRelAlgebra);
 /// # Ok(())
@@ -186,30 +192,43 @@
             DataType::Float16,
             DataType::Float32,
             DataType::Float64,
         ];
 
         match name {
             "year" => {
-                let sig = generate_signatures(vec![numeric_datatypes]);
+                let sig = Signature::exact(
+                    vec![DataType::Timestamp(TimeUnit::Nanosecond, None)],
+                    Volatility::Immutable,
+                );
                 let rtf: ReturnTypeFunction = Arc::new(|_| Ok(Arc::new(DataType::Int64)));
                 return Some(Arc::new(ScalarUDF::new(name, &sig, &rtf, &fun)));
             }
             "last_day" => {
                 let sig = Signature::exact(
                     vec![DataType::Timestamp(TimeUnit::Nanosecond, None)],
                     Volatility::Immutable,
                 );
                 let rtf: ReturnTypeFunction =
                     Arc::new(|_| Ok(Arc::new(DataType::Timestamp(TimeUnit::Nanosecond, None))));
                 return Some(Arc::new(ScalarUDF::new(name, &sig, &rtf, &fun)));
             }
             "timestampceil" | "timestampfloor" => {
-                let sig = Signature::exact(
-                    vec![DataType::Date64, DataType::Utf8],
+                // let sig = Signature::exact(
+                //     vec![DataType::Timestamp(TimeUnit::Nanosecond, None), DataType::Date64, DataType::Utf8],
+                //     Volatility::Immutable,
+                // );
+                let sig = Signature::one_of(
+                    vec![
+                        TypeSignature::Exact(vec![DataType::Date64, DataType::Utf8]),
+                        TypeSignature::Exact(vec![
+                            DataType::Timestamp(TimeUnit::Nanosecond, None),
+                            DataType::Utf8,
+                        ]),
+                    ],
                     Volatility::Immutable,
                 );
                 let rtf: ReturnTypeFunction = Arc::new(|_| Ok(Arc::new(DataType::Date64)));
                 return Some(Arc::new(ScalarUDF::new(name, &sig, &rtf, &fun)));
             }
             "timestampadd" => {
                 let sig = Signature::one_of(
@@ -352,15 +371,16 @@
             DataType::Float16,
             DataType::Float32,
             DataType::Float64,
         ];
 
         match name {
             "every" => {
-                let sig = generate_signatures(vec![numeric_datatypes]);
+                // let sig = generate_signatures(vec![DataType::Boolean]);
+                let sig = Signature::exact(vec![DataType::Boolean], Volatility::Immutable);
                 let rtf: ReturnTypeFunction = Arc::new(|_| Ok(Arc::new(DataType::Boolean)));
                 return Some(Arc::new(AggregateUDF::new(name, &sig, &rtf, &acc, &st)));
             }
             "bit_and" | "bit_or" => {
                 let sig = generate_signatures(vec![numeric_datatypes]);
                 let rtf: ReturnTypeFunction = Arc::new(|_| Ok(Arc::new(DataType::Int64)));
                 return Some(Arc::new(AggregateUDF::new(name, &sig, &rtf, &acc, &st)));
@@ -514,28 +534,29 @@
     pub fn optimize_relational_algebra(
         &self,
         existing_plan: logical::PyLogicalPlan,
     ) -> PyResult<logical::PyLogicalPlan> {
         // Certain queries cannot be optimized. Ex: `EXPLAIN SELECT * FROM test` simply return those plans as is
         let mut visitor = OptimizablePlanVisitor {};
 
-        match existing_plan.original_plan.accept(&mut visitor) {
+        match existing_plan.original_plan.visit(&mut visitor) {
             Ok(valid) => {
-                if valid {
-                    optimizer::DaskSqlOptimizer::new()
+                match valid {
+                    VisitRecursion::Stop => {
+                        // This LogicalPlan does not support Optimization. Return original
+                        warn!("This LogicalPlan does not support Optimization. Returning original");
+                        Ok(existing_plan)
+                    }
+                    _ => optimizer::DaskSqlOptimizer::new()
                         .optimize(existing_plan.original_plan)
                         .map(|k| PyLogicalPlan {
                             original_plan: k,
                             current_node: None,
                         })
-                        .map_err(py_optimization_exp)
-                } else {
-                    // This LogicalPlan does not support Optimization. Return original
-                    warn!("This LogicalPlan does not support Optimization. Returning original");
-                    Ok(existing_plan)
+                        .map_err(py_optimization_exp),
                 }
             }
             Err(e) => Err(py_optimization_exp(e)),
         }
     }
 }
 
@@ -690,27 +711,27 @@
         }
     }
 }
 
 /// Visits each AST node to determine if the plan is valid for optimization or not
 pub struct OptimizablePlanVisitor;
 
-impl PlanVisitor for OptimizablePlanVisitor {
-    type Error = DataFusionError;
+impl TreeNodeVisitor for OptimizablePlanVisitor {
+    type N = LogicalPlan;
 
-    fn pre_visit(&mut self, plan: &LogicalPlan) -> std::result::Result<bool, DataFusionError> {
+    fn pre_visit(&mut self, plan: &LogicalPlan) -> Result<VisitRecursion, DataFusionError> {
         // If the plan contains an unsupported Node type we flag the plan as un-optimizable here
         match plan {
-            LogicalPlan::Explain(..) => Ok(false),
-            _ => Ok(true),
+            LogicalPlan::Explain(..) => Ok(VisitRecursion::Stop),
+            _ => Ok(VisitRecursion::Continue),
         }
     }
 
-    fn post_visit(&mut self, _plan: &LogicalPlan) -> std::result::Result<bool, DataFusionError> {
-        Ok(true)
+    fn post_visit(&mut self, _plan: &LogicalPlan) -> Result<VisitRecursion, DataFusionError> {
+        Ok(VisitRecursion::Continue)
     }
 }
 
 fn generate_signatures(cartesian_setup: Vec<Vec<DataType>>) -> Signature {
     let mut exact_vector = vec![];
     let mut datatypes_iter = cartesian_setup.iter();
     // First pass
@@ -739,16 +760,18 @@
     }
 
     Signature::one_of(one_of_vector.clone(), Volatility::Immutable)
 }
 
 #[cfg(test)]
 mod test {
-    use datafusion::arrow::datatypes::DataType;
-    use datafusion_expr::{Signature, TypeSignature, Volatility};
+    use datafusion_python::{
+        datafusion::arrow::datatypes::DataType,
+        datafusion_expr::{Signature, TypeSignature, Volatility},
+    };
 
     use crate::sql::generate_signatures;
 
     #[test]
     fn test_generate_signatures() {
         let sig = generate_signatures(vec![
             vec![DataType::Int64, DataType::Float64],
```

### Comparing `dask_sql-2023.4.0/dask_sql/_compat.py` & `dask_sql-2023.6.0/dask_sql/_compat.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 import prompt_toolkit
 from packaging.version import parse as parseVersion
 
 _pandas_version = parseVersion(pd.__version__)
 _prompt_toolkit_version = parseVersion(prompt_toolkit.__version__)
 _dask_version = parseVersion(dask.__version__)
 
-FLOAT_NAN_IMPLEMENTED = _pandas_version >= parseVersion("1.2.0")
-INT_NAN_IMPLEMENTED = _pandas_version >= parseVersion("1.0.0")
 INDEXER_WINDOW_STEP_IMPLEMENTED = _pandas_version >= parseVersion("1.5.0")
 
 # TODO: remove if prompt-toolkit min version gets bumped
 PIPE_INPUT_CONTEXT_MANAGER = _prompt_toolkit_version >= parseVersion("3.0.29")
 
 # TODO: remove when dask min version gets bumped
 BROADCAST_JOIN_SUPPORT_WORKING = _dask_version > parseVersion("2023.1.0")
+
+# Parquet predicate-support version checks
+PQ_NOT_IN_SUPPORT = parseVersion(dask.__version__) > parseVersion("2023.5.1")
+PQ_IS_SUPPORT = parseVersion(dask.__version__) >= parseVersion("2023.3.1")
```

### Comparing `dask_sql-2023.4.0/dask_sql/cmd.py` & `dask_sql-2023.6.0/dask_sql/cmd.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/context.py` & `dask_sql-2023.6.0/dask_sql/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from collections import Counter
 from typing import Any, Callable, Dict, List, Tuple, Union
 
 import dask.dataframe as dd
 import pandas as pd
 from dask import config as dask_config
 from dask.base import optimize
+from dask.utils_test import hlg_layer
 
 from dask_planner.rust import (
     DaskSchema,
     DaskSQLContext,
     DaskTable,
     DFOptimizationException,
     DFParsingException,
@@ -243,14 +244,23 @@
             gpu=gpu,
             **kwargs,
         )
 
         if type(input_table) == str:
             dc.filepath = input_table
             self.schema[schema_name].filepaths[table_name.lower()] = input_table
+        elif hasattr(input_table, "dask") and dd.utils.is_dataframe_like(input_table):
+            try:
+                dask_filepath = hlg_layer(
+                    input_table.dask, "read-parquet"
+                ).creation_info["args"][0]
+                dc.filepath = dask_filepath
+                self.schema[schema_name].filepaths[table_name.lower()] = dask_filepath
+            except KeyError:
+                logger.debug("Expected 'read-parquet' layer")
 
         if parquet_statistics and not statistics:
             statistics = parquet_statistics(dc.df)
             if statistics:
                 row_count = 0
                 for d in statistics:
                     row_count += d["num-rows"]
```

### Comparing `dask_sql-2023.4.0/dask_sql/datacontainer.py` & `dask_sql-2023.6.0/dask_sql/datacontainer.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/input_utils/convert.py` & `dask_sql-2023.6.0/dask_sql/input_utils/convert.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/input_utils/dask.py` & `dask_sql-2023.6.0/dask_sql/input_utils/dask.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/input_utils/hive.py` & `dask_sql-2023.6.0/dask_sql/input_utils/hive.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/input_utils/intake.py` & `dask_sql-2023.6.0/dask_sql/input_utils/intake.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/input_utils/location.py` & `dask_sql-2023.6.0/dask_sql/input_utils/location.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/input_utils/pandaslike.py` & `dask_sql-2023.6.0/dask_sql/input_utils/pandaslike.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/input_utils/sqlalchemy.py` & `dask_sql-2023.6.0/dask_sql/input_utils/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/integrations/fugue.py` & `dask_sql-2023.6.0/dask_sql/integrations/fugue.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/integrations/ipython.py` & `dask_sql-2023.6.0/dask_sql/integrations/ipython.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/mappings.py` & `dask_sql-2023.6.0/dask_sql/mappings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import logging
+from datetime import datetime
 from typing import Any
 
 import dask.array as da
+import dask.config as dask_config
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 
 from dask_planner.rust import DaskTypeMap, SqlTypeName
-from dask_sql._compat import FLOAT_NAN_IMPLEMENTED
 
 logger = logging.getLogger(__name__)
 
+
 # Default mapping between python types and SQL types
 _PYTHON_TO_SQL = {
     np.float64: SqlTypeName.DOUBLE,
+    pd.Float64Dtype(): SqlTypeName.DOUBLE,
     float: SqlTypeName.FLOAT,
     np.float32: SqlTypeName.FLOAT,
+    pd.Float32Dtype(): SqlTypeName.FLOAT,
     np.int64: SqlTypeName.BIGINT,
     pd.Int64Dtype(): SqlTypeName.BIGINT,
     int: SqlTypeName.INTEGER,
     np.int32: SqlTypeName.INTEGER,
     pd.Int32Dtype(): SqlTypeName.INTEGER,
     np.int16: SqlTypeName.SMALLINT,
     pd.Int16Dtype(): SqlTypeName.SMALLINT,
@@ -37,19 +41,14 @@
     pd.BooleanDtype(): SqlTypeName.BOOLEAN,
     str: SqlTypeName.VARCHAR,
     np.object_: SqlTypeName.VARCHAR,
     pd.StringDtype(): SqlTypeName.VARCHAR,
     np.datetime64: SqlTypeName.TIMESTAMP,
 }
 
-if FLOAT_NAN_IMPLEMENTED:  # pragma: no cover
-    _PYTHON_TO_SQL.update(
-        {pd.Float32Dtype(): SqlTypeName.FLOAT, pd.Float64Dtype(): SqlTypeName.DOUBLE}
-    )
-
 # Default mapping between SQL types and python types
 # for values
 _SQL_TO_PYTHON_SCALARS = {
     "SqlTypeName.DOUBLE": np.float64,
     "SqlTypeName.FLOAT": np.float32,
     "SqlTypeName.DECIMAL": np.float32,
     "SqlTypeName.BIGINT": np.int64,
@@ -81,14 +80,15 @@
     ),  # TODO: ideally this would be np.dtype("<M8[D]") but that doesn't work for Pandas
     "SqlTypeName.TIME": np.dtype("<M8[ns]"),
     "SqlTypeName.TIMESTAMP": np.dtype("<M8[ns]"),
     "SqlTypeName.TIMESTAMP_WITH_LOCAL_TIME_ZONE": pd.DatetimeTZDtype(
         unit="ns", tz="UTC"
     ),  # Everything is converted to UTC. So far, this did not break
     "SqlTypeName.INTERVAL_DAY": np.dtype("<m8[ns]"),
+    "SqlTypeName.INTERVAL_MONTH_DAY_NANOSECOND": np.dtype("<m8[ns]"),
     "SqlTypeName.NULL": type(None),
 }
 
 
 def python_to_sql_type(python_type) -> "DaskTypeMap":
     """Mapping between python and SQL types."""
 
@@ -103,22 +103,49 @@
     if pd.api.types.is_datetime64tz_dtype(python_type):
         return DaskTypeMap(
             SqlTypeName.TIMESTAMP_WITH_LOCAL_TIME_ZONE,
             unit=str(python_type.unit),
             tz=str(python_type.tz),
         )
 
+    if is_decimal(python_type):
+        return DaskTypeMap(
+            SqlTypeName.DECIMAL,
+            precision=python_type.precision,
+            scale=python_type.scale,
+        )
+
     try:
         return DaskTypeMap(_PYTHON_TO_SQL[python_type])
     except KeyError:  # pragma: no cover
         raise NotImplementedError(
             f"The python type {python_type} is not implemented (yet)"
         )
 
 
+def parse_datetime(obj):
+    formats = [
+        "%Y-%m-%d %H:%M:%S",
+        "%Y-%m-%d",
+        "%d-%m-%Y %H:%M:%S",
+        "%d-%m-%Y",
+        "%m/%d/%Y %H:%M:%S",
+        "%m/%d/%Y",
+    ]
+
+    for f in formats:
+        try:
+            datetime_obj = datetime.strptime(obj, f)
+            return datetime_obj
+        except ValueError:
+            pass
+
+    raise ValueError("Unable to parse datetime: " + obj)
+
+
 def sql_to_python_value(sql_type: "SqlTypeName", literal_value: Any) -> Any:
     """Mapping between SQL and python values (of correct type)."""
     # In most of the cases, we turn the value first into a string.
     # That might not be the most efficient thing to do,
     # but works for all types (so far)
     # Additionally, a literal type is not used
     # so often anyways.
@@ -135,14 +162,22 @@
             encoding, literal_value = literal_value.split("'", 1)
             literal_value = literal_value.rstrip("'")
             literal_value = literal_value.encode(encoding=encoding)
             return literal_value.decode(encoding=encoding)
 
         return literal_value
 
+    elif (
+        sql_type == SqlTypeName.DECIMAL
+        and dask_config.get("sql.mappings.decimal_support") == "cudf"
+    ):
+        from decimal import Decimal
+
+        python_type = Decimal
+
     elif sql_type == SqlTypeName.INTERVAL_DAY:
         return np.timedelta64(literal_value[0], "D") + np.timedelta64(
             literal_value[1], "ms"
         )
     elif sql_type == SqlTypeName.INTERVAL:
         # check for finer granular interval types, e.g., INTERVAL MONTH, INTERVAL YEAR
         try:
@@ -158,35 +193,37 @@
         except TypeError:  # pragma: no cover
             # interval type is not recognized, fall back to default case
             pass
 
         # Calcite will always convert INTERVAL types except YEAR, QUATER, MONTH to milliseconds
         # Issue: if sql_type is INTERVAL MICROSECOND, and value <= 1000, literal_value will be rounded to 0
         return np.timedelta64(literal_value, "ms")
+    elif sql_type == SqlTypeName.INTERVAL_MONTH_DAY_NANOSECOND:
+        # DataFusion assumes 30 days per month. Therefore we multiply number of months by 30 and add to days
+        return np.timedelta64(
+            (literal_value[0] * 30) + literal_value[1], "D"
+        ) + np.timedelta64(literal_value[2], "ns")
 
     elif sql_type == SqlTypeName.BOOLEAN:
         return bool(literal_value)
 
     elif (
         sql_type == SqlTypeName.TIMESTAMP
         or sql_type == SqlTypeName.TIME
         or sql_type == SqlTypeName.DATE
     ):
         if isinstance(literal_value, str):
+            literal_value = parse_datetime(literal_value)
             literal_value = np.datetime64(literal_value)
         elif str(literal_value) == "None":
             # NULL time
             return pd.NaT  # pragma: no cover
         if sql_type == SqlTypeName.DATE:
             return literal_value.astype("<M8[D]")
         return literal_value.astype("<M8[ns]")
-    elif sql_type == SqlTypeName.DECIMAL:
-        # We use np.float64 always, even though we might
-        # be able to use a smaller type
-        python_type = np.float64
     else:
         try:
             python_type = _SQL_TO_PYTHON_SCALARS[str(sql_type)]
         except KeyError:  # pragma: no cover
             raise NotImplementedError(
                 f"The SQL type {sql_type} is not implemented (yet)"
             )
@@ -199,17 +236,28 @@
             return np.NaN
         else:
             return pd.NA
 
     return python_type(literal_value)
 
 
-def sql_to_python_type(sql_type: "SqlTypeName") -> type:
+def sql_to_python_type(sql_type: "SqlTypeName", *args) -> type:
     """Turn an SQL type into a dataframe dtype"""
     try:
+        if (
+            sql_type == SqlTypeName.DECIMAL
+            and dask_config.get("sql.mappings.decimal_support") == "cudf"
+        ):
+            try:
+                import cudf
+            except ImportError:
+                raise ModuleNotFoundError(
+                    "Setting `sql.mappings.decimal_support=cudf` requires cudf"
+                )
+            return cudf.Decimal128Dtype(*args)
         return _SQL_TO_PYTHON_FRAMES[str(sql_type)]
     except KeyError:  # pragma: no cover
         raise NotImplementedError(
             f"The SQL type {str(sql_type)} is not implemented (yet)"
         )
 
 
@@ -235,23 +283,28 @@
     is_bool = pdt.is_bool_dtype
 
     checks = [
         is_uint,
         is_sint,
         is_float,
         is_object,
-        is_string,
+        # is_string_dtype considers decimal columns to be string columns
+        lambda x: is_string(x) and not is_decimal(x),
         is_dt_tz,
         is_dt_ntz,
         is_td_ns,
         is_bool,
+        is_decimal,
     ]
 
     for check in checks:
         if check(lhs) and check(rhs):
+            # check that decimal columns have equal precision/scale
+            if check is is_decimal:
+                return lhs.precision == rhs.precision and lhs.scale == rhs.scale
             return True
 
     return False
 
 
 def cast_column_type(
     df: dd.DataFrame, column_name: str, expected_type: type
@@ -294,7 +347,14 @@
             col = da.trunc(col.fillna(value=np.NaN))
         elif pd.api.types.is_timedelta64_dtype(current_type):
             logger.debug(f"Explicitly casting from {current_type} to np.int64")
             return col.astype(np.int64)
 
     logger.debug(f"Need to cast from {current_type} to {expected_type}")
     return col.astype(expected_type)
+
+
+def is_decimal(dtype):
+    """
+    Check if dtype is a decimal type
+    """
+    return "decimal" in str(dtype).lower()
```

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/base.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -100,12 +100,18 @@
 
         field_types = {
             str(field.getQualifiedName()): field.getType()
             for field in row_type.getFieldList()
         }
 
         for field_name, field_type in field_types.items():
-            expected_type = sql_to_python_type(field_type.getSqlType())
+            sql_type = field_type.getSqlType()
+            sql_type_args = tuple()
+
+            if str(sql_type) == "SqlTypeName.DECIMAL":
+                sql_type_args = field_type.getDataType().getPrecisionScale()
+
+            expected_type = sql_to_python_type(sql_type, *sql_type_args)
             df_field_name = cc.get_backend_by_frontend_name(field_name)
             df = cast_column_type(df, df_field_name, expected_type)
 
         return DataContainer(df, dc.column_container)
```

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/convert.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/convert.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/__init__.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/alter.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/alter.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/analyze_table.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/analyze_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/create_catalog_schema.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_catalog_schema.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/create_experiment.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_experiment.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/create_memory_table.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_memory_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/create_model.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/create_table.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/create_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/describe_model.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/describe_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/distributeby.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/distributeby.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/drop_model.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/drop_schema.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_schema.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/drop_table.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/drop_table.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/export_model.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/export_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/metrics.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/metrics.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/predict_model.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/predict_model.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/show_columns.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_columns.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/show_models.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_models.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/show_schemas.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_schemas.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/show_tables.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/show_tables.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/use_schema.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/use_schema.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/custom/wrappers.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/custom/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 import sklearn.metrics
 from dask.delayed import Delayed
 from dask.highlevelgraph import HighLevelGraph
 from sklearn.metrics import check_scoring as sklearn_check_scoring
 from sklearn.metrics import make_scorer
 from sklearn.utils.validation import check_is_fitted
 
-from dask_sql.utils import make_pickable_without_dask_sql
-
 try:
     import sklearn.base
     import sklearn.metrics
 except ImportError:  # pragma: no cover
     raise ImportError("sklearn must be installed")
 
 from dask_sql.physical.rel.custom.metrics import (
@@ -593,33 +591,30 @@
             shape[0] = 0
         ar = type(output_meta)(shape, dtype=output_meta.dtype)
         return ar
     elif hasattr(output_meta, "iloc"):
         return output_meta.iloc[:0, :]
 
 
-@make_pickable_without_dask_sql
 def _predict(part, estimator, output_meta=None):
     if part.shape[0] == 0 and output_meta is not None:
         empty_output = handle_empty_partitions(output_meta)
         if empty_output is not None:
             return empty_output
     return estimator.predict(part)
 
 
-@make_pickable_without_dask_sql
 def _predict_proba(part, estimator, output_meta=None):
     if part.shape[0] == 0 and output_meta is not None:
         empty_output = handle_empty_partitions(output_meta)
         if empty_output is not None:
             return empty_output
     return estimator.predict_proba(part)
 
 
-@make_pickable_without_dask_sql
 def _transform(part, estimator, output_meta=None):
     if part.shape[0] == 0 and output_meta is not None:
         empty_output = handle_empty_partitions(output_meta)
         if empty_output is not None:
             return empty_output
     return estimator.transform(part)
```

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/__init__.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/aggregate.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/aggregate.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/cross_join.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/cross_join.py`

 * *Files 25% similar despite different names*

```diff
@@ -33,9 +33,21 @@
         cross_join_key = utils.new_temporary_column(df_lhs)
         df_lhs[cross_join_key] = 1
         df_rhs[cross_join_key] = 1
 
         result = df_lhs.merge(df_rhs, on=cross_join_key, suffixes=("", "0")).drop(
             cross_join_key, 1
         )
+        cc = ColumnContainer(result.columns)
 
-        return DataContainer(result, ColumnContainer(result.columns))
+        # Rename columns like the rel specifies
+        row_type = rel.getRowType()
+        field_specifications = [str(f) for f in row_type.getFieldNames()]
+
+        cc = cc.rename(
+            {
+                from_col: to_col
+                for from_col, to_col in zip(cc.columns, field_specifications)
+            }
+        )
+        cc = self.fix_column_to_row_type(cc, row_type)
+        return DataContainer(result, cc)
```

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/empty.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/empty.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/filter.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/filter.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/join.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/join.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -213,23 +213,14 @@
         df_lhs_renamed: dd.DataFrame,
         df_rhs_renamed: dd.DataFrame,
         lhs_on: List[str],
         rhs_on: List[str],
         join_type: str,
     ) -> dd.DataFrame:
 
-        lhs_columns_to_add = {
-            f"common_{i}": df_lhs_renamed["lhs_" + str(index)]
-            for i, index in enumerate(lhs_on)
-        }
-        rhs_columns_to_add = {
-            f"common_{i}": df_rhs_renamed.iloc[:, index]
-            for i, index in enumerate(rhs_on)
-        }
-
         # SQL compatibility: when joining on columns that
         # contain NULLs, pandas will actually happily
         # keep those NULLs. That is however not compatible with
         # SQL, so we get rid of them here
         if join_type in ["inner", "right"]:
             df_lhs_filter = reduce(
                 operator.and_,
@@ -239,14 +230,23 @@
         if join_type in ["inner", "left"]:
             df_rhs_filter = reduce(
                 operator.and_,
                 [~df_rhs_renamed.iloc[:, index].isna() for index in rhs_on],
             )
             df_rhs_renamed = df_rhs_renamed[df_rhs_filter]
 
+        lhs_columns_to_add = {
+            f"common_{i}": df_lhs_renamed["lhs_" + str(index)]
+            for i, index in enumerate(lhs_on)
+        }
+        rhs_columns_to_add = {
+            f"common_{i}": df_rhs_renamed.iloc[:, index]
+            for i, index in enumerate(rhs_on)
+        }
+
         df_lhs_with_tmp = df_lhs_renamed.assign(**lhs_columns_to_add)
         df_rhs_with_tmp = df_rhs_renamed.assign(**rhs_columns_to_add)
         added_columns = list(lhs_columns_to_add.keys())
 
         broadcast = dask_config.get("sql.join.broadcast")
         if not BROADCAST_JOIN_SUPPORT_WORKING and (
             isinstance(broadcast, float) or broadcast
```

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/limit.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/limit.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/project.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/project.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/sample.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/sample.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/sort.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/sort.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/subquery_alias.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/subquery_alias.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/table_scan.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/table_scan.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/union.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/union.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/values.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/values.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rel/logical/window.py` & `dask_sql-2023.6.0/dask_sql/physical/rel/logical/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,15 @@
 from pandas.api.indexers import BaseIndexer
 
 from dask_sql._compat import INDEXER_WINDOW_STEP_IMPLEMENTED
 from dask_sql.datacontainer import ColumnContainer, DataContainer
 from dask_sql.physical.rel.base import BaseRelPlugin
 from dask_sql.physical.rex.convert import RexConverter
 from dask_sql.physical.utils.sort import sort_partition_func
-from dask_sql.utils import (
-    LoggableDataFrame,
-    make_pickable_without_dask_sql,
-    new_temporary_column,
-)
+from dask_sql.utils import LoggableDataFrame, new_temporary_column
 
 if TYPE_CHECKING:
     import dask_sql
     from dask_planner.rust import LogicalPlan
 
 logger = logging.getLogger(__name__)
 
@@ -243,14 +239,15 @@
     }
 
     def convert(self, rel: "LogicalPlan", context: "dask_sql.Context") -> DataContainer:
         (dc,) = self.assert_inputs(rel, 1, context)
 
         # Output to the right field names right away
         field_names = rel.getRowType().getFieldNames()
+
         for window in rel.window().getGroups():
             dc = self._apply_window(rel, window, dc, field_names, context)
 
         # Finally, fix the output schema if needed
         df = dc.df
         cc = dc.column_container
         cc = self.fix_column_to_row_type(cc, rel.getRowType())
@@ -340,27 +337,24 @@
             upper_bound=upper_bound,
             operations=operations,
         )
 
         # TODO: That is a bit of a hack. We should really use the real column dtype
         meta = df._meta.assign(**{col: 0.0 for col in newly_created_columns})
 
-        df = df.groupby(group_columns, dropna=False).apply(
-            make_pickable_without_dask_sql(filled_map), meta=meta
-        )
+        df = df.groupby(group_columns, dropna=False).apply(filled_map, meta=meta)
         logger.debug(
             f"Having created a dataframe {LoggableDataFrame(df)} after windowing. Will now drop {temporary_columns}."
         )
         df = df.drop(columns=temporary_columns).reset_index(drop=True)
 
         dc = DataContainer(df, cc)
         df = dc.df
         cc = dc.column_container
         for c in newly_created_columns:
-            # the fields are in the correct order by definition
             field_name = field_names[len(cc.columns)]
             cc = cc.add(field_name, c)
         dc = DataContainer(df, cc)
         logger.debug(
             f"Removed unneeded columns and registered new ones: {LoggableDataFrame(dc)}."
         )
         return dc
```

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rex/base.py` & `dask_sql-2023.6.0/dask_sql/physical/rex/base.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rex/convert.py` & `dask_sql-2023.6.0/dask_sql/physical/rex/convert.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rex/core/alias.py` & `dask_sql-2023.6.0/dask_sql/physical/rex/core/alias.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rex/core/call.py` & `dask_sql-2023.6.0/dask_sql/physical/rex/core/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from dask_sql.physical.rex.core.literal import SargPythonImplementation
 from dask_sql.utils import (
     LoggableDataFrame,
     convert_to_datetime,
     is_cudf_type,
     is_datetime,
     is_frame,
-    make_pickable_without_dask_sql,
 )
 
 if TYPE_CHECKING:
     import dask_sql
     from dask_planner.rust import Expression, LogicalPlan
 
 logger = logging.getLogger(__name__)
@@ -239,21 +238,26 @@
 
     needs_rex = True
 
     def __init__(self):
         super().__init__(self.cast)
 
     def cast(self, operand, rex=None) -> SeriesOrScalar:
-        output_type = str(rex.getType())
-        sql_type = SqlTypeName.fromString(output_type.upper())
+        output_type = rex.getType()
+        sql_type = SqlTypeName.fromString(output_type)
+        sql_type_args = ()
+
+        # decimal datatypes require precision and scale
+        if output_type == "DECIMAL":
+            sql_type_args = rex.getPrecisionScale()
 
         if not is_frame(operand):  # pragma: no cover
             return sql_to_python_value(sql_type, operand)
 
-        python_type = sql_to_python_type(sql_type)
+        python_type = sql_to_python_type(sql_type, *sql_type_args)
 
         return_column = cast_column_to_type(operand, python_type)
 
         if return_column is None:
             return_column = operand
 
         # TODO: ideally we don't want to directly access the datetimes,
@@ -430,50 +434,55 @@
 
             transformed_regex += char
 
         # the SQL like always goes over the full string
         transformed_regex = "^" + transformed_regex + "$"
 
         # Finally, apply the string
+        flags = re.DOTALL | re.IGNORECASE if not self.case_sensitive else re.DOTALL
         if is_frame(test):
-            return test.str.match(transformed_regex).astype("boolean")
+            return test.str.match(transformed_regex, flags=flags).astype("boolean")
         else:
-            return bool(re.match(transformed_regex, test))
+            return bool(re.match(transformed_regex, test, flags=flags))
 
 
 class LikeOperation(RegexOperation):
-    replacement_chars = [
-        "#",
-        "$",
-        "^",
-        ".",
-        "|",
-        "~",
-        "-",
-        "+",
-        "*",
-        "?",
-        "(",
-        ")",
-        "{",
-        "}",
-        "[",
-        "]",
-    ]
+    def __init__(self, case_sensitive: bool = True):
+        self.case_sensitive = case_sensitive
+        self.replacement_chars = [
+            "#",
+            "$",
+            "^",
+            ".",
+            "|",
+            "~",
+            "-",
+            "+",
+            "*",
+            "?",
+            "(",
+            ")",
+            "{",
+            "}",
+            "[",
+            "]",
+        ]
+        super().__init__()
 
 
 class SimilarOperation(RegexOperation):
     replacement_chars = [
         "#",
         "$",
         "^",
         ".",
         "~",
         "-",
     ]
+    case_sensitive = True
 
 
 class PositionOperation(Operation):
     """The position operator (get the position of a string)"""
 
     def __init__(self):
         super().__init__(self.position)
@@ -795,15 +804,15 @@
         # for each partition
         df = dc.df
         name = "sample-" + tokenize(df, random_state)
 
         state_data = random_state_data(df.npartitions, random_state)
         dsk = {
             (name, i): (
-                make_pickable_without_dask_sql(self.random_function),
+                self.random_function,
                 (df._name, i),
                 np.random.RandomState(state),
                 kwargs,
             )
             for i, state in enumerate(state_data)
         }
 
@@ -993,16 +1002,19 @@
         "*": ReduceOperation(operation=operator.mul),
         "is distinct from": NotOperation().of(IsNotDistinctOperation()),
         "is not distinct from": IsNotDistinctOperation(),
         "/int": IntDivisionOperator(),
         # special operations
         "cast": CastOperation(),
         "case": CaseOperation(),
-        "not like": NotOperation().of(LikeOperation()),
-        "like": LikeOperation(),
+        "not like": NotOperation().of(LikeOperation(case_sensitive=True)),
+        "like": LikeOperation(case_sensitive=True),
+        "not ilike": NotOperation().of(LikeOperation(case_sensitive=False)),
+        "ilike": LikeOperation(case_sensitive=False),
+        "not similar to": NotOperation().of(SimilarOperation()),
         "similar to": SimilarOperation(),
         "negative": NegativeOperation(),
         "not": NotOperation(),
         "in list": InListOperation(),
         "is null": IsNullOperation(),
         "is not null": NotOperation().of(IsNullOperation()),
         "is true": IsTrueOperation(),
```

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rex/core/input_ref.py` & `dask_sql-2023.6.0/dask_sql/physical/rex/core/input_ref.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rex/core/literal.py` & `dask_sql-2023.6.0/dask_sql/physical/rex/core/literal.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,17 @@
             literal_type = SqlTypeName.TIME
         elif literal_type == "Null":
             literal_type = SqlTypeName.NULL
             literal_value = None
         elif literal_type == "IntervalDayTime":
             literal_type = SqlTypeName.INTERVAL_DAY
             literal_value = rex.getIntervalDayTimeValue()
+        elif literal_type == "IntervalMonthDayNano":
+            literal_type = SqlTypeName.INTERVAL_MONTH_DAY_NANOSECOND
+            literal_value = rex.getIntervalMonthDayNanoValue()
         elif literal_type in {
             "TimestampSecond",
             "TimestampMillisecond",
             "TimestampMicrosecond",
             "TimestampNanosecond",
         }:
             unit_mapping = {
```

### Comparing `dask_sql-2023.4.0/dask_sql/physical/rex/core/subquery.py` & `dask_sql-2023.6.0/dask_sql/physical/rex/core/subquery.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/utils/filter.py` & `dask_sql-2023.6.0/dask_sql/physical/utils/filter.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import itertools
 import logging
 import operator
 
 import dask.dataframe as dd
 import numpy as np
 from dask.blockwise import Blockwise
-from dask.highlevelgraph import HighLevelGraph
+from dask.highlevelgraph import HighLevelGraph, MaterializedLayer
 from dask.layers import DataFrameIOLayer
 from dask.utils import M, apply, is_arraylike
 
+from dask_sql._compat import PQ_IS_SUPPORT, PQ_NOT_IN_SUPPORT
+
 logger = logging.getLogger(__name__)
 
 
 def attempt_predicate_pushdown(ddf: dd.DataFrame) -> dd.DataFrame:
     """Use graph information to update IO-level filters
 
     The original `ddf` will be returned if/when the
@@ -55,14 +57,21 @@
                 # No filters support, or filters is already set
                 return ddf
     if len(io_layer) != 1:
         # Not a single IO layer
         return ddf
     io_layer = io_layer.pop()
 
+    # Bail if any filters are already present in ddf
+    existing_filters = (
+        ddf.dask.layers[io_layer].creation_info.get("kwargs", {}).get("filters")
+    )
+    if existing_filters:
+        return ddf
+
     # Start by converting the HLG to a `RegenerableGraph`.
     # Succeeding here means that all layers in the graph
     # are regenerable.
     try:
         dsk = RegenerableGraph.from_hlg(ddf.dask)
     except (ValueError, TypeError):
         logger.warning(
@@ -75,15 +84,15 @@
     name = ddf._name
     try:
         filters = dsk.layers[name]._dnf_filter_expression(dsk)
         if not isinstance(filters, frozenset):
             # No filters encountered
             return ddf
         filters = filters.to_list_tuple()
-    except ValueError:
+    except (ValueError, TypeError):
         # DNF dispatching failed for 1+ layers
         logger.warning(
             "Predicate pushdown optimization skipped. One or more "
             "layers has an unknown filter expression."
         )
         return ddf
 
@@ -138,21 +147,24 @@
 
 
 def to_dnf(expr):
     """Normalize a boolean filter expression to disjunctive normal form (DNF)"""
 
     # Credit: https://stackoverflow.com/a/58372345
     if not isinstance(expr, (Or, And)):
+        if not isinstance(expr, tuple):
+            raise TypeError(f"expected tuple, got {expr}")
         result = Or((And((expr,)),))
     elif isinstance(expr, Or):
         result = Or(se for e in expr for se in to_dnf(e))
     elif isinstance(expr, And):
         total = []
         for c in itertools.product(*[to_dnf(e) for e in expr]):
-            total.append(And(se for e in c for se in e))
+            conjunction = [se for e in c for se in e if isinstance(se, tuple)]
+            total.append(And(conjunction))
         result = Or(total)
     return result
 
 
 # Define all supported comparison functions
 # (and their mapping to a string expression)
 _comparison_symbols = {
@@ -166,28 +178,73 @@
     np.greater_equal: ">=",
     np.less: "<",
     np.less_equal: "<=",
     np.equal: "==",
     np.not_equal: "!=",
 }
 
+# Define all regenerable "pass-through" ops
+# that do not affect filters.
+_pass_through_ops = {M.fillna, M.astype}
+
 # Define set of all "regenerable" operations.
 # Predicate pushdown is supported for graphs
 # comprised of `Blockwise` layers based on these
 # operations
-_regenerable_ops = set(_comparison_symbols.keys()) | {
-    operator.and_,
-    operator.or_,
-    operator.getitem,
-    M.fillna,
-}
+_regenerable_ops = (
+    set(_comparison_symbols.keys())
+    | {
+        operator.and_,
+        operator.or_,
+        operator.getitem,
+        operator.inv,
+        M.isin,
+        M.isna,
+    }
+    | _pass_through_ops
+)
 
 # Specify functions that must be generated with
 # a different API at the dataframe-collection level
-_special_op_mappings = {M.fillna: dd._Frame.fillna}
+_special_op_mappings = {
+    M.fillna: dd._Frame.fillna,
+    M.isin: dd._Frame.isin,
+    M.isna: dd._Frame.isna,
+    M.astype: dd._Frame.astype,
+}
+
+# Convert _pass_through_ops to respect "special" mappings
+_pass_through_ops = {_special_op_mappings.get(op, op) for op in _pass_through_ops}
+
+
+def _preprocess_layers(input_layers):
+    # NOTE: This is a Layer-specific work-around to deal with
+    # the fact that `dd._Frame.isin(values)` will add a distinct
+    # `MaterializedLayer` for the `values` argument.
+    # See: https://github.com/dask-contrib/dask-sql/issues/607
+    skip = set()
+    layers = input_layers.copy()
+    for key, layer in layers.items():
+        if key.startswith("isin-") and isinstance(layer, Blockwise):
+            indices = list(layer.indices)
+            for i, (k, ind) in enumerate(layer.indices):
+                if (
+                    ind is None
+                    and isinstance(layers.get(k), MaterializedLayer)
+                    and isinstance(layers[k].get(k), (np.ndarray, tuple))
+                ):
+                    # Replace `indices[i]` with a literal value and
+                    # make sure we skip the `MaterializedLayer` that
+                    # we are now fusing into the `isin`
+                    value = layers[k][k]
+                    value = value[0](*value[1:]) if callable(value[0]) else value
+                    indices[i] = (value, None)
+                    skip.add(k)
+            layer.indices = tuple(indices)
+    return {k: v for k, v in layers.items() if k not in skip}
 
 
 class RegenerableLayer:
     """Regenerable Layer
 
     Wraps ``dask.highlevelgraph.Blockwise`` to ensure that a
     ``creation_info`` attribute  is defined. This class
@@ -257,16 +314,22 @@
         op = self.creation_info["func"]
         if op in _comparison_symbols.keys():
             func = _blockwise_comparison_dnf
         elif op in (operator.and_, operator.or_):
             func = _blockwise_logical_dnf
         elif op == operator.getitem:
             func = _blockwise_getitem_dnf
-        elif op == dd._Frame.fillna:
-            func = _blockwise_fillna_dnf
+        elif op == dd._Frame.isin:
+            func = _blockwise_isin_dnf
+        elif op == dd._Frame.isna:
+            func = _blockwise_isna_dnf
+        elif op == operator.inv:
+            func = _blockwise_inv_dnf
+        elif op in _pass_through_ops:
+            func = _blockwise_pass_through_dnf
         else:
             raise ValueError(f"No DNF expression for {op}")
 
         return func(op, self.layer.indices, dsk)
 
 
 class RegenerableGraph:
@@ -284,15 +347,15 @@
     def from_hlg(cls, hlg: HighLevelGraph):
         """Construct a ``RegenerableGraph`` from a ``HighLevelGraph``"""
 
         if not isinstance(hlg, HighLevelGraph):
             raise TypeError(f"Expected HighLevelGraph, got {type(hlg)}")
 
         _layers = {}
-        for key, layer in hlg.layers.items():
+        for key, layer in _preprocess_layers(hlg.layers).items():
             regenerable_layer = None
             if isinstance(layer, DataFrameIOLayer):
                 regenerable_layer = RegenerableLayer(layer, layer.creation_info or {})
             elif isinstance(layer, Blockwise):
                 tasks = list(layer.dsk.values())
                 if len(tasks) == 1 and tasks[0]:
                     kwargs = {}
@@ -331,50 +394,97 @@
     # for a Blockwise layer (using indices)
     key = indices[input_index][0]
     if indices[input_index][1] is None:
         return key
     return dsk.layers[key]._dnf_filter_expression(dsk)
 
 
+def _inv(symbol: str):
+    if symbol == "in" and not PQ_NOT_IN_SUPPORT:
+        raise ValueError("This version of dask does not support 'not in'")
+    return {
+        ">": "<",
+        "<": ">",
+        ">=": "<=",
+        "<=": ">=",
+        "in": "not in",
+        "not in": "in",
+        "is": "is not",
+        "is not": "is",
+    }.get(symbol, symbol)
+
+
 def _blockwise_comparison_dnf(op, indices: list, dsk: RegenerableGraph):
     # Return DNF expression pattern for a simple comparison
     left = _get_blockwise_input(0, indices, dsk)
     right = _get_blockwise_input(1, indices, dsk)
 
-    def _inv(symbol: str):
-        return {
-            ">": "<",
-            "<": ">",
-            ">=": "<=",
-            "<=": ">=",
-        }.get(symbol, symbol)
-
     if is_arraylike(left) and hasattr(left, "item") and left.size == 1:
         left = left.item()
         # Need inverse comparison in read_parquet
-        return (right, _inv(_comparison_symbols[op]), left)
+        return to_dnf((right, _inv(_comparison_symbols[op]), left))
     if is_arraylike(right) and hasattr(right, "item") and right.size == 1:
         right = right.item()
     return to_dnf((left, _comparison_symbols[op], right))
 
 
 def _blockwise_logical_dnf(op, indices: list, dsk: RegenerableGraph):
     # Return DNF expression pattern for logical "and" or "or"
     left = _get_blockwise_input(0, indices, dsk)
     right = _get_blockwise_input(1, indices, dsk)
+
+    vals = []
+    for val in [left, right]:
+        if not isinstance(val, (tuple, Or, And)):
+            raise TypeError(f"Invalid logical operand: {val}")
+        vals.append(to_dnf(val))
+
     if op == operator.or_:
-        return to_dnf(Or([left, right]))
+        return to_dnf(Or(vals))
     elif op == operator.and_:
-        return to_dnf(And([left, right]))
+        return to_dnf(And(vals))
     else:
         raise ValueError
 
 
 def _blockwise_getitem_dnf(op, indices: list, dsk: RegenerableGraph):
     # Return dnf of key (selected by getitem)
     key = _get_blockwise_input(1, indices, dsk)
     return key
 
 
-def _blockwise_fillna_dnf(op, indices: list, dsk: RegenerableGraph):
+def _blockwise_pass_through_dnf(op, indices: list, dsk: RegenerableGraph):
     # Return dnf of input collection
     return _get_blockwise_input(0, indices, dsk)
+
+
+def _blockwise_isin_dnf(op, indices: list, dsk: RegenerableGraph):
+    # Return DNF expression pattern for a simple "in" comparison
+    left = _get_blockwise_input(0, indices, dsk)
+    right = _get_blockwise_input(1, indices, dsk)
+    return to_dnf((left, "in", tuple(right)))
+
+
+def _blockwise_isna_dnf(op, indices: list, dsk: RegenerableGraph):
+    # Return DNF expression pattern for `isna`
+    if not PQ_IS_SUPPORT:
+        raise ValueError("This version of dask does not support 'is' predicates.")
+    left = _get_blockwise_input(0, indices, dsk)
+    return to_dnf((left, "is", None))
+
+
+def _blockwise_inv_dnf(op, indices: list, dsk: RegenerableGraph):
+    # Return DNF expression pattern for the inverse of a comparison
+    expr = _get_blockwise_input(0, indices, dsk).to_list_tuple()
+    new_expr = []
+    count = 0
+    for conjunction in expr:
+        new_conjunction = []
+        for col, op, val in conjunction:
+            count += 1
+            new_conjunction.append((col, _inv(op), val))
+        new_expr.append(And(new_conjunction))
+    if count > 1:
+        # Havent taken the time to think through
+        # general inversion yet.
+        raise ValueError("inv(DNF) case not implemented.")
+    return to_dnf(Or(new_expr))
```

### Comparing `dask_sql-2023.4.0/dask_sql/physical/utils/groupby.py` & `dask_sql-2023.6.0/dask_sql/physical/utils/groupby.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/utils/ml_classes.py` & `dask_sql-2023.6.0/dask_sql/physical/utils/ml_classes.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/physical/utils/sort.py` & `dask_sql-2023.6.0/dask_sql/physical/utils/sort.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List
 
 import dask.dataframe as dd
 import pandas as pd
 from dask import config as dask_config
 from dask.utils import M
 
-from dask_sql.utils import is_cudf_type, make_pickable_without_dask_sql
+from dask_sql.utils import is_cudf_type
 
 
 def apply_sort(
     df: dd.DataFrame,
     sort_columns: List[str],
     sort_ascending: List[bool],
     sort_null_first: List[bool],
@@ -64,15 +64,15 @@
 
     # if standard `sort_values` can't handle ascending / null position params,
     # we extend it using our custom sort function
     return df.sort_values(
         by=sort_columns[0],
         ascending=sort_ascending[0],
         na_position="first" if sort_null_first[0] else "last",
-        sort_function=make_pickable_without_dask_sql(sort_partition_func),
+        sort_function=(sort_partition_func),
         sort_function_kwargs={
             "sort_columns": sort_columns,
             "sort_ascending": sort_ascending,
             "sort_null_first": sort_null_first,
         },
     ).persist()
```

### Comparing `dask_sql-2023.4.0/dask_sql/physical/utils/statistics.py` & `dask_sql-2023.6.0/dask_sql/physical/utils/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,14 @@
 from dask.dataframe.io.parquet.arrow import ArrowDatasetEngine
 from dask.dataframe.io.parquet.core import ParquetFunctionWrapper
 from dask.dataframe.io.utils import _is_local_fs
 from dask.delayed import delayed
 from dask.layers import DataFrameIOLayer
 from dask.utils_test import hlg_layer
 
-from dask_sql.utils import make_pickable_without_dask_sql
-
 logger = logging.getLogger(__name__)
 
 
 def parquet_statistics(
     ddf: dd.DataFrame,
     columns: List | None = None,
     parallel: int | False | None = None,
@@ -141,15 +139,14 @@
         )[0]
         return list(itertools.chain(*result))
     else:
         # Serial computation on client
         return _read_partition_stats_group(parts, fs, engine, columns=columns)
 
 
-@make_pickable_without_dask_sql
 def _read_partition_stats_group(parts, fs, engine, columns=None):
     def _read_partition_stats(part, fs, columns=None):
         # Helper function to read Parquet-metadata
         # statistics for a single partition
 
         if not isinstance(part, list):
             part = [part]
```

### Comparing `dask_sql-2023.4.0/dask_sql/server/app.py` & `dask_sql-2023.6.0/dask_sql/server/app.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/server/presto_jdbc.py` & `dask_sql-2023.6.0/dask_sql/server/presto_jdbc.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/server/responses.py` & `dask_sql-2023.6.0/dask_sql/server/responses.py`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/dask_sql/sql-schema.yaml` & `dask_sql-2023.6.0/dask_sql/sql-schema.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -71,7 +71,16 @@
           topk-nelem-limit:
             type: integer
             description: |
               Total number of elements below which dask-sql should attempt to apply the top-k
               optimization (when possible). ``nelem`` is defined as the limit or ``k`` value times the
               number of columns. Default is 1000000, corresponding to a LIMIT clause of 1 million in a
               1 column table.
+
+      mappings:
+        type: object
+        properties:
+
+          decimal_support:
+            type: string
+            description:
+              Decides how to handle decimal scalars/columns. ``"pandas"`` handling will treat decimals scalars and columns as floats and float64 columns, respectively, while ``"cudf"`` handling treats decimal scalars as ``decimal.Decimal`` objects and decimal columns as ``cudf.Decimal128Dtype`` columns, handling precision/scale accordingly. Default is ``"pandas"``, but ``"cudf"`` should be used if attempting to work with decimal columns on GPU.
```

### Comparing `dask_sql-2023.4.0/dask_sql.egg-info/PKG-INFO` & `dask_sql-2023.6.0/dask_sql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-sql
-Version: 2023.4.0
+Version: 2023.6.0
 Summary: SQL query layer for Dask
 Home-page: https://github.com/dask-contrib/dask-sql/
 Maintainer: Nils Braun
 Maintainer-email: nilslennartbraun@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -30,15 +30,15 @@
 if you need it.
 
 * **Combine the power of Python and SQL**: load your data with Python, transform it with SQL, enhance it with Python and query it with SQL - or the other way round.
   With `dask-sql` you can mix the well known Python dataframe API of `pandas` and `Dask` with common SQL operations, to
   process your data in exactly the way that is easiest for you.
 * **Infinite Scaling**: using the power of the great `Dask` ecosystem, your computations can scale as you need it - from your laptop to your super cluster - without changing any line of SQL code. From k8s to cloud deployments, from batch systems to YARN - if `Dask` [supports it](https://docs.dask.org/en/latest/setup.html), so will `dask-sql`.
 * **Your data - your queries**: Use Python user-defined functions (UDFs) in SQL without any performance drawback and extend your SQL queries with the large number of Python libraries, e.g. machine learning, different complicated input formats, complex statistics.
-* **Easy to install and maintain**: `dask-sql` is just a pip/conda install away (or a docker run if you prefer). No need for complicated cluster setups - `dask-sql` will run out of the box on your machine and can be easily connected to your computing cluster.
+* **Easy to install and maintain**: `dask-sql` is just a pip/conda install away (or a docker run if you prefer).
 * **Use SQL from wherever you like**: `dask-sql` integrates with your jupyter notebook, your normal Python module or can be used as a standalone SQL server from any BI tool. It even integrates natively with [Apache Hue](https://gethue.com/).
 * **GPU Support**: `dask-sql` supports running SQL queries on CUDA-enabled GPUs by utilizing [RAPIDS](https://rapids.ai) libraries like [`cuDF`](https://github.com/rapidsai/cudf), enabling accelerated compute for SQL.
 
 Read more in the [documentation](https://dask-sql.readthedocs.io/en/latest/).
 
 <div align="center">
     <img src="./.github/animation.gif" alt="dask-sql GIF">
```

### Comparing `dask_sql-2023.4.0/dask_sql.egg-info/SOURCES.txt` & `dask_sql-2023.6.0/dask_sql.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 dask_planner/.classpath
 dask_planner/.gitignore
 dask_planner/Cargo.lock
 dask_planner/Cargo.toml
 dask_planner/MANIFEST.in
 dask_planner/README.md
 dask_planner/pyproject.toml
 dask_planner/update-dependencies.sh
+dask_planner/.cargo/config.toml
 dask_planner/.settings/org.eclipse.core.resources.prefs
 dask_planner/.settings/org.eclipse.jdt.apt.core.prefs
 dask_planner/.settings/org.eclipse.jdt.core.prefs
 dask_planner/.settings/org.eclipse.m2e.core.prefs
 dask_planner/src/dialect.rs
 dask_planner/src/error.rs
 dask_planner/src/expression.rs
@@ -59,15 +61,14 @@
 dask_planner/src/sql/logical/show_schemas.rs
 dask_planner/src/sql/logical/show_tables.rs
 dask_planner/src/sql/logical/sort.rs
 dask_planner/src/sql/logical/subquery_alias.rs
 dask_planner/src/sql/logical/table_scan.rs
 dask_planner/src/sql/logical/use_schema.rs
 dask_planner/src/sql/logical/window.rs
-dask_planner/src/sql/optimizer/filter_columns_post_join.rs
 dask_planner/src/sql/optimizer/join_reorder.rs
 dask_planner/src/sql/types/rel_data_type.rs
 dask_planner/src/sql/types/rel_data_type_field.rs
 dask_sql/__init__.py
 dask_sql/_compat.py
 dask_sql/_version.py
 dask_sql/cmd.py
```

### Comparing `dask_sql-2023.4.0/setup.cfg` & `dask_sql-2023.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dask_sql-2023.4.0/setup.py` & `dask_sql-2023.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,16 @@
             path="dask_planner/Cargo.toml",
             debug=debug_build,
         )
     ],
     python_requires=">=3.8",
     setup_requires=sphinx_requirements,
     install_requires=[
-        "dask[dataframe]>=2022.3.0,<=2023.3.2",
-        "distributed>=2022.3.0,<2023.3.3.0a0",
+        "dask[dataframe]>=2022.3.0,<=2023.5.1",
+        "distributed>=2022.3.0,<=2023.5.1",
         "pandas>=1.4.0",
         # FIXME: handling is needed for httpx-based fastapi>=0.87.0
         "fastapi>=0.69.0,<0.87.0",
         "uvicorn>=0.13.4",
         "tzlocal>=2.1",
         "prompt_toolkit>=3.0.8",
         "pygments>=2.7.1",
```

### Comparing `dask_sql-2023.4.0/versioneer.py` & `dask_sql-2023.6.0/versioneer.py`

 * *Files identical despite different names*

