# Comparing `tmp/mindsdb_sql-0.6.2.tar.gz` & `tmp/mindsdb_sql-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mindsdb_sql-0.6.2.tar", last modified: Tue May 23 14:41:16 2023, max compression
+gzip compressed data, was "dist\mindsdb_sql-0.6.3.tar", last modified: Thu Jun  8 19:18:28 2023, max compression
```

## Comparing `mindsdb_sql-0.6.2.tar` & `mindsdb_sql-0.6.3.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/
--rw-rw-rw-   0        0        0      535 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     7245 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/
--rw-rw-rw-   0        0        0      365 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/__about__.py
--rw-rw-rw-   0        0        0     1195 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/__init__.py
--rw-rw-rw-   0        0        0      170 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/
--rw-rw-rw-   0        0        0      537 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/__init__.py
--rw-rw-rw-   0        0        0      842 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/alter_table.py
--rw-rw-rw-   0        0        0     1343 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/base.py
--rw-rw-rw-   0        0        0      460 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/commit_transaction.py
--rw-rw-rw-   0        0        0     2287 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/create.py
--rw-rw-rw-   0        0        0      994 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/delete.py
--rw-rw-rw-   0        0        0      942 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/describe.py
--rw-rw-rw-   0        0        0     3056 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/drop.py
--rw-rw-rw-   0        0        0      659 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/explain.py
--rw-rw-rw-   0        0        0     3260 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/insert.py
--rw-rw-rw-   0        0        0      466 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/rollback_transaction.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/
--rw-rw-rw-   0        0        0      567 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/__init__.py
--rw-rw-rw-   0        0        0     1482 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/case.py
--rw-rw-rw-   0        0        0     1113 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/common_table_expression.py
--rw-rw-rw-   0        0        0     1593 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/constant.py
--rw-rw-rw-   0        0        0     3136 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/identifier.py
--rw-rw-rw-   0        0        0     1381 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/join.py
--rw-rw-rw-   0        0        0      662 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/native_query.py
--rw-rw-rw-   0        0        0     5949 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/operation.py
--rw-rw-rw-   0        0        0      806 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/order_by.py
--rw-rw-rw-   0        0        0      464 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/parameter.py
--rw-rw-rw-   0        0        0     5904 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/select.py
--rw-rw-rw-   0        0        0      504 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/star.py
--rw-rw-rw-   0        0        0      648 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/tuple.py
--rw-rw-rw-   0        0        0      774 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/type_cast.py
--rw-rw-rw-   0        0        0     1178 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/union.py
--rw-rw-rw-   0        0        0     3296 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/set.py
--rw-rw-rw-   0        0        0     2979 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/show.py
--rw-rw-rw-   0        0        0      469 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/start_transaction.py
--rw-rw-rw-   0        0        0     2407 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/update.py
--rw-rw-rw-   0        0        0      639 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/use.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/
--rw-rw-rw-   0        0        0      769 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/__init__.py
--rw-rw-rw-   0        0        0     1818 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
--rw-rw-rw-   0        0        0     1595 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_database.py
--rw-rw-rw-   0        0        0      953 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_file.py
--rw-rw-rw-   0        0        0     2078 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_job.py
--rw-rw-rw-   0        0        0     1201 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
--rw-rw-rw-   0        0        0     5361 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
--rw-rw-rw-   0        0        0     1534 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_view.py
--rw-rw-rw-   0        0        0      704 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
--rw-rw-rw-   0        0        0      713 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
--rw-rw-rw-   0        0        0      737 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
--rw-rw-rw-   0        0        0      692 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
--rw-rw-rw-   0        0        0      708 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
--rw-rw-rw-   0        0        0      906 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
--rw-rw-rw-   0        0        0     1313 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
--rw-rw-rw-   0        0        0      223 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
--rw-rw-rw-   0        0        0      359 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/latest.py
--rw-rw-rw-   0        0        0     8140 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/lexer.py
--rw-rw-rw-   0        0        0    44911 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/parser.py
--rw-rw-rw-   0        0        0      311 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/
--rw-rw-rw-   0        0        0       67 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/__init__.py
--rw-rw-rw-   0        0        0     1046 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/lexer.py
--rw-rw-rw-   0        0        0    29491 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/parser.py
--rw-rw-rw-   0        0        0      904 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/show_index.py
--rw-rw-rw-   0        0        0      686 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/variable.py
--rw-rw-rw-   0        0        0     6226 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/lexer.py
--rw-rw-rw-   0        0        0      751 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/logger.py
--rw-rw-rw-   0        0        0    21382 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/parser.py
--rw-rw-rw-   0        0        0     2497 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/
--rw-rw-rw-   0        0        0      150 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/__init__.py
--rw-rw-rw-   0        0        0      878 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/query_plan.py
--rw-rw-rw-   0        0        0    50030 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/query_planner.py
--rw-rw-rw-   0        0        0    21367 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/query_prepare.py
--rw-rw-rw-   0        0        0      536 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/step_result.py
--rw-rw-rw-   0        0        0     8276 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/steps.py
--rw-rw-rw-   0        0        0     2981 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/ts_utils.py
--rw-rw-rw-   0        0        0    17922 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/planner/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql/render/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/render/__init__.py
--rw-rw-rw-   0        0        0    20561 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/mindsdb_sql/render/sqlalchemy_render.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/
--rw-rw-rw-   0        0        0      535 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5282 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/mindsdb_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      843 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/test_parser/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/__init__.py
--rw-rw-rw-   0        0        0      776 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_ast.py
--rw-rw-rw-   0        0        0    11910 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_base_lexer.py
--rw-rw-rw-   0        0        0      223 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_base_sql.py
--rw-rw-rw-   0        0        0     1480 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_create.py
--rw-rw-rw-   0        0        0     2481 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_ddl.py
--rw-rw-rw-   0        0        0     1075 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_delete.py
--rw-rw-rw-   0        0        0     1094 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_describe.py
--rw-rw-rw-   0        0        0     2426 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_insert.py
--rw-rw-rw-   0        0        0     6945 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_misc_sql_queries.py
--rw-rw-rw-   0        0        0     3625 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_common_table_expression.py
--rw-rw-rw-   0        0        0    24799 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_operations.py
--rw-rw-rw-   0        0        0    45563 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_structure.py
--rw-rw-rw-   0        0        0    13620 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_show.py
--rw-rw-rw-   0        0        0     3114 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_union.py
--rw-rw-rw-   0        0        0     2462 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_update.py
--rw-rw-rw-   0        0        0      514 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_use.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/__init__.py
--rw-rw-rw-   0        0        0     1643 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_chatbots.py
--rw-rw-rw-   0        0        0      605 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_file.py
--rw-rw-rw-   0        0        0     4203 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_integration.py
--rw-rw-rw-   0        0        0     6617 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_predictor.py
--rw-rw-rw-   0        0        0     2651 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_view.py
--rw-rw-rw-   0        0        0      520 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_dataset.py
--rw-rw-rw-   0        0        0      861 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_datasource.py
--rw-rw-rw-   0        0        0      866 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_integration.py
--rw-rw-rw-   0        0        0     1708 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_predictor.py
--rw-rw-rw-   0        0        0     1824 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_evaluate.py
--rw-rw-rw-   0        0        0     1339 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_finetune_predictor.py
--rw-rw-rw-   0        0        0     2056 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_jobs.py
--rw-rw-rw-   0        0        0     1587 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_ml_engine.py
--rw-rw-rw-   0        0        0     2242 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_retrain_predictor.py
--rw-rw-rw-   0        0        0     3572 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_selects.py
--rw-rw-rw-   0        0        0     1226 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_show_mindsdb.py
--rw-rw-rw-   0        0        0      959 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_timeseries.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mysql/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mysql/__init__.py
--rw-rw-rw-   0        0        0      714 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mysql/test_mysql_lexer.py
--rw-rw-rw-   0        0        0     3050 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_parser/test_mysql/test_mysql_parser.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:41:16.000000 mindsdb_sql-0.6.2/tests/test_render/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_render/__init__.py
--rw-rw-rw-   0        0        0     6391 2023-05-23 14:40:55.000000 mindsdb_sql-0.6.2/tests/test_render/test_sqlalchemyrender.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/
+-rw-rw-rw-   0        0        0      535 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7245 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/
+-rw-rw-rw-   0        0        0      365 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/__about__.py
+-rw-rw-rw-   0        0        0     1195 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/__init__.py
+-rw-rw-rw-   0        0        0      170 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/
+-rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/
+-rw-rw-rw-   0        0        0      537 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/alter_table.py
+-rw-rw-rw-   0        0        0     1343 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/base.py
+-rw-rw-rw-   0        0        0      460 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/commit_transaction.py
+-rw-rw-rw-   0        0        0     2287 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/create.py
+-rw-rw-rw-   0        0        0      994 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/delete.py
+-rw-rw-rw-   0        0        0      942 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/describe.py
+-rw-rw-rw-   0        0        0     3056 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/drop.py
+-rw-rw-rw-   0        0        0      659 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/explain.py
+-rw-rw-rw-   0        0        0     3260 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/insert.py
+-rw-rw-rw-   0        0        0      466 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/rollback_transaction.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/
+-rw-rw-rw-   0        0        0      567 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/__init__.py
+-rw-rw-rw-   0        0        0     1482 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/case.py
+-rw-rw-rw-   0        0        0     1113 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/common_table_expression.py
+-rw-rw-rw-   0        0        0     1593 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/constant.py
+-rw-rw-rw-   0        0        0     3136 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/identifier.py
+-rw-rw-rw-   0        0        0     1381 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/join.py
+-rw-rw-rw-   0        0        0      662 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/native_query.py
+-rw-rw-rw-   0        0        0     5949 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/operation.py
+-rw-rw-rw-   0        0        0      806 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/order_by.py
+-rw-rw-rw-   0        0        0      464 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/parameter.py
+-rw-rw-rw-   0        0        0     5904 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/select.py
+-rw-rw-rw-   0        0        0      504 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/star.py
+-rw-rw-rw-   0        0        0      648 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/tuple.py
+-rw-rw-rw-   0        0        0      774 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/type_cast.py
+-rw-rw-rw-   0        0        0     1178 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/union.py
+-rw-rw-rw-   0        0        0     3296 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/set.py
+-rw-rw-rw-   0        0        0     2979 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/show.py
+-rw-rw-rw-   0        0        0      469 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/start_transaction.py
+-rw-rw-rw-   0        0        0     2407 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/update.py
+-rw-rw-rw-   0        0        0      639 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/use.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/
+-rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/
+-rw-rw-rw-   0        0        0      769 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     1818 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
+-rw-rw-rw-   0        0        0     1595 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_database.py
+-rw-rw-rw-   0        0        0      953 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_file.py
+-rw-rw-rw-   0        0        0     2078 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_job.py
+-rw-rw-rw-   0        0        0     1201 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
+-rw-rw-rw-   0        0        0     5361 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
+-rw-rw-rw-   0        0        0     1534 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_view.py
+-rw-rw-rw-   0        0        0      704 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
+-rw-rw-rw-   0        0        0      713 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
+-rw-rw-rw-   0        0        0      737 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py
+-rw-rw-rw-   0        0        0      692 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
+-rw-rw-rw-   0        0        0      708 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
+-rw-rw-rw-   0        0        0      906 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
+-rw-rw-rw-   0        0        0     1313 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
+-rw-rw-rw-   0        0        0      223 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
+-rw-rw-rw-   0        0        0      359 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/latest.py
+-rw-rw-rw-   0        0        0     8140 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/lexer.py
+-rw-rw-rw-   0        0        0    44911 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/parser.py
+-rw-rw-rw-   0        0        0      311 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/
+-rw-rw-rw-   0        0        0       67 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/__init__.py
+-rw-rw-rw-   0        0        0     1046 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/lexer.py
+-rw-rw-rw-   0        0        0    29491 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/parser.py
+-rw-rw-rw-   0        0        0      904 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/show_index.py
+-rw-rw-rw-   0        0        0      686 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/variable.py
+-rw-rw-rw-   0        0        0     6226 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/lexer.py
+-rw-rw-rw-   0        0        0      751 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/logger.py
+-rw-rw-rw-   0        0        0    21382 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/parser.py
+-rw-rw-rw-   0        0        0     2497 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/
+-rw-rw-rw-   0        0        0      150 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/query_plan.py
+-rw-rw-rw-   0        0        0    50304 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/query_planner.py
+-rw-rw-rw-   0        0        0    21344 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/query_prepare.py
+-rw-rw-rw-   0        0        0      536 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/step_result.py
+-rw-rw-rw-   0        0        0     8276 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/steps.py
+-rw-rw-rw-   0        0        0     2981 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/ts_utils.py
+-rw-rw-rw-   0        0        0    13228 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/planner/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql/render/
+-rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/render/__init__.py
+-rw-rw-rw-   0        0        0    20561 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/mindsdb_sql/render/sqlalchemy_render.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5282 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/mindsdb_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      843 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/test_parser/
+-rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/
+-rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/__init__.py
+-rw-rw-rw-   0        0        0      776 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_ast.py
+-rw-rw-rw-   0        0        0    11910 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_base_lexer.py
+-rw-rw-rw-   0        0        0      223 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_base_sql.py
+-rw-rw-rw-   0        0        0     1480 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_create.py
+-rw-rw-rw-   0        0        0     2481 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_ddl.py
+-rw-rw-rw-   0        0        0     1075 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_delete.py
+-rw-rw-rw-   0        0        0     1094 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_describe.py
+-rw-rw-rw-   0        0        0     2426 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_insert.py
+-rw-rw-rw-   0        0        0     6945 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_misc_sql_queries.py
+-rw-rw-rw-   0        0        0     3625 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_common_table_expression.py
+-rw-rw-rw-   0        0        0    24799 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_operations.py
+-rw-rw-rw-   0        0        0    45563 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_structure.py
+-rw-rw-rw-   0        0        0    13620 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_show.py
+-rw-rw-rw-   0        0        0     3114 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_union.py
+-rw-rw-rw-   0        0        0     2462 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_update.py
+-rw-rw-rw-   0        0        0      514 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_use.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/
+-rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     1643 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_chatbots.py
+-rw-rw-rw-   0        0        0      605 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_file.py
+-rw-rw-rw-   0        0        0     4203 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_integration.py
+-rw-rw-rw-   0        0        0     6617 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_predictor.py
+-rw-rw-rw-   0        0        0     2651 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_view.py
+-rw-rw-rw-   0        0        0      520 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_dataset.py
+-rw-rw-rw-   0        0        0      861 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_datasource.py
+-rw-rw-rw-   0        0        0      866 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_integration.py
+-rw-rw-rw-   0        0        0     1708 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_predictor.py
+-rw-rw-rw-   0        0        0     1824 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_evaluate.py
+-rw-rw-rw-   0        0        0     1339 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_finetune_predictor.py
+-rw-rw-rw-   0        0        0     2056 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_jobs.py
+-rw-rw-rw-   0        0        0     1587 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_ml_engine.py
+-rw-rw-rw-   0        0        0     2242 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_retrain_predictor.py
+-rw-rw-rw-   0        0        0     3572 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_selects.py
+-rw-rw-rw-   0        0        0     1226 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_show_mindsdb.py
+-rw-rw-rw-   0        0        0      959 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_timeseries.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mysql/
+-rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mysql/__init__.py
+-rw-rw-rw-   0        0        0      714 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mysql/test_mysql_lexer.py
+-rw-rw-rw-   0        0        0     3050 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_parser/test_mysql/test_mysql_parser.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:18:28.000000 mindsdb_sql-0.6.3/tests/test_render/
+-rw-rw-rw-   0        0        0        0 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_render/__init__.py
+-rw-rw-rw-   0        0        0     6391 2023-06-08 19:18:01.000000 mindsdb_sql-0.6.3/tests/test_render/test_sqlalchemyrender.py
```

### Comparing `mindsdb_sql-0.6.2/PKG-INFO` & `mindsdb_sql-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb_sql
-Version: 0.6.2
+Version: 0.6.3
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.2/README.md` & `mindsdb_sql-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/__init__.py` & `mindsdb_sql-0.6.3/mindsdb_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/__init__.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/alter_table.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/alter_table.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/base.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/base.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/create.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/delete.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/describe.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/drop.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/drop.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/explain.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/explain.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/insert.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/insert.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/__init__.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/case.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/case.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/common_table_expression.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/constant.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/constant.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/identifier.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/identifier.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/join.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/join.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/native_query.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/native_query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/operation.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/operation.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/order_by.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/order_by.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/select.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/select.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/tuple.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/tuple.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/type_cast.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/type_cast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/select/union.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/select/union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/set.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/set.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/show.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/update.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/update.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/ast/use.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/ast/use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/__init__.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/chatbot.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/chatbot.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_database.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_database.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_file.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_job.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/create_view.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_job.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/evaluate.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/evaluate.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/lexer.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mindsdb/parser.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mindsdb/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/lexer.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/parser.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/show_index.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/show_index.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/dialects/mysql/variable.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/dialects/mysql/variable.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/lexer.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/logger.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/logger.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/parser.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/parser/utils.py` & `mindsdb_sql-0.6.3/mindsdb_sql/parser/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/planner/query_plan.py` & `mindsdb_sql-0.6.3/mindsdb_sql/planner/query_plan.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/planner/query_planner.py` & `mindsdb_sql-0.6.3/mindsdb_sql/planner/query_planner.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from mindsdb_sql.parser.dialects.mindsdb.latest import Latest
 from mindsdb_sql.planner.steps import (FetchDataframeStep, ProjectStep, JoinStep, ApplyPredictorStep,
                                        ApplyPredictorRowStep, FilterStep, GroupByStep, LimitOffsetStep, OrderByStep,
                                        UnionStep, MapReduceStep, MultipleSteps, ApplyTimeseriesPredictorStep,
                                        GetPredictorColumns, SaveToTable, InsertToTable, UpdateToTable, SubSelectStep)
 from mindsdb_sql.planner.ts_utils import (validate_ts_where_condition, find_time_filter, replace_time_filter,
                                           find_and_remove_time_filter)
-from mindsdb_sql.planner.utils import (get_integration_path_from_identifier,
-                                       disambiguate_integration_column_identifier,
-                                       disambiguate_predictor_column_identifier, recursively_disambiguate_identifiers,
+from mindsdb_sql.planner.utils import (disambiguate_predictor_column_identifier,
                                        get_deepest_select,
                                        recursively_extract_column_values,
                                        recursively_check_join_identifiers_for_ambiguity,
                                        query_traversal)
 from mindsdb_sql.planner.query_plan import QueryPlan
 from mindsdb_sql.planner import utils
 from .query_prepare import PreparedStatementPlanner
@@ -33,50 +31,67 @@
                  integrations: list = None,
                  predictor_namespace=None,
                  predictor_metadata: list = None,
                  default_namespace: str = None):
         self.query = query
         self.plan = QueryPlan()
 
-        self.integrations = [int.lower() for int in integrations] if integrations else []
+        _projects = set()
+        self.integrations = {}
+        if integrations is not None:
+            for integration in integrations:
+                if isinstance(integration, dict):
+                    integration_name = integration['name'].lower()
+                    # it is project of system database
+                    if integration['type'] != 'data':
+                        _projects.add(integration_name)
+                        continue
+                else:
+                    integration_name = integration.lower()
+                    integration = {'name': integration}
+                self.integrations[integration_name] = integration
+
+        # allow to select from mindsdb namespace
+        _projects.add('mindsdb')
+
         self.default_namespace = default_namespace
 
         # legacy parameter
         self.predictor_namespace = predictor_namespace.lower() if predictor_namespace else 'mindsdb'
 
         # map for lower names of predictors
 
         self.predictor_info = {}
         if isinstance(predictor_metadata, list):
             # convert to dict
-            if predictor_metadata is not None:
-                for predictor in predictor_metadata:
-                    if 'integration_name' in predictor:
-                        integration_name = predictor['integration_name']
-                    else:
-                        integration_name = self.predictor_namespace
-                        predictor['integration_name'] = integration_name
-                    idx = f'{integration_name}.{predictor["name"]}'.lower()
-                    self.predictor_info[idx] = predictor
+            for predictor in predictor_metadata:
+                if 'integration_name' in predictor:
+                    integration_name = predictor['integration_name']
+                else:
+                    integration_name = self.predictor_namespace
+                    predictor['integration_name'] = integration_name
+                idx = f'{integration_name}.{predictor["name"]}'.lower()
+                self.predictor_info[idx] = predictor
+                _projects.add(integration_name.lower())
         elif isinstance(predictor_metadata, dict):
             # legacy behaviour
             for name, predictor in predictor_metadata.items():
                 if '.' not in name:
                     if 'integration_name' in predictor:
                         integration_name = predictor['integration_name']
                     else:
                         integration_name = self.predictor_namespace
                         predictor['integration_name'] = integration_name
                     name = f'{integration_name}.{name}'.lower()
+                    _projects.add(integration_name.lower())
 
                 self.predictor_info[name] = predictor
 
-        # allow to select from mindsdb namespace
-        if 'mindsdb' not in self.integrations:
-            self.integrations.append('mindsdb')
+        self.projects = list(_projects)
+        self.databases = list(self.integrations.keys()) + self.projects
 
         self.statement = None
 
     def is_predictor(self, identifier):
         return self.get_predictor(identifier) is not None
 
     def get_predictor(self, identifier):
@@ -104,87 +119,126 @@
         idx = '.'.join(idx_ar).lower()
         info = self.predictor_info.get(idx)
         if info is not None:
             info['version'] = version
             info['name'] = name
         return info
 
-    def get_integration_path_from_identifier_or_error(self, identifier, recurse=True):
-        try:
-            integration_name, table = get_integration_path_from_identifier(identifier)
-            if not integration_name.lower() in self.integrations:
-                raise PlanningException(f'Unknown integration {integration_name} for table {str(identifier)}. Available integrations: {", ".join(self.integrations)}')
-        except PlanningException:
-            if not recurse or not self.default_namespace:
-                raise
-            else:
-                new_identifier = copy.deepcopy(identifier)
-                new_identifier.parts = [self.default_namespace, *identifier.parts]
-                return self.get_integration_path_from_identifier_or_error(new_identifier, recurse=False)
-        return integration_name, table
+    def prepare_integration_select(self, database, query):
+        # replacement for 'utils.recursively_disambiguate_*' functions from utils
+        #   main purpose: make tests working (don't change planner outputs)
+        # can be removed in future (with adapting the tests) except 'cut integration part' block
+
+        def _prepare_integration_select(node, is_table, is_target, parent_query, **kwargs):
+            if not isinstance(node, Identifier):
+                return
+
+            # cut integration part
+            if len(node.parts) > 1 and node.parts[0].lower() == database:
+                node.parts.pop(0)
+
+            if not hasattr(parent_query, 'from_table'):
+                return
+
+            table = parent_query.from_table
+            if not is_table:
+                # add table name or alias for identifiers
+
+                if table.alias is not None:
+                    prefix = table.alias.parts
+                else:
+                    prefix = table.parts
+
+                if len(node.parts) > 1:
+                    if node.parts[:len(prefix)] != prefix:
+                        raise PlanningException(f'Tried to query column {node.to_string()} from table'
+                                                f' {table.to_string()}, but a different table name has been specified.')
+                else:
+                    node.parts = prefix + node.parts
+
+                # keep column name for target
+                if is_target:
+                    if node.alias is None:
+                        node.alias = Identifier(parts=[node.parts[-1]])
+
+        utils.query_traversal(query, _prepare_integration_select)
 
     def get_integration_select_step(self, select):
-        integration_name, table = self.get_integration_path_from_identifier_or_error(select.from_table)
+        integration_name, table = self.resolve_database_table(select.from_table)
 
         fetch_df_select = copy.deepcopy(select)
-        recursively_disambiguate_identifiers(fetch_df_select, integration_name, table)
+        self.prepare_integration_select(integration_name, fetch_df_select)
 
         # remove predictor params
         if fetch_df_select.using is not None:
             fetch_df_select.using = None
 
         return FetchDataframeStep(integration=integration_name, query=fetch_df_select)
 
     def plan_integration_select(self, select):
         """Plan for a select query that can be fully executed in an integration"""
 
         return self.plan.add_step(self.get_integration_select_step(select))
 
-    def get_integration_name(self, node: Identifier):
-        if len(node.parts) > 1 and node.parts[0] in self.integrations:
-            return node.parts[0]
+    def resolve_database_table(self, node: Identifier):
+        # resolves integration name and table name
+
+        parts = node.parts.copy()
+        alias = None
+        if node.alias is not None:
+            alias = node.alias.copy()
+
+        database = self.default_namespace
+
+        if len(parts) > 1:
+            if parts[0].lower() in self.databases:
+                database = parts.pop(0).lower()
+
+        return database, Identifier(parts=parts, alias=alias)
 
     def get_query_info(self, query):
         # get all predictors
         mdb_entities = []
-        projects = []
+        predictors = []
+        # projects = set()
         integrations = set()
 
         def find_predictors(node, is_table, **kwargs):
-            if isinstance(node, ast.NativeQuery):
-                # has NativeQuery syntax
-                mdb_entities.append(node)
 
             if is_table and isinstance(node, ast.Identifier):
-                integration = self.get_integration_name(node)
+                integration, _ = self.resolve_database_table(node)
 
                 if self.is_predictor(node):
+                    predictors.append(node)
+
+                if integration in self.projects:
+                    # it is project
                     mdb_entities.append(node)
-                    if integration is not None:
-                        projects.append(integration)
-                    return
 
-                if integration is not None and not integration in projects:
+                elif integration is not None:
                     integrations.add(integration)
 
         utils.query_traversal(query, find_predictors)
-        return {'mdb_entities': mdb_entities, 'integrations': integrations}
+        return {'mdb_entities': mdb_entities, 'integrations': integrations, 'predictors': predictors}
 
     def plan_select_identifier(self, query):
         query_info = self.get_query_info(query)
 
-        if len(query_info['integrations']) == 0 and len(query_info['mdb_entities']) >= 1:
+        if len(query_info['integrations']) == 0 and len(query_info['predictors']) >= 1:
             # select from predictor
             return self.plan_select_from_predictor(query)
-        elif len(query_info['integrations']) <= 1 and len(query_info['mdb_entities']) == 0:
-            # one integration without predictors
-            return self.plan_integration_select(query)
+        elif len(query_info['integrations']) == 1 and len(query_info['mdb_entities']) == 0:
+
+            int_name = list(query_info['integrations'])[0]
+            if self.integrations.get(int_name, {}).get('class_type') != 'api':
+                # one integration without predictors, send all query to integration
+                return self.plan_integration_select(query)
 
         # find subselects
-        main_integration = self.get_integration_name(query.from_table)
+        main_integration, _ = self.resolve_database_table(query.from_table)
 
         def find_selects(node, **kwargs):
             if isinstance(node, Select):
                 query_info2 = self.get_query_info(node)
                 if (
                         len(query_info2['integrations']) > 1 or
                         main_integration not in query_info2['integrations'] or
@@ -197,37 +251,44 @@
                     node2 = Parameter(last_step.result)
 
                     return node2
 
         query.targets = utils.query_traversal(query.targets, find_selects)
         utils.query_traversal(query.where, find_selects)
 
-        self.plan_select_identifier(query)
+        if len(query_info['predictors']) >= 1:
+            # select from predictor
+            return self.plan_select_from_predictor(query)
+        else:
+            return self.plan_integration_select(query)
 
     def plan_nested_select(self, select):
 
         query_info = self.get_query_info(select)
         # get all predictors
 
         if (
             len(query_info['mdb_entities']) == 0
-            and len(query_info['integrations']) < 2
-            and not 'files' in query_info['integrations']
-            and not 'views' in query_info['integrations']
+            and len(query_info['integrations']) == 1
+            and 'files' not in query_info['integrations']
+            and 'views' not in query_info['integrations']
         ):
-            # if no predictor inside = run as is
-            return self.plan_integration_nested_select(select)
-        else:
-            return self.plan_mdb_nested_select(select)
+            int_name = list(query_info['integrations'])[0]
+            if self.integrations.get(int_name, {}).get('class_type') != 'api':
+
+                # if no predictor inside = run as is
+                return self.plan_integration_nested_select(select)
+
+        return self.plan_mdb_nested_select(select)
 
     def plan_integration_nested_select(self, select):
         fetch_df_select = copy.deepcopy(select)
         deepest_select = get_deepest_select(fetch_df_select)
-        integration_name, table = self.get_integration_path_from_identifier_or_error(deepest_select.from_table)
-        recursively_disambiguate_identifiers(deepest_select, integration_name, table)
+        integration_name, table = self.resolve_database_table(deepest_select.from_table)
+        self.prepare_integration_select(integration_name, deepest_select)
         return self.plan.add_step(FetchDataframeStep(integration=integration_name, query=fetch_df_select))
 
     def plan_mdb_nested_select(self, select):
         # plan nested select
 
         # if select.limit == 0:
             # TODO don't run predictor if limit is 0
@@ -246,51 +307,14 @@
         sup_select = self.sub_select_step(select, last_step)
         if sup_select is not None:
             self.plan.add_step(sup_select)
             last_step = sup_select
 
         return last_step
 
-        # if select.where is not None:
-        #     # remove subselect alias
-        #     where_query = select.where
-        #     if subselect_alias is not None:
-        #         def remove_aliases(node, **kwargs):
-        #             if isinstance(node, Identifier):
-        #
-        #                 if len(node.parts) > 1:
-        #                     if node.parts[0] == subselect_alias:
-        #                         node.parts = node.parts[1:]
-        #
-        #         query_traversal(where_query, remove_aliases)
-        #
-        #     last_step = self.plan.add_step(FilterStep(dataframe=last_step.result, query=where_query))
-        #
-        # group_step = self.plan_group(select, last_step)
-        # if group_step is not None:
-        #     self.plan.add_step(group_step)
-        #     # don't do project step
-        #
-        # else:
-        #     # do we need projection?
-        #     if len(select.targets) != 1 or not isinstance(select.targets[0], Star):
-        #         # remove prefix alias
-        #         if subselect_alias is not None:
-        #             for t in select.targets:
-        #                 if isinstance(t, Identifier) and t.parts[0] == subselect_alias:
-        #                     t.parts.pop(0)
-        #
-        #         self.plan_project(select, last_step.result, ignore_doubles=True)
-
-        # do we need limit?
-        # last_step = self.plan.steps[-1]
-        # if select.limit is not None:
-        #     last_step = self.plan.add_step(LimitOffsetStep(dataframe=last_step.result, limit=select.limit.value))
-        # return last_step
-
     def get_predictor_namespace_and_name_from_identifier(self, identifier):
         new_identifier = copy.deepcopy(identifier)
 
         info = self.get_predictor(identifier)
         namespace = info['integration_name']
 
         parts = [namespace, info['name']]
@@ -647,15 +671,15 @@
                     parts = table.parts[i:]
                     parts = tuple(map(str.lower, parts))
                     aliases.append(parts)
 
             # try to use default namespace
             integration = self.default_namespace
             if len(table.parts) > 0:
-                if table.parts[0] in self.integrations:
+                if table.parts[0] in self.databases:
                     integration = table.parts.pop(0)
                 else:
                     integration = self.default_namespace
 
             if integration is None:
                 raise PlanningException(f'Integration not found for: {table}')
 
@@ -922,15 +946,15 @@
             query_traversal(query.where, add_aliases)
 
             if isinstance(query.from_table, Identifier):
                 # DBT workaround: allow use tables without integration.
                 #   if table.part[0] not in integration - take integration name from create table command
                 if (
                     integration is not None
-                    and query.from_table.parts[0] not in self.integrations
+                    and query.from_table.parts[0] not in self.databases
                 ):
                     # add integration name to table
                     query.from_table.parts.insert(0, integration)
 
             join_left = join_left.from_table
 
             if orig_query.limit is not None:
@@ -1005,15 +1029,15 @@
             # Both arguments are tables, join results of 2 dataframe fetches
 
             join_step = self.plan_join_tables(query)
             last_step = join_step
             if query.where:
                 # FIXME: Tableau workaround, INFORMATION_SCHEMA with Where
                 if isinstance(join.right, Identifier) \
-                   and self.get_integration_path_from_identifier_or_error(join.right)[0] == 'INFORMATION_SCHEMA':
+                   and self.resolve_database_table(join.right)[0] == 'INFORMATION_SCHEMA':
                     pass
                 else:
                     last_step = self.plan.add_step(FilterStep(dataframe=last_step.result, query=query.where))
 
             if query.group_by:
                 group_by_targets = []
                 for t in query.targets:
```

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/planner/query_prepare.py` & `mindsdb_sql-0.6.3/mindsdb_sql/planner/query_prepare.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,15 @@
     def table_from_identifier(self, table):
         # disambiguate
         if self.planner.is_predictor(table):
             ds, table = self.planner.get_predictor_namespace_and_name_from_identifier(table)
             is_predictor = True
 
         else:
-            ds, table = self.planner.get_integration_path_from_identifier_or_error(table)
+            ds, table = self.planner.resolve_database_table(table)
             is_predictor = False
 
         if table.alias is not None:
             # access by alias if table is having alias
             keys = [to_string(table.alias)]
 
         else:
```

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/planner/step_result.py` & `mindsdb_sql-0.6.3/mindsdb_sql/planner/step_result.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/planner/steps.py` & `mindsdb_sql-0.6.3/mindsdb_sql/planner/steps.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/planner/ts_utils.py` & `mindsdb_sql-0.6.3/mindsdb_sql/planner/ts_utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql/render/sqlalchemy_render.py` & `mindsdb_sql-0.6.3/mindsdb_sql/render/sqlalchemy_render.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql.egg-info/PKG-INFO` & `mindsdb_sql-0.6.3/mindsdb_sql.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb-sql
-Version: 0.6.2
+Version: 0.6.3
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.6.2/mindsdb_sql.egg-info/SOURCES.txt` & `mindsdb_sql-0.6.3/mindsdb_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/setup.py` & `mindsdb_sql-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_ast.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_ast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_base_lexer.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_base_lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_create.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_ddl.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_ddl.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_delete.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_describe.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_insert.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_insert.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_misc_sql_queries.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_misc_sql_queries.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_common_table_expression.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_operations.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_operations.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_select_structure.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_select_structure.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_show.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_union.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_update.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_update.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_base_sql/test_use.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_base_sql/test_use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_chatbots.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_chatbots.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_file.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_integration.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_predictor.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_create_view.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_dataset.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_datasource.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_integration.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_integration.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_drop_predictor.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_evaluate.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_finetune_predictor.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_finetune_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_jobs.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_jobs.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_ml_engine.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_retrain_predictor.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_retrain_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_selects.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_selects.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_show_mindsdb.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_show_mindsdb.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mindsdb/test_timeseries.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mindsdb/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mysql/test_mysql_lexer.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mysql/test_mysql_lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_parser/test_mysql/test_mysql_parser.py` & `mindsdb_sql-0.6.3/tests/test_parser/test_mysql/test_mysql_parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.6.2/tests/test_render/test_sqlalchemyrender.py` & `mindsdb_sql-0.6.3/tests/test_render/test_sqlalchemyrender.py`

 * *Files identical despite different names*

