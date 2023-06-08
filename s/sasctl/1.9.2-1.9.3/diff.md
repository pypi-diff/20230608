# Comparing `tmp/sasctl-1.9.2.tar.gz` & `tmp/sasctl-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sasctl-1.9.2.tar", last modified: Wed May 17 22:22:28 2023, max compression
+gzip compressed data, was "sasctl-1.9.3.tar", last modified: Thu Jun  8 18:32:49 2023, max compression
```

## Comparing `sasctl-1.9.2.tar` & `sasctl-1.9.3.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-05-17 22:22:18.000000 sasctl-1.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-17 22:22:18.000000 sasctl-1.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-17 22:22:18.000000 sasctl-1.9.2/ContributorAgreement.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 22:22:18.000000 sasctl-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-17 22:22:18.000000 sasctl-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-05-17 22:22:28.986489 sasctl-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-05-17 22:22:18.000000 sasctl-1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-17 22:22:18.000000 sasctl-1.9.2/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:22:28.986489 sasctl-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-17 22:22:19.000000 sasctl-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.978489 sasctl-1.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.982489 sasctl-1.9.2/src/sasctl/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.982489 sasctl-1.9.2/src/sasctl/_services/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/cas_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/concepts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/data_sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/folders.py
--rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/microanalytic_score.py
--rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/model_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/model_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)    28696 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/model_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/report_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/saslogon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/sentiment_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/text_categorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/text_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/_services/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    74999 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.982489 sasctl-1.9.2/src/sasctl/pzmm/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16653 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/gitIntegration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/import_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/mlflow_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/model_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/pickle_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.982489 sasctl-1.9.2/src/sasctl/pzmm/template_files/
--rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_fitstat.json
--rw-r--r--   0 runner    (1001) docker     (123)    51874 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_lift.json
--rw-r--r--   0 runner    (1001) docker     (123)   193713 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_roc.json
--rw-r--r--   0 runner    (1001) docker     (123)    82150 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/write_json_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    63504 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/write_score_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/pzmm/zip_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    33574 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/astore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/model_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/pymas/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pymas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pymas/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pymas/ds2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pymas/python.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/pyml2ds/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/pyml2ds/basic/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/basic/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.986489 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-17 22:22:19.000000 sasctl-1.9.2/src/sasctl/utils/pyml2ds/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:22:28.982489 sasctl-1.9.2/src/sasctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 22:22:28.000000 sasctl-1.9.2/src/sasctl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.928073 sasctl-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-06-08 18:32:36.000000 sasctl-1.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-08 18:32:36.000000 sasctl-1.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-08 18:32:36.000000 sasctl-1.9.3/ContributorAgreement.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 18:32:36.000000 sasctl-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-08 18:32:36.000000 sasctl-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-08 18:32:49.928073 sasctl-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-06-08 18:32:36.000000 sasctl-1.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 18:32:36.000000 sasctl-1.9.3/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:32:49.928073 sasctl-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-08 18:32:36.000000 sasctl-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.912073 sasctl-1.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.916072 sasctl-1.9.3/src/sasctl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.920072 sasctl-1.9.3/src/sasctl/_services/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19546 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/cas_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/concepts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/data_sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/folders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11901 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/microanalytic_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18619 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/model_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/model_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28696 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/model_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/report_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/saslogon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/sentiment_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13771 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/text_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/text_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/_services/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74999 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/pzmm/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17973 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/git_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17213 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/import_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/mlflow_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/model_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/pickle_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/pzmm/template_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_fitstat.json
+-rw-r--r--   0 runner    (1001) docker     (123)    51874 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_lift.json
+-rw-r--r--   0 runner    (1001) docker     (123)   193713 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_roc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    82560 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/write_json_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63812 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/write_score_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/pzmm/zip_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33574 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16435 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/astore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/model_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/utils/pymas/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pymas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22824 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pymas/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pymas/ds2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pymas/python.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/utils/pyml2ds/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/utils/pyml2ds/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/basic/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.924072 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.928073 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-06-08 18:32:36.000000 sasctl-1.9.3/src/sasctl/utils/pyml2ds/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:32:49.916072 sasctl-1.9.3/src/sasctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 18:32:49.000000 sasctl-1.9.3/src/sasctl.egg-info/top_level.txt
```

### Comparing `sasctl-1.9.2/CHANGELOG.md` & `sasctl-1.9.3/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 Unreleased
 ----------
 **Improvements**
  - Refactor `tasks.py` to utilize `sasctl.pzmm` functions.
  - Add `model_info` class to better capture model information.
 
+v1.9.3 (2023-06-08)
+----------
+**Improvements**
+ - Refactored gitIntegration.py to `git_integration.py` and added unit tests for better test coverage.
+
+**Bugfixes**
+ - Fixed issue with ROC and Lift charts not properly being written to disk.
+ - Fixed JSON conversion for Lift charts that caused TRAIN and TEST charts to be incorrect.
+ - Fixed issue with H2O score code and number of curly brackets.
+ - Updated score code logic for H2O to account for incompatibility with Path objects.
+ - Fixed issue where inputVar.json could supply invalid values to SAS Model Manager upon model import.
+ - Fixed issue with `services.model_publish.list_models`, which was using an older API format that is not valid in SAS Viya 3.5 or SAS Viya 4.
+
 v1.9.2 (2023-05-17)
 ----------
 **Improvements**
  - Add recursive folder creation and an example.
  - Add example for migrating models from SAS Viya 3.5 to SAS Viya 4.
 
 **Bugfixes**
```

### Comparing `sasctl-1.9.2/CONTRIBUTING.md` & `sasctl-1.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/ContributorAgreement.txt` & `sasctl-1.9.3/ContributorAgreement.txt`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/LICENSE` & `sasctl-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/PKG-INFO` & `sasctl-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sasctl
-Version: 1.9.2
+Version: 1.9.3
 Summary: SAS Viya Python Client
 Home-page: https://github.com/sassoftware/python-sasctl/
 Author: SAS
 License: Apache v2.0
 Project-URL: Bug Tracker, https://github.com/sassoftware/python-sasctl/issues
 Project-URL: Documentation, https://sassoftware.github.io/python-sasctl/
 Project-URL: Source Code, https://github.com/sassoftware/python-sasctl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sasctl Version: 1.9.2 Summary: SAS Viya Python
+Metadata-Version: 2.1 Name: sasctl Version: 1.9.3 Summary: SAS Viya Python
 Client Home-page: https://github.com/sassoftware/python-sasctl/ Author: SAS
 License: Apache v2.0 Project-URL: Bug Tracker, https://github.com/sassoftware/
 python-sasctl/issues Project-URL: Documentation, https://sassoftware.github.io/
 python-sasctl/ Project-URL: Source Code, https://github.com/sassoftware/python-
 sasctl Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Environment ::
 Console Classifier: Intended Audience :: Science/Research Classifier: Intended
```

### Comparing `sasctl-1.9.2/README.md` & `sasctl-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/setup.py` & `sasctl-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/__init__.py` & `sasctl-1.9.3/src/sasctl/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # encoding: utf-8
 #
 # Copyright © 2019, SAS Institute Inc., Cary, NC, USA.  All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 
-__version__ = "1.9.2"
+__version__ = "1.9.3"
 __author__ = "SAS"
 __credits__ = [
     "Yi Jian Ching",
     "Lucas De Paula",
     "James Kochuba",
     "Peter Tobac",
     "Chris Toth",
```

### Comparing `sasctl-1.9.2/src/sasctl/_services/cas_management.py` & `sasctl-1.9.3/src/sasctl/_services/cas_management.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/concepts.py` & `sasctl-1.9.3/src/sasctl/_services/concepts.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/data_sources.py` & `sasctl-1.9.3/src/sasctl/_services/data_sources.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/files.py` & `sasctl-1.9.3/src/sasctl/_services/files.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/folders.py` & `sasctl-1.9.3/src/sasctl/_services/folders.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/microanalytic_score.py` & `sasctl-1.9.3/src/sasctl/_services/microanalytic_score.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/model_management.py` & `sasctl-1.9.3/src/sasctl/_services/model_management.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/model_publish.py` & `sasctl-1.9.3/src/sasctl/_services/model_publish.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if re.match(r"\d", name):
             name = "_" + name
 
         return name
 
     @classmethod
     def list_models(cls):
-        return cls.get("/models").get("items", [])
+        return cls.get("/models")
 
     list_destinations, get_destination, update_destination, _ = Service._crud_funcs(
         "/destinations", "destination"
     )
 
     # @sasctl_command('delete')
     @classmethod
```

### Comparing `sasctl-1.9.2/src/sasctl/_services/model_repository.py` & `sasctl-1.9.3/src/sasctl/_services/model_repository.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/projects.py` & `sasctl-1.9.3/src/sasctl/_services/projects.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/relationships.py` & `sasctl-1.9.3/src/sasctl/_services/relationships.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/report_images.py` & `sasctl-1.9.3/src/sasctl/_services/report_images.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/reports.py` & `sasctl-1.9.3/src/sasctl/_services/reports.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/saslogon.py` & `sasctl-1.9.3/src/sasctl/_services/saslogon.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/sentiment_analysis.py` & `sasctl-1.9.3/src/sasctl/_services/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/service.py` & `sasctl-1.9.3/src/sasctl/_services/service.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/text_categorization.py` & `sasctl-1.9.3/src/sasctl/_services/text_categorization.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/text_parsing.py` & `sasctl-1.9.3/src/sasctl/_services/text_parsing.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/_services/workflow.py` & `sasctl-1.9.3/src/sasctl/_services/workflow.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/core.py` & `sasctl-1.9.3/src/sasctl/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/exceptions.py` & `sasctl-1.9.3/src/sasctl/exceptions.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/gitIntegration.py` & `sasctl-1.9.3/src/sasctl/pzmm/git_integration.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # Copyright (c) 2022, SAS Institute Inc., Cary, NC, USA.  All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 import io
 import zipfile
 from pathlib import Path
+from typing import Optional, Union
 from uuid import UUID
 from warnings import warn
 
 from .._services.model_repository import ModelRepository as mr
-from ..core import RestObj
+from ..core import is_uuid, RestObj
 
 try:
     import git
     from git import Repo
 except ImportError:
     git = None
+    Repo = None
 
 
-def checkGitStatus():
-    """Check to see if GitPython has been installed and if a valid git executable
+def check_git_status() -> None:
+    """
+    Check to see if GitPython has been installed and if a valid git executable
     exists on the target system. If one of those two conditions is not met, then
     a RunTime error is raised.
 
     Raises
     ------
     RuntimeError
         Raised if an invalid git setup for git integration is detected.
@@ -30,71 +33,97 @@
     if git is None:
         raise RuntimeError(
             "The 'GitPython' package and a valid git executable are required"
             + " for use of the git integration functions."
         )
 
 
-def getZippedModel(model, gPath, project=None):
-    """Retrieve a zipped file containing all of the model contents or a specified
-    model. The project argument is only needed if the model argument is not a valid
+def get_zipped_model(
+    model: Union[str, RestObj],
+    git_path: Union[str, Path],
+    project: Optional[Union[str, RestObj]] = None,
+) -> (str, str):
+    """
+    Retrieve a zipped file containing all the model contents of a specified
+    model.
+
+    The project argument is only needed if the model argument is not a valid
     UUID or RestObj.
 
     Parameters
     ----------
     model : string or RestObj
         Model name, UUID, or RestObj which identifies the model. If only the model name
         is provided, the project name must also be supplied.
-    gPath : string or Path
+    git_path : string or Path
         Base directory of the git repository.
     project : string or RestObj, optional
-        Project identifier, which is required when only the model name is supplied. Default
-        is None.
+        Project identifier, which is required when only the model name is supplied.
+        Default is None.
+
+    Returns
+    -------
+    model_name : string
+        Name of the model retrieved from SAS Model Manager.
+    project_name : string
+        Name of the project the model was retrieved from in SAS Model Manager.
     """
-    params = {"format": "zip"}
-    modelZip = mr.get(f"models/{model}", params=params, format_="content")
-    modelName = mr.get_model(model).name
-    # Check project argument to determine project name
-    if isinstance(project, RestObj):
-        projectName = project.name
-    elif project is None:
-        projectName = mr.get_model(model).projectName
+    # Find the specified model and pull down the contents in a zip format
+    if isinstance(model, RestObj):
+        model = mr.get_model(model)
+    elif is_uuid(model):
+        model = mr.get_model(model)
     else:
-        projectName = mr.get_project(project).name
+        if not project:
+            raise ValueError(
+                "The model cannot be determined accurately from just the model name. "
+                "Please provide either the model UUID or the project name."
+            )
+        else:
+            project = mr.get_project(project)
+        model = mr.list_models(
+            filter=f"and(eq(projectName,'{project.name}'),eq(name,'{model}'))"
+        )[0]
+    params = {"format": "zip"}
+    model_zip = mr.get(f"models/{model.id}", params=params, format_="content")
+    model_name = model.name
+    project_name = model.projectName
+
     # Check to see if project folder exists
-    if (Path(gPath) / projectName).exists():
+    if (Path(git_path) / project_name).exists():
         # Check to see if model folder exists
-        if (Path(gPath) / projectName / modelName).exists():
+        if (Path(git_path) / project_name / model_name).exists():
             with open(
-                Path(gPath) / projectName / modelName / (modelName + ".zip"), "wb"
-            ) as zFile:
-                zFile.write(modelZip)
+                Path(git_path) / project_name / model_name / (model_name + ".zip"), "wb"
+            ) as zip_file:
+                zip_file.write(model_zip)
         else:
-            newDir = Path(gPath) / projectName / modelName
-            newDir.mkdir(parents=True, exist_ok=True)
+            new_dir = Path(git_path) / project_name / model_name
+            new_dir.mkdir(parents=True, exist_ok=True)
             with open(
-                Path(gPath) / projectName / modelName / (modelName + ".zip"), "wb"
-            ) as zFile:
-                zFile.write(modelZip)
+                Path(git_path) / project_name / model_name / (model_name + ".zip"), "wb"
+            ) as zip_file:
+                zip_file.write(model_zip)
     else:
-        newDir = Path(gPath) / projectName
-        newDir.mkdir(parents=True, exist_ok=True)
-        newDir = Path(gPath) / projectName / modelName
-        newDir.mkdir(parents=True, exist_ok=True)
+        new_dir = Path(git_path) / project_name
+        new_dir.mkdir(parents=True, exist_ok=True)
+        new_dir = Path(git_path) / project_name / model_name
+        new_dir.mkdir(parents=True, exist_ok=True)
         with open(
-            Path(gPath) / (projectName + "/" + modelName + "/" + modelName + ".zip"),
+            Path(git_path) / f"{project_name}/{model_name}/{model_name}.zip",
             "wb",
-        ) as zFile:
-            zFile.write(modelZip)
+        ) as zip_file:
+            zip_file.write(model_zip)
 
-    return modelName, projectName
+    return model_name, project_name
 
 
 def project_exists(response, project):
-    """Checks if project exists on SAS Viya. If the project does not exist, then a new
+    """
+    Checks if project exists on SAS Viya. If the project does not exist, then a new
     project is created or an error is raised.
 
     Parameters
     ----------
     response : RestObj
         JSON response of the get_project() call to model repository service.
     project : string or RestObj
@@ -111,16 +140,17 @@
         Alerts user that API calls cannot continue until a valid project is provided.
     """
     if response is None:
         try:
             warn(f"No project with the name or UUID {project} was found.")
             UUID(project)
             raise SystemError(
-                "The provided UUID does not match any projects found in SAS Model Manager. "
-                + "Please enter a valid UUID or a new name for a project to be created."
+                "The provided UUID does not match any projects found in SAS Model "
+                "Manager. Please enter a valid UUID or a new name for a project to be "
+                "created."
             )
         except ValueError:
             repo = mr.default_repository().get("id")
             response = mr.create_project(project, repo)
             print(f"A new project named {response.name} was created.")
             return response
     else:
@@ -142,47 +172,47 @@
     Raises
     ------
     ValueError
         Model repository API cannot overwrite an already existing model with the upload model call.
         Alerts user of the force argument to allow multi-call API overwriting.
     """
     project = mr.get_project(project)
-    projectId = project["id"]
-    projectModels = mr.get(f"/projects/{projectId}/models")
+    project_id = project["id"]
+    project_models = mr.get(f"/projects/{project_id}/models")
 
-    for model in projectModels:
+    for model in project_models:
         # Throws a TypeError if only one model is in the project
         try:
             if model["name"] == name:
                 if force:
                     mr.delete_model(model.id)
                 else:
                     raise ValueError(
-                        "A model with the same model name exists in project {}. Include the force=True argument to overwrite models with the same name.".format(
-                            project.name
-                        )
+                        f"A model with the same model name exists in project "
+                        f"{project.name}. Include the force=True argument to overwrite "
+                        f"models with the same name."
                     )
         except TypeError:
-            if projectModels["name"] == name:
+            if project_models["name"] == name:
                 if force:
-                    mr.delete_model(projectModels.id)
+                    mr.delete_model(project_models.id)
                 else:
                     raise ValueError(
-                        "A model with the same model name exists in project {}. Include the force=True argument to overwrite models with the same name.".format(
-                            project.name
-                        )
+                        f"A model with the same model name exists in project "
+                        f"{project.name}. Include the force=True argument to overwrite "
+                        f"models with the same name."
                     )
 
 
 class GitIntegrate:
     @classmethod
-    def pullViyaModel(
+    def pull_viya_model(
         cls,
         model,
-        gPath,
+        git_path,
         project=None,
     ):
         """Send an API request in order to pull a model from a project in
         SAS Model Manager in a zipped format. The contents of the zip file
         include all files found in SAS Model Manager's model UI, except that
         read-only json files are updated to match the current state of the model.
 
@@ -193,221 +223,236 @@
         be supplied as well. Models in the model repository are allowed duplicate
         names, therefore we need a method of parsing the returned models.
 
         Parameters
         ----------
         model : string or RestObj
             A string or JSON response representing the model to be pulled down
-        gPath : string or Path
+        git_path : string or Path
             Base directory of the git repository.
         project : string or RestObj, optional
             A string or JSON response representing the project the model exists in, default is None.
         """
         # Try to pull down the model assuming a UUID or RestObj is provided
         try:
             if isinstance(model, RestObj):
                 model = model.id
             else:
                 UUID(model)
-            projectName = mr.get_model(model).projectName
-            modelName, projectName = getZippedModel(model, gPath, projectName)
-        # If a name is provided instead, use the provided project name or UUID to find the correct model
+            project_name = mr.get_model(model).projectName
+            model_name, project_name = get_zipped_model(model, git_path, project_name)
+        # If a name is provided instead, use the provided project name or UUID to find
+        # the correct model
         except ValueError:
-            projectResponse = mr.get_project(project)
-            if projectResponse is None:
+            project_response = mr.get_project(project)
+            if project_response is None:
                 raise SystemError(
-                    "For models with only a provided name, a project name or UUID must also be supplied."
+                    "For models with only a provided name, a project name or UUID must "
+                    "also be supplied."
                 )
-            projectName = projectResponse["name"]
-            projectId = projectResponse["id"]
-            projectModels = mr.get(f"/projects/{projectId}/models")
-            for model in projectModels:
+            project_name = project_response["name"]
+            project_id = project_response["id"]
+            project_models = mr.get(f"/projects/{project_id}/models")
+            for model in project_models:
                 # Throws a TypeError if only one model is in the project
                 try:
                     if model["name"] == model:
-                        modelId = model.id
-                        modelName, projectName = getZippedModel(
-                            modelId, gPath, projectName
+                        model_id = model.id
+                        model_name, project_name = get_zipped_model(
+                            model_id, git_path, project_name
                         )
                 except TypeError:
-                    if projectModels["name"] == model:
-                        modelId = projectModels.id
-                        modelName, projectName = getZippedModel(
-                            modelId, gPath, projectName
+                    if project_models["name"] == model:
+                        model_id = project_models.id
+                        model_name, project_name = get_zipped_model(
+                            model_id, git_path, project_name
                         )
 
         # Unpack the pulled down zip model and overwrite any duplicate files
-        mPath = Path(gPath) / f"{projectName}/{modelName}"
-        with zipfile.ZipFile(str(mPath / (modelName + ".zip")), mode="r") as zFile:
-            zFile.extractall(str(mPath))
-
-        # Delete the zip model objects in the directory to minimize confusion when uploading back to SAS Model Manager
-        for zipFile in mPath.glob("*.zip"):
-            zipFile.unlink()
+        model_path = Path(git_path) / f"{project_name}/{model_name}"
+        with zipfile.ZipFile(
+            str(model_path / (model_name + ".zip")), mode="r"
+        ) as zFile:
+            zFile.extractall(str(model_path))
+
+        # Delete the zip model objects in the directory to minimize confusion when
+        # uploading back to SAS Model Manager
+        for zip_file in model_path.glob("*.zip"):
+            zip_file.unlink()
 
     @classmethod
-    def pushGitModel(
-        cls, gPath, modelName=None, projectName=None, projectVersion="latest"
+    def push_git_model(
+        cls, git_path, model_name=None, project_name=None, project_version="latest"
     ):
-        """Push a single model in the git repository up to SAS Model Manager. This function
-        creates an archive of all files in the directory and imports the zipped model.
+        """Push a single model in the git repository up to SAS Model Manager. This
+        function creates an archive of all files in the directory and imports the zipped
+        model.
 
         Parameters
         ----------
-        gPath : string or Path
-            Base directory of the git repository or path which includes project and model directories.
-        modelName : string, optional
+        git_path : string or Path
+            Base directory of the git repository or path which includes project and
+            model directories.
+        model_name : string, optional
             Name of model to be imported, by default None
-        projectName : string, optional
+        project_name : string, optional
             Name of project the model is imported from, by default None
-        projectVersion : str, optional
+        project_version : str, optional
             Name of project version to import model in to. Default
             value is "latest".
         """
-        if modelName is None and projectName is None:
-            modelDir = gPath
-            modelName = modelDir.name
-            projectName = modelDir.parent.name
+        if model_name is None and project_name is None:
+            model_dir = git_path
+            model_name = model_dir.name
+            project_name = model_dir.parent.name
         else:
-            modelDir = Path(gPath) / (projectName + "/" + modelName)
-        for zipFile in modelDir.glob("*.zip"):
-            zipFile.unlink()
-        fileNames = []
-        fileNames.extend(sorted(Path(modelDir).glob("*")))
+            model_dir = Path(git_path) / (project_name + "/" + model_name)
+        for zip_file in model_dir.glob("*.zip"):
+            zip_file.unlink()
+        file_names = []
+        file_names.extend(sorted(Path(model_dir).glob("*")))
         with zipfile.ZipFile(
-            str(modelDir / (modelDir.name + ".zip")), mode="w"
+            str(model_dir / (model_dir.name + ".zip")), mode="w"
         ) as zFile:
-            for file in fileNames:
+            for file in file_names:
                 zFile.write(str(file), arcname=file.name)
-        with open(modelDir / (modelDir.name + ".zip"), "rb") as zFile:
-            zipIOFile = io.BytesIO(zFile.read())
-            # Check to see if provided project argument is a valid project on SAS Model Manager
-            projectResponse = mr.get_project(projectName)
-            project = project_exists(projectResponse, projectName)
-            projectName = project.name
-            # Check if model with same name already exists in project. Delete if it exists.
-            model_exists(projectName, modelName, True)
+        with open(model_dir / (model_dir.name + ".zip"), "rb") as zFile:
+            zip_io_file = io.BytesIO(zFile.read())
+            # Check to see if provided project argument is a valid project on SAS Model
+            # Manager
+            project_response = mr.get_project(project_name)
+            project = project_exists(project_response, project_name)
+            project_name = project.name
+            # Check if model with same name already exists in project. Delete if it
+            # exists.
+            model_exists(project_name, model_name, True)
             mr.import_model_from_zip(
-                modelName, projectName, zipIOFile, projectVersion=projectVersion
+                model_name, project_name, zip_io_file, version=project_version
             )
 
     @classmethod
-    def gitRepoPush(cls, gPath, commitMessage, remote="origin", branch="main"):
-        """Create a new commit with new files, then push changes from the local repository to a remote
-        branch. The default remote branch is origin.
+    def git_repo_push(cls, git_path, commit_message, remote="origin", branch="main"):
+        """Create a new commit with new files, then push changes from the local
+        repository to a remote branch. The default remote branch is origin.
 
         Parameters
         ----------
-        gPath : string or Path
+        git_path : string or Path
             Base directory of the git repository.
-        commitMessage : string
+        commit_message : string
             Commit message for the new commit
         remote : str, optional
             Remote name for the remote repository, by default 'origin'
         branch : string
             Branch name for the target pull branch from remote, by default 'main'
         """
-        checkGitStatus()
+        check_git_status()
 
-        repo = Repo(gPath)
+        repo = Repo(git_path)
         repo.git.add(all=True)
-        repo.index.commit(commitMessage)
+        repo.index.commit(commit_message)
         repo.git.push(remote, branch)
 
     @classmethod
-    def gitRepoPull(cls, gPath, remote="origin", branch="main"):
+    def git_repo_pull(cls, git_path, remote="origin", branch="main"):
         """Pull down any changes from a remote branch of the git repository. The default branch is
         origin.
 
         Parameters
         ----------
-        gPath : string or Path
+        git_path : string or Path
             Base directory of the git repository.
         remote : string
             Remote name for the remote repository, by default 'origin'
         branch : string
             Branch name for the target pull branch from remote, by default 'main'
         """
-        checkGitStatus()
+        check_git_status()
 
-        repo = git.Git(gPath)
+        repo = git.Git(git_path)
         repo.pull(remote, branch)
 
     @classmethod
-    def pushGitProject(cls, gPath, project=None):
-        """Using a user provided project name, search for the project in the specified git repository,
-        check if the project already exists on SAS Model Manager (create a new project if it does not),
-        then upload each model found in the git project to SAS Model Manager
+    def push_git_project(cls, git_path, project=None):
+        """Using a user provided project name, search for the project in the specified
+        git repository, check if the project already exists on SAS Model Manager (create
+        a new project if it does not), then upload each model found in the git project
+        to SAS Model Manager
 
         Parameters
         ----------
-        gPath : string or Path
+        git_path : string or Path
             Base directory of the git repository or the project directory.
         project : string or RestObj
             Project name, UUID, or JSON response from SAS Model Manager.
         """
-        # Check to see if provided project argument is a valid project on SAS Model Manager
-        projectResponse = mr.get_project(project)
-        project = project_exists(projectResponse, project)
-        projectName = project.name
+        # Check to see if provided project argument is a valid project on SAS Model
+        # Manager
+        project_response = mr.get_project(project)
+        project = project_exists(project_response, project)
+        project_name = project.name
 
         # Check if project exists in git path and produce an error if it does not
-        pPath = Path(gPath) / projectName
-        if pPath.exists():
-            models = [x for x in pPath.glob("*") if x.is_dir()]
+        project_path = Path(git_path) / project_name
+        if project_path.exists():
+            models = [x for x in project_path.glob("*") if x.is_dir()]
             if len(models) == 0:
-                print(f"No models were found in project {projectName}.")
-            print(f"{len(models)} models were found in project {projectName}.")
+                print(f"No models were found in project {project_name}.")
+            print(f"{len(models)} models were found in project {project_name}.")
         else:
             raise FileNotFoundError(
                 "No directory with the name {} was found in the specified git path.".format(
                     project
                 )
             )
 
         # Loop through paths of models and upload each to SAS Model Manager
         for model in models:
             # Remove any extra zip objects in the directory
-            for zipFile in model.glob("*.zip"):
-                zipFile.unlink()
-            cls.pushGitModel(model)
+            for zip_file in model.glob("*.zip"):
+                zip_file.unlink()
+            cls.push_git_model(model)
 
     @classmethod
-    def pullMMProject(cls, gPath, project):
+    def pull_mm_project(cls, git_path, project):
         """Following the user provided project argument, pull down all models from the
         corresponding SAS Model Manager project into the mapped git directories.
 
         Parameters
         ----------
-        gPath : string or Path
+        git_path : string or Path
             Base directory of the git repository.
         project : string or RestObj
-            The name or id of the model project, or a RestObj representation of the project.
+            The name or id of the model project, or a RestObj representation of the
+            project.
         """
-        # Check to see if provided project argument is a valid project on SAS Model Manager
-        projectResponse = mr.get_project(project)
-        project = project_exists(projectResponse, project)
-        projectName = project.name
+        # Check to see if provided project argument is a valid project on SAS Model
+        # Manager
+        project_response = mr.get_project(project)
+        project = project_exists(project_response, project)
+        project_name = project.name
         # Check if project exists in git path and create it if it does not
-        pPath = Path(gPath) / projectName
-        if not pPath.exists():
-            Path(pPath).mkdir(parents=True, exist_ok=True)
+        project_path = Path(git_path) / project_name
+        if not project_path.exists():
+            Path(project_path).mkdir(parents=True, exist_ok=True)
 
         # Return a list of model names from SAS Model Manager project
-        modelResponse = mr.get(f"projects/{project.id}/models")
-        if modelResponse == []:
+        model_response = mr.get(f"projects/{project.id}/models")
+        if not model_response:
             raise FileNotFoundError(
                 "No models were found in the specified project. A new project folder "
-                + "has been created if it did not already exist within the git repository."
+                "has been created if it did not already exist within the git "
+                "repository."
             )
-        modelNames = []
-        modelId = []
-        for model in modelResponse:
-            modelNames.append(model.name)
-            modelId.append(model.id)
-        # For each model, search for an appropriate model directory in the project directory and pull down the model
-        for name, id in zip(modelNames, modelId):
-            mPath = pPath / name
+        model_names = []
+        model_id = []
+        for model in model_response:
+            model_names.append(model.name)
+            model_id.append(model.id)
+        # For each model, search for an appropriate model directory in the project
+        # directory and pull down the model
+        for name, m_id in zip(model_names, model_id):
+            model_path = project_path / name
             # If the model directory does not exist, create one in the project directory
-            if not mPath.exists():
-                Path(mPath).mkdir(parents=True, exist_ok=True)
-            cls.pullViyaModel(id, mPath.parents[1])
+            if not model_path.exists():
+                Path(model_path).mkdir(parents=True, exist_ok=True)
+            cls.pull_viya_model(m_id, model_path.parents[1])
```

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/import_model.py` & `sasctl-1.9.3/src/sasctl/pzmm/import_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/mlflow_model.py` & `sasctl-1.9.3/src/sasctl/pzmm/mlflow_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/model_parameters.py` & `sasctl-1.9.3/src/sasctl/pzmm/model_parameters.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/pickle_model.py` & `sasctl-1.9.3/src/sasctl/pzmm/pickle_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_fitstat.json` & `sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_fitstat.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_lift.json` & `sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_lift.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/template_files/dmcas_roc.json` & `sasctl-1.9.3/src/sasctl/pzmm/template_files/dmcas_roc.json`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/write_json_files.py` & `sasctl-1.9.3/src/sasctl/pzmm/write_json_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
             var_dict = {"name": name}
             if is_str:
                 var_dict.update(
                     {
                         "level": "nominal",
                         "type": "string",
-                        "length": predict.str.len().max(),
+                        "length": int(predict.str.len().max()),
                     }
                 )
             else:
                 if data_type == "category":
                     var_dict.update({"level": "nominal"})
                 else:
                     var_dict.update({"level": "interval"})
@@ -871,22 +871,22 @@
 
             roc_df = pd.DataFrame(conn.CASTable("ROC", caslib="Public").to_frame())
             roc_dict = cls.apply_dataframe_to_json(json_dict[1]["data"], i, roc_df)
             for j in range(len(roc_dict)):
                 json_dict[1]["data"][j].update(roc_dict[j])
 
             lift_df = pd.DataFrame(conn.CASTable("Lift", caslib="Public").to_frame())
-            lift_dict = cls.apply_dataframe_to_json(json_dict[2]["data"], i, lift_df)
+            lift_dict = cls.apply_dataframe_to_json(json_dict[2]["data"], i, lift_df, 1)
             for j in range(len(lift_dict)):
                 json_dict[2]["data"][j].update(lift_dict[j])
 
         if json_path:
-            for name in [FITSTAT, ROC, LIFT]:
+            for i, name in enumerate([FITSTAT, ROC, LIFT]):
                 with open(Path(json_path) / name, "w") as json_file:
-                    json_file.write(json.dumps(json_dict, indent=4, cls=NpEncoder))
+                    json_file.write(json.dumps(json_dict[i], indent=4, cls=NpEncoder))
                 if cls.notebook_output:
                     print(
                         f"{name} was successfully written and saved to "
                         f"{Path(json_path) / name}"
                     )
         else:
             return {
@@ -1015,38 +1015,48 @@
                 "Please provide the data in a list of lists, dataframe, or numpy array."
             )
 
         return data
 
     @staticmethod
     def apply_dataframe_to_json(
-        json_dict: dict, partition: int, stat_df: DataFrame
+        json_dict: dict, partition: int, stat_df: DataFrame, is_lift: bool = False
     ) -> dict:
         """
         Map the values of the ROC or Lift charts from SAS CAS to the dictionary
         representation of the respective json file.
 
         Parameters
         ----------
         json_dict : dict
             Dictionary representation of the ROC or Lift chart json file.
         partition : int
             Numerical representation of the data partition. Either 0, 1, or 2.
         stat_df : pandas.DataFrame
             ROC or Lift DataFrame generated from the SAS CAS percentile action set.
+        is_lift : bool
+            Specify whether to use logic for Lift or ROC row counting. Default value is
+            False.
 
         Returns
         -------
         json_dict : dict
             Dictionary representation of the ROC or Lift chart json file, with the
             values from the SAS CAS percentile action set added in.
         """
         for row_num in range(len(stat_df)):
             row_dict = stat_df.iloc[row_num].replace(float("nan"), None).to_dict()
-            json_dict[row_num + partition * len(stat_df)]["dataMap"].update(row_dict)
+            if is_lift:
+                json_dict[(row_num + partition + 1) + partition * len(stat_df)][
+                    "dataMap"
+                ].update(row_dict)
+            else:
+                json_dict[row_num + (partition * len(stat_df))]["dataMap"].update(
+                    row_dict
+                )
         return json_dict
 
     # noinspection PyCallingNonCallable, PyNestedDecorators
     @deprecated(
         "Please use the calculate_model_statistics method instead.",
         version="1.9",
         removed_in="1.10",
```

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/write_score_code.py` & `sasctl-1.9.3/src/sasctl/pzmm/write_score_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,19 +503,31 @@
         binary_h2o_model : boolean, optional
             Flag to indicate that the model is a H2O.ai binary model. The default value
             is None.
         """
         pickle_type = pickle_type if pickle_type else "pickle"
 
         if mojo_model:
-            cls.score_code += "model = h2o.import_mojo(Path(settings.pickle_path))\n\n"
-            return f"{'':8}model = h2o.import_mojo(Path(settings.pickle_path))\n\n"
+            cls.score_code += (
+                f"model = h2o.import_mojo(str(Path(settings.pickle_path"
+                f") / {model_file_name}))\n\n"
+            )
+            return (
+                f"{'':8}model = h2o.import_mojo(str(Path(settings.pickle_path) / "
+                f"{model_file_name}))\n\n"
+            )
         elif binary_h2o_model:
-            cls.score_code += "model = h2o.load(Path(settings.pickle_path))\n\n"
-            return f"{'':8}model = h2o.load(Path(settings.pickle_path))\n\n"
+            cls.score_code += (
+                f"model = h2o.load(str(Path(settings.pickle_path) / "
+                f"{model_file_name}))\n\n"
+            )
+            return (
+                f"{'':8}model = h2o.load(str(Path(settings.pickle_path) / "
+                f"{model_file_name}))\n\n"
+            )
         else:
             cls.score_code += (
                 f"with open(Path(settings.pickle_path) / "
                 f'"{model_file_name}", "rb") as pickle_model:\n    '
                 f"model = {pickle_type}.load(pickle_model)\n\n"
             )
             return (
@@ -627,15 +639,15 @@
                 else:
                     col_type = "string"
                 column_types.append(f'"{var}" : "{col_type}"')
             cls.score_code += (
                 f"{'':4}input_array = pd.DataFrame("
                 f"[[{', '.join(var_list)}]],\n{'':31}columns=["
                 f"{column_names}],\n{'':31}dtype=float,\n{'':31}"
-                f"index=[0])\n{'':4}column_types = {{column_types}}\n"
+                f"index=[0])\n{'':4}column_types = {column_types}\n"
                 f"{'':4}h2o_array = h2o.H2OFrame(input_array, "
                 f"column_types=column_types)\n{'':4}prediction = "
                 f"model.{method.__name__}(h2o_array)\n{'':4}prediction"
                 f" = h2o.as_list(prediction, use_pandas=False)\n"
             )
         # Statsmodels models
         elif statsmodels_model:
```

### Comparing `sasctl-1.9.2/src/sasctl/pzmm/zip_model.py` & `sasctl-1.9.3/src/sasctl/pzmm/zip_model.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/services.py` & `sasctl-1.9.3/src/sasctl/services.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/tasks.py` & `sasctl-1.9.3/src/sasctl/tasks.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/astore.py` & `sasctl-1.9.3/src/sasctl/utils/astore.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/cli.py` & `sasctl-1.9.3/src/sasctl/utils/cli.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/decorators.py` & `sasctl-1.9.3/src/sasctl/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/misc.py` & `sasctl-1.9.3/src/sasctl/utils/misc.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/model_migration.py` & `sasctl-1.9.3/src/sasctl/utils/model_migration.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/pymas/core.py` & `sasctl-1.9.3/src/sasctl/utils/pymas/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/pymas/ds2.py` & `sasctl-1.9.3/src/sasctl/utils/pymas/ds2.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/pymas/python.py` & `sasctl-1.9.3/src/sasctl/utils/pymas/python.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/pyml2ds/basic/tree.py` & `sasctl-1.9.3/src/sasctl/utils/pyml2ds/basic/tree.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py` & `sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py` & `sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/lgb.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py` & `sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/pmml.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py` & `sasctl-1.9.3/src/sasctl/utils/pyml2ds/connectors/ensembles/xgb.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl/utils/pyml2ds/core.py` & `sasctl-1.9.3/src/sasctl/utils/pyml2ds/core.py`

 * *Files identical despite different names*

### Comparing `sasctl-1.9.2/src/sasctl.egg-info/PKG-INFO` & `sasctl-1.9.3/src/sasctl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sasctl
-Version: 1.9.2
+Version: 1.9.3
 Summary: SAS Viya Python Client
 Home-page: https://github.com/sassoftware/python-sasctl/
 Author: SAS
 License: Apache v2.0
 Project-URL: Bug Tracker, https://github.com/sassoftware/python-sasctl/issues
 Project-URL: Documentation, https://sassoftware.github.io/python-sasctl/
 Project-URL: Source Code, https://github.com/sassoftware/python-sasctl
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sasctl Version: 1.9.2 Summary: SAS Viya Python
+Metadata-Version: 2.1 Name: sasctl Version: 1.9.3 Summary: SAS Viya Python
 Client Home-page: https://github.com/sassoftware/python-sasctl/ Author: SAS
 License: Apache v2.0 Project-URL: Bug Tracker, https://github.com/sassoftware/
 python-sasctl/issues Project-URL: Documentation, https://sassoftware.github.io/
 python-sasctl/ Project-URL: Source Code, https://github.com/sassoftware/python-
 sasctl Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Environment ::
 Console Classifier: Intended Audience :: Science/Research Classifier: Intended
```

### Comparing `sasctl-1.9.2/src/sasctl.egg-info/SOURCES.txt` & `sasctl-1.9.3/src/sasctl.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 src/sasctl/_services/saslogon.py
 src/sasctl/_services/sentiment_analysis.py
 src/sasctl/_services/service.py
 src/sasctl/_services/text_categorization.py
 src/sasctl/_services/text_parsing.py
 src/sasctl/_services/workflow.py
 src/sasctl/pzmm/__init__.py
-src/sasctl/pzmm/gitIntegration.py
+src/sasctl/pzmm/git_integration.py
 src/sasctl/pzmm/import_model.py
 src/sasctl/pzmm/mlflow_model.py
 src/sasctl/pzmm/model_parameters.py
 src/sasctl/pzmm/pickle_model.py
 src/sasctl/pzmm/write_json_files.py
 src/sasctl/pzmm/write_score_code.py
 src/sasctl/pzmm/zip_model.py
```

