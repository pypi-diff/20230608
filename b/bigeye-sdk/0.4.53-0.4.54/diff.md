# Comparing `tmp/bigeye_sdk-0.4.53.tar.gz` & `tmp/bigeye_sdk-0.4.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigeye_sdk-0.4.53.tar", max compression
+gzip compressed data, was "bigeye_sdk-0.4.54.tar", max compression
```

## Comparing `bigeye_sdk-0.4.53.tar` & `bigeye_sdk-0.4.54.tar`

### file list

```diff
@@ -1,69 +1,68 @@
--rw-r--r--   0        0        0     2092 2023-01-13 19:29:40.987774 bigeye_sdk-0.4.53/LICENSE
--rw-r--r--   0        0        0      873 2022-09-21 14:26:02.564243 bigeye_sdk-0.4.53/README.md
--rw-r--r--   0        0        0     3727 2022-09-21 19:14:17.084238 bigeye_sdk-0.4.53/bigeye_sdk/__init__.py
--rw-r--r--   0        0        0       82 2022-09-21 19:14:17.084343 bigeye_sdk-0.4.53/bigeye_sdk/__version__.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.564505 bigeye_sdk-0.4.53/bigeye_sdk/authentication/__init__.py
--rw-r--r--   0        0        0    17489 2023-03-24 00:17:08.953130 bigeye_sdk-0.4.53/bigeye_sdk/authentication/api_authentication.py
--rw-r--r--   0        0        0     2122 2023-04-21 16:45:36.590395 bigeye_sdk-0.4.53/bigeye_sdk/authentication/credentials.py
--rw-r--r--   0        0        0      734 2022-09-21 14:26:02.564714 bigeye_sdk-0.4.53/bigeye_sdk/authentication/enums.py
--rw-r--r--   0        0        0        0 2022-09-21 19:14:17.084676 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/__init__.py
--rw-r--r--   0        0        0    10264 2023-05-03 14:18:05.249247 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/big_config_reports.py
--rw-r--r--   0        0        0     8116 2023-03-24 00:17:08.953740 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_context.py
--rw-r--r--   0        0        0     1579 2023-03-24 00:17:08.953972 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_functions.py
--rw-r--r--   0        0        0      701 2022-09-21 19:14:17.085326 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_models.py
--rw-r--r--   0        0        0     9206 2023-03-24 00:17:08.954155 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/yaml_model_base.py
--rw-r--r--   0        0        0     3042 2023-03-24 00:17:08.954346 bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.565379 bigeye_sdk-0.4.53/bigeye_sdk/class_ext/__init__.py
--rw-r--r--   0        0        0      233 2022-09-21 14:26:02.565502 bigeye_sdk-0.4.53/bigeye_sdk/class_ext/dataclass_ext.py
--rw-r--r--   0        0        0      402 2022-10-11 14:47:52.093321 bigeye_sdk-0.4.53/bigeye_sdk/class_ext/enum_ext.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.565649 bigeye_sdk-0.4.53/bigeye_sdk/client/__init__.py
--rw-r--r--   0        0        0      389 2022-12-01 16:53:45.901990 bigeye_sdk-0.4.53/bigeye_sdk/client/base_client.py
--rw-r--r--   0        0        0    39770 2023-03-24 00:17:08.954904 bigeye_sdk-0.4.53/bigeye_sdk/client/datawatch_client.py
--rw-r--r--   0        0        0      201 2022-09-21 14:26:02.566284 bigeye_sdk-0.4.53/bigeye_sdk/client/enum.py
--rw-r--r--   0        0        0    38235 2023-04-21 16:45:36.591609 bigeye_sdk-0.4.53/bigeye_sdk/client/generated_datawatch_client.py
--rw-r--r--   0        0        0        0 2022-09-21 19:14:17.086145 bigeye_sdk-0.4.53/bigeye_sdk/controller/__init__.py
--rw-r--r--   0        0        0      390 2022-11-30 18:19:48.731219 bigeye_sdk-0.4.53/bigeye_sdk/controller/metric_controller.py
--rw-r--r--   0        0        0    32795 2023-05-03 14:18:05.249942 bigeye_sdk-0.4.53/bigeye_sdk/controller/metric_suite_controller.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.566925 bigeye_sdk-0.4.53/bigeye_sdk/decorators/__init__.py
--rw-r--r--   0        0        0      307 2022-09-21 19:14:17.086414 bigeye_sdk-0.4.53/bigeye_sdk/decorators/dataclass_decorators.py
--rw-r--r--   0        0        0       97 2022-09-21 14:26:02.567122 bigeye_sdk-0.4.53/bigeye_sdk/exceptions/__init__.py
--rw-r--r--   0        0        0      907 2023-03-24 00:17:08.955789 bigeye_sdk-0.4.53/bigeye_sdk/exceptions/exceptions.py
--rw-r--r--   0        0        0        0 2022-09-21 14:26:02.567221 bigeye_sdk-0.4.53/bigeye_sdk/functions/__init__.py
--rw-r--r--   0        0        0     4469 2023-01-13 19:29:40.988379 bigeye_sdk-0.4.53/bigeye_sdk/functions/athena.py
--rw-r--r--   0        0        0     5202 2022-10-18 15:49:05.166354 bigeye_sdk-0.4.53/bigeye_sdk/functions/aws.py
--rw-r--r--   0        0        0     3343 2023-02-03 22:21:16.752839 bigeye_sdk-0.4.53/bigeye_sdk/functions/bigconfig_functions.py
--rw-r--r--   0        0        0     3469 2022-09-21 14:26:02.567414 bigeye_sdk-0.4.53/bigeye_sdk/functions/casing.py
--rw-r--r--   0        0        0     3215 2022-09-21 19:14:17.086730 bigeye_sdk-0.4.53/bigeye_sdk/functions/core_py_functs.py
--rw-r--r--   0        0        0     4517 2022-11-30 18:19:48.731507 bigeye_sdk-0.4.53/bigeye_sdk/functions/delta_functions.py
--rw-r--r--   0        0        0     2544 2023-03-24 00:17:08.955960 bigeye_sdk-0.4.53/bigeye_sdk/functions/file_functs.py
--rw-r--r--   0        0        0      117 2023-04-21 16:45:36.592265 bigeye_sdk-0.4.53/bigeye_sdk/functions/helpers.py
--rw-r--r--   0        0        0    20235 2023-04-26 20:01:53.246118 bigeye_sdk-0.4.53/bigeye_sdk/functions/metric_functions.py
--rw-r--r--   0        0        0     1554 2022-12-01 16:53:45.902364 bigeye_sdk-0.4.53/bigeye_sdk/functions/metric_run_functions.py
--rw-r--r--   0        0        0     1227 2022-10-11 14:47:52.094658 bigeye_sdk-0.4.53/bigeye_sdk/functions/s3.py
--rw-r--r--   0        0        0     1676 2023-01-13 19:29:40.988609 bigeye_sdk-0.4.53/bigeye_sdk/functions/schema_functions.py
--rw-r--r--   0        0        0     5089 2023-03-24 00:17:08.956184 bigeye_sdk-0.4.53/bigeye_sdk/functions/search_and_match_functions.py
--rw-r--r--   0        0        0     4032 2023-03-24 00:17:08.956445 bigeye_sdk-0.4.53/bigeye_sdk/functions/table_functions.py
--rw-r--r--   0        0        0     1701 2023-04-21 16:45:36.592782 bigeye_sdk-0.4.53/bigeye_sdk/functions/urlfuncts.py
--rw-r--r--   0        0        0        0 2023-05-03 15:16:32.073745 bigeye_sdk-0.4.53/bigeye_sdk/generated/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:16:32.073842 bigeye_sdk-0.4.53/bigeye_sdk/generated/com/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:16:32.073917 bigeye_sdk-0.4.53/bigeye_sdk/generated/com/bigeye/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 15:16:32.073968 bigeye_sdk-0.4.53/bigeye_sdk/generated/com/bigeye/models/__init__.py
--rw-r--r--   0        0        0   206459 2023-05-03 15:16:32.074052 bigeye_sdk-0.4.53/bigeye_sdk/generated/com/bigeye/models/generated.py
--rw-r--r--   0        0        0        0 2023-05-03 15:16:32.074184 bigeye_sdk-0.4.53/bigeye_sdk/generated/google/__init__.py
--rw-r--r--   0        0        0    14816 2023-05-03 15:16:32.074235 bigeye_sdk-0.4.53/bigeye_sdk/generated/google/api.py
--rw-r--r--   0        0        0      507 2022-09-21 14:26:02.569285 bigeye_sdk-0.4.53/bigeye_sdk/log/__init__.py
--rw-r--r--   0        0        0        1 2022-09-21 19:14:17.088368 bigeye_sdk-0.4.53/bigeye_sdk/model/__init__.py
--rw-r--r--   0        0        0      489 2022-09-21 19:14:17.088495 bigeye_sdk-0.4.53/bigeye_sdk/model/base_datawatch_facade.py
--rw-r--r--   0        0        0    22303 2023-03-24 00:17:08.956794 bigeye_sdk-0.4.53/bigeye_sdk/model/big_config.py
--rw-r--r--   0        0        0      778 2023-02-23 17:53:03.561875 bigeye_sdk-0.4.53/bigeye_sdk/model/collection_models.py
--rw-r--r--   0        0        0     3948 2023-05-03 14:18:05.251140 bigeye_sdk-0.4.53/bigeye_sdk/model/dbt_schema.py
--rw-r--r--   0        0        0     3504 2023-03-24 00:17:08.957102 bigeye_sdk-0.4.53/bigeye_sdk/model/delta_facade.py
--rw-r--r--   0        0        0     9456 2023-01-13 19:29:40.989263 bigeye_sdk-0.4.53/bigeye_sdk/model/metric_facade.py
--rw-r--r--   0        0        0     8396 2023-04-21 16:45:36.594969 bigeye_sdk-0.4.53/bigeye_sdk/model/protobuf_enum_facade.py
--rw-r--r--   0        0        0      220 2022-11-30 18:19:48.733054 bigeye_sdk-0.4.53/bigeye_sdk/model/protobuf_extensions.py
--rw-r--r--   0        0        0    45112 2023-04-25 19:45:34.950560 bigeye_sdk-0.4.53/bigeye_sdk/model/protobuf_message_facade.py
--rw-r--r--   0        0        0      865 2023-02-22 23:48:15.904646 bigeye_sdk-0.4.53/bigeye_sdk/model/sla_models.py
--rw-r--r--   0        0        0     7114 2023-04-20 17:39:55.335256 bigeye_sdk-0.4.53/bigeye_sdk/serializable.py
--rw-r--r--   0        0        0     3709 2023-05-03 14:18:05.251555 bigeye_sdk-0.4.53/pyproject.toml
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.53/setup.py
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.53/PKG-INFO
+-rw-r--r--   0        0        0     2092 2023-01-13 19:29:40.987774 bigeye_sdk-0.4.54/LICENSE
+-rw-r--r--   0        0        0      873 2022-09-21 14:26:02.564243 bigeye_sdk-0.4.54/README.md
+-rw-r--r--   0        0        0     3727 2022-09-21 19:14:17.084238 bigeye_sdk-0.4.54/bigeye_sdk/__init__.py
+-rw-r--r--   0        0        0       82 2022-09-21 19:14:17.084343 bigeye_sdk-0.4.54/bigeye_sdk/__version__.py
+-rw-r--r--   0        0        0        0 2022-09-21 14:26:02.564505 bigeye_sdk-0.4.54/bigeye_sdk/authentication/__init__.py
+-rw-r--r--   0        0        0    17489 2023-06-08 16:16:24.658685 bigeye_sdk-0.4.54/bigeye_sdk/authentication/api_authentication.py
+-rw-r--r--   0        0        0     2009 2023-06-08 16:16:18.009998 bigeye_sdk-0.4.54/bigeye_sdk/authentication/credentials.py
+-rw-r--r--   0        0        0      734 2022-09-21 14:26:02.564714 bigeye_sdk-0.4.54/bigeye_sdk/authentication/enums.py
+-rw-r--r--   0        0        0        0 2022-09-21 19:14:17.084676 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/__init__.py
+-rw-r--r--   0        0        0    10264 2023-06-08 16:16:24.658832 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/big_config_reports.py
+-rw-r--r--   0        0        0     8116 2023-06-08 16:16:24.658990 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_context.py
+-rw-r--r--   0        0        0     1579 2023-06-08 16:16:24.659119 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_functions.py
+-rw-r--r--   0        0        0      701 2022-09-21 19:14:17.085326 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_models.py
+-rw-r--r--   0        0        0     9206 2023-06-08 16:16:24.659227 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/yaml_model_base.py
+-rw-r--r--   0        0        0     3042 2023-06-08 16:16:24.659331 bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py
+-rw-r--r--   0        0        0        0 2022-09-21 14:26:02.565379 bigeye_sdk-0.4.54/bigeye_sdk/class_ext/__init__.py
+-rw-r--r--   0        0        0      233 2022-09-21 14:26:02.565502 bigeye_sdk-0.4.54/bigeye_sdk/class_ext/dataclass_ext.py
+-rw-r--r--   0        0        0      402 2022-10-11 14:47:52.093321 bigeye_sdk-0.4.54/bigeye_sdk/class_ext/enum_ext.py
+-rw-r--r--   0        0        0        0 2022-09-21 14:26:02.565649 bigeye_sdk-0.4.54/bigeye_sdk/client/__init__.py
+-rw-r--r--   0        0        0      389 2022-12-01 16:53:45.901990 bigeye_sdk-0.4.54/bigeye_sdk/client/base_client.py
+-rw-r--r--   0        0        0    39770 2023-06-08 16:16:24.659558 bigeye_sdk-0.4.54/bigeye_sdk/client/datawatch_client.py
+-rw-r--r--   0        0        0      201 2022-09-21 14:26:02.566284 bigeye_sdk-0.4.54/bigeye_sdk/client/enum.py
+-rw-r--r--   0        0        0    38235 2023-06-08 16:16:24.659795 bigeye_sdk-0.4.54/bigeye_sdk/client/generated_datawatch_client.py
+-rw-r--r--   0        0        0        0 2022-09-21 19:14:17.086145 bigeye_sdk-0.4.54/bigeye_sdk/controller/__init__.py
+-rw-r--r--   0        0        0      390 2022-11-30 18:19:48.731219 bigeye_sdk-0.4.54/bigeye_sdk/controller/metric_controller.py
+-rw-r--r--   0        0        0    32893 2023-06-08 16:16:24.660068 bigeye_sdk-0.4.54/bigeye_sdk/controller/metric_suite_controller.py
+-rw-r--r--   0        0        0        0 2022-09-21 14:26:02.566925 bigeye_sdk-0.4.54/bigeye_sdk/decorators/__init__.py
+-rw-r--r--   0        0        0      307 2022-09-21 19:14:17.086414 bigeye_sdk-0.4.54/bigeye_sdk/decorators/dataclass_decorators.py
+-rw-r--r--   0        0        0       97 2022-09-21 14:26:02.567122 bigeye_sdk-0.4.54/bigeye_sdk/exceptions/__init__.py
+-rw-r--r--   0        0        0     1018 2023-06-08 16:16:24.660218 bigeye_sdk-0.4.54/bigeye_sdk/exceptions/exceptions.py
+-rw-r--r--   0        0        0        0 2022-09-21 14:26:02.567221 bigeye_sdk-0.4.54/bigeye_sdk/functions/__init__.py
+-rw-r--r--   0        0        0     4469 2023-01-13 19:29:40.988379 bigeye_sdk-0.4.54/bigeye_sdk/functions/athena.py
+-rw-r--r--   0        0        0     5202 2022-10-18 15:49:05.166354 bigeye_sdk-0.4.54/bigeye_sdk/functions/aws.py
+-rw-r--r--   0        0        0     3343 2023-02-03 22:21:16.752839 bigeye_sdk-0.4.54/bigeye_sdk/functions/bigconfig_functions.py
+-rw-r--r--   0        0        0     3469 2022-09-21 14:26:02.567414 bigeye_sdk-0.4.54/bigeye_sdk/functions/casing.py
+-rw-r--r--   0        0        0     3215 2022-09-21 19:14:17.086730 bigeye_sdk-0.4.54/bigeye_sdk/functions/core_py_functs.py
+-rw-r--r--   0        0        0     4517 2022-11-30 18:19:48.731507 bigeye_sdk-0.4.54/bigeye_sdk/functions/delta_functions.py
+-rw-r--r--   0        0        0     2544 2023-06-08 16:16:24.660379 bigeye_sdk-0.4.54/bigeye_sdk/functions/file_functs.py
+-rw-r--r--   0        0        0      117 2023-06-08 16:16:24.660510 bigeye_sdk-0.4.54/bigeye_sdk/functions/helpers.py
+-rw-r--r--   0        0        0    20235 2023-06-08 16:16:24.660721 bigeye_sdk-0.4.54/bigeye_sdk/functions/metric_functions.py
+-rw-r--r--   0        0        0     1554 2023-06-08 16:16:18.012698 bigeye_sdk-0.4.54/bigeye_sdk/functions/metric_run_functions.py
+-rw-r--r--   0        0        0     1227 2022-10-11 14:47:52.094658 bigeye_sdk-0.4.54/bigeye_sdk/functions/s3.py
+-rw-r--r--   0        0        0     1676 2023-01-13 19:29:40.988609 bigeye_sdk-0.4.54/bigeye_sdk/functions/schema_functions.py
+-rw-r--r--   0        0        0     5089 2023-06-08 16:16:24.660877 bigeye_sdk-0.4.54/bigeye_sdk/functions/search_and_match_functions.py
+-rw-r--r--   0        0        0     4032 2023-06-08 16:16:24.661012 bigeye_sdk-0.4.54/bigeye_sdk/functions/table_functions.py
+-rw-r--r--   0        0        0     1701 2023-06-08 16:16:24.661143 bigeye_sdk-0.4.54/bigeye_sdk/functions/urlfuncts.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:07:54.354138 bigeye_sdk-0.4.54/bigeye_sdk/generated/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:07:54.354225 bigeye_sdk-0.4.54/bigeye_sdk/generated/com/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:07:54.354300 bigeye_sdk-0.4.54/bigeye_sdk/generated/com/bigeye/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:07:54.354356 bigeye_sdk-0.4.54/bigeye_sdk/generated/com/bigeye/models/__init__.py
+-rw-r--r--   0        0        0   213399 2023-06-08 16:16:24.661924 bigeye_sdk-0.4.54/bigeye_sdk/generated/com/bigeye/models/generated.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:07:54.354553 bigeye_sdk-0.4.54/bigeye_sdk/generated/google/__init__.py
+-rw-r--r--   0        0        0    14816 2023-06-08 15:07:54.354602 bigeye_sdk-0.4.54/bigeye_sdk/generated/google/api.py
+-rw-r--r--   0        0        0      507 2022-09-21 14:26:02.569285 bigeye_sdk-0.4.54/bigeye_sdk/log/__init__.py
+-rw-r--r--   0        0        0        1 2022-09-21 19:14:17.088368 bigeye_sdk-0.4.54/bigeye_sdk/model/__init__.py
+-rw-r--r--   0        0        0      489 2022-09-21 19:14:17.088495 bigeye_sdk-0.4.54/bigeye_sdk/model/base_datawatch_facade.py
+-rw-r--r--   0        0        0    22303 2023-06-08 16:16:24.662241 bigeye_sdk-0.4.54/bigeye_sdk/model/big_config.py
+-rw-r--r--   0        0        0      778 2023-02-23 17:53:03.561875 bigeye_sdk-0.4.54/bigeye_sdk/model/collection_models.py
+-rw-r--r--   0        0        0     3948 2023-06-08 16:16:24.662434 bigeye_sdk-0.4.54/bigeye_sdk/model/dbt_schema.py
+-rw-r--r--   0        0        0     3504 2023-06-08 16:16:24.662568 bigeye_sdk-0.4.54/bigeye_sdk/model/delta_facade.py
+-rw-r--r--   0        0        0     9456 2023-01-13 19:29:40.989263 bigeye_sdk-0.4.54/bigeye_sdk/model/metric_facade.py
+-rw-r--r--   0        0        0     8396 2023-06-08 16:16:24.662714 bigeye_sdk-0.4.54/bigeye_sdk/model/protobuf_enum_facade.py
+-rw-r--r--   0        0        0      220 2022-11-30 18:19:48.733054 bigeye_sdk-0.4.54/bigeye_sdk/model/protobuf_extensions.py
+-rw-r--r--   0        0        0    44904 2023-06-08 16:16:24.662961 bigeye_sdk-0.4.54/bigeye_sdk/model/protobuf_message_facade.py
+-rw-r--r--   0        0        0      865 2023-02-22 23:48:15.904646 bigeye_sdk-0.4.54/bigeye_sdk/model/sla_models.py
+-rw-r--r--   0        0        0     7114 2023-06-08 16:16:24.663118 bigeye_sdk-0.4.54/bigeye_sdk/serializable.py
+-rw-r--r--   0        0        0     3709 2023-06-08 16:16:24.664385 bigeye_sdk-0.4.54/pyproject.toml
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 bigeye_sdk-0.4.54/PKG-INFO
```

### Comparing `bigeye_sdk-0.4.53/LICENSE` & `bigeye_sdk-0.4.54/LICENSE`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/README.md` & `bigeye_sdk-0.4.54/README.md`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/__init__.py` & `bigeye_sdk-0.4.54/bigeye_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/authentication/api_authentication.py` & `bigeye_sdk-0.4.54/bigeye_sdk/authentication/api_authentication.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/authentication/credentials.py` & `bigeye_sdk-0.4.54/bigeye_sdk/authentication/credentials.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,41 +4,40 @@
 import json
 from dataclasses import dataclass
 from typing import TypeVar
 
 from bigeye_sdk.functions.aws import get_secret
 
 from bigeye_sdk.log import get_logger
-from bigeye_sdk.serializable import PydanticSubtypeSerializable
 
 log = get_logger(__file__)
 
 
-class Credential(abc.ABC, PydanticSubtypeSerializable):
+class Credential(abc.ABC):
     pass
 
 
 CREDENTIAL = TypeVar('CREDENTIAL', bound='Credential')
 
 
 class LocalFileCredential(Credential):
 
     @classmethod
     def load_from_file(cls, file: str) -> CREDENTIAL:
         log.info(f'Loading API Conf: {file}')
         with open(file) as fin:
-            return cls.parse_obj(**json.load(fin))
+            return cls(**json.load(fin))
 
 
 class AwsSecretCredential(Credential):
 
     @classmethod
     def load_from_aws_secret(cls, secret_name: str, region_name: str = 'us-west-2') -> CREDENTIAL:
         log.info(f'Loading Secret: {secret_name}')
-        return cls.parse_obj(**get_secret(region_name=region_name, secret_name=secret_name))
+        return cls(**get_secret(region_name=region_name, secret_name=secret_name))
 
 
 class LoadableCredential(LocalFileCredential, AwsSecretCredential):
     pass
 
 
 class DatabaseCredential(LoadableCredential):
```

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/authentication/enums.py` & `bigeye_sdk-0.4.54/bigeye_sdk/authentication/enums.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/big_config_reports.py` & `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/big_config_reports.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_context.py` & `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_context.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_functions.py` & `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/validation_models.py` & `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/validation_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/yaml_model_base.py` & `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/yaml_model_base.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py` & `bigeye_sdk-0.4.54/bigeye_sdk/bigconfig_validation/yaml_validation_error_messages.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/client/datawatch_client.py` & `bigeye_sdk-0.4.54/bigeye_sdk/client/datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/client/generated_datawatch_client.py` & `bigeye_sdk-0.4.54/bigeye_sdk/client/generated_datawatch_client.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/controller/metric_suite_controller.py` & `bigeye_sdk-0.4.54/bigeye_sdk/controller/metric_suite_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from bigeye_sdk.bigconfig_validation.big_config_reports import raise_files_contain_error_exception, MetricSuiteReport, \
     process_reports, ProcessStage
 from bigeye_sdk.bigconfig_validation.validation_context import process_validation_errors, \
     get_validation_error_cnt, get_all_validation_errors_flat
 from bigeye_sdk.bigconfig_validation.yaml_validation_error_messages import SRC_NOT_EXISTS_FOR_DEPLOYMENT_ERRMSG, \
     METRIC_APPLICATION_ERROR, MISMATCHED_ATTRIBUTE_ACROSS_MULTIPLE_FILES
 from bigeye_sdk.client.datawatch_client import DatawatchClient
-from bigeye_sdk.exceptions.exceptions import FileLoadException, BigConfigValidationException, NoSourcesFoundException
+from bigeye_sdk.exceptions.exceptions import FileLoadException, BigConfigValidationException, NoSourcesFoundException, FileNotFoundException
 from bigeye_sdk.functions.metric_functions import _is_table_level_metric
 from bigeye_sdk.functions.search_and_match_functions import wildcard_search
 from bigeye_sdk.generated.com.bigeye.models.generated import Source, CohortDefinition, \
     MetricSuite, CohortAndMetricDefinition, CatalogEntityType, MetricDefinition, FieldType, NamedSchedule
 from bigeye_sdk.log import get_logger
 from bigeye_sdk.model.big_config import BigConfig, RowCreationTimes, TagDeployment, TableDeployment, \
     SavedMetricDefinitions
@@ -41,35 +41,35 @@
 
     if not source_name:
         return r
     else:
         return f'{source_name}.{r}'
 
 
-def _find_bigconfig_files(source_paths: List[str] = [], recursive: bool = False) -> List[BIGCONFIG_FILE]:
+def _find_bigconfig_files(input_paths: List[str] = [], recursive: bool = False) -> List[BIGCONFIG_FILE]:
     """
-    Finds bigconfig files either in specified source path or in working directory
+    Finds bigconfig files either in specified input path or in working directory
     Args:
-        source_paths: specify List of source paths or working directory will be used.
+        input_paths: specify List of input paths or working directory will be used.
 
     Returns: None
 
     """
     files: List[Path] = []
-    for sp in source_paths:
-        if os.path.isfile(sp):
-            files.append(Path(sp))
+    for ip in input_paths:
+        if os.path.isfile(ip):
+            files.append(Path(ip))
         elif recursive:
-            files.extend(list(Path(sp).rglob('*.y*ml')))
+            files.extend(list(Path(ip).rglob('*.y*ml')))
         else:
-            files.extend(list(Path(sp).glob('*.y*ml')))
+            files.extend(list(Path(ip).glob('*.y*ml')))
 
     if not files:
-        """Assumes driver run in directory containing Bigconfig YAML."""
-        files = list(Path.cwd().rglob('*.y*ml')) if recursive else list(Path.cwd().glob('*.y*ml'))
+        """No YAML files were found at the given input path or current working directory, raise error for user to fix input paths."""
+        raise FileNotFoundException(f'No YAML files for the given input paths or current working directory were found.')
 
     bigeye_files: List[BIGCONFIG_FILE] = []
     file: BIGCONFIG_FILE
     for file in files:
         try:
             """Loading Bigconfig YAML.  If file is not of Bigconfig type then the error will be caught and passed."""
             bigeye_files.append(File.load(str(file)))
@@ -113,15 +113,15 @@
         merged_or_new: SimpleCollection
         deployment_collections = []
 
         for collection in bigconfig.get_collections():
             if collection.name in existing_collections.keys():
                 """If the collection exists, send the collection ID as part of a plan and only update for apply"""
                 existing = SimpleCollection.from_datawatch_object(existing_collections[collection.name])
-                merged_or_new = collection.merge_for_upsert(existing=existing, overwrite=overwrite)
+                merged_or_new = collection.merge_for_upsert(existing=existing)
                 deployment_collections.append(merged_or_new)
                 if apply:
                     self.client.update_collection(collection=merged_or_new.to_datawatch_object())
             elif apply:
                 """If it doesn't exist, only create it during apply"""
                 c = collection.to_datawatch_object()
                 c = self.client.create_collection(
@@ -543,15 +543,15 @@
             apply: If true then Big Config will be applied to the workspace.  If false then a plan will be generated.
             no_queue: If true, the bigconfig will be run without queuing
             recursive: If true, search for files recursively
             strict_mode: If true errors from the API raise an exception.
         Returns: None
 
         """
-        files: List[BIGCONFIG_FILE] = _find_bigconfig_files(input_path, recursive=recursive)
+        files: List[BIGCONFIG_FILE] = _find_bigconfig_files(input_paths=input_path, recursive=recursive)
 
         bigconfig: BigConfig = combine_bigconfigs(files)
 
         if get_validation_error_cnt():
             """Processing validation errors if any exist and throw exception."""
             fixme_file_list = process_validation_errors(output_path)
             unmatched_validations_errors = get_all_validation_errors_flat(only_unmatched=True)
@@ -571,17 +571,17 @@
             fixme_file_list = process_validation_errors(output_path)
             unmatched_validations_errors = get_all_validation_errors_flat(only_unmatched=True)
             raise_files_contain_error_exception(validation_error_cnt=get_validation_error_cnt(),
                                                 unmatched_validations_errors=unmatched_validations_errors,
                                                 fixme_file_list=fixme_file_list)
 
         # Applies changes and overwrites once local validations have passed.
-        if apply:
-            self._upsert_collections(bigconfig=bigconfig, overwrite=True,
-                                     apply=apply)  # Will always overwrite for Bigconfig.
+        # if apply:
+        #     self._upsert_collections(bigconfig=bigconfig, overwrite=True,
+        #                              apply=apply)  # Will always overwrite for Bigconfig.
 
         for metric_suite in metric_suites:
             j = metric_suite.to_json()
             if not apply or no_queue:
                 response = self.client.post_metric_suite(metric_suite=metric_suite, apply=apply)
             else:
                 response = self.client.post_metric_suite_queue(metric_suite=metric_suite)
```

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/exceptions/exceptions.py` & `bigeye_sdk-0.4.54/bigeye_sdk/exceptions/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 class FileLoadException(Exception):
     def __init__(self, message: str):
         self.message = message
 
 
+class FileNotFoundException(Exception):
+    def __init__(self, message: str):
+        self.message = message
+
+
 class AttributeTypeException(Exception):
     def __init__(self, message: str):
         self.message = message
 
 
 class InvalidConfigurationException(Exception):
     def __init__(self, message: str):
```

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/athena.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/athena.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/aws.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/aws.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/bigconfig_functions.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/bigconfig_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/casing.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/casing.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/core_py_functs.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/core_py_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/delta_functions.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/delta_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/file_functs.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/file_functs.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/metric_functions.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/metric_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/metric_run_functions.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/metric_run_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/s3.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/s3.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/schema_functions.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/schema_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/search_and_match_functions.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/search_and_match_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/table_functions.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/table_functions.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/functions/urlfuncts.py` & `bigeye_sdk-0.4.54/bigeye_sdk/functions/urlfuncts.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/generated/com/bigeye/models/generated.py` & `bigeye_sdk-0.4.54/bigeye_sdk/generated/com/bigeye/models/generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
     DATABASE_TYPE_REDSHIFT = 8
     DATABASE_TYPE_SAP_HANA = 9
     DATABASE_TYPE_SNOWFLAKE = 10
     DATABASE_TYPE_SQL_SERVER = 11
     DATABASE_TYPE_SYNAPSE = 12
     DATABASE_TYPE_ROCKSET = 13
     DATABASE_TYPE_VERTICA = 14
+    DATABASE_TYPE_AVATICA = 15
 
 
 class ConfigValueType(betterproto.Enum):
     VALUE_TYPE_UNSPECIFIED = 0
     VALUE_TYPE_STRING = 1
     VALUE_TYPE_BOOL = 2
     VALUE_TYPE_INTEGER = 3
@@ -213,14 +214,19 @@
     MIN_AGGREGATION_TYPE = 3
     MAX_AGGREGATION_TYPE = 4
     AVG_AGGREGATION_TYPE = 5
     SUM_AGGREGATION_TYPE = 6
 
 
 class MetricCategory(betterproto.Enum):
+    """
+    Note: The enum order is also the sorting order when sorting issues by
+    metric category
+    """
+
     METRIC_CATEGORY_UNSPECIFIED = 0
     METRIC_CATEGORY_PIPELINE_RELIABILITY = 1
     METRIC_CATEGORY_UNIQUENESS = 2
     METRIC_CATEGORY_COMPLETENESS = 3
     METRIC_CATEGORY_DISTRIBUTIONS = 4
     METRIC_CATEGORY_VALIDITY = 5
     METRIC_CATEGORY_CUSTOM = 6
@@ -258,14 +264,15 @@
     COLLECTION_SORT_FIELD_ISSUE_COUNT = 2
     COLLECTION_SORT_FIELD_METRIC_COUNT = 3
     COLLECTION_SORT_FIELD_UPDATED_AT = 4
     COLLECTION_SORT_FIELD_NAME = 5
 
 
 class MetricRunStatus(betterproto.Enum):
+    # deprecated in favor of MetricStatus
     METRIC_RUN_STATUS_UNSPECIFIED = 0
     METRIC_RUN_STATUS_UPPERBOUND_CRITICAL = 1
     METRIC_RUN_STATUS_LOWERBOUND_CRITICAL = 2
     METRIC_RUN_STATUS_OK = 3
     # METRIC_RUN_STATUS_GROUPS_CRITICAL is not a valid value for MetricRun.status
     # (it only applies to MetricInfo.status)
     METRIC_RUN_STATUS_GROUPS_CRITICAL = 4
@@ -400,14 +407,18 @@
     GROUP_BY_ENTITY_TYPE_TABLE = 3
     GROUP_BY_ENTITY_TYPE_COLUMN = 4
     GROUP_BY_ENTITY_TYPE_SLA = 5
     GROUP_BY_ENTITY_TYPE_SCHEMA_ID = 6
     GROUP_BY_ENTITY_TYPE_METRIC_RUN_LABEL = 7
     GROUP_BY_ENTITY_TYPE_TABLE_ID = 8
     GROUP_BY_ENTITY_TYPE_ISSUE_PRIORITY = 9
+    GROUP_BY_ENTITY_TYPE_ISSUE_STATUS = 10
+    GROUP_BY_ENTITY_TYPE_METRIC_STATUS = 11
+    GROUP_BY_ENTITY_TYPE_METRIC_TYPE = 12
+    GROUP_BY_ENTITY_TYPE_METRIC_CATEGORY = 13
 
 
 class IssueStatus(betterproto.Enum):
     ISSUE_STATUS_UNSPECIFIED = 0
     ISSUE_STATUS_NEW = 1
     ISSUE_STATUS_ACKNOWLEDGED = 2
     ISSUE_STATUS_CLOSED = 3
@@ -428,14 +439,16 @@
     ISSUE_SORT_FIELD_CLOSED_AT = 3
     ISSUE_SORT_FIELD_NEW_COUNT = 4
     ISSUE_SORT_FIELD_ACKNOWLEDGED_COUNT = 5
     ISSUE_SORT_FIELD_CLOSED_COUNT = 6
     ISSUE_SORT_FIELD_TABLE_NAME = 7
     ISSUE_SORT_FIELD_SCHEMA_NAME = 8
     ISSUE_SORT_FIELD_MONITORING_COUNT = 9
+    ISSUE_SORT_FIELD_STATUS = 10
+    ISSUE_SORT_FIELD_METRIC_CATEGORY = 11
 
 
 class MetricSortField(betterproto.Enum):
     METRIC_SORT_FIELD_UNSPECIFIED = 0
     METRIC_SORT_FIELD_METRIC_NAME = 1
     METRIC_SORT_FIELD_RAN_AT = 2
     METRIC_SORT_FIELD_ALERTING = 3
@@ -446,14 +459,15 @@
 
 
 class MetricStatus(betterproto.Enum):
     METRIC_STATUS_UNSPECIFIED = 0
     METRIC_STATUS_ALERTING = 1
     METRIC_STATUS_FAILED = 2
     METRIC_STATUS_HEALTHY = 3
+    METRIC_STATUS_NO_OBSERVED_VALUE = 4
 
 
 class CacheOperation(betterproto.Enum):
     CACHE_OPERATION_UNSPECIFIED = 0
     CACHE_OPERATION_CLEAR_CONFIG = 1
     CACHE_OPERATION_CLEAR_USERS = 2
     CACHE_OPERATION_CLEAR_KEYS = 3
@@ -554,14 +568,15 @@
     WORKFLOW_PROCESSING_TYPE_METADATA_METRICS = 5
     WORKFLOW_PROCESSING_TYPE_GENERATE_AUTOMETRICS = 6
     WORKFLOW_PROCESSING_TYPE_GENERATE_POP_SCORES = 7
     WORKFLOW_PROCESSING_TYPE_CATALOG_INDEX_INTEGRATION = 8
     WORKFLOW_PROCESSING_TYPE_APPLY_BIGCONFIG = 9
     WORKFLOW_PROCESSING_TYPE_RUN_DELTA = 10
     WORKFLOW_PROCESSING_TYPE_RUN_COMPARISON_TABLE = 11
+    WORKFLOW_PROCESSING_TYPE_RUN_METRIC_BATCH = 12
 
 
 class CatalogIndexOperationType(betterproto.Enum):
     CATALOG_INDEX_OPERATION_TYPE_UNSPECIFIED = 0
     CATALOG_INDEX_OPERATION_TYPE_ADD = 1
     CATALOG_INDEX_OPERATION_TYPE_UPDATE = 2
     CATALOG_INDEX_OPERATION_TYPE_DELETE = 3
@@ -589,17 +604,49 @@
     REVISION_TYPE_UNSPECIFIED = 0
     REVISION_TYPE_CREATE = 1
     REVISION_TYPE_UPDATE = 2
     REVISION_TYPE_DELETE = 3
 
 
 class DashboardDataPointType(betterproto.Enum):
-    NUMBER_OPEN_ISSUES = 0
-    AVERAGE_ISSUE_TIME_TO_ACTION = 1
-    AVERAGE_ISSUE_TIME_TO_CLOSE = 2
+    DASHBOARD_DATA_POINT_TYPE_UNSPECIFIED = 0
+    DASHBOARD_DATA_POINT_TYPE_NUMBER_OPEN_ISSUES = 1
+    DASHBOARD_DATA_POINT_TYPE_AVERAGE_ISSUE_TIME_TO_ACTION = 2
+    DASHBOARD_DATA_POINT_TYPE_AVERAGE_ISSUE_TIME_TO_CLOSE = 3
+    DASHBOARD_DATA_POINT_TYPE_NUMBER_OPEN_ISSUES_BY_COLLECTION = 4
+    DASHBOARD_DATA_POINT_TYPE_NUMBER_METRICS_BY_COLLECTION = 5
+    DASHBOARD_DATA_POINT_TYPE_NUMBER_ISSUES_CLOSED_BY_USER = 6
+    DASHBOARD_DATA_POINT_TYPE_NUMBER_BILLABLE_TABLES = 7
+    DASHBOARD_DATA_POINT_TYPE_NUMBER_ISSUES_CLOSED = 8
+    DASHBOARD_DATA_POINT_TYPE_TOTAL_HOURS_TO_CLOSE = 9
+    DASHBOARD_DATA_POINT_TYPE_NUMBER_METRICS_WITH_ISSUE_BY_CATEGORY = 10
+    DASHBOARD_DATA_POINT_TYPE_NUMBER_METRICS_BY_CATEGORY = 11
+    DASHBOARD_DATA_POINT_TYPE_PCT_METRICS_WO_ISSUE_BY_CATEGORY = 12
+    DASHBOARD_DATA_POINT_TYPE_TOTAL_TABLES = 13
+    DASHBOARD_DATA_POINT_TYPE_TOTAL_TABLES_WITH_METRICS = 14
+    DASHBOARD_DATA_POINT_TYPE_PCT_TABLES_WITH_METRICS = 15
+    DASHBOARD_DATA_POINT_TYPE_TOTAL_TABLES_WITH_METRICS_BY_CATEGORY = 16
+    DASHBOARD_DATA_POINT_TYPE_PCT_TABLES_WITH_METRICS_BY_CATEGORY = 17
+    DASHBOARD_DATA_POINT_TYPE_TOTAL_TABLES_WITH_ISSUE_BY_CATEGORY = 18
+    DASHBOARD_DATA_POINT_TYPE_NUMBER_ISSUES_INTERACTED = 19
+    DASHBOARD_DATA_POINT_TYPE_NUMBER_ISSUES_OPENED = 20
+    DASHBOARD_DATA_POINT_TYPE_PCT_ISSUES_INTERACTED = 21
+    DASHBOARD_DATA_POINT_TYPE_PCT_TABLES_WITHOUT_ISSUE_BY_CATEGORY = 22
+
+
+class GroupUserOperation(betterproto.Enum):
+    GROUP_USER_OPERATION_UNSPECIFIED = 0
+    GROUP_USER_OPERATION_ADD = 1
+    GROUP_USER_OPERATION_REMOVE = 2
+
+
+class RoleOperation(betterproto.Enum):
+    ROLE_OPERATION_UNSPECIFIED = 0
+    ROLE_OPERATION_GRANT = 1
+    ROLE_OPERATION_REVOKE = 2
 
 
 class ModelTypes(betterproto.Enum):
     MODEL_TYPE_UNDEFINED = 0
     MODEL_TYPE_MONOCLE = 1
 
 
@@ -639,22 +686,39 @@
     hmac: str = betterproto.string_field(7)
     company_id: int = betterproto.int32_field(8)
     company_name: str = betterproto.string_field(9)
     company_uuid: str = betterproto.string_field(10)
     id: int = betterproto.int32_field(11)
     advanced_configs: List["ConfigValue"] = betterproto.message_field(12)
     tos_accepted_epoch_seconds: int = betterproto.int64_field(13)
+    is_v2_admin: bool = betterproto.bool_field(14)
+    workspaces: List["WorkspaceIdNameAndRole"] = betterproto.message_field(15)
+
+
+@dataclass
+class WorkspaceIdNameAndRole(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    name: str = betterproto.string_field(2)
+    role_name: str = betterproto.string_field(3)
 
 
 @dataclass
 class User(betterproto.Message):
     id: int = betterproto.int32_field(1)
     name: str = betterproto.string_field(2)
     email: str = betterproto.string_field(3)
     role: "Role" = betterproto.enum_field(4)
+    groups: List["IdAndDisplayName"] = betterproto.message_field(5)
+
+
+@dataclass
+class UserInviteRequest(betterproto.Message):
+    name: str = betterproto.string_field(1)
+    email: str = betterproto.string_field(2)
+    group_ids: List[int] = betterproto.int32_field(3)
 
 
 @dataclass
 class CompanyInfo(betterproto.Message):
     needs_admin: bool = betterproto.bool_field(1)
 
 
@@ -870,14 +934,21 @@
 class BatchRunMetricsRequest(betterproto.Message):
     # IDs of the metrics to be run -- only metrics with the same dataset, grain
     # size, groups, and lookback type can be run as a batch
     metric_ids: List[int] = betterproto.int32_field(1)
 
 
 @dataclass
+class QueuedMetricsRequest(betterproto.Message):
+    workflow_id: int = betterproto.int64_field(1)
+    workflow_process_id: int = betterproto.int64_field(2)
+    metric_ids: List[int] = betterproto.int32_field(3)
+
+
+@dataclass
 class WorkflowInfo(betterproto.Message):
     workflow_id: int = betterproto.int64_field(1)
     workflow_process_id: int = betterproto.int64_field(2)
     workflow_processing_type: "WorkflowProcessingType" = betterproto.enum_field(3)
 
 
 @dataclass
@@ -1130,14 +1201,15 @@
     grain_end_epoch_seconds: int = betterproto.int64_field(7)
     metric_run_annotation: "MetricRunAnnotation" = betterproto.message_field(8)
     group_dimensions: List["MetricGroupDimension"] = betterproto.message_field(9)
     id: int = betterproto.int32_field(10)
     group_name: str = betterproto.string_field(11)
     exception_class: str = betterproto.string_field(12)
     exception_message: str = betterproto.string_field(13)
+    summary_status: "MetricStatus" = betterproto.enum_field(14)
 
 
 @dataclass
 class MetricMetadata(betterproto.Message):
     statistic_name: str = betterproto.string_field(1)
     statistic_full_name: str = betterproto.string_field(2)
     dataset_name: str = betterproto.string_field(3)
@@ -1229,14 +1301,33 @@
     sort_direction: "SortDirection" = betterproto.enum_field(14)
     issue_id: int = betterproto.int32_field(15)
     start_epoch_seconds: int = betterproto.int64_field(16)
     end_epoch_seconds: int = betterproto.int64_field(17)
 
 
 @dataclass
+class GetMetricRunsBulkRequest(betterproto.Message):
+    metric_identifier: List["MetricIdentifier"] = betterproto.message_field(1)
+    days_of_history: int = betterproto.int32_field(2)
+    start_epoch_seconds: int = betterproto.int64_field(3)
+    end_epoch_seconds: int = betterproto.int64_field(4)
+
+
+@dataclass
+class MetricWithRuns(betterproto.Message):
+    metric_identifier: "MetricIdentifier" = betterproto.message_field(1)
+    metric_runs: List["MetricRun"] = betterproto.message_field(2)
+
+
+@dataclass
+class GetMetricRunsBulkResponse(betterproto.Message):
+    metrics: List["MetricWithRuns"] = betterproto.message_field(1)
+
+
+@dataclass
 class MetricSuiteRequest(betterproto.Message):
     metric_suite: "MetricSuite" = betterproto.message_field(1)
     workflow_info: "WorkflowInfo" = betterproto.message_field(2)
 
 
 @dataclass
 class MetricSuite(betterproto.Message):
@@ -1605,14 +1696,15 @@
     warehouse_name: str = betterproto.string_field(12)
     warehouse_vendor: "WarehouseType" = betterproto.enum_field(14)
     data_node_id: int = betterproto.int32_field(15)
     num_queries_latest_period: int = betterproto.int32_field(16)
     schema_change_info: "SchemaChangeInfo" = betterproto.message_field(17)
     table_type: "TableType" = betterproto.enum_field(18)
     is_favorite: bool = betterproto.bool_field(19)
+    requires_partition_filter: bool = betterproto.bool_field(20)
 
 
 @dataclass
 class VirtualTable(betterproto.Message):
     """*Representation of a virtual table made from a SQL query"""
 
     table: "Table" = betterproto.message_field(1)
@@ -1628,14 +1720,15 @@
     type: str = betterproto.string_field(3)
     parent_column_id: int = betterproto.int32_field(4)
     is_metric_time: bool = betterproto.bool_field(5)
     can_be_metric_time: bool = betterproto.bool_field(6)
     schema_change_info: "SchemaChangeInfo" = betterproto.message_field(7)
     full_type: str = betterproto.string_field(8)
     is_favorite: bool = betterproto.bool_field(9)
+    is_partition_field: bool = betterproto.bool_field(10)
 
 
 @dataclass
 class TableList(betterproto.Message):
     """* Representation of a list of tables for API purposes"""
 
     tables: List["Table"] = betterproto.message_field(1)
@@ -2199,14 +2292,19 @@
     schema_id: int = betterproto.int32_field(5, group="filter")
     issue_status: "IssueStatus" = betterproto.enum_field(6, group="filter")
     metric_id: int = betterproto.int32_field(7, group="filter")
     start_epoch_seconds: int = betterproto.int64_field(8, group="filter")
     end_epoch_seconds: int = betterproto.int64_field(9, group="filter")
     start_issue_closed_epoch_seconds: int = betterproto.int64_field(10, group="filter")
     end_issue_closed_epoch_seconds: int = betterproto.int64_field(11, group="filter")
+    issue_priority: "IssuePriority" = betterproto.enum_field(12, group="filter")
+    metric_status: "MetricStatus" = betterproto.enum_field(13, group="filter")
+    collection_id: int = betterproto.int32_field(14, group="filter")
+    metric_type: "MetricType" = betterproto.message_field(15, group="filter")
+    metric_category: "MetricCategory" = betterproto.enum_field(16, group="filter")
 
 
 @dataclass
 class CountsQuery(betterproto.Message):
     fields: List["AggregateField"] = betterproto.enum_field(1)
     filters: List["SearchFilter"] = betterproto.message_field(2)
     group_by_entity_type: "GroupByEntityType" = betterproto.enum_field(3)
@@ -2229,15 +2327,20 @@
     schema_name: str = betterproto.string_field(3, group="entity_id")
     table_id: int = betterproto.int32_field(4, group="entity_id")
     column_id: int = betterproto.int32_field(5, group="entity_id")
     schema_id: int = betterproto.int32_field(6, group="entity_id")
     sla_id: int = betterproto.int32_field(7, group="entity_id")
     metric_run_label: "MetricRunLabel" = betterproto.enum_field(8, group="entity_id")
     issue_priority: "IssuePriority" = betterproto.enum_field(9, group="entity_id")
+    issue_status: "IssueStatus" = betterproto.enum_field(10, group="entity_id")
+    metric_status: "MetricStatus" = betterproto.enum_field(11, group="entity_id")
+    metric_type: "MetricType" = betterproto.message_field(12, group="entity_id")
+    metric_category: "MetricCategory" = betterproto.enum_field(13, group="entity_id")
     counts_for_fields: List["CountForField"] = betterproto.message_field(2)
+    entity: "IdAndDisplayName" = betterproto.message_field(14)
 
 
 @dataclass
 class GetCountsResponse(betterproto.Message):
     query_results: List["CountsQueryResult"] = betterproto.message_field(1)
 
 
@@ -2482,14 +2585,21 @@
     sla_ids: List[int] = betterproto.int32_field(21)
     related_issue_ids: List[int] = betterproto.int32_field(22)
     priority: List["IssuePriority"] = betterproto.enum_field(23)
     metric_status: List["MetricStatus"] = betterproto.enum_field(24)
     metric_type: List["MetricType"] = betterproto.message_field(25)
     min_opened_time: int = betterproto.int64_field(26)
     max_opened_time: int = betterproto.int64_field(27)
+    sort_options: List["IssueSortOption"] = betterproto.message_field(28)
+
+
+@dataclass
+class IssueSortOption(betterproto.Message):
+    sort_direction: "SortDirection" = betterproto.enum_field(1)
+    sort_field: "IssueSortField" = betterproto.enum_field(2)
 
 
 @dataclass
 class GetIssuesResponse(betterproto.Message):
     issue: List["Issue"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -2564,14 +2674,15 @@
 
 
 @dataclass
 class PaginationInfo(betterproto.Message):
     prev_cursor: str = betterproto.string_field(1)
     next_cursor: str = betterproto.string_field(2)
     num_records: int = betterproto.int32_field(3)
+    first_sort_distinct_values: int = betterproto.int64_field(4)
 
 
 @dataclass
 class ColumnSearchRequest(betterproto.Message):
     table_id: int = betterproto.int32_field(1)
     column_ids: List[int] = betterproto.int32_field(2)
 
@@ -2854,14 +2965,15 @@
     query_timeout_seconds: int = betterproto.int32_field(11)
     schema_change_info: "SchemaChangeInfo" = betterproto.message_field(12)
     alation_source_id: int = betterproto.int32_field(13)
     is_favorite: bool = betterproto.bool_field(14)
     atlan_connection_id: str = betterproto.string_field(15)
     temporal_agent_uuid: str = betterproto.string_field(16)
     target_bigquery_project_id: str = betterproto.string_field(17)
+    bigquery_query_project_ids: str = betterproto.string_field(18)
 
 
 @dataclass
 class CreateSourceRequest(betterproto.Message):
     id: int = betterproto.int32_field(1)
     name: str = betterproto.string_field(2)
     hostname: str = betterproto.string_field(3)
@@ -2875,14 +2987,15 @@
     private_key_file: str = betterproto.string_field(10)
     query_timeout_seconds: int = betterproto.int32_field(11)
     skip_indexing: bool = betterproto.bool_field(12)
     alation_source_id: int = betterproto.int32_field(13)
     atlan_connection_id: str = betterproto.string_field(14)
     temporal_agent_secret: str = betterproto.string_field(15)
     target_bigquery_project_id: str = betterproto.string_field(16)
+    bigquery_query_project_ids: str = betterproto.string_field(17)
 
 
 @dataclass
 class MetadataSchemaRequest(betterproto.Message):
     source_id: int = betterproto.int32_field(1)
     schema_name: List[str] = betterproto.string_field(2)
 
@@ -3258,14 +3371,15 @@
     comparison_table_configurations: List[
         "ComparisonTableConfiguration"
     ] = betterproto.message_field(10)
     source_warehouse_type: "WarehouseType" = betterproto.enum_field(11)
     source_schema: "IdAndDisplayName" = betterproto.message_field(12)
     source_source: "IdAndDisplayName" = betterproto.message_field(13)
     notification_channels: List["NotificationChannel"] = betterproto.message_field(14)
+    is_source_table_deleted: bool = betterproto.bool_field(15)
 
 
 @dataclass
 class DeltaIdRequest(betterproto.Message):
     delta_id: int = betterproto.int32_field(1)
 
 
@@ -3292,25 +3406,31 @@
     alerting_metric_count: int = betterproto.int32_field(6)
     source_row_count: float = betterproto.double_field(7)
     target_row_count: float = betterproto.double_field(8)
     target_table: "IdAndDisplayName" = betterproto.message_field(9)
     target_warehouse_type: "WarehouseType" = betterproto.enum_field(10)
     target_schema: "IdAndDisplayName" = betterproto.message_field(11)
     target_source: "IdAndDisplayName" = betterproto.message_field(12)
+    total_group_count: int = betterproto.int32_field(13)
+    failed_group_count: int = betterproto.int32_field(14)
+    alerting_group_count: int = betterproto.int32_field(15)
 
 
 @dataclass
 class ComparisonColumnInfo(betterproto.Message):
     source_column: "IdAndDisplayName" = betterproto.message_field(1)
     target_column: "IdAndDisplayName" = betterproto.message_field(2)
     metrics: List["MetricType"] = betterproto.message_field(3)
     user_defined: bool = betterproto.bool_field(4)
     total_metric_count: int = betterproto.int32_field(5)
     failed_metric_count: int = betterproto.int32_field(6)
     alerting_metric_count: int = betterproto.int32_field(7)
+    total_group_count: int = betterproto.int32_field(8)
+    failed_group_count: int = betterproto.int32_field(9)
+    alerting_group_count: int = betterproto.int32_field(10)
 
 
 @dataclass
 class GetDeltaInfosResponse(betterproto.Message):
     delta_infos: List["DeltaInfo"] = betterproto.message_field(1)
     pagination_info: "PaginationInfo" = betterproto.message_field(2)
 
@@ -3325,14 +3445,19 @@
     id: int = betterproto.int32_field(1)
     name: str = betterproto.string_field(2)
     is_default: bool = betterproto.bool_field(3)
     sources: List["Source"] = betterproto.message_field(4)
 
 
 @dataclass
+class WorkspaceListResponse(betterproto.Message):
+    workspaces: List["Workspace"] = betterproto.message_field(1)
+
+
+@dataclass
 class CreateOrUpdateWorkspaceRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
 
 
 @dataclass
 class RevisionInfo(betterproto.Message):
     type: "RevisionType" = betterproto.enum_field(1)
@@ -3366,58 +3491,75 @@
 class CalculateDashboardDataPointsRequest(betterproto.Message):
     source_id: List[int] = betterproto.int32_field(1)
     timestamp: int = betterproto.int64_field(2)
 
 
 @dataclass
 class DashboardDataPointsRequest(betterproto.Message):
-    company_id: str = betterproto.string_field(1)
-    workspace_ids: List[str] = betterproto.string_field(2)
+    company_id: int = betterproto.int32_field(1)
+    workspace_ids: List[int] = betterproto.int32_field(2)
     source_ids: List[int] = betterproto.int32_field(3)
     starting_timestamp: int = betterproto.int64_field(4)
     ending_timestamp: int = betterproto.int64_field(5)
     data_point_types: List["DashboardDataPointType"] = betterproto.enum_field(6)
 
 
 @dataclass
 class DashboardDataPointsResponse(betterproto.Message):
-    company_id: str = betterproto.string_field(1)
-    workspace_id: str = betterproto.string_field(2)
-    source_id: int = betterproto.int32_field(3)
+    company_id: int = betterproto.int32_field(1)
+    workspace_ids: List[int] = betterproto.int32_field(2)
+    source_ids: List[int] = betterproto.int32_field(3)
     starting_timestamp: int = betterproto.int64_field(4)
     ending_timestamp: int = betterproto.int64_field(5)
     data_point_types: List["DashboardDataPointType"] = betterproto.enum_field(6)
     data_point_series: List["DashboardDataPointSeries"] = betterproto.message_field(7)
 
 
 @dataclass
 class DashboardDataPointSeries(betterproto.Message):
-    company_id: str = betterproto.string_field(1)
-    workspace_id: str = betterproto.string_field(2)
-    source_id: int = betterproto.int32_field(3)
+    company_id: int = betterproto.int32_field(1)
+    workspace_ids: List[int] = betterproto.int32_field(2)
+    source_ids: List[int] = betterproto.int32_field(3)
     key: str = betterproto.string_field(4)
     starting_timestamp: int = betterproto.int64_field(5)
     ending_timestamp: int = betterproto.int64_field(6)
     data_point_type: "DashboardDataPointType" = betterproto.enum_field(7)
     data_points: List["DashboardDataPoint"] = betterproto.message_field(8)
 
 
 @dataclass
 class DashboardDataPoint(betterproto.Message):
-    company_id: str = betterproto.string_field(1)
-    workspace_id: str = betterproto.string_field(2)
-    source_id: int = betterproto.int32_field(3)
+    company_id: int = betterproto.int32_field(1)
+    workspace_ids: List[int] = betterproto.int32_field(2)
+    source_ids: List[int] = betterproto.int32_field(3)
     key: str = betterproto.string_field(4)
     data_timestamp: int = betterproto.int64_field(5)
     data_point_type: "DashboardDataPointType" = betterproto.enum_field(6)
     value: float = betterproto.double_field(7)
     collected_timestamp: int = betterproto.int64_field(8)
 
 
 @dataclass
+class Group(betterproto.Message):
+    id: int = betterproto.int32_field(1)
+    name: str = betterproto.string_field(2)
+    users: List["IdAndDisplayName"] = betterproto.message_field(3)
+
+
+@dataclass
+class GroupListResponse(betterproto.Message):
+    groups: List["Group"] = betterproto.message_field(1)
+
+
+@dataclass
+class CreateOrUpdateGroupRequest(betterproto.Message):
+    name: str = betterproto.string_field(1)
+
+
+@dataclass
 class Empty(betterproto.Message):
     pass
 
 
 @dataclass
 class DimensionRun(betterproto.Message):
     dim_name: str = betterproto.string_field(1)
@@ -3620,14 +3762,31 @@
 
 
 @dataclass
 class RebuildSingleTableResponse(betterproto.Message):
     table: "Table" = betterproto.message_field(1)
 
 
+@dataclass
+class CreateUserAndCompanyRequest(betterproto.Message):
+    name: str = betterproto.string_field(1)
+    email: str = betterproto.string_field(2)
+    password: str = betterproto.string_field(3)
+    company_name: str = betterproto.string_field(4)
+
+
+@dataclass
+class AddUserRequest(betterproto.Message):
+    name: str = betterproto.string_field(1)
+    email: str = betterproto.string_field(2)
+    password: str = betterproto.string_field(3)
+    company_name: str = betterproto.string_field(4)
+    role: str = betterproto.string_field(5)
+
+
 class MetricServiceStub(betterproto.ServiceStub):
     """Metrics"""
 
     async def search_metric_configuration(
         self,
         *,
         ids: List[int] = [],
@@ -5027,14 +5186,15 @@
         sla_ids: List[int] = [],
         related_issue_ids: List[int] = [],
         priority: List["IssuePriority"] = [],
         metric_status: List["MetricStatus"] = [],
         metric_type: List["MetricType"] = [],
         min_opened_time: int = 0,
         max_opened_time: int = 0,
+        sort_options: List["IssueSortOption"] = [],
     ) -> GetIssuesResponse:
         """Get issues"""
 
         request = GetIssuesRequest()
         request.issue_ids = issue_ids
         request.current_status = current_status
         request.metric_ids = metric_ids
@@ -5053,14 +5213,16 @@
         request.related_issue_ids = related_issue_ids
         request.priority = priority
         request.metric_status = metric_status
         if metric_type is not None:
             request.metric_type = metric_type
         request.min_opened_time = min_opened_time
         request.max_opened_time = max_opened_time
+        if sort_options is not None:
+            request.sort_options = sort_options
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.IssueService/GetIssues",
             request,
             GetIssuesResponse,
         )
 
@@ -5237,14 +5399,15 @@
         private_key_file: str = "",
         query_timeout_seconds: int = 0,
         skip_indexing: bool = False,
         alation_source_id: int = 0,
         atlan_connection_id: str = "",
         temporal_agent_secret: str = "",
         target_bigquery_project_id: str = "",
+        bigquery_query_project_ids: str = "",
     ) -> SourceValidationResponse:
         """Validate source"""
 
         request = CreateSourceRequest()
         request.id = id
         request.name = name
         request.hostname = hostname
@@ -5257,14 +5420,15 @@
         request.private_key_file = private_key_file
         request.query_timeout_seconds = query_timeout_seconds
         request.skip_indexing = skip_indexing
         request.alation_source_id = alation_source_id
         request.atlan_connection_id = atlan_connection_id
         request.temporal_agent_secret = temporal_agent_secret
         request.target_bigquery_project_id = target_bigquery_project_id
+        request.bigquery_query_project_ids = bigquery_query_project_ids
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.SourceService/ValidateSource",
             request,
             SourceValidationResponse,
         )
 
@@ -5283,14 +5447,15 @@
         private_key_file: str = "",
         query_timeout_seconds: int = 0,
         skip_indexing: bool = False,
         alation_source_id: int = 0,
         atlan_connection_id: str = "",
         temporal_agent_secret: str = "",
         target_bigquery_project_id: str = "",
+        bigquery_query_project_ids: str = "",
     ) -> CreateSourceResponse:
         """Create or update source"""
 
         request = CreateSourceRequest()
         request.id = id
         request.name = name
         request.hostname = hostname
@@ -5303,14 +5468,15 @@
         request.private_key_file = private_key_file
         request.query_timeout_seconds = query_timeout_seconds
         request.skip_indexing = skip_indexing
         request.alation_source_id = alation_source_id
         request.atlan_connection_id = atlan_connection_id
         request.temporal_agent_secret = temporal_agent_secret
         request.target_bigquery_project_id = target_bigquery_project_id
+        request.bigquery_query_project_ids = bigquery_query_project_ids
 
         return await self._unary_unary(
             "/com.bigeye.models.generated.SourceService/CreateOrUpdateSource",
             request,
             CreateSourceResponse,
         )
```

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/generated/google/api.py` & `bigeye_sdk-0.4.54/bigeye_sdk/generated/google/api.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/model/big_config.py` & `bigeye_sdk-0.4.54/bigeye_sdk/model/big_config.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/model/collection_models.py` & `bigeye_sdk-0.4.54/bigeye_sdk/model/collection_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/model/dbt_schema.py` & `bigeye_sdk-0.4.54/bigeye_sdk/model/dbt_schema.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/model/delta_facade.py` & `bigeye_sdk-0.4.54/bigeye_sdk/model/delta_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/model/metric_facade.py` & `bigeye_sdk-0.4.54/bigeye_sdk/model/metric_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/model/protobuf_enum_facade.py` & `bigeye_sdk-0.4.54/bigeye_sdk/model/protobuf_enum_facade.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/model/protobuf_message_facade.py` & `bigeye_sdk-0.4.54/bigeye_sdk/model/protobuf_message_facade.py`

 * *Files 2% similar despite different names*

```diff
@@ -630,15 +630,15 @@
     @root_validator(pre=True)
     def must_be_list(cls, values):
         must_be_list_validator(clazz=SimpleCollection, attribute_name='metric_ids', values=values)
         must_be_list_validator(clazz=SimpleCollection, attribute_name='notification_channels', values=values)
 
         return values
 
-    def merge_for_upsert(self, existing: SimpleCollection, overwrite: bool = True) -> SimpleCollection:
+    def merge_for_upsert(self, existing: SimpleCollection) -> SimpleCollection:
         """
         Merges this collection and existing collection.  Attributes that will be merged include: notification channels and metric ids.
 
         If not overwriting: missing names, descriptions, and muted_until_timestamp will be populated with
         existing values.
 
         If overwriting: (current default strategy) new attributes will replace the old -- even if empty.
@@ -651,34 +651,28 @@
 
         """
         new_collection = self.copy(deep=True)
 
         # set existing SLA ID.
         new_collection.id = existing.id
 
-        if not overwrite:
-            """If we are not overwriting then we want to merge notification channels and metric ids."""
-            if not new_collection.name:
-                new_collection.name = existing.name
-
-            if not new_collection.description:
-                new_collection.description = existing.description
-
-            if not new_collection.muted_until_timestamp:
-                new_collection.muted_until_timestamp = existing.muted_until_timestamp
-
-            if new_collection.notification_channels:
-                new_collection.notification_channels.extend(existing.notification_channels)
-            else:
-                new_collection.notification_channels = existing.notification_channels
-
-            if new_collection.metric_ids:
-                new_collection.metric_ids.extend(existing.metric_ids)
-            else:
-                new_collection.metric_ids = existing.metric_ids
+        """We match on name. If users want to edit description or the muted_until_timestamp values."""
+        if not new_collection.description:
+            new_collection.description = existing.description
+
+        if not new_collection.muted_until_timestamp:
+            new_collection.muted_until_timestamp = existing.muted_until_timestamp
+
+        """Notification channels are missing because those will always be controlled by incoming bigconfig."""
+
+        """This will ensure that the collection will retain metrics when the above fields are updated."""
+        if new_collection.metric_ids:
+            new_collection.metric_ids.extend(existing.metric_ids)
+        else:
+            new_collection.metric_ids = existing.metric_ids
 
         return new_collection
 
     @classmethod
     def from_datawatch_object(cls, obj: Collection) -> SimpleCollection:
         collection = SimpleCollection(
             id=obj.id,
```

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/model/sla_models.py` & `bigeye_sdk-0.4.54/bigeye_sdk/model/sla_models.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/bigeye_sdk/serializable.py` & `bigeye_sdk-0.4.54/bigeye_sdk/serializable.py`

 * *Files identical despite different names*

### Comparing `bigeye_sdk-0.4.53/pyproject.toml` & `bigeye_sdk-0.4.54/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bigeye-sdk"
-version = "0.4.53"
+version = "0.4.54"
 description = "Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically."
 license = "Proprietary"
 authors = ["Bigeye <support@bigeye.com>"]
 readme = "README.md"
 homepage = "https://docs.bigeye.com/docs"
 
 [[tool.poetry.source]]
```

### Comparing `bigeye_sdk-0.4.53/PKG-INFO` & `bigeye_sdk-0.4.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bigeye-sdk
-Version: 0.4.53
+Version: 0.4.54
 Summary: Bigeye SDK offers developer tools and clients to interact with Bigeye programmatically.
 Home-page: https://docs.bigeye.com/docs
 License: Proprietary
 Author: Bigeye
 Author-email: support@bigeye.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: Other/Proprietary License
```

