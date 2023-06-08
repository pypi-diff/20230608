# Comparing `tmp/cognite_sdk-6.3.1.tar.gz` & `tmp/cognite_sdk-6.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.3.1.tar", max compression
+gzip compressed data, was "cognite_sdk-6.3.2.tar", max compression
```

## Comparing `cognite_sdk-6.3.1.tar` & `cognite_sdk-6.3.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
--rw-r--r--   0        0        0    11349 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/README.md
--rw-r--r--   0        0        0      574 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49083 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1013 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     7924 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     8454 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0     6468 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     7894 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11025 2023-06-07 13:19:35.589553 cognite_sdk-6.3.1/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87459 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21276 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17320 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45329 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49915 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9466 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27887 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21811 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4589 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9525 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-07 13:19:35.593552 cognite_sdk-6.3.1/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    37481 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      178 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_constants.py
--rw-r--r--   0        0        0     6501 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/config.py
--rw-r--r--   0        0        0    18062 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34178 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     2935 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0    12346 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7240 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     3651 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     3877 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0     2524 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    14625 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6682 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33940 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14299 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-06-07 13:19:35.597551 cognite_sdk-6.3.1/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/py.typed
--rw-r--r--   0        0        0     8865 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     8165 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7422 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4149 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-07 13:19:35.601550 cognite_sdk-6.3.1/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2132 2023-06-07 13:19:35.605548 cognite_sdk-6.3.1/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/README.md
+-rw-r--r--   0        0        0      574 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49083 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1013 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     7924 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     8454 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0     6468 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     7894 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11025 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87459 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12474 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21276 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17320 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41397 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45329 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49915 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9466 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27887 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21811 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4589 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9525 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1869 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    37722 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      178 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/config.py
+-rw-r--r--   0        0        0    19252 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    18565 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8741 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34178 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33582 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     2935 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0    12346 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7240 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     3651 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     3877 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0     2524 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    14625 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6682 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33940 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11008 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14299 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13657 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16631 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16465 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6003 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5868 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4098 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12253 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17651 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16814 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11789 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12078 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11425 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2354 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2451 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2742 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/py.typed
+-rw-r--r--   0        0        0     8865 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     8165 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7422 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2151 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.3.2/PKG-INFO
```

### Comparing `cognite_sdk-6.3.1/LICENSE` & `cognite_sdk-6.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/README.md` & `cognite_sdk-6.3.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/__init__.py` & `cognite_sdk-6.3.2/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/annotations.py` & `cognite_sdk-6.3.2/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/assets.py` & `cognite_sdk-6.3.2/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.3.2/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.3.2/cognite/client/_api/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.3.2/cognite/client/_api/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.3.2/cognite/client/_api/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.3.2/cognite/client/_api/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/data_sets.py` & `cognite_sdk-6.3.2/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.3.2/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/datapoints.py` & `cognite_sdk-6.3.2/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/diagrams.py` & `cognite_sdk-6.3.2/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.3.2/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/events.py` & `cognite_sdk-6.3.2/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.3.2/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/files.py` & `cognite_sdk-6.3.2/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/functions.py` & `cognite_sdk-6.3.2/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/geospatial.py` & `cognite_sdk-6.3.2/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/iam.py` & `cognite_sdk-6.3.2/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/labels.py` & `cognite_sdk-6.3.2/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/raw.py` & `cognite_sdk-6.3.2/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/relationships.py` & `cognite_sdk-6.3.2/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/sequences.py` & `cognite_sdk-6.3.2/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.3.2/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/templates.py` & `cognite_sdk-6.3.2/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/three_d.py` & `cognite_sdk-6.3.2/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/time_series.py` & `cognite_sdk-6.3.2/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.3.2/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.3.2/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.3.2/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.3.2/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.3.2/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api/vision.py` & `cognite_sdk-6.3.2/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_api_client.py` & `cognite_sdk-6.3.2/cognite/client/_api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,26 +96,28 @@
                 max_backoff_seconds=global_config.max_retry_backoff,
                 max_retries_total=global_config.max_retries,
                 max_retries_read=0,
                 max_retries_connect=global_config.max_retries_connect,
                 max_retries_status=global_config.max_retries,
             ),
             session=session,
+            refresh_auth_header=self._refresh_auth_header,
         )
         self._http_client_with_retry = HTTPClient(
             config=HTTPClientConfig(
                 status_codes_to_retry=global_config.status_forcelist,
                 backoff_factor=0.5,
                 max_backoff_seconds=global_config.max_retry_backoff,
                 max_retries_total=global_config.max_retries,
                 max_retries_read=global_config.max_retries,
                 max_retries_connect=global_config.max_retries_connect,
                 max_retries_status=global_config.max_retries,
             ),
             session=session,
+            refresh_auth_header=self._refresh_auth_header,
         )
 
     def _delete(
         self, url_path: str, params: Optional[Dict[str, Any]] = None, headers: Optional[Dict[str, Any]] = None
     ) -> Response:
         return self._do_request("DELETE", url_path, params=params, headers=headers, timeout=self._config.timeout)
 
@@ -182,28 +184,31 @@
         stream = kwargs.get("stream")
         self._log_request(res, payload=json_payload, stream=stream)
         return res
 
     def _configure_headers(self, accept: str, additional_headers: Dict[str, str]) -> MutableMapping[str, Any]:
         headers: MutableMapping[str, Any] = CaseInsensitiveDict()
         headers.update(requests.utils.default_headers())
-        auth_header_name, auth_header_value = self._config.credentials.authorization_header()
-        headers[auth_header_name] = auth_header_value
+        self._refresh_auth_header(headers)
         headers["content-type"] = "application/json"
         headers["accept"] = accept
         headers["x-cdp-sdk"] = f"CognitePythonSDK:{utils._auxiliary.get_current_sdk_version()}"
         headers["x-cdp-app"] = self._config.client_name
         headers["cdf-version"] = self._api_subversion
         if "User-Agent" in headers:
             headers["User-Agent"] += " " + utils._auxiliary.get_user_agent()
         else:
             headers["User-Agent"] = utils._auxiliary.get_user_agent()
         headers.update(additional_headers)
         return headers
 
+    def _refresh_auth_header(self, headers: MutableMapping[str, Any]) -> None:
+        auth_header_name, auth_header_value = self._config.credentials.authorization_header()
+        headers[auth_header_name] = auth_header_value
+
     def _resolve_url(self, method: str, url_path: str) -> Tuple[bool, str]:
         if not url_path.startswith("/"):
             raise ValueError("URL path must start with '/'")
         base_url = self._get_base_url_with_base_path()
         full_url = base_url + url_path
         is_retryable = self._is_retryable(method, full_url)
         return is_retryable, full_url
```

### Comparing `cognite_sdk-6.3.1/cognite/client/_cognite_client.py` & `cognite_sdk-6.3.2/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_http_client.py` & `cognite_sdk-6.3.2/cognite/client/_http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import functools
 import random
 import socket
 import time
 from http import cookiejar
-from typing import Any, Callable, Optional, Set, Tuple, Type, Union
+from typing import Any, Callable, MutableMapping, Optional, Set, Tuple, Type, Union
 
 import requests
 import requests.adapters
 import urllib3
 
 from cognite.client.config import global_config
 from cognite.client.exceptions import CogniteConnectionError, CogniteConnectionRefused, CogniteReadTimeout
@@ -92,22 +92,25 @@
 
 
 class HTTPClient:
     def __init__(
         self,
         config: HTTPClientConfig,
         session: requests.Session,
+        refresh_auth_header: Callable[[MutableMapping[str, Any]], None],
         retry_tracker_factory: Callable[[HTTPClientConfig], _RetryTracker] = _RetryTracker,
     ):
         self.session = session
         self.config = config
+        self.refresh_auth_header = refresh_auth_header
         self.retry_tracker_factory = retry_tracker_factory  # needed for tests
 
     def request(self, method: str, url: str, **kwargs: Any) -> requests.Response:
         retry_tracker = self.retry_tracker_factory(self.config)
+        headers = kwargs.get("headers")
         last_status = None
         while True:
             try:
                 res = self._do_request(method=method, url=url, **kwargs)
                 last_status = res.status_code
                 retry_tracker.status += 1
                 if not retry_tracker.should_retry(status_code=last_status):
@@ -118,15 +121,20 @@
                 retry_tracker.read += 1
                 if not retry_tracker.should_retry(status_code=last_status):
                     raise e
             except CogniteConnectionError as e:
                 retry_tracker.connect += 1
                 if not retry_tracker.should_retry(status_code=last_status):
                     raise e
+
+            # During a backoff loop, our credentials might expire, so we check and maybe refresh:
             time.sleep(retry_tracker.get_backoff_time())
+            if headers is not None:
+                # TODO: Refactoring needed to make this "prettier"
+                self.refresh_auth_header(headers)
 
     def _do_request(self, method: str, url: str, **kwargs: Any) -> requests.Response:
         """requests/urllib3 adds 2 or 3 layers of exceptions on top of built-in networking exceptions.
 
         Sometimes the appropriate built-in networking exception is not in the context, sometimes the requests
         exception is not in the context, so we need to check for the appropriate built-in exceptions,
         urllib3 exceptions, and requests exceptions.
```

### Comparing `cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.3.2/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.3.2/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.3.2/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/config.py` & `cognite_sdk-6.3.2/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/credentials.py` & `cognite_sdk-6.3.2/cognite/client/credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 from msal import ConfidentialClientApplication, PublicClientApplication, SerializableTokenCache
 from oauthlib.oauth2 import BackendApplicationClient, OAuth2Error
 from requests_oauthlib import OAuth2Session
 
 from cognite.client.exceptions import CogniteAuthError
 
+_TOKEN_EXPIRY_LEEWAY_SECONDS_DEFAULT = 15  # Do not change without also updating all the docstrings using it
+
 
 class CredentialProvider(Protocol):
     @abstractmethod
     def authorization_header(self) -> Tuple[str, str]:
         raise NotImplementedError
 
 
@@ -56,18 +58,18 @@
             raise TypeError(f"'token' must be a string or a no-argument-callable returning a string, not {type(token)}")
 
     def authorization_header(self) -> Tuple[str, str]:
         return "Authorization", f"Bearer {self.__token_factory()}"
 
 
 class _OAuthCredentialProviderWithTokenRefresh(CredentialProvider):
-    # This ensures we don't return a token which expires immediately, but within minimum 3 seconds.
-    __TOKEN_EXPIRY_LEEWAY_SECONDS = 3
+    def __init__(self, token_expiry_leeway_seconds: int = _TOKEN_EXPIRY_LEEWAY_SECONDS_DEFAULT) -> None:
+        # This ensures we don't return a token which expires immediately:
+        self.token_expiry_leeway_seconds = token_expiry_leeway_seconds
 
-    def __init__(self) -> None:
         self.__token_refresh_lock = threading.Lock()
         self.__access_token: Optional[str] = None
         self.__access_token_expires_at: Optional[float] = None
 
     def __getstate__(self) -> dict[str, Any]:
         # threading.Lock is not picklable, temporarily remove:
         lock_tmp, self.__token_refresh_lock = self.__token_refresh_lock, None  # type: ignore [assignment]
@@ -80,18 +82,17 @@
         self.__token_refresh_lock = threading.Lock()
 
     @abstractmethod
     def _refresh_access_token(self) -> Tuple[str, float]:
         """This method should return the access_token and expiry time"""
         raise NotImplementedError
 
-    @classmethod
-    def __should_refresh_token(cls, token: Optional[str], expires_at: Optional[float]) -> bool:
+    def __should_refresh_token(self, token: Optional[str], expires_at: Optional[float]) -> bool:
         no_token = token is None
-        token_is_expired = expires_at is None or time.time() > expires_at - cls.__TOKEN_EXPIRY_LEEWAY_SECONDS
+        token_is_expired = expires_at is None or time.time() > expires_at - self.token_expiry_leeway_seconds
         return no_token or token_is_expired
 
     @staticmethod
     def _verify_credentials(credentials: Dict[str, Any]) -> None:
         """The msal library doesnt raise anything when auth fails, but returns a dictionary with varying keys"""
         if "access_token" in credentials and "expires_in" in credentials:
             return
@@ -149,16 +150,16 @@
 class OAuthDeviceCode(_OAuthCredentialProviderWithTokenRefresh, _WithMsalSerializableTokenCache):
     """OAuth credential provider for the device code login flow.
 
     Args:
         authority_url (str): OAuth authority url
         client_id (str): Your application's client id.
         scopes (List[str]): A list of scopes.
-        token_cache_path (Path): Location to store token cache, defaults to
-                                 os temp directory/cognitetokencache.{client_id}.bin.
+        token_cache_path (Path): Location to store token cache, defaults to os temp directory/cognitetokencache.{client_id}.bin.
+        token_expiry_leeway_seconds (int): The token is refreshed at the earliest when this number of seconds is left before expiry. Default: 15 sec
 
     Examples:
 
             >>> from cognite.client.credentials import OAuthDeviceCode
             >>> oauth_provider = OAuthDeviceCode(
             ...     authority_url="https://login.microsoftonline.com/xyz",
             ...     client_id="abcd",
@@ -168,16 +169,17 @@
 
     def __init__(
         self,
         authority_url: str,
         client_id: str,
         scopes: List[str],
         token_cache_path: Path = None,
+        token_expiry_leeway_seconds: int = _TOKEN_EXPIRY_LEEWAY_SECONDS_DEFAULT,
     ) -> None:
-        super().__init__()
+        super().__init__(token_expiry_leeway_seconds)
         self.__authority_url = authority_url
         self.__client_id = client_id
         self.__scopes = scopes
 
         self._token_cache_path = self._resolve_token_cache_path(token_cache_path, client_id)
         self.__app = self._create_client_app(self._token_cache_path, client_id, authority_url)
 
@@ -225,16 +227,16 @@
     Make sure you have http://localhost:port in Redirect URI in App Registration as type "Mobile and desktop applications".
 
     Args:
         authority_url (str): OAuth authority url
         client_id (str): Your application's client id.
         scopes (List[str]): A list of scopes.
         redirect_port (List[str]): Redirect port defaults to 53000.
-        token_cache_path (Path): Location to store token cache, defaults to
-                                 os temp directory/cognitetokencache.{client_id}.bin.
+        token_cache_path (Path): Location to store token cache, defaults to os temp directory/cognitetokencache.{client_id}.bin.
+        token_expiry_leeway_seconds (int): The token is refreshed at the earliest when this number of seconds is left before expiry. Default: 15 sec
 
     Examples:
 
             >>> from cognite.client.credentials import OAuthInteractive
             >>> oauth_provider = OAuthInteractive(
             ...     authority_url="https://login.microsoftonline.com/xyz",
             ...     client_id="abcd",
@@ -245,17 +247,18 @@
     def __init__(
         self,
         authority_url: str,
         client_id: str,
         scopes: List[str],
         redirect_port: int = 53000,
         token_cache_path: Path = None,
+        token_expiry_leeway_seconds: int = _TOKEN_EXPIRY_LEEWAY_SECONDS_DEFAULT,
     ) -> None:
 
-        super().__init__()
+        super().__init__(token_expiry_leeway_seconds)
         self.__authority_url = authority_url
         self.__client_id = client_id
         self.__scopes = scopes
         self.__redirect_port = redirect_port
 
         self._token_cache_path = self._resolve_token_cache_path(token_cache_path, client_id)
         self.__app = self._create_client_app(self._token_cache_path, client_id, authority_url)
@@ -299,14 +302,15 @@
     """OAuth credential provider for the "Client Credentials" flow.
 
     Args:
         token_url (str): OAuth token url
         client_id (str): Your application's client id.
         client_secret (str): Your application's client secret
         scopes (List[str]): A list of scopes.
+        token_expiry_leeway_seconds (int): The token is refreshed at the earliest when this number of seconds is left before expiry. Default: 15 sec
         **token_custom_args (Any): Optional additional arguments to pass as query parameters to the token fetch request.
 
     Examples:
 
             >>> from cognite.client.credentials import OAuthClientCredentials
             >>> import os
             >>> oauth_provider = OAuthClientCredentials(
@@ -321,17 +325,18 @@
 
     def __init__(
         self,
         token_url: str,
         client_id: str,
         client_secret: str,
         scopes: List[str],
+        token_expiry_leeway_seconds: int = _TOKEN_EXPIRY_LEEWAY_SECONDS_DEFAULT,
         **token_custom_args: Any,
     ):
-        super().__init__()
+        super().__init__(token_expiry_leeway_seconds)
         self.__token_url = token_url
         self.__client_id = client_id
         self.__client_secret = client_secret
         self.__scopes = scopes
         self.__token_custom_args: Dict[str, Any] = token_custom_args
         self.__oauth = self._create_oauth_session()
         self._validate_token_custom_args()
@@ -402,30 +407,39 @@
 
     Args:
         authority_url (str): OAuth authority url
         client_id (str): Your application's client id.
         cert_thumbprint (str): Your certificate's thumbprint. You get it when you upload your certificate to Azure AD.
         certificate (str): Your private certificate, typically read from a .pem file
         scopes (List[str]): A list of scopes.
+        token_expiry_leeway_seconds (int): The token is refreshed at the earliest when this number of seconds is left before expiry. Default: 15 sec
 
     Examples:
 
             >>> from cognite.client.credentials import OAuthClientCertificate
             >>> from pathlib import Path
             >>> oauth_provider = OAuthClientCertificate(
             ...     authority_url="https://login.microsoftonline.com/xyz",
             ...     client_id="abcd",
             ...     cert_thumbprint="XYZ123",
             ...     certificate=Path("certificate.pem").read_text(),
             ...     scopes=["https://greenfield.cognitedata.com/.default"],
             ... )
     """
 
-    def __init__(self, authority_url: str, client_id: str, cert_thumbprint: str, certificate: str, scopes: List[str]):
-        super().__init__()
+    def __init__(
+        self,
+        authority_url: str,
+        client_id: str,
+        cert_thumbprint: str,
+        certificate: str,
+        scopes: List[str],
+        token_expiry_leeway_seconds: int = _TOKEN_EXPIRY_LEEWAY_SECONDS_DEFAULT,
+    ):
+        super().__init__(token_expiry_leeway_seconds)
         self.__authority_url = authority_url
         self.__client_id = client_id
         self.__cert_thumbprint = cert_thumbprint
         self.__certificate = certificate
         self.__scopes = scopes
 
         self.__app = ConfidentialClientApplication(
```

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/_base.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/assets.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/containers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/ids.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/views.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/events.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/files.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/functions.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/iam.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/labels.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/raw.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/shared.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/templates.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/exceptions.py` & `cognite_sdk-6.3.2/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/testing.py` & `cognite_sdk-6.3.2/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/__init__.py` & `cognite_sdk-6.3.2/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.3.2/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.3.2/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_graph.py` & `cognite_sdk-6.3.2/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_identifier.py` & `cognite_sdk-6.3.2/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_logging.py` & `cognite_sdk-6.3.2/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.3.2/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.3.2/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.3.2/cognite/client/utils/_pyodide_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
 import warnings
-from typing import TYPE_CHECKING, Callable, Dict, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Callable, Dict, MutableMapping, Optional, Tuple
 
 import cognite.client as cc
 from cognite.client._http_client import _RetryTracker
 from cognite.client.config import ClientConfig
 from cognite.client.credentials import CredentialProvider
 
 if TYPE_CHECKING:
@@ -58,19 +58,20 @@
         cc.config.global_config.default_client_config = FusionNotebookConfig()
 
 
 def http_client__init__(
     self: HTTPClient,
     config: HTTPClientConfig,
     session: Session,
+    refresh_auth_header: Callable[[MutableMapping[str, Any]], None],
     retry_tracker_factory: Callable[[HTTPClientConfig], _RetryTracker] = _RetryTracker,
 ) -> None:
     import pyodide_http  # type: ignore [import]
 
-    self._old__init__(config, session, retry_tracker_factory)  # type: ignore [attr-defined]
+    self._old__init__(config, session, refresh_auth_header, retry_tracker_factory)  # type: ignore [attr-defined]
     self.session.mount("https://", pyodide_http._requests.PyodideHTTPAdapter())
     self.session.mount("http://", pyodide_http._requests.PyodideHTTPAdapter())
 
 
 class EnvVarToken(CredentialProvider):
     """Credential provider that always reads token from an environment variable just-in-time,
     allowing refreshing the value by another entity.
```

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_text.py` & `cognite_sdk-6.3.2/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_time.py` & `cognite_sdk-6.3.2/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_validation.py` & `cognite_sdk-6.3.2/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.3.2/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.1/pyproject.toml` & `cognite_sdk-6.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.3.1"
+version = "6.3.2"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
 
@@ -63,11 +63,12 @@
 python-dotenv = "^0.20.0"
 mypy = "^0.981"
 types-urllib3 = "^1.26.16"
 types-requests = "^2.28.1"
 pep8-naming = "^0"
 types-backports = "^0.1.3"
 types-protobuf = "^4.22.0.2"
+packaging = ">=23"
 
 [build-system]
 requires = ["poetry>=1.0"]
 build-backend = "poetry.masonry.api"
```

### Comparing `cognite_sdk-6.3.1/PKG-INFO` & `cognite_sdk-6.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.3.1
+Version: 6.3.2
 Summary: Cognite Python SDK
 License: Apache-2.0
 Author: Erlend Vollset
 Author-email: erlend.vollset@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.3.1 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.3.2 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

