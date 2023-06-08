# Comparing `tmp/taipy-core-2.3.0.dev1.tar.gz` & `tmp/taipy-core-2.3.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-core-2.3.0.dev1.tar", last modified: Mon Jun  5 16:01:49 2023, max compression
+gzip compressed data, was "taipy-core-2.3.0.dev2.tar", last modified: Thu Jun  8 19:30:39 2023, max compression
```

## Comparing `taipy-core-2.3.0.dev1.tar` & `taipy-core-2.3.0.dev2.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.872070 taipy-core-2.3.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-05 16:01:49.872070 taipy-core-2.3.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:01:49.872070 taipy-core-2.3.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.848070 taipy-core-2.3.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.848070 taipy-core-2.3.0.dev1/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/_backup/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_backup/_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_core_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/_entity/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_labeled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_reload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_entity/_submittable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_manager/_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_abstract_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.852070 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_orchestrator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.856070 taipy-core-2.3.0.dev1/src/taipy/core/_repository/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_filesystem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_sql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_repository/_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.856070 taipy-core-2.3.0.dev1/src/taipy/core/_version/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.856070 taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/_bcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/_version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.856070 taipy-core-2.3.0.dev1/src/taipy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/_listattributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/default_custom_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/common/warn_if_inputs_not_ready.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.856070 taipy-core-2.3.0.dev1/src/taipy/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/_core_section.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.860070 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_config_id_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10814 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_data_node_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_global_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_job_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_pipeline_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_scenario_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_task_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    40959 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/data_node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/job_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/scenario_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/config/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.860070 taipy-core-2.3.0.dev1/src/taipy/core/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/cycle/cycle_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.864070 taipy-core-2.3.0.dev1/src/taipy/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_data_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/abstract_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/abstract_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/data_node_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/data/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.864070 taipy-core-2.3.0.dev1/src/taipy/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.864070 taipy-core-2.3.0.dev1/src/taipy/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/_job_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/job_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/job/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.864070 taipy-core-2.3.0.dev1/src/taipy/core/notification/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/core_event_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/registration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/notification/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.868070 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/pipeline/pipeline_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.868070 taipy-core-2.3.0.dev1/src/taipy/core/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/scenario/scenario_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    25672 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/taipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.868070 taipy-core-2.3.0.dev1/src/taipy/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/_task_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/task/task_id.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/src/taipy/core/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.872070 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-05 16:01:49.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-05 16:01:49.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:01:49.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:01:42.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-05 16:01:49.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 16:01:49.000000 taipy-core-2.3.0.dev1/src/taipy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:01:49.872070 taipy-core-2.3.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/tests/test_complex_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    29447 2023-06-05 16:01:37.000000 taipy-core-2.3.0.dev1/tests/test_taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.011577 taipy-core-2.3.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-08 19:30:39.011577 taipy-core-2.3.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:30:39.011577 taipy-core-2.3.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.987577 taipy-core-2.3.0.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.987577 taipy-core-2.3.0.dev2/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.987577 taipy-core-2.3.0.dev2/src/taipy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.987577 taipy-core-2.3.0.dev2/src/taipy/core/_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_backup/_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_core_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.987577 taipy-core-2.3.0.dev2/src/taipy/core/_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_labeled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_entity/_submittable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.991577 taipy-core-2.3.0.dev2/src/taipy/core/_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_manager/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_manager/_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.991577 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_abstract_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.991577 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_orchestrator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.991577 taipy-core-2.3.0.dev2/src/taipy/core/_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_filesystem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_sql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_repository/_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.991577 taipy-core-2.3.0.dev2/src/taipy/core/_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.995577 taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/_bcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/_version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.995577 taipy-core-2.3.0.dev2/src/taipy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/_listattributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/default_custom_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/common/warn_if_inputs_not_ready.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.995577 taipy-core-2.3.0.dev2/src/taipy/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/_core_section.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.995577 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_config_id_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_data_node_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_global_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_job_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_pipeline_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_scenario_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_task_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    49075 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/data_node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/job_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/scenario_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/config/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:38.999577 taipy-core-2.3.0.dev2/src/taipy/core/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/cycle/cycle_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.003577 taipy-core-2.3.0.dev2/src/taipy/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_data_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/abstract_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9860 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/abstract_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/data_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/data/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.003577 taipy-core-2.3.0.dev2/src/taipy/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.003577 taipy-core-2.3.0.dev2/src/taipy/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/_job_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/job_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/job/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.003577 taipy-core-2.3.0.dev2/src/taipy/core/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/core_event_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/registration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/notification/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.007577 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/pipeline/pipeline_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.007577 taipy-core-2.3.0.dev2/src/taipy/core/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13465 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/scenario/scenario_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26101 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.007577 taipy-core-2.3.0.dev2/src/taipy/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/_task_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/task/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/src/taipy/core/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.007577 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-08 19:30:38.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-08 19:30:38.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:30:38.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:30:31.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-08 19:30:38.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 19:30:38.000000 taipy-core-2.3.0.dev2/src/taipy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:30:39.011577 taipy-core-2.3.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/tests/test_complex_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30198 2023-06-08 19:30:26.000000 taipy-core-2.3.0.dev2/tests/test_taipy.py
```

### Comparing `taipy-core-2.3.0.dev1/LICENSE` & `taipy-core-2.3.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/PKG-INFO` & `taipy-core-2.3.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.3.0.dev1
+Version: 2.3.0.dev2
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.3.0.dev1/README.md` & `taipy-core-2.3.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/setup.py` & `taipy-core-2.3.0.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,56 +24,28 @@
         from taipy.core.job.job import Job
         from taipy.core.job.job_id import JobId
         from taipy.core.job.status import Status
         from taipy.core.pipeline.pipeline import Pipeline
         from taipy.core.pipeline.pipeline_id import PipelineId
         from taipy.core.scenario.scenario import Scenario
         from taipy.core.scenario.scenario_id import ScenarioId
-        from taipy.core.taipy import (
-            cancel_job,
-            clean_all_entities,
-            clean_all_entities_by_version,
-            compare_scenarios,
-            create_pipeline,
-            create_scenario,
-            delete,
-            delete_job,
-            delete_jobs,
-            export_scenario,
-            get,
-            get_cycles,
-            get_cycles_scenarios,
-            get_data_nodes,
-            get_jobs,
-            get_latest_job,
-            get_parents,
-            get_pipelines,
-            get_primary,
-            get_primary_scenarios,
-            get_scenarios,
-            get_tasks,
-            set,
-            set_primary,
-            submit,
-            subscribe_pipeline,
-            subscribe_scenario,
-            tag,
-            unsubscribe_pipeline,
-            unsubscribe_scenario,
-            untag,
-        )
         from taipy.core.task.task import Task
         from taipy.core.task.task_id import TaskId
 
     if find_spec("taipy.gui"):
         from taipy.gui import Gui
 
+        if find_spec("taipy.gui_core"):
+            from taipy.gui_core.GuiCoreLib import GuiCore
+
+            Gui.add_library(GuiCore())
+
         if find_spec("taipy.enterprise") and find_spec("taipy.enterprise.gui"):
             from taipy.enterprise.gui import _init_gui_enterprise
 
             _init_gui_enterprise(Gui)
 
     if find_spec("taipy.rest"):
         from taipy.rest import Rest
 
     if find_spec("taipy._run"):
-        from taipy._run import _run as run
+        pass
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     get_latest_job,
     get_parents,
     get_pipelines,
     get_primary,
     get_primary_scenarios,
     get_scenarios,
     get_tasks,
+    is_deletable,
     set,
     set_primary,
     submit,
     subscribe_pipeline,
     subscribe_scenario,
     tag,
     unsubscribe_pipeline,
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_backup/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_backup/_backup.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_backup/_backup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,42 +8,53 @@
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 
 import os
 
+from taipy import Config
+
 __BACKUP_FILE_PATH_ENVIRONMENT_VARIABLE_NAME = "TAIPY_BACKUP_FILE_PATH"
 
 
-def _append_to_backup_file(new_file_path: str):
+def _init_backup_file_with_storage_folder():
     if preserve_file_path := os.getenv(__BACKUP_FILE_PATH_ENVIRONMENT_VARIABLE_NAME):
         with open(preserve_file_path, "a") as f:
-            f.write(f"{new_file_path}\n")
+            f.write(f"{Config.global_config.storage_folder}\n")
+
+
+def _append_to_backup_file(new_file_path: str):
+    if preserve_file_path := os.getenv(__BACKUP_FILE_PATH_ENVIRONMENT_VARIABLE_NAME):
+        storage_folder = os.path.abspath(Config.global_config.storage_folder) + os.sep
+        if not os.path.abspath(new_file_path).startswith(storage_folder):
+            with open(preserve_file_path, "a") as f:
+                f.write(f"{new_file_path}\n")
 
 
 def _remove_from_backup_file(to_remove_file_path: str):
-    preserve_file_path = os.getenv(__BACKUP_FILE_PATH_ENVIRONMENT_VARIABLE_NAME, None)
-    if preserve_file_path:
-        try:
-            with open(preserve_file_path, "r+") as f:
-                old_backup = f.read()
-                to_remove_file_path = to_remove_file_path + "\n"
-
-                # To avoid removing the file path of different data nodes that are pointing
-                # to the same file. We will only replace the file path only once.
-                if old_backup.startswith(to_remove_file_path):
-                    new_backup = old_backup.replace(to_remove_file_path, "", 1)
-                else:
-                    new_backup = old_backup.replace("\n" + to_remove_file_path, "\n", 1)
-
-                if new_backup is not old_backup:
-                    f.seek(0)
-                    f.write(new_backup)
-                    f.truncate()
-        except Exception:
-            pass
+    if preserve_file_path := os.getenv(__BACKUP_FILE_PATH_ENVIRONMENT_VARIABLE_NAME, None):
+        storage_folder = os.path.abspath(Config.global_config.storage_folder) + os.sep
+        if not os.path.abspath(to_remove_file_path).startswith(storage_folder):
+            try:
+                with open(preserve_file_path, "r+") as f:
+                    old_backup = f.read()
+                    to_remove_file_path = to_remove_file_path + "\n"
+
+                    # To avoid removing the file path of different data nodes that are pointing
+                    # to the same file. We will only replace the file path only once.
+                    if old_backup.startswith(to_remove_file_path):
+                        new_backup = old_backup.replace(to_remove_file_path, "", 1)
+                    else:
+                        new_backup = old_backup.replace("\n" + to_remove_file_path, "\n", 1)
+
+                    if new_backup is not old_backup:
+                        f.seek(0)
+                        f.write(new_backup)
+                        f.truncate()
+            except Exception:
+                pass
 
 
 def _replace_in_backup_file(old_file_path: str, new_file_path: str):
     _remove_from_backup_file(old_file_path)
     _append_to_backup_file(new_file_path)
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_core.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 # specific language governing permissions and limitations under the License.
 
 from typing import Optional
 
 from taipy.config import Config
 from taipy.logger._taipy_logger import _TaipyLogger
 
+from ._backup._backup import _init_backup_file_with_storage_folder
 from ._core_cli import _CoreCLI
 from ._orchestrator._dispatcher._job_dispatcher import _JobDispatcher
 from ._orchestrator._orchestrator import _Orchestrator
 from ._orchestrator._orchestrator_factory import _OrchestratorFactory
 from ._version._version_manager_factory import _VersionManagerFactory
+from .config import CoreSection
 
 
 class Core:
     """
     Core service
     """
 
@@ -59,17 +61,18 @@
         if self._dispatcher:
             self._dispatcher = _OrchestratorFactory._remove_dispatcher()
             self.__logger.info("Core service has been stopped.")
 
     @staticmethod
     def __update_and_check_config():
         _CoreCLI.create_parser()
-        Config._applied_config._unique_sections["core"]._update(_CoreCLI.parse_arguments())
+        Config._applied_config._unique_sections[CoreSection.name]._update(_CoreCLI.parse_arguments())
         Config.check()
         Config.block_update()
+        _init_backup_file_with_storage_folder()
 
     @staticmethod
     def __manage_version():
         _VersionManagerFactory._build_manager()._manage_version()
 
     def __start_dispatcher(self, force_restart):
         if dispatcher := _OrchestratorFactory._build_dispatcher(force_restart=force_restart):
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_core_cli.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_core_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_entity/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_dag.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_dag.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_entity.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_entity.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_entity_ids.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_entity_ids.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_labeled.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_labeled.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_properties.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_properties.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,40 +7,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 from collections import UserDict
 
-from ..notification import EventEntityType, EventOperation, _publish_event
+from ..notification import _ENTITY_TO_EVENT_ENTITY_TYPE, EventOperation, _publish_event
 
 
 class _Properties(UserDict):
-
-    __ENTITY_TO_EVENT_ENTITY_TYPE = {
-        "scenario": EventEntityType.SCENARIO,
-        "pipeline": EventEntityType.PIPELINE,
-        "task": EventEntityType.TASK,
-        "data": EventEntityType.DATA_NODE,
-        "job": EventEntityType.JOB,
-        "cycle": EventEntityType.CYCLE,
-    }
-
     def __init__(self, entity_owner, **kwargs):
         super().__init__(**kwargs)
         self._entity_owner = entity_owner
 
     def __setitem__(self, key, value):
         super(_Properties, self).__setitem__(key, value)
         from ... import core as tp
 
         if hasattr(self, "_entity_owner"):
             tp.set(self._entity_owner)
             _publish_event(
-                self.__ENTITY_TO_EVENT_ENTITY_TYPE[self._entity_owner._MANAGER_NAME],
+                _ENTITY_TO_EVENT_ENTITY_TYPE[self._entity_owner._MANAGER_NAME],
                 self._entity_owner.id,
                 EventOperation.UPDATE,
                 key,
             )
 
     def __getitem__(self, key):
         from taipy.config.common._template_handler import _TemplateHandler as _tpl
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_reload.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_reload.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import functools
 
-from ..notification import EventEntityType, EventOperation, _publish_event
+from ..notification import EventOperation, _publish_event
 
 
 @functools.lru_cache
 def _get_manager(manager: str):
     from ..cycle._cycle_manager_factory import _CycleManagerFactory
     from ..data._data_manager_factory import _DataManagerFactory
     from ..job._job_manager_factory import _JobManagerFactory
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_entity/_submittable.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_entity/_submittable.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_manager/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_manager/_manager.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_manager/_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_manager/_manager_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_manager/_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_abstract_orchestrator.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_abstract_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_orchestrator.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/_orchestrator_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/_orchestrator_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_orchestrator/utils.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_repository/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_filesystem_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_filesystem_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository_adapter.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_repository_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_sql_model.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_sql_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_repository/_sql_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_repository/_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/_bcolor.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/_bcolor.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_cli/_version_cli.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_cli/_version_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_utils.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_fs_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_manager.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_manager_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_model.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_repository_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/_version/_version_sql_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/_version/_version_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/common/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/common/_listattributes.py` & `taipy-core-2.3.0.dev2/src/taipy/core/common/_listattributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     def __set_self(self):
         from ... import core as tp
 
         if hasattr(self, "_parent"):
             tp.set(self._parent)
 
     def __add__(self, value):
-        # TODO: publish event of changing attributes
         if hasattr(value, "__iter__"):
             self.__add_iterable(value)
         else:
             self.append(value)
         return self
 
     def extend(self, value) -> None:
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/common/_repr_enum.py` & `taipy-core-2.3.0.dev2/src/taipy/core/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/common/_utils.py` & `taipy-core-2.3.0.dev2/src/taipy/core/common/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/common/_warnings.py` & `taipy-core-2.3.0.dev2/src/taipy/core/common/_warnings.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/common/default_custom_document.py` & `taipy-core-2.3.0.dev2/src/taipy/core/common/default_custom_document.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/common/warn_if_inputs_not_ready.py` & `taipy-core-2.3.0.dev2/src/taipy/core/common/warn_if_inputs_not_ready.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/_core_section.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/_core_section.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from taipy.config import Config, UniqueSection
 from taipy.config._config import _Config
 from taipy.config.common._template_handler import _TemplateHandler as _tpl
 
 
 class CoreSection(UniqueSection):
-    name = "core"
+    name = "CORE"
     _MODE_KEY = "mode"
     _DEVELOPMENT_MODE = "development"
     _EXPERIMENT_MODE = "experiment"
     _PRODUCTION_MODE = "production"
     _DEFAULT_MODE = _DEVELOPMENT_MODE
     _VERSION_NUMBER_KEY = "version_number"
     _DEFAULT_VERSION_NUMBER = ""
@@ -50,14 +50,21 @@
 
     @classmethod
     def default_config(cls):
         return CoreSection(
             cls._DEFAULT_MODE, cls._DEFAULT_VERSION_NUMBER, cls._DEFAULT_TAIPY_FORCE, cls._DEFAULT_CLEAN_ENTITIES
         )
 
+    def _clean(self):
+        self.mode = self._DEFAULT_MODE
+        self.version_number = self._DEFAULT_VERSION_NUMBER
+        self.force = self._DEFAULT_TAIPY_FORCE
+        self.clean_entities = self._DEFAULT_CLEAN_ENTITIES
+        self._properties.clear()
+
     def _to_dict(self):
         as_dict = {}
         if self.mode is not None:
             as_dict[self._MODE_KEY] = self.mode
         if self.version_number is not None:
             as_dict[self._VERSION_NUMBER_KEY] = self.version_number
         if self.force is not None:
@@ -97,14 +104,22 @@
         force: Optional[bool] = None,
         clean_entities: Optional[bool] = None,
         **properties,
     ):
         """Configure the Core service.
 
         Parameters:
+            mode (Optional[str], optional): Indicates the mode of the version management system.
+                Possible values are *"development"*, *"experiment"*, or *"production"*.
+            version_number (Optional[str], optional): The string identifier of the version.
+                 In development mode, the version number is ignored.
+            force (Optional[bool], optional): If True, Taipy will override a version even if the configuration
+                has changed and run the application.
+            clean_entities (Optional[bool], optional): If True, running a Taipy Core service will clean all current
+                version entities before running the application.
             **properties (Dict[str, Any]): A keyworded variable length list of additional arguments configure the
                 behavior of the `Core^` service.
         Returns:
             The Core configuration.
         """
         section = CoreSection(
             mode=mode, version_number=version_number, force=force, clean_entities=clean_entities, **properties
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_config_id_checker.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_config_id_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_data_node_config_checker.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_data_node_config_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 #
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
+from datetime import timedelta
 from typing import Dict
 
 from taipy.config._config import _Config
 from taipy.config.checker._checker import _ConfigChecker
 from taipy.config.checker.issue_collector import IssueCollector
 from taipy.config.common.scope import Scope
 
@@ -26,14 +27,15 @@
     def _check(self) -> IssueCollector:
         data_node_configs: Dict[str, DataNodeConfig] = self._config._sections[DataNodeConfig.name]
         for data_node_config_id, data_node_config in data_node_configs.items():
             self._check_existing_config_id(data_node_config)
             self._check_if_entity_property_key_used_is_predefined(data_node_config)
             self._check_storage_type(data_node_config_id, data_node_config)
             self._check_scope(data_node_config_id, data_node_config)
+            self._check_validity_period(data_node_config_id, data_node_config)
             self._check_required_properties(data_node_config_id, data_node_config)
             self._check_callable(data_node_config_id, data_node_config)
             self._check_generic_read_write_fct_and_args(data_node_config_id, data_node_config)
             self._check_exposed_type(data_node_config_id, data_node_config)
         return self._collector
 
     def _check_storage_type(self, data_node_config_id: str, data_node_config: DataNodeConfig):
@@ -56,14 +58,23 @@
         if data_node_config.scope == Scope.PIPELINE:
             self._warning(
                 data_node_config._SCOPE_KEY,
                 data_node_config.scope,
                 f"`{Scope.PIPELINE}` is deprecated. Please use other `Scope` value instead.",
             )
 
+    def _check_validity_period(self, data_node_config_id: str, data_node_config: DataNodeConfig):
+        if data_node_config.validity_period and not isinstance(data_node_config.validity_period, timedelta):
+            self._error(
+                data_node_config._VALIDITY_PERIOD_KEY,
+                data_node_config.validity_period,
+                f"`{data_node_config._VALIDITY_PERIOD_KEY}` field of DataNodeConfig `{data_node_config_id}` must be"
+                f" None or populated with a timedelta value.",
+            )
+
     def _check_required_properties(self, data_node_config_id: str, data_node_config: DataNodeConfig):
         if storage_type := data_node_config.storage_type:
             if storage_type in DataNodeConfig._REQUIRED_PROPERTIES:
                 required_properties = DataNodeConfig._REQUIRED_PROPERTIES[storage_type]
                 if storage_type == DataNodeConfig._STORAGE_TYPE_VALUE_SQL:
                     if data_node_config.properties:
                         if engine := data_node_config.properties.get(DataNodeConfig._REQUIRED_DB_ENGINE_SQL_PROPERTY):
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_global_config_checker.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_global_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_job_config_checker.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_job_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_pipeline_config_checker.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_pipeline_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_scenario_config_checker.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_scenario_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/checkers/_task_config_checker.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/checkers/_task_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/config.schema.json` & `taipy-core-2.3.0.dev2/src/taipy/core/config/config.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999897875816993%*

 * *Differences: {"'properties'": "{'DATA_NODE': {'additionalProperties': {'properties': {'validity_period': "*

 * *                 "OrderedDict([('description', 'A timedelta value as a string: The duration since "*

 * *                 'the last edit date for which the data node can be considered up-to-date. If '*

 * *                 "*validity_period* is set to None, the data node is always up-to-date.'), "*

 * *                 "('type', 'string')])}}}}"}*

```diff
@@ -227,14 +227,18 @@
                         "type": "string"
                     },
                     "then": {
                         "required": [
                             "default_path"
                         ]
                     },
+                    "validity_period": {
+                        "description": "A timedelta value as a string: The duration since the last edit date for which the data node can be considered up-to-date. If *validity_period* is set to None, the data node is always up-to-date.",
+                        "type": "string"
+                    },
                     "write_fct": {
                         "description": "storage_type: generic specific.",
                         "taipy_function": true,
                         "type": "string"
                     },
                     "write_fct_args": {
                         "description": "storage_type: generic specific.",
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/data_node_config.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/data_node_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 import json
 from copy import copy
+from datetime import timedelta
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from taipy.config._config import _Config
 from taipy.config.common._config_blocker import _ConfigBlocker
 from taipy.config.common._template_handler import _TemplateHandler as _tpl
 from taipy.config.common.scope import Scope
 from taipy.config.config import Config
@@ -231,21 +232,32 @@
             _OPTIONAL_EXPOSED_TYPE_PARQUET_PROPERTY: _DEFAULT_EXPOSED_TYPE,
         },
     }
 
     _SCOPE_KEY = "scope"
     _DEFAULT_SCOPE = Scope.SCENARIO
 
-    def __init__(self, id: str, storage_type: Optional[str] = None, scope: Scope = None, **properties):
+    _VALIDITY_PERIOD_KEY = "validity_period"
+    _DEFAULT_VALIDITY_PERIOD = None
+
+    def __init__(
+        self,
+        id: str,
+        storage_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
+        **properties,
+    ):
         self._storage_type = storage_type
         self._scope = scope
+        self._validity_period = validity_period
         super().__init__(id, **properties)
 
     def __copy__(self):
-        return DataNodeConfig(self.id, self._storage_type, self._scope, **copy(self._properties))
+        return DataNodeConfig(self.id, self._storage_type, self._scope, self._validity_period, **copy(self._properties))
 
     def __getattr__(self, item: str) -> Optional[Any]:
         return _tpl._replace_templates(self._properties.get(item))
 
     @property
     def storage_type(self):
         return _tpl._replace_templates(self._storage_type)
@@ -261,14 +273,23 @@
 
     @scope.setter  # type: ignore
     @_ConfigBlocker._check()
     def scope(self, val):
         self._scope = val
 
     @property
+    def validity_period(self):
+        return _tpl._replace_templates(self._validity_period)
+
+    @validity_period.setter  # type: ignore
+    @_ConfigBlocker._check()
+    def validity_period(self, val):
+        self._validity_period = val
+
+    @property
     def cacheable(self):
         _warn_deprecated("cacheable", suggest="the skippable feature")
         cacheable = self._properties.get("cacheable")
         if cacheable is not None:
             return _tpl._replace_templates(cacheable)
         else:
             return False
@@ -277,95 +298,127 @@
     @_ConfigBlocker._check()
     def cacheable(self, val):
         _warn_deprecated("cacheable", suggest="the skippable feature")
         self._properties["cacheable"] = val
 
     @classmethod
     def default_config(cls):
-        return DataNodeConfig(cls._DEFAULT_KEY, cls._DEFAULT_STORAGE_TYPE, cls._DEFAULT_SCOPE)
+        return DataNodeConfig(
+            cls._DEFAULT_KEY, cls._DEFAULT_STORAGE_TYPE, cls._DEFAULT_SCOPE, cls._DEFAULT_VALIDITY_PERIOD
+        )
+
+    def _clean(self):
+        self._storage_type = self._DEFAULT_STORAGE_TYPE
+        self._scope = self._DEFAULT_SCOPE
+        self._validity_period = self._DEFAULT_VALIDITY_PERIOD
+        self._properties.clear()
 
     def _to_dict(self):
         as_dict = {}
         if self._storage_type is not None:
             as_dict[self._STORAGE_TYPE_KEY] = self._storage_type
         if self._scope is not None:
             as_dict[self._SCOPE_KEY] = self._scope
+        if self._validity_period is not None:
+            as_dict[self._VALIDITY_PERIOD_KEY] = self._validity_period
         as_dict.update(self._properties)
         return as_dict
 
     @classmethod
     def _from_dict(cls, as_dict: Dict[str, Any], id: str, config: Optional[_Config] = None):
         as_dict.pop(cls._ID_KEY, id)
         storage_type = as_dict.pop(cls._STORAGE_TYPE_KEY, None)
         scope = as_dict.pop(cls._SCOPE_KEY, None)
-        return DataNodeConfig(id=id, storage_type=storage_type, scope=scope, **as_dict)
+        validity_perid = as_dict.pop(cls._VALIDITY_PERIOD_KEY, None)
+        return DataNodeConfig(id=id, storage_type=storage_type, scope=scope, validity_period=validity_perid, **as_dict)
 
     def _update(self, as_dict, default_section=None):
         self._storage_type = as_dict.pop(self._STORAGE_TYPE_KEY, self._storage_type)
         if self._storage_type is None and default_section:
             self._storage_type = default_section.storage_type
 
         self._scope = as_dict.pop(self._SCOPE_KEY, self._scope)
         if self._scope is None and default_section:
             if default_section.scope and self._storage_type == default_section.storage_type:
                 self._scope = default_section.scope
             else:
                 self._scope = self._DEFAULT_SCOPE
 
+        self._validity_period = as_dict.pop(self._VALIDITY_PERIOD_KEY, self._validity_period)
+        if self._validity_period is None and default_section:
+            self._validity_period = default_section.validity_period
+
         self._properties.update(as_dict)
         if default_section and self._storage_type == default_section.storage_type:
             self._properties = {**default_section.properties, **self._properties}
 
         # Assign default value to optional properties if not defined by user
         if self._OPTIONAL_PROPERTIES.get(self._storage_type):
             for optional_property, default_value in self._OPTIONAL_PROPERTIES[self._storage_type].items():
                 if default_value is not None and self._properties.get(optional_property) is None:
                     self._properties[optional_property] = default_value
 
     @staticmethod
-    def _configure_default(storage_type: str, scope: Optional[Scope] = None, **properties) -> "DataNodeConfig":
+    def _configure_default(
+        storage_type: str, scope: Optional[Scope] = None, validity_period: Optional[timedelta] = None, **properties
+    ) -> "DataNodeConfig":
         """Configure the default values for data node configurations.
 
         This function creates the _default data node configuration_ object,
         where all data node configuration objects will find their default
         values when needed.
 
         Parameters:
             storage_type (str): The default storage type for all data node configurations.
                 The possible values are *"pickle"* (the default value), *"csv"*, *"excel"*,
                 *"sql"*, *"mongo_collection"*, *"in_memory"*, *"json"*, *"parquet"* or
                 *"generic"*.
             scope (Optional[Scope^]): The default scope for all data node configurations.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The default data node configuration.
         """
-        section = DataNodeConfig(_Config.DEFAULT_KEY, storage_type, scope, **properties)
+        section = DataNodeConfig(_Config.DEFAULT_KEY, storage_type, scope, validity_period, **properties)
         Config._register_default(section)
         return Config.sections[DataNodeConfig.name][_Config.DEFAULT_KEY]
 
     @classmethod
     def _configure(
-        cls, id: str, storage_type: Optional[str] = None, scope: Optional[Scope] = None, **properties
+        cls,
+        id: str,
+        storage_type: Optional[str] = None,
+        scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
+        **properties,
     ) -> "DataNodeConfig":
         """Configure a new data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new data node configuration.
             storage_type (Optional[str]): The data node configuration storage type. The possible values
                 are None (which is the default value of *"pickle"*, unless it has been overloaded by the
                 *storage_type* value set in the default data node configuration
                 (see `(Config.)configure_default_data_node()^`)), *"pickle"*, *"csv"*, *"excel"*,
                 *"sql_table"*, *"sql"*, *"json"*, *"parquet"*, *"mongo_collection"*, *"in_memory"*, or
                 *"generic"*.
             scope (Optional[Scope^]): The scope of the data node configuration.<br/>
                 The default value is `Scope.SCENARIO` (or the one specified in
                 `(Config.)configure_default_data_node()^`).
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new data node configuration.
         """
         configuration_map: Dict[str, Callable] = {
             cls._STORAGE_TYPE_VALUE_PICKLE: cls._configure_pickle,
@@ -377,95 +430,108 @@
             cls._STORAGE_TYPE_VALUE_IN_MEMORY: cls._configure_in_memory,
             cls._STORAGE_TYPE_VALUE_GENERIC: cls._configure_generic,
             cls._STORAGE_TYPE_VALUE_JSON: cls._configure_json,
             cls._STORAGE_TYPE_VALUE_PARQUET: cls._configure_parquet,
         }
 
         if storage_type in cls._ALL_STORAGE_TYPES:
-            return configuration_map[storage_type](id=id, scope=scope, **properties)
+            return configuration_map[storage_type](id=id, scope=scope, validity_period=validity_period, **properties)
 
-        return cls.__configure(id, storage_type, scope, **properties)
+        return cls.__configure(id, storage_type, scope, validity_period, **properties)
 
     @classmethod
     def _configure_csv(
         cls,
         id: str,
         default_path: Optional[str] = None,
         has_header: Optional[bool] = None,
         exposed_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new CSV data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new CSV data node configuration.
             default_path (Optional[str]): The default path of the CSV file.
             has_header (Optional[bool]): If True, indicates that the CSV file has a header.
             exposed_type (Optional[str]): The exposed type of the data read from CSV file.<br/>
                 The default value is `pandas`.
             scope (Optional[Scope^]): The scope of the CSV data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new CSV data node configuration.
         """
         if default_path is not None:
             properties[cls._OPTIONAL_DEFAULT_PATH_CSV_PROPERTY] = default_path
         if has_header is not None:
             properties[cls._OPTIONAL_HAS_HEADER_CSV_PROPERTY] = has_header
         if exposed_type is not None:
             properties[cls._OPTIONAL_EXPOSED_TYPE_CSV_PROPERTY] = exposed_type
 
-        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_CSV, scope, **properties)
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_CSV, scope, validity_period, **properties)
 
     @classmethod
     def _configure_json(
         cls,
         id: str,
         default_path: Optional[str] = None,
         encoder: Optional[json.JSONEncoder] = None,
         decoder: Optional[json.JSONDecoder] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new JSON data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new JSON data node configuration.
             default_path (Optional[str]): The default path of the JSON file.
             encoder (Optional[json.JSONEncoder]): The JSON encoder used to write data into the JSON file.
             decoder (Optional[json.JSONDecoder]): The JSON decoder used to read data from the JSON file.
             scope (Optional[Scope^]): The scope of the JSON data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new JSON data node configuration.
         """
         if default_path is not None:
             properties[cls._OPTIONAL_DEFAULT_PATH_JSON_PROPERTY] = default_path
         if encoder is not None:
             properties[cls._OPTIONAL_ENCODER_JSON_PROPERTY] = encoder
         if decoder is not None:
             properties[cls._OPTIONAL_DECODER_JSON_PROPERTY] = decoder
 
-        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_JSON, scope, **properties)
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_JSON, scope, validity_period, **properties)
 
     @classmethod
     def _configure_parquet(
         cls,
         id: str,
         default_path: Optional[str] = None,
         engine: Optional[str] = None,
         compression: Optional[str] = None,
         read_kwargs: Optional[Dict] = None,
         write_kwargs: Optional[Dict] = None,
         exposed_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new Parquet data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new Parquet data node configuration.
             default_path (Optional[str]): The default path of the Parquet file.
@@ -480,14 +546,19 @@
                 `pandas.DataFrame.write_parquet()` function.<br/>
                 The parameters in *read_kwargs* and *write_kwargs* have a **higher precedence** than the
                 top-level parameters which are also passed to Pandas.
             exposed_type (Optional[str]): The exposed type of the data read from Parquet file.<br/>
                 The default value is `pandas`.
             scope (Optional[Scope^]): The scope of the Parquet data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Parquet data node configuration.
         """
         if default_path is not None:
             properties[cls._OPTIONAL_DEFAULT_PATH_PARQUET_PROPERTY] = default_path
@@ -498,64 +569,71 @@
         if read_kwargs is not None:
             properties[cls._OPTIONAL_READ_KWARGS_PARQUET_PROPERTY] = read_kwargs
         if write_kwargs is not None:
             properties[cls._OPTIONAL_WRITE_KWARGS_PARQUET_PROPERTY] = write_kwargs
         if exposed_type is not None:
             properties[cls._OPTIONAL_EXPOSED_TYPE_PARQUET_PROPERTY] = exposed_type
 
-        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_PARQUET, scope, **properties)
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_PARQUET, scope, validity_period, **properties)
 
     @classmethod
     def _configure_excel(
         cls,
         id: str,
         default_path: Optional[str] = None,
         has_header: Optional[bool] = None,
         sheet_name: Optional[Union[List[str], str]] = None,
         exposed_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new Excel data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new Excel data node configuration.
             default_path (Optional[str]): The path of the Excel file.
             has_header (Optional[bool]): If True, indicates that the Excel file has a header.
             sheet_name (Optional[Union[List[str], str]]): The list of sheet names to be used.
                 This can be a unique name.
             exposed_type (Optional[str]): The exposed type of the data read from Excel file.<br/>
                 The default value is `pandas`.
             scope (Optional[Scope^]): The scope of the Excel data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Excel data node configuration.
         """
         if default_path is not None:
             properties[cls._OPTIONAL_DEFAULT_PATH_EXCEL_PROPERTY] = default_path
         if has_header is not None:
             properties[cls._OPTIONAL_HAS_HEADER_EXCEL_PROPERTY] = has_header
         if sheet_name is not None:
             properties[cls._OPTIONAL_SHEET_NAME_EXCEL_PROPERTY] = sheet_name
         if exposed_type is not None:
             properties[cls._OPTIONAL_EXPOSED_TYPE_EXCEL_PROPERTY] = exposed_type
 
-        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_EXCEL, scope, **properties)
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_EXCEL, scope, validity_period, **properties)
 
     @classmethod
     def _configure_generic(
         cls,
         id: str,
         read_fct: Optional[Callable] = None,
         write_fct: Optional[Callable] = None,
         read_fct_args: Optional[List] = None,
         write_fct_args: Optional[List] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new generic data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new generic data node configuration.
             read_fct (Optional[Callable]): The Python function called to read the data.
@@ -563,80 +641,101 @@
                 The provided function must have at least one parameter that receives the data to be written.
             read_fct_args (Optional[List]): The list of arguments that are passed to the function
                 *read_fct* to read data.
             write_fct_args (Optional[List]): The list of arguments that are passed to the function
                 *write_fct* to write the data.
             scope (Optional[Scope^]): The scope of the Generic data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new Generic data node configuration.
         """
         if read_fct is not None:
             properties[cls._OPTIONAL_READ_FUNCTION_GENERIC_PROPERTY] = read_fct
         if write_fct is not None:
             properties[cls._OPTIONAL_WRITE_FUNCTION_GENERIC_PROPERTY] = write_fct
         if read_fct_args is not None:
             properties[cls._OPTIONAL_READ_FUNCTION_ARGS_GENERIC_PROPERTY] = read_fct_args
         if write_fct_args is not None:
             properties[cls._OPTIONAL_WRITE_FUNCTION_ARGS_GENERIC_PROPERTY] = write_fct_args
 
-        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_GENERIC, scope, **properties)
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_GENERIC, scope, validity_period, **properties)
 
     @classmethod
     def _configure_in_memory(
-        cls, id: str, default_data: Optional[Any] = None, scope: Optional[Scope] = None, **properties
+        cls,
+        id: str,
+        default_data: Optional[Any] = None,
+        scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
+        **properties,
     ) -> "DataNodeConfig":
         """Configure a new *in-memory* data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new in_memory data node configuration.
             default_data (Optional[any]): The default data of the data nodes instantiated from
                 this in_memory data node configuration.
             scope (Optional[Scope^]): The scope of the in_memory data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new *in-memory* data node configuration.
         """
         if default_data is not None:
             properties[cls._OPTIONAL_DEFAULT_DATA_IN_MEMORY_PROPERTY] = default_data
 
-        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_IN_MEMORY, scope, **properties)
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_IN_MEMORY, scope, validity_period, **properties)
 
     @classmethod
     def _configure_pickle(
         cls,
         id: str,
         default_path: Optional[str] = None,
         default_data: Optional[Any] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new pickle data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new pickle data node configuration.
             default_path (Optional[str]): The path of the pickle file.
             default_data (Optional[any]): The default data of the data nodes instantiated from
                 this pickle data node configuration.
             scope (Optional[Scope^]): The scope of the pickle data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new pickle data node configuration.
         """
         if default_path is not None:
             properties[cls._OPTIONAL_DEFAULT_PATH_PICKLE_PROPERTY] = default_path
         if default_data is not None:
             properties[cls._OPTIONAL_DEFAULT_DATA_PICKLE_PROPERTY] = default_data
 
-        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_PICKLE, scope, **properties)
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_PICKLE, scope, validity_period, **properties)
 
     @classmethod
     def _configure_sql_table(
         cls,
         id: str,
         db_name: str,
         db_engine: str,
@@ -647,14 +746,15 @@
         db_port: Optional[int] = None,
         db_driver: Optional[str] = None,
         sqlite_folder_path: Optional[str] = None,
         sqlite_file_extension: Optional[str] = None,
         db_extra_args: Optional[Dict[str, Any]] = None,
         exposed_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new SQL table data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new SQL data node configuration.
             db_name (str): The database name, or the name of the SQLite database file.
@@ -676,14 +776,19 @@
                 The default value is ".db".
             db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
                 into database connection string.
             exposed_type (Optional[str]): The exposed type of the data read from SQL table.<br/>
                 The default value is "pandas".
             scope (Optional[Scope^]): The scope of the SQL data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new SQL data node configuration.
         """
         properties.update(
             {
@@ -708,15 +813,15 @@
         if sqlite_file_extension is not None:
             properties[cls._OPTIONAL_FILE_EXTENSION_SQLITE_PROPERTY] = sqlite_file_extension
         if db_extra_args is not None:
             properties[cls._OPTIONAL_DB_EXTRA_ARGS_SQL_PROPERTY] = db_extra_args
         if exposed_type is not None:
             properties[cls._OPTIONAL_EXPOSED_TYPE_SQL_PROPERTY] = exposed_type
 
-        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_SQL_TABLE, scope, **properties)
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_SQL_TABLE, scope, validity_period, **properties)
 
     @classmethod
     def _configure_sql(
         cls,
         id: str,
         db_name: str,
         db_engine: str,
@@ -728,14 +833,15 @@
         db_port: Optional[int] = None,
         db_driver: Optional[str] = None,
         sqlite_folder_path: Optional[str] = None,
         sqlite_file_extension: Optional[str] = None,
         db_extra_args: Optional[Dict[str, Any]] = None,
         exposed_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new SQL data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new SQL data node configuration.
             db_name (str): The database name, or the name of the SQLite database file.
@@ -759,14 +865,19 @@
                 The default value is ".db".
             db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
                 into database connection string.
             exposed_type (Optional[str]): The exposed type of the data read from SQL query.<br/>
                 The default value is "pandas".
             scope (Optional[Scope^]): The scope of the SQL data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
         Returns:
             The new SQL data node configuration.
         """
         properties.update(
             {
                 cls._REQUIRED_DB_NAME_SQL_PROPERTY: db_name,
@@ -791,29 +902,30 @@
         if sqlite_file_extension is not None:
             properties[cls._OPTIONAL_FILE_EXTENSION_SQLITE_PROPERTY] = sqlite_file_extension
         if db_extra_args is not None:
             properties[cls._OPTIONAL_DB_EXTRA_ARGS_SQL_PROPERTY] = db_extra_args
         if exposed_type is not None:
             properties[cls._OPTIONAL_EXPOSED_TYPE_SQL_PROPERTY] = exposed_type
 
-        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_SQL, scope, **properties)
+        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_SQL, scope, validity_period, **properties)
 
     @classmethod
     def _configure_mongo_collection(
         cls,
         id: str,
         db_name: str,
         collection_name: str,
         custom_document: Optional[Any] = None,
         db_username: Optional[str] = None,
         db_password: Optional[str] = None,
         db_host: Optional[str] = None,
         db_port: Optional[int] = None,
         db_extra_args: Optional[Dict[str, Any]] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ) -> "DataNodeConfig":
         """Configure a new Mongo collection data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new Mongo collection data node configuration.
             db_name (str): The database name.
@@ -829,14 +941,19 @@
                 The default value is "localhost".
             db_port (Optional[int]): The database port.<br/>
                 The default value is 27017.
             db_extra_args (Optional[dict[str, any]]): A dictionary of additional arguments to be passed
                 into database connection string.
             scope (Optional[Scope^]): The scope of the Mongo collection data node configuration.<br/>
                 The default value is `Scope.SCENARIO`.
+            validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
+                considered up-to-date. Once the validity period has passed, the data node is considered stale and
+                relevant tasks will run even if they are skippable (see the
+                [Task configs page](../core/config/task-config.md) for more details).
+                If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
 
         Returns:
             The new Mongo collection data node configuration.
         """
         properties.update(
             {
@@ -854,19 +971,22 @@
         if db_host is not None:
             properties[cls._OPTIONAL_HOST_MONGO_PROPERTY] = db_host
         if db_port is not None:
             properties[cls._OPTIONAL_PORT_MONGO_PROPERTY] = db_port
         if db_extra_args is not None:
             properties[cls._OPTIONAL_DB_EXTRA_ARGS_MONGO_PROPERTY] = db_extra_args
 
-        return cls.__configure(id, DataNodeConfig._STORAGE_TYPE_VALUE_MONGO_COLLECTION, scope, **properties)
+        return cls.__configure(
+            id, DataNodeConfig._STORAGE_TYPE_VALUE_MONGO_COLLECTION, scope, validity_period, **properties
+        )
 
     @staticmethod
     def __configure(
         id: str,
         storage_type: Optional[str] = None,
         scope: Optional[Scope] = None,
+        validity_period: Optional[timedelta] = None,
         **properties,
     ):
-        section = DataNodeConfig(id, storage_type, scope, **properties)
+        section = DataNodeConfig(id, storage_type, scope, validity_period, **properties)
         Config._register(section)
         return Config.sections[DataNodeConfig.name][id]
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/job_config.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/job_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,28 +34,33 @@
 
     _MODE_KEY = "mode"
     _STANDALONE_MODE = "standalone"
     _DEVELOPMENT_MODE = "development"
     _DEFAULT_MODE = _DEVELOPMENT_MODE
     _MODES = [_STANDALONE_MODE, _DEVELOPMENT_MODE]
 
-    def __init__(self, mode: str = None, **properties):
+    def __init__(self, mode: Optional[str] = None, **properties):
         self.mode = mode or self._DEFAULT_MODE
         self._config = self._create_config(self.mode, **properties)
+        super().__init__(**properties)
 
     def __copy__(self):
         return JobConfig(self.mode, **copy(self._properties))
 
     def __getattr__(self, key: str) -> Optional[Any]:
         return self._config.get(key, None)
 
     @classmethod
     def default_config(cls):
         return JobConfig(cls._DEFAULT_MODE)
 
+    def _clean(self):
+        self.mode = self._DEFAULT_MODE
+        self._config = self._create_config(self.mode)
+
     def _to_dict(self):
         as_dict = {}
         if self.mode is not None:
             as_dict[self._MODE_KEY] = self.mode
         as_dict.update(self._config)
         return as_dict
 
@@ -71,15 +76,18 @@
             self.mode = mode
             self._config = self._create_config(self.mode, **as_dict)
         if self._config is not None:
             self._update_config(as_dict)
 
     @staticmethod
     def _configure(
-        mode: str = None, nb_of_workers: Union[int, str] = None, max_nb_of_workers: Union[int, str] = None, **properties
+        mode: Optional[str] = None,
+        nb_of_workers: Optional[Union[int, str]] = None,
+        max_nb_of_workers: Optional[Union[int, str]] = None,
+        **properties
     ) -> "JobConfig":
         """Configure job execution.
 
         Parameters:
             mode (Optional[str]): The job execution mode.
                 Possible values are: *"standalone"* (the default value) or *"development"*.
             max_nb_of_workers (Optional[int, str]): Parameter used only in default *"standalone"* mode.
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/pipeline_config.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/pipeline_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,18 @@
     def tasks(self) -> List[TaskConfig]:
         return self._tasks
 
     @classmethod
     def default_config(cls):
         return PipelineConfig(cls._DEFAULT_KEY, [])
 
+    def _clean(self):
+        self._tasks = []
+        self._properties.clear()
+
     def _to_dict(self):
         return {self._TASK_KEY: self._tasks, **self._properties}
 
     @classmethod
     def _from_dict(cls, as_dict: Dict[str, Any], id: str, config: Optional[_Config]):
         as_dict.pop(cls._ID_KEY, id)
         t_configs = config._sections[TaskConfig.name]  # type: ignore
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/scenario_config.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/scenario_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,20 @@
         _warn_deprecated("PipelineConfig")
         return self._pipelines
 
     @classmethod
     def default_config(cls):
         return ScenarioConfig(cls._DEFAULT_KEY, [], None, dict())
 
+    def _clean(self):
+        self._pipelines = []
+        self.frequency = None
+        self.comparators = dict()
+        self._properties.clear()
+
     def _to_dict(self):
         return {
             self._COMPARATOR_KEY: self.comparators,
             self._PIPELINE_KEY: self._pipelines,
             self._FREQUENCY_KEY: self.frequency,
             **self._properties,
         }
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/config/task_config.py` & `taipy-core-2.3.0.dev2/src/taipy/core/config/task_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,17 @@
         else:
             self._outputs = []
         self._skippable = skippable
         self.function = function
         super().__init__(id, **properties)
 
     def __copy__(self):
-        return TaskConfig(self.id, copy(self._inputs), self.function, copy(self._outputs), **copy(self._properties))
+        return TaskConfig(
+            self.id, self.function, copy(self._inputs), copy(self._outputs), self.skippable, **copy(self._properties)
+        )
 
     def __getattr__(self, item: str) -> Optional[Any]:
         return _tpl._replace_templates(self._properties.get(item))
 
     @property
     def input_configs(self) -> List[DataNodeConfig]:
         return list(self._inputs)
@@ -101,18 +103,25 @@
     def skippable(self):
         return _tpl._replace_templates(self._skippable)
 
     @classmethod
     def default_config(cls):
         return TaskConfig(cls._DEFAULT_KEY, None, [], [], False)
 
+    def _clean(self):
+        self.function = None
+        self._inputs = []
+        self._outputs = []
+        self._skippable = False
+        self._properties.clear()
+
     def _to_dict(self):
         return {
-            self._INPUT_KEY: self._inputs,
             self._FUNCTION: self.function,
+            self._INPUT_KEY: self._inputs,
             self._OUTPUT_KEY: self._outputs,
             self._IS_SKIPPABLE_KEY: self._skippable,
             **self._properties,
         }
 
     @classmethod
     def _from_dict(cls, as_dict: Dict[str, Any], id: str, config: Optional[_Config]):
@@ -125,23 +134,23 @@
         outputs = []
         if outputs_as_str := as_dict.pop(cls._OUTPUT_KEY, None):
             outputs = [dn_configs[ds_id] for ds_id in outputs_as_str if ds_id in dn_configs]
         skippable = as_dict.pop(cls._IS_SKIPPABLE_KEY, False)
         return TaskConfig(id=id, function=funct, inputs=inputs, outputs=outputs, skippable=skippable, **as_dict)
 
     def _update(self, as_dict, default_section=None):
+        function = as_dict.pop(self._FUNCTION, None)
+        if function is not None and type(function) is not str:
+            self.function = function
         self._inputs = as_dict.pop(self._INPUT_KEY, self._inputs)
         if self._inputs is None and default_section:
             self._inputs = default_section._inputs
         self._outputs = as_dict.pop(self._OUTPUT_KEY, self._outputs)
         if self._outputs is None and default_section:
             self._outputs = default_section._outputs
-        function = as_dict.pop(self._FUNCTION, None)
-        if function is not None and type(function) is not str:
-            self.function = function
         self._skippable = as_dict.pop(self._IS_SKIPPABLE_KEY, self._skippable)
         self._properties.update(as_dict)
         if default_section:
             self._properties = {**default_section.properties, **self._properties}
 
     @staticmethod
     def _configure(
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/cycle/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_fs_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_manager.py` & `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_manager_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_model.py` & `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_repository_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/cycle/_cycle_sql_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/cycle/_cycle_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/cycle/cycle.py` & `taipy-core-2.3.0.dev2/src/taipy/core/cycle/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/cycle/cycle_id.py` & `taipy-core-2.3.0.dev2/src/taipy/core/cycle/cycle_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_fs_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_manager.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,28 +81,27 @@
     @classmethod
     def __create(
         cls, data_node_config: DataNodeConfig, owner_id: Optional[str], parent_ids: Optional[Set[str]]
     ) -> DataNode:
         try:
             version = _VersionManagerFactory._build_manager()._get_latest_version()
             props = data_node_config._properties.copy()
-            validity_period = props.pop("validity_period", None)
 
             if data_node_config.storage_type:
                 storage_type = data_node_config.storage_type
             else:
                 storage_type = Config.sections[DataNodeConfig.name][_Config.DEFAULT_KEY].storage_type
 
             return cls.__DATA_NODE_CLASS_MAP[storage_type](
                 config_id=data_node_config.id,
                 scope=data_node_config.scope or DataNodeConfig._DEFAULT_SCOPE,
+                validity_period=data_node_config.validity_period,
                 owner_id=owner_id,
                 parent_ids=parent_ids,
                 version=version,
-                validity_period=validity_period,
                 properties=props,
             )
         except KeyError:
             raise InvalidDataNodeType(data_node_config.storage_type)
 
     @classmethod
     def _clean_pickle_file(cls, data_node: DataNode):
@@ -120,16 +119,15 @@
     def _remove_dn_file_path_in_backup_file(cls, data_node: DataNode):
         if isinstance(data_node, _AbstractFileDataNode):
             _remove_from_backup_file(to_remove_file_path=data_node.path)
 
     @classmethod
     def _remove_dn_file_paths_in_backup_file(cls, data_nodes: Iterable[DataNode]):
         for data_node in data_nodes:
-            if isinstance(data_node, _AbstractFileDataNode):
-                _remove_from_backup_file(to_remove_file_path=data_node.path)
+            cls._remove_dn_file_path_in_backup_file(data_node)
 
     @classmethod
     def _delete(cls, data_node_id: DataNodeId):
         data_node = cls._get(data_node_id, None)
         if data_node:
             cls._clean_pickle_file(data_node)
             cls._remove_dn_file_path_in_backup_file(data_node)
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_manager_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_model.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_repository_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/_data_sql_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/_data_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/_filter.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/_filter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/abstract_file.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/abstract_file.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/abstract_sql.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/abstract_sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/csv.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/csv.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/data_node.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/data_node.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/data_node_id.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/data_node_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/excel.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/excel.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/generic.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/generic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/in_memory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/in_memory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/json.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/json.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/mongo.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/mongo.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/operator.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/operator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/parquet.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/parquet.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/pickle.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/pickle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/sql.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/data/sql_table.py` & `taipy-core-2.3.0.dev2/src/taipy/core/data/sql_table.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/exceptions/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/exceptions/exceptions.py` & `taipy-core-2.3.0.dev2/src/taipy/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_fs_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_manager.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_manager_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_model.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_repository_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/_job_sql_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/_job_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/job.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/job.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/job_id.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/job_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/job/status.py` & `taipy-core-2.3.0.dev2/src/taipy/core/job/status.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/notification/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/notification/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations under the License.
 
 
 from .core_event_consumer import CoreEventConsumerBase
-from .event import EventEntityType, EventOperation
+from .event import _ENTITY_TO_EVENT_ENTITY_TYPE, EventEntityType, EventOperation
 from .notifier import _publish_event
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/notification/core_event_consumer.py` & `taipy-core-2.3.0.dev2/src/taipy/core/notification/core_event_consumer.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/notification/event.py` & `taipy-core-2.3.0.dev2/src/taipy/core/notification/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,22 @@
     TASK = 4
     DATA_NODE = 5
     JOB = 6
 
 
 _NO_ATTRIBUTE_NAME_OPERATIONS = set([EventOperation.CREATION, EventOperation.DELETION, EventOperation.SUBMISSION])
 _UNSUBMITTABLE_ENTITY_TYPES = (EventEntityType.CYCLE, EventEntityType.DATA_NODE, EventEntityType.JOB)
+_ENTITY_TO_EVENT_ENTITY_TYPE = {
+    "scenario": EventEntityType.SCENARIO,
+    "pipeline": EventEntityType.PIPELINE,
+    "task": EventEntityType.TASK,
+    "data": EventEntityType.DATA_NODE,
+    "job": EventEntityType.JOB,
+    "cycle": EventEntityType.CYCLE,
+}
 
 
 class Event:
     def __init__(
         self,
         entity_type: EventEntityType,
         entity_id: Optional[str],
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/notification/notifier.py` & `taipy-core-2.3.0.dev2/src/taipy/core/notification/notifier.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/notification/registration.py` & `taipy-core-2.3.0.dev2/src/taipy/core/notification/registration.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/notification/registration_id.py` & `taipy-core-2.3.0.dev2/src/taipy/core/notification/registration_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/notification/topic.py` & `taipy-core-2.3.0.dev2/src/taipy/core/notification/topic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_fs_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_manager.py` & `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,20 +66,20 @@
             return
 
         cls.__remove_subscriber(callback, params, pipeline)
 
     @classmethod
     def __add_subscriber(cls, callback, params, pipeline):
         pipeline._add_subscriber(callback, params)
-        cls._set(pipeline)
+        _publish_event(cls._EVENT_ENTITY_TYPE, pipeline.id, EventOperation.UPDATE, "subscribers")
 
     @classmethod
     def __remove_subscriber(cls, callback, params, pipeline):
         pipeline._remove_subscriber(callback, params)
-        cls._set(pipeline)
+        _publish_event(cls._EVENT_ENTITY_TYPE, pipeline.id, EventOperation.UPDATE, "subscribers")
 
     @classmethod
     def _get_or_create(
         cls,
         pipeline_config: PipelineConfig,
         cycle_id: Optional[CycleId] = None,
         scenario_id: Optional[ScenarioId] = None,
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_manager_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_model.py` & `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_repository_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/_pipeline_sql_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/_pipeline_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/pipeline.py` & `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/pipeline/pipeline_id.py` & `taipy-core-2.3.0.dev2/src/taipy/core/pipeline/pipeline_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/scenario/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_fs_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_manager.py` & `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,20 +78,20 @@
             return
 
         cls.__remove_subscriber(callback, params, scenario)
 
     @classmethod
     def __add_subscriber(cls, callback, params, scenario):
         scenario._add_subscriber(callback, params)
-        cls._set(scenario)
+        _publish_event(cls._EVENT_ENTITY_TYPE, scenario.id, EventOperation.UPDATE, "subscribers")
 
     @classmethod
     def __remove_subscriber(cls, callback, params, scenario):
         scenario._remove_subscriber(callback, params)
-        cls._set(scenario)
+        _publish_event(cls._EVENT_ENTITY_TYPE, scenario.id, EventOperation.UPDATE, "subscribers")
 
     @classmethod
     def _create(
         cls,
         config: ScenarioConfig,
         creation_date: Optional[datetime.datetime] = None,
         name: Optional[str] = None,
@@ -204,18 +204,16 @@
         return primary_scenarios
 
     @classmethod
     def _set_primary(cls, scenario: Scenario):
         if scenario.cycle:
             primary_scenario = cls._get_primary(scenario.cycle)
             if primary_scenario:
-                primary_scenario._primary_scenario = False
-                cls._set(primary_scenario)
-            scenario._primary_scenario = True
-            cls._set(scenario)
+                primary_scenario.is_primary = False  # type: ignore
+            scenario.is_primary = True  # type: ignore
         else:
             raise DoesNotBelongToACycle(
                 f"Can't set scenario {scenario.id} to primary because it doesn't belong to a cycle."
             )
 
     @classmethod
     def _tag(cls, scenario: Scenario, tag: str):
@@ -225,31 +223,21 @@
         if scenario.cycle:
             old_tagged_scenario = cls._get_by_tag(scenario.cycle, tag)
             if old_tagged_scenario:
                 old_tagged_scenario.remove_tag(tag)
                 cls._set(old_tagged_scenario)
         scenario._add_tag(tag)
         cls._set(scenario)
+        _publish_event(cls._EVENT_ENTITY_TYPE, scenario.id, EventOperation.UPDATE, "tags")
 
     @classmethod
     def _untag(cls, scenario: Scenario, tag: str):
         scenario._remove_tag(tag)
         cls._set(scenario)
-
-    @classmethod
-    def _delete(cls, scenario_id: ScenarioId):
-        scenario = cls._get(scenario_id)
-        if scenario.is_primary:
-            if len(cls._get_all_by_cycle(scenario.cycle)) > 1:
-                raise DeletingPrimaryScenario(
-                    f"Scenario {scenario.id}, which has config id {scenario.config_id}, is primary and there are "
-                    f"other scenarios in the same cycle. "
-                )
-            _CycleManagerFactory._build_manager()._delete(scenario.cycle.id)
-        super()._delete(scenario_id)
+        _publish_event(cls._EVENT_ENTITY_TYPE, scenario.id, EventOperation.UPDATE, "tags")
 
     @classmethod
     def _compare(cls, *scenarios: Scenario, data_node_config_id: Optional[str] = None):
         if len(scenarios) < 2:
             raise InsufficientScenarioToCompare("At least two scenarios are required to compare.")
 
         if not all(scenarios[0].config_id == scenario.config_id for scenario in scenarios):
@@ -277,27 +265,48 @@
             raise NonExistingScenarioConfig(scenarios[0].config_id)
 
     @staticmethod
     def __get_config(scenario: Scenario):
         return Config.scenarios.get(scenario.config_id, None)
 
     @classmethod
+    def _is_deletable(cls, scenario: Union[Scenario, ScenarioId]) -> bool:
+        if isinstance(scenario, str):
+            scenario = cls._get(scenario)
+        if scenario.is_primary:
+            if len(cls._get_all_by_cycle(scenario.cycle)) > 1:
+                return False
+        return True
+
+    @classmethod
+    def _delete(cls, scenario_id: ScenarioId):
+        scenario = cls._get(scenario_id)
+        if not cls._is_deletable(scenario):
+            raise DeletingPrimaryScenario(
+                f"Scenario {scenario.id}, which has config id {scenario.config_id}, is primary and there are "
+                f"other scenarios in the same cycle. "
+            )
+        if scenario.is_primary:
+            _CycleManagerFactory._build_manager()._delete(scenario.cycle.id)
+        super()._delete(scenario_id)
+
+    @classmethod
     def _hard_delete(cls, scenario_id: ScenarioId):
         scenario = cls._get(scenario_id)
+        if not cls._is_deletable(scenario):
+            raise DeletingPrimaryScenario(
+                f"Scenario {scenario.id}, which has config id {scenario.config_id}, is primary and there are "
+                f"other scenarios in the same cycle. "
+            )
         if scenario.is_primary:
-            if len(cls._get_all_by_cycle(scenario.cycle)) > 1:
-                raise DeletingPrimaryScenario(
-                    f"Scenario {scenario.id}, which has config id {scenario.config_id}, is primary and there are "
-                    f"other scenarios in the same cycle. "
-                )
             _CycleManagerFactory._build_manager()._hard_delete(scenario.cycle.id)
-            return
-        entity_ids_to_delete = cls._get_children_entity_ids(scenario)
-        entity_ids_to_delete.scenario_ids.add(scenario.id)
-        cls._delete_entities_of_multiple_types(entity_ids_to_delete)
+        else:
+            entity_ids_to_delete = cls._get_children_entity_ids(scenario)
+            entity_ids_to_delete.scenario_ids.add(scenario.id)
+            cls._delete_entities_of_multiple_types(entity_ids_to_delete)
 
     @classmethod
     def _delete_by_version(cls, version_number: str):
         """
         Deletes scenario by the version number.
 
         Check if the cycle is only attached to this scenario, then delete it.
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_manager_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_model.py` & `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_repository_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/scenario/_scenario_sql_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/scenario/_scenario_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/scenario/scenario.py` & `taipy-core-2.3.0.dev2/src/taipy/core/scenario/scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,14 +359,24 @@
         Parameters:
             tag (str): The tag to remove from the set of the scenario's tags.
         """
         from ... import core as tp
 
         return tp.untag(self, tag)
 
+    def is_deletable(self) -> bool:
+        """Indicate if the scenario can be deleted.
+
+        Returns:
+            True if the scenario can be deleted. False otherwise.
+        """
+        from ... import core as tp
+
+        return tp.is_deletable(self)
+
     def __get_pipelines(self):
         pipelines = {}
         pipeline_manager = _PipelineManagerFactory._build_manager()
 
         for pipeline_or_id in self._pipelines:
             p = pipeline_manager._get(pipeline_or_id, pipeline_or_id)
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/scenario/scenario_id.py` & `taipy-core-2.3.0.dev2/src/taipy/core/scenario/scenario_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/taipy.py` & `taipy-core-2.3.0.dev2/src/taipy/core/taipy.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import Any, Callable, Dict, List, Optional, Set, Union, overload
 
 from taipy.config.config import Config
 from taipy.logger._taipy_logger import _TaipyLogger
 
 from ._entity._entity import _Entity
 from ._version._version_manager_factory import _VersionManagerFactory
-from .common._warnings import _warn_no_core_service
+from .common._warnings import _warn_deprecated, _warn_no_core_service
 from .config.pipeline_config import PipelineConfig
 from .config.scenario_config import ScenarioConfig
 from .cycle._cycle_manager_factory import _CycleManagerFactory
 from .cycle.cycle import Cycle
 from .cycle.cycle_id import CycleId
 from .data._data_manager_factory import _DataManagerFactory
 from .data.data_node import DataNode
@@ -167,24 +167,34 @@
 
     Returns:
         The list of tasks.
     """
     return _TaskManagerFactory._build_manager()._get_all()
 
 
+def is_deletable(scenario: Union[Scenario, ScenarioId]) -> bool:
+    """Indicate if a scenario can be deleted.
+
+    Returns:
+        True if the given scenario can be deleted. False otherwise.
+    """
+    return _ScenarioManagerFactory._build_manager()._is_deletable(scenario)
+
+
 def delete(entity_id: Union[TaskId, DataNodeId, PipelineId, ScenarioId, JobId, CycleId]):
     """Delete an entity and its nested entities.
 
     The given entity is deleted. The deletion is propagated to all nested entities that are
     not shared by another entity.
 
     - If a `CycleId^` is provided, the nested scenarios, pipelines, data nodes, and jobs are deleted.
     - If a `ScenarioId^` is provided, the nested pipelines, tasks, data nodes, and jobs are deleted.
-    - If the scenario is primary, it can only be deleted if it is the only scenario in the cycle. In that case, its
-        cycle is also deleted.
+        If the scenario is primary, it can only be deleted if it is the only scenario in the cycle.
+        In that case, its cycle is also deleted. Please use the `is_deletable()` function to check if
+        the scenario can be deleted.
     - If a `PipelineId^` is provided, the nested tasks, data nodes, and jobs are deleted.
     - If a `TaskId^` is provided, the nested data nodes, and jobs are deleted.
 
     Parameters:
         entity_id (Union[TaskId^, DataNodeId^, PipelineId^, ScenarioId^, JobId^, CycleId^]): The
             identifier of the entity to delete.
     Raises:
@@ -486,14 +496,15 @@
     """Create and return a new pipeline from a pipeline configuration.
 
     Parameters:
         config (PipelineConfig^): The pipeline configuration.
     Returns:
         The new pipeline.
     """
+    _warn_deprecated("create_pipeline")
     return _PipelineManagerFactory._build_manager()._get_or_create(config)
 
 
 def clean_all_entities() -> bool:
     """Delete all entities from the Taipy data folder.
 
     !!! important
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/task/__init__.py` & `taipy-core-2.3.0.dev2/src/taipy/core/task/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_fs_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_manager.py` & `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_manager_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_model.py` & `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_repository_factory.py` & `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/task/_task_sql_repository.py` & `taipy-core-2.3.0.dev2/src/taipy/core/task/_task_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/task/task.py` & `taipy-core-2.3.0.dev2/src/taipy/core/task/task.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy/core/task/task_id.py` & `taipy-core-2.3.0.dev2/src/taipy/core/task/task_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/src/taipy_core.egg-info/PKG-INFO` & `taipy-core-2.3.0.dev2/src/taipy_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.3.0.dev1
+Version: 2.3.0.dev2
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.3.0.dev1/src/taipy_core.egg-info/SOURCES.txt` & `taipy-core-2.3.0.dev2/src/taipy_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/tests/test_complex_application.py` & `taipy-core-2.3.0.dev2/tests/test_complex_application.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.3.0.dev1/tests/test_taipy.py` & `taipy-core-2.3.0.dev2/tests/test_taipy.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import pathlib
 import shutil
 from unittest import mock
 
 import pytest
 
 import src.taipy.core.taipy as tp
-from src.taipy.core import Core, CycleId, JobId, PipelineId, ScenarioId, TaskId
+from src.taipy.core import Core, CycleId, JobId, PipelineId, Scenario, ScenarioId, TaskId
 from src.taipy.core._orchestrator._orchestrator_factory import _OrchestratorFactory
 from src.taipy.core._version._version_manager import _VersionManager
 from src.taipy.core.config.job_config import JobConfig
 from src.taipy.core.config.pipeline_config import PipelineConfig
 from src.taipy.core.config.scenario_config import ScenarioConfig
 from src.taipy.core.cycle._cycle_manager import _CycleManager
 from src.taipy.core.data._data_manager import _DataManager
@@ -102,14 +102,25 @@
 
     def test_get_task(self, task):
         with mock.patch("src.taipy.core.task._task_manager._TaskManager._get") as mck:
             task_id = TaskId("TASK_id")
             tp.get(task_id)
             mck.assert_called_once_with(task_id)
 
+    def test_is_deletable(self):
+        with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._is_deletable") as mck:
+            scenario_id = ScenarioId("SCENARIO_id")
+            tp.is_deletable(scenario_id)
+            mck.assert_called_once_with(scenario_id)
+
+        with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._is_deletable") as mck:
+            scenario = Scenario("config_id", [], {})
+            tp.is_deletable(scenario)
+            mck.assert_called_once_with(scenario)
+
     def test_delete_scenario(self):
         with mock.patch("src.taipy.core.scenario._scenario_manager._ScenarioManager._hard_delete") as mck:
             scenario_id = ScenarioId("SCENARIO_id")
             tp.delete(scenario_id)
             mck.assert_called_once_with(scenario_id)
 
     def test_delete(self):
@@ -315,14 +326,19 @@
 
     def test_create_pipeline(self):
         pipeline_config = PipelineConfig("pipeline_config")
         with mock.patch("src.taipy.core.pipeline._pipeline_manager._PipelineManager._get_or_create") as mck:
             tp.create_pipeline(pipeline_config)
             mck.assert_called_once_with(pipeline_config)
 
+    def test_create_pipeline_deprecated(self):
+        pipeline_config = PipelineConfig("pipeline_config")
+        with pytest.warns(DeprecationWarning):
+            tp.create_pipeline(pipeline_config)
+
     def test_clean_all_entities(self, cycle):
         data_node_1_config = Config.configure_data_node(id="d1", storage_type="in_memory", scope=Scope.SCENARIO)
         data_node_2_config = Config.configure_data_node(
             id="d2", storage_type="pickle", default_data="abc", scope=Scope.SCENARIO
         )
         task_config = Config.configure_task(
             "my_task", print, data_node_1_config, data_node_2_config, scope=Scope.SCENARIO
```

