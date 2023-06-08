# Comparing `tmp/featurebyte-0.3.0.tar.gz` & `tmp/featurebyte-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurebyte-0.3.0.tar", max compression
+gzip compressed data, was "featurebyte-0.3.1.tar", max compression
```

## Comparing `featurebyte-0.3.0.tar` & `featurebyte-0.3.1.tar`

### file list

```diff
@@ -1,526 +1,526 @@
--rw-r--r--   0        0        0     3860 2023-06-05 04:27:45.211716 featurebyte-0.3.0/LICENSE
--rw-r--r--   0        0        0    19816 2023-06-05 04:27:45.211716 featurebyte-0.3.0/README.md
--rw-r--r--   0        0        0    14195 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/__init__.py
--rw-r--r--   0        0        0     2017 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/__main__.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/__init__.py
--rw-r--r--   0        0        0    30557 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/api_object.py
--rw-r--r--   0        0        0     3975 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/api_object_util.py
--rw-r--r--   0        0        0     4985 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/asat_aggregator.py
--rw-r--r--   0        0        0     5521 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/base_aggregator.py
--rw-r--r--   0        0        0    37589 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/base_table.py
--rw-r--r--   0        0        0     4790 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/batch_feature_table.py
--rw-r--r--   0        0        0     5019 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/batch_request_table.py
--rw-r--r--   0        0        0    35381 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/catalog.py
--rw-r--r--   0        0        0     1475 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/catalog_decorator.py
--rw-r--r--   0        0        0    10842 2023-06-05 04:27:45.215716 featurebyte-0.3.0/featurebyte/api/catalog_get_by_id_mixin.py
--rw-r--r--   0        0        0    11517 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/change_view.py
--rw-r--r--   0        0        0     6600 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/credential.py
--rw-r--r--   0        0        0     6540 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/data_source.py
--rw-r--r--   0        0        0    13660 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/deployment.py
--rw-r--r--   0        0        0     9699 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/dimension_table.py
--rw-r--r--   0        0        0     3107 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/dimension_view.py
--rw-r--r--   0        0        0    12242 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/entity.py
--rw-r--r--   0        0        0    22561 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/event_table.py
--rw-r--r--   0        0        0    16044 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/event_view.py
--rw-r--r--   0        0        0    46149 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature.py
--rw-r--r--   0        0        0    15414 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_group.py
--rw-r--r--   0        0        0    15001 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_job.py
--rw-r--r--   0        0        0     8770 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_job_setting_analysis.py
--rw-r--r--   0        0        0    62689 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_list.py
--rw-r--r--   0        0        0     4116 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_namespace.py
--rw-r--r--   0        0        0    10016 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_store.py
--rw-r--r--   0        0        0     1999 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_util.py
--rw-r--r--   0        0        0      557 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/feature_validation_util.py
--rw-r--r--   0        0        0    18206 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/groupby.py
--rw-r--r--   0        0        0     4927 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/historical_feature_table.py
--rw-r--r--   0        0        0    16661 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/item_table.py
--rw-r--r--   0        0        0    11752 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/item_view.py
--rw-r--r--   0        0        0     2909 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/lag.py
--rw-r--r--   0        0        0     4909 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/materialized_table.py
--rw-r--r--   0        0        0     4952 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/observation_table.py
--rw-r--r--   0        0        0      721 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/periodic_task.py
--rw-r--r--   0        0        0     8442 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/relationship.py
--rw-r--r--   0        0        0     3474 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/request_column.py
--rw-r--r--   0        0        0     5018 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/savable_api_object.py
--rw-r--r--   0        0        0    21162 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/scd_table.py
--rw-r--r--   0        0        0     6023 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/scd_view.py
--rw-r--r--   0        0        0     3119 2023-06-05 04:27:45.219716 featurebyte-0.3.0/featurebyte/api/simple_aggregator.py
--rw-r--r--   0        0        0    46157 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/source_table.py
--rw-r--r--   0        0        0     5522 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/table.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/templates/online_serving/__init__.py
--rw-r--r--   0        0        0      707 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/templates/online_serving/python.tpl
--rw-r--r--   0        0        0      132 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/templates/online_serving/shell.tpl
--rw-r--r--   0        0        0    60163 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/view.py
--rw-r--r--   0        0        0     8368 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/window_aggregator.py
--rw-r--r--   0        0        0     1607 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/api/window_validator.py
--rw-r--r--   0        0        0     6870 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/app.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/__init__.py
--rw-r--r--   0        0        0     3116 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/date_util.py
--rw-r--r--   0        0        0      956 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/descriptor.py
--rw-r--r--   0        0        0      636 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/dict_util.py
--rw-r--r--   0        0        0     2090 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/doc_util.py
--rw-r--r--   0        0        0      692 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/allowed_classes.py
--rw-r--r--   0        0        0    16036 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/autodoc_processor.py
--rw-r--r--   0        0        0     1419 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/constants.py
--rw-r--r--   0        0        0     4280 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/custom_nav.py
--rw-r--r--   0        0        0     8560 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/doc_types.py
--rw-r--r--   0        0        0    43070 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/documentation_layout.py
--rw-r--r--   0        0        0     7430 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/extract_csv.py
--rw-r--r--   0        0        0     3479 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/formatters.py
--rw-r--r--   0        0        0    31657 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/gen_ref_pages_docs_builder.py
--rw-r--r--   0        0        0      877 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/markdown_extension/extension.py
--rw-r--r--   0        0        0     5660 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/pydantic_field_docs.py
--rw-r--r--   0        0        0    16371 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/resource_extractor.py
--rw-r--r--   0        0        0      519 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/resource_util.py
--rw-r--r--   0        0        0      200 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/documentation/util.py
--rw-r--r--   0        0        0     1262 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/env_util.py
--rw-r--r--   0        0        0     6740 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/formatting_util.py
--rw-r--r--   0        0        0     3925 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/join_utils.py
--rw-r--r--   0        0        0     4198 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/model_util.py
--rw-r--r--   0        0        0      815 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/path_util.py
--rw-r--r--   0        0        0     1062 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/progress.py
--rw-r--r--   0        0        0      451 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/singleton.py
--rw-r--r--   0        0        0     1084 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/tile_util.py
--rw-r--r--   0        0        0     2629 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/typing.py
--rw-r--r--   0        0        0    10491 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/utils.py
--rw-r--r--   0        0        0     4699 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/common/validator.py
--rw-r--r--   0        0        0    12486 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/config.py
--rw-r--r--   0        0        0     1366 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/conftest.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/__init__.py
--rw-r--r--   0        0        0    15412 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/count_dict.py
--rw-r--r--   0        0        0    23735 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/datetime.py
--rw-r--r--   0        0        0    10051 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/feature_datetime.py
--rw-r--r--   0        0        0     8454 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/feature_string.py
--rw-r--r--   0        0        0    15765 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/accessor/string.py
--rw-r--r--   0        0        0     8902 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/frame.py
--rw-r--r--   0        0        0    11843 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/generic.py
--rw-r--r--   0        0        0    16742 2023-06-05 04:27:45.223716 featurebyte-0.3.0/featurebyte/core/mixin.py
--rw-r--r--   0        0        0    37956 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/core/series.py
--rw-r--r--   0        0        0     1484 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/core/timedelta.py
--rw-r--r--   0        0        0     6393 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/core/util.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/__init__.py
--rw-r--r--   0        0        0      697 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/__main__.py
--rw-r--r--   0        0        0     5546 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/app.py
--rw-r--r--   0        0        0     3125 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/creditcard.sql
--rw-r--r--   0        0        0     1154 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/doctest_grocery.sql
--rw-r--r--   0        0        0     2200 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/grocery.sql
--rw-r--r--   0        0        0     5757 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/datasets/healthcare.sql
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/docker/__init__.py
--rw-r--r--   0        0        0     4518 2023-06-05 04:28:22.551558 featurebyte-0.3.0/featurebyte/docker/featurebyte.yml
--rw-r--r--   0        0        0    10343 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/docker/manager.py
--rw-r--r--   0        0        0     9199 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/enum.py
--rw-r--r--   0        0        0     9244 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/exception.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/feature_manager/__init__.py
--rw-r--r--   0        0        0    10392 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/feature_manager/manager.py
--rw-r--r--   0        0        0     2911 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/feature_manager/model.py
--rw-r--r--   0        0        0     3997 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/feature_manager/sql_template.py
--rw-r--r--   0        0        0     3667 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/feature_utility.py
--rw-r--r--   0        0        0     4145 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/logging.py
--rw-r--r--   0        0        0     7839 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/middleware.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/__init__.py
--rw-r--r--   0        0        0      604 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/migration_data_service.py
--rw-r--r--   0        0        0     1664 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/model.py
--rw-r--r--   0        0        0     8423 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/run.py
--rw-r--r--   0        0        0     1442 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/service/__init__.py
--rw-r--r--   0        0        0     9762 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/service/data_warehouse.py
--rw-r--r--   0        0        0     9181 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/migration/service/mixin.py
--rw-r--r--   0        0        0      646 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/__init__.py
--rw-r--r--   0        0        0    10813 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/base.py
--rw-r--r--   0        0        0      617 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/batch_feature_table.py
--rw-r--r--   0        0        0     1726 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/batch_request_table.py
--rw-r--r--   0        0        0     2377 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/catalog.py
--rw-r--r--   0        0        0     1572 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/context.py
--rw-r--r--   0        0        0     8513 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/credential.py
--rw-r--r--   0        0        0     1333 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/deployment.py
--rw-r--r--   0        0        0     2026 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/dimension_table.py
--rw-r--r--   0        0        0     3618 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/entity.py
--rw-r--r--   0        0        0     3051 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/entity_validation.py
--rw-r--r--   0        0        0     3551 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/event_table.py
--rw-r--r--   0        0        0    11926 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/feature.py
--rw-r--r--   0        0        0     3750 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/feature_job_setting_analysis.py
--rw-r--r--   0        0        0    21070 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/feature_list.py
--rw-r--r--   0        0        0     7606 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/feature_store.py
--rw-r--r--   0        0        0      644 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/historical_feature_table.py
--rw-r--r--   0        0        0     2919 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/item_table.py
--rw-r--r--   0        0        0     1620 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/materialized_table.py
--rw-r--r--   0        0        0     2113 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/observation_table.py
--rw-r--r--   0        0        0     3738 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/online_store.py
--rw-r--r--   0        0        0     1433 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/parent_serving.py
--rw-r--r--   0        0        0     2891 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/periodic_task.py
--rw-r--r--   0        0        0     1492 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/persistent.py
--rw-r--r--   0        0        0     1024 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/proxy_table.py
--rw-r--r--   0        0        0     4330 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/relationship.py
--rw-r--r--   0        0        0      944 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/relationship_analysis.py
--rw-r--r--   0        0        0     7865 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/request_input.py
--rw-r--r--   0        0        0     3554 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/scd_table.py
--rw-r--r--   0        0        0     1435 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/semantic.py
--rw-r--r--   0        0        0     1085 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/task.py
--rw-r--r--   0        0        0     3269 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/models/tile.py
--rw-r--r--   0        0        0      154 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/persistent/__init__.py
--rw-r--r--   0        0        0     9396 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/persistent/audit.py
--rw-r--r--   0        0        0    21712 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/persistent/base.py
--rw-r--r--   0        0        0     9824 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/persistent/mongo.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/query_graph/__init__.py
--rw-r--r--   0        0        0     2533 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/query_graph/algorithm.py
--rw-r--r--   0        0        0     2988 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/query_graph/enum.py
--rw-r--r--   0        0        0    16847 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/query_graph/graph.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.227716 featurebyte-0.3.0/featurebyte/query_graph/graph_node/__init__.py
--rw-r--r--   0        0        0     4592 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/graph_node/base.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/__init__.py
--rw-r--r--   0        0        0      873 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/column_info.py
--rw-r--r--   0        0        0    12700 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/common_table.py
--rw-r--r--   0        0        0     1707 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/critical_data_info.py
--rw-r--r--   0        0        0     6699 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/feature_job_setting.py
--rw-r--r--   0        0        0    19282 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/graph.py
--rw-r--r--   0        0        0    23872 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/model/table.py
--rw-r--r--   0        0        0     1076 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/__init__.py
--rw-r--r--   0        0        0     5236 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/agg_func.py
--rw-r--r--   0        0        0    28374 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/base.py
--rw-r--r--   0        0        0     5224 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/binary.py
--rw-r--r--   0        0        0    17953 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/cleaning_operation.py
--rw-r--r--   0        0        0     7797 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/count_dict.py
--rw-r--r--   0        0        0     7293 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/date.py
--rw-r--r--   0        0        0    60575 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/generic.py
--rw-r--r--   0        0        0    17049 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/input.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/metadata/__init__.py
--rw-r--r--   0        0        0      873 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/metadata/column.py
--rw-r--r--   0        0        0    21929 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/metadata/operation.py
--rw-r--r--   0        0        0    19397 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/metadata/sdk_code.py
--rw-r--r--   0        0        0       47 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/metadata/templates/sdk_code.tpl
--rw-r--r--   0        0        0     7393 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/mixin.py
--rw-r--r--   0        0        0    21084 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/nested.py
--rw-r--r--   0        0        0     3272 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/request.py
--rw-r--r--   0        0        0     2054 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/scalar.py
--rw-r--r--   0        0        0     6696 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/schema.py
--rw-r--r--   0        0        0     5461 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/string.py
--rw-r--r--   0        0        0     4824 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/unary.py
--rw-r--r--   0        0        0     1042 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/node/validator.py
--rw-r--r--   0        0        0     1050 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/pruning_util.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/__init__.py
--rw-r--r--   0        0        0    27339 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/adapter.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/__init__.py
--rw-r--r--   0        0        0     7198 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/asat.py
--rw-r--r--   0        0        0    16281 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/base.py
--rw-r--r--   0        0        0     5739 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/item.py
--rw-r--r--   0        0        0     3801 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/latest.py
--rw-r--r--   0        0        0     9549 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/lookup.py
--rw-r--r--   0        0        0     3811 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/request_table.py
--rw-r--r--   0        0        0    26795 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/window.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/__init__.py
--rw-r--r--   0        0        0     5560 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/aggregate.py
--rw-r--r--   0        0        0    12647 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/base.py
--rw-r--r--   0        0        0     2723 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/binary.py
--rw-r--r--   0        0        0     5740 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/count_dict.py
--rw-r--r--   0        0        0    10724 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/datetime.py
--rw-r--r--   0        0        0     7163 2023-06-05 04:27:45.231716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/generic.py
--rw-r--r--   0        0        0     2409 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/groupby.py
--rw-r--r--   0        0        0     2593 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/input.py
--rw-r--r--   0        0        0     1449 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/is_in.py
--rw-r--r--   0        0        0     6208 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/join.py
--rw-r--r--   0        0        0     6138 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/join_feature.py
--rw-r--r--   0        0        0     2291 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/literal.py
--rw-r--r--   0        0        0      878 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/request.py
--rw-r--r--   0        0        0     8360 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/string.py
--rw-r--r--   0        0        0    11741 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/tile.py
--rw-r--r--   0        0        0     5170 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/track_changes.py
--rw-r--r--   0        0        0     5157 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/unary.py
--rw-r--r--   0        0        0     2536 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/ast/util.py
--rw-r--r--   0        0        0     7070 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/builder.py
--rw-r--r--   0        0        0     4909 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/common.py
--rw-r--r--   0        0        0     1704 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/dataframe.py
--rw-r--r--   0        0        0     1966 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/expression.py
--rw-r--r--   0        0        0    20348 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/feature_compute.py
--rw-r--r--   0        0        0    28059 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/feature_historical.py
--rw-r--r--   0        0        0     3694 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/feature_preview.py
--rw-r--r--   0        0        0     4449 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/groupby_helper.py
--rw-r--r--   0        0        0      426 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/__init__.py
--rw-r--r--   0        0        0     3344 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/base.py
--rw-r--r--   0        0        0    27934 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/preview.py
--rw-r--r--   0        0        0     6685 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/tile.py
--rw-r--r--   0        0        0     4027 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/materialisation.py
--rw-r--r--   0        0        0    17988 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/online_serving.py
--rw-r--r--   0        0        0      659 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/online_serving_util.py
--rw-r--r--   0        0        0     5042 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/parent_serving.py
--rw-r--r--   0        0        0    15948 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/scd_helper.py
--rw-r--r--   0        0        0    20783 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/specs.py
--rw-r--r--   0        0        0     2206 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/template.py
--rw-r--r--   0        0        0    13029 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/tile_compute.py
--rw-r--r--   0        0        0     3793 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/tile_util.py
--rw-r--r--   0        0        0     9354 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/sql/tiling.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/__init__.py
--rw-r--r--   0        0        0     5184 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/base.py
--rw-r--r--   0        0        0     5201 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/flattening.py
--rw-r--r--   0        0        0     6716 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/operation_structure.py
--rw-r--r--   0        0        0    20327 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/pruning.py
--rw-r--r--   0        0        0    10248 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/reconstruction.py
--rw-r--r--   0        0        0    13262 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/transform/sdk_code.py
--rw-r--r--   0        0        0     5951 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/query_graph/util.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/__init__.py
--rw-r--r--   0        0        0     4367 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/app_container.py
--rw-r--r--   0        0        0     4340 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/app_container_config.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_feature_table/__init__.py
--rw-r--r--   0        0        0     4832 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_feature_table/api.py
--rw-r--r--   0        0        0     4616 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_feature_table/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_request_table/__init__.py
--rw-r--r--   0        0        0     4860 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_request_table/api.py
--rw-r--r--   0        0        0     3137 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/batch_request_table/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/catalog/__init__.py
--rw-r--r--   0        0        0     4307 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/catalog/api.py
--rw-r--r--   0        0        0     2524 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/catalog/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.235716 featurebyte-0.3.0/featurebyte/routes/common/__init__.py
--rw-r--r--   0        0        0    10579 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/common/base.py
--rw-r--r--   0        0        0     3761 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/common/base_materialized_table.py
--rw-r--r--   0        0        0     5515 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/common/base_table.py
--rw-r--r--   0        0        0      886 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/common/schema.py
--rw-r--r--   0        0        0      400 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/common/util.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/context/__init__.py
--rw-r--r--   0        0        0     3107 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/context/api.py
--rw-r--r--   0        0        0     1596 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/context/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/credential/__init__.py
--rw-r--r--   0        0        0     4605 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/credential/api.py
--rw-r--r--   0        0        0     3071 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/credential/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/deployment/__init__.py
--rw-r--r--   0        0        0     5604 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/deployment/api.py
--rw-r--r--   0        0        0    10416 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/deployment/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/dimension_table/__init__.py
--rw-r--r--   0        0        0     4181 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/dimension_table/api.py
--rw-r--r--   0        0        0     1674 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/dimension_table/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/entity/__init__.py
--rw-r--r--   0        0        0     5145 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/entity/api.py
--rw-r--r--   0        0        0     2718 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/entity/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/event_table/__init__.py
--rw-r--r--   0        0        0     4689 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/event_table/api.py
--rw-r--r--   0        0        0     1818 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/event_table/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature/__init__.py
--rw-r--r--   0        0        0     6378 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature/api.py
--rw-r--r--   0        0        0    15348 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_job_setting_analysis/__init__.py
--rw-r--r--   0        0        0     5449 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_job_setting_analysis/api.py
--rw-r--r--   0        0        0     4703 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_job_setting_analysis/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list/__init__.py
--rw-r--r--   0        0        0     7085 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list/api.py
--rw-r--r--   0        0        0    13578 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list_namespace/__init__.py
--rw-r--r--   0        0        0     4324 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list_namespace/api.py
--rw-r--r--   0        0        0     6989 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_list_namespace/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_namespace/__init__.py
--rw-r--r--   0        0        0     3960 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_namespace/api.py
--rw-r--r--   0        0        0     7126 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_namespace/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_store/__init__.py
--rw-r--r--   0        0        0     7999 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_store/api.py
--rw-r--r--   0        0        0    12891 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/feature_store/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/historical_feature_table/__init__.py
--rw-r--r--   0        0        0     5367 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/historical_feature_table/api.py
--rw-r--r--   0        0        0     5557 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/historical_feature_table/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/item_table/__init__.py
--rw-r--r--   0        0        0     3832 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/item_table/api.py
--rw-r--r--   0        0        0     1514 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/item_table/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/observation_table/__init__.py
--rw-r--r--   0        0        0     4768 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/observation_table/api.py
--rw-r--r--   0        0        0     3157 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/observation_table/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/periodic_tasks/__init__.py
--rw-r--r--   0        0        0     1583 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/periodic_tasks/api.py
--rw-r--r--   0        0        0      540 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/periodic_tasks/controller.py
--rw-r--r--   0        0        0    16128 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/registry.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/relationship_info/__init__.py
--rw-r--r--   0        0        0     4202 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/relationship_info/api.py
--rw-r--r--   0        0        0     4602 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/relationship_info/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/scd_table/__init__.py
--rw-r--r--   0        0        0     3768 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/scd_table/api.py
--rw-r--r--   0        0        0     1969 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/scd_table/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/semantic/__init__.py
--rw-r--r--   0        0        0     3733 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/semantic/api.py
--rw-r--r--   0        0        0     1362 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/semantic/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/table/__init__.py
--rw-r--r--   0        0        0     1469 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/table/api.py
--rw-r--r--   0        0        0      464 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/table/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/task/__init__.py
--rw-r--r--   0        0        0     1045 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/task/api.py
--rw-r--r--   0        0        0     1837 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/task/controller.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/temp_data/__init__.py
--rw-r--r--   0        0        0      581 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/temp_data/api.py
--rw-r--r--   0        0        0     1353 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/routes/temp_data/controller.py
--rw-r--r--   0        0        0      180 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/__init__.py
--rw-r--r--   0        0        0     1431 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/batch_feature_table.py
--rw-r--r--   0        0        0      842 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/batch_request_table.py
--rw-r--r--   0        0        0     1511 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/catalog.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/common/__init__.py
--rw-r--r--   0        0        0     1068 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/common/base.py
--rw-r--r--   0        0        0     3662 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/common/operation.py
--rw-r--r--   0        0        0     1508 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/context.py
--rw-r--r--   0        0        0     3658 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/credential.py
--rw-r--r--   0        0        0     1686 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/deployment.py
--rw-r--r--   0        0        0      981 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/dimension_table.py
--rw-r--r--   0        0        0     1684 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/entity.py
--rw-r--r--   0        0        0     2391 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/event_table.py
--rw-r--r--   0        0        0     7337 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature.py
--rw-r--r--   0        0        0     4664 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature_job_setting_analysis.py
--rw-r--r--   0        0        0     3758 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature_list.py
--rw-r--r--   0        0        0     1460 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature_list_namespace.py
--rw-r--r--   0        0        0     1965 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature_namespace.py
--rw-r--r--   0        0        0     3589 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/feature_store.py
--rw-r--r--   0        0        0     1591 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/historical_feature_table.py
--rw-r--r--   0        0        0    10583 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/info.py
--rw-r--r--   0        0        0      991 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/item_table.py
--rw-r--r--   0        0        0      599 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/materialized_table.py
--rw-r--r--   0        0        0      909 2023-06-05 04:27:45.239716 featurebyte-0.3.0/featurebyte/schema/observation_table.py
--rw-r--r--   0        0        0      459 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/periodic_task.py
--rw-r--r--   0        0        0     1460 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/relationship_info.py
--rw-r--r--   0        0        0     1190 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/request_table.py
--rw-r--r--   0        0        0     1376 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/scd_table.py
--rw-r--r--   0        0        0      914 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/semantic.py
--rw-r--r--   0        0        0     2415 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/table.py
--rw-r--r--   0        0        0     1012 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/task.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/__init__.py
--rw-r--r--   0        0        0      333 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/progress.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/__init__.py
--rw-r--r--   0        0        0     2829 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/base.py
--rw-r--r--   0        0        0      520 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/batch_feature_create.py
--rw-r--r--   0        0        0      610 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/batch_feature_table.py
--rw-r--r--   0        0        0      602 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/batch_request_table.py
--rw-r--r--   0        0        0     1382 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/deployment_create_update.py
--rw-r--r--   0        0        0     1328 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/feature_job_setting_analysis.py
--rw-r--r--   0        0        0      725 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/historical_feature_table.py
--rw-r--r--   0        0        0     1215 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/materialized_table_delete.py
--rw-r--r--   0        0        0      589 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/observation_table.py
--rw-r--r--   0        0        0      500 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/test.py
--rw-r--r--   0        0        0      416 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/schema/worker/task/tile.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/__init__.py
--rw-r--r--   0        0        0    28027 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/base_document.py
--rw-r--r--   0        0        0      524 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/base_service.py
--rw-r--r--   0        0        0     5195 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/base_table_document.py
--rw-r--r--   0        0        0     1846 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/batch_feature_table.py
--rw-r--r--   0        0        0     2715 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/batch_request_table.py
--rw-r--r--   0        0        0     2303 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/catalog.py
--rw-r--r--   0        0        0     5515 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/context.py
--rw-r--r--   0        0        0     5558 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/credential.py
--rw-r--r--   0        0        0     4782 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/default_version_mode.py
--rw-r--r--   0        0        0    18158 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/deploy.py
--rw-r--r--   0        0        0      478 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/deployment.py
--rw-r--r--   0        0        0      674 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/dimension_table.py
--rw-r--r--   0        0        0     2199 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/entity.py
--rw-r--r--   0        0        0     7515 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/entity_validation.py
--rw-r--r--   0        0        0      618 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/event_table.py
--rw-r--r--   0        0        0    11435 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature.py
--rw-r--r--   0        0        0     3535 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_job_setting_analysis.py
--rw-r--r--   0        0        0    10881 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_list.py
--rw-r--r--   0        0        0      572 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_list_namespace.py
--rw-r--r--   0        0        0     4048 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_list_status.py
--rw-r--r--   0        0        0      564 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_namespace.py
--rw-r--r--   0        0        0    15409 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_readiness.py
--rw-r--r--   0        0        0      603 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_store.py
--rw-r--r--   0        0        0    15423 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/feature_store_warehouse.py
--rw-r--r--   0        0        0     2939 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/historical_feature_table.py
--rw-r--r--   0        0        0    42750 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/info.py
--rw-r--r--   0        0        0      604 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/item_table.py
--rw-r--r--   0        0        0     4788 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/materialized_table.py
--rw-r--r--   0        0        0     4396 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/mixin.py
--rw-r--r--   0        0        0     6202 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/observation_table.py
--rw-r--r--   0        0        0     9257 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/online_enable.py
--rw-r--r--   0        0        0     4504 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/online_serving.py
--rw-r--r--   0        0        0     7266 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/parent_serving.py
--rw-r--r--   0        0        0      437 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/periodic_task.py
--rw-r--r--   0        0        0    25370 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/preview.py
--rw-r--r--   0        0        0     9285 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/relationship.py
--rw-r--r--   0        0        0     2303 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/relationship_info.py
--rw-r--r--   0        0        0      590 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/scd_table.py
--rw-r--r--   0        0        0      600 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/semantic.py
--rw-r--r--   0        0        0     2703 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/session_manager.py
--rw-r--r--   0        0        0     7932 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/session_validator.py
--rw-r--r--   0        0        0     1051 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/table.py
--rw-r--r--   0        0        0    16758 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/table_columns_info.py
--rw-r--r--   0        0        0     2241 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/table_status.py
--rw-r--r--   0        0        0    10862 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/task_manager.py
--rw-r--r--   0        0        0      779 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/user_service.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/validator/__init__.py
--rw-r--r--   0        0        0     3704 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/validator/materialized_table_delete.py
--rw-r--r--   0        0        0    11567 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/validator/production_ready_validator.py
--rw-r--r--   0        0        0    15798 2023-06-05 04:27:45.243716 featurebyte-0.3.0/featurebyte/service/version.py
--rw-r--r--   0        0        0    14878 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/service/view_construction.py
--rw-r--r--   0        0        0     4180 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/service/working_schema.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/__init__.py
--rw-r--r--   0        0        0    26478 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/base.py
--rw-r--r--   0        0        0    14634 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/base_spark.py
--rw-r--r--   0        0        0     5643 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/databricks.py
--rw-r--r--   0        0        0      434 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/enum.py
--rw-r--r--   0        0        0     4993 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/hive.py
--rw-r--r--   0        0        0     5107 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/manager.py
--rw-r--r--   0        0        0     7592 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/simple_storage.py
--rw-r--r--   0        0        0    14756 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/snowflake.py
--rw-r--r--   0        0        0     8393 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/spark.py
--rw-r--r--   0        0        0     3479 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/session/sqlite.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/__init__.py
--rw-r--r--   0        0        0     3198 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/base.py
--rw-r--r--   0        0        0     2743 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/common.py
--rw-r--r--   0        0        0        6 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/databricks/.gitignore
--rw-r--r--   0        0        0      957 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql
--rw-r--r--   0        0        0      476 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_ENTROPY.sql
--rw-r--r--   0        0        0      171 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT.sql
--rw-r--r--   0        0        0      610 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql
--rw-r--r--   0        0        0      177 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_VALUE.sql
--rw-r--r--   0        0        0      188 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_NUM_UNIQUE.sql
--rw-r--r--   0        0        0     1491 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_GET_RANK.sql
--rw-r--r--   0        0        0      397 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_GET_RELATIVE_FREQUENCY.sql
--rw-r--r--   0        0        0      559 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql
--rw-r--r--   0        0        0      559 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql
--rw-r--r--   0        0        0      653 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql
--rw-r--r--   0        0        0      292 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/T_ONLINE_STORE_MAPPING.sql
--rw-r--r--   0        0        0      299 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/T_TILE_FEATURE_MAPPING.sql
--rw-r--r--   0        0        0      212 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/T_TILE_JOB_MONITOR.sql
--rw-r--r--   0        0        0      153 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/T_TILE_MONITOR_SUMMARY.sql
--rw-r--r--   0        0        0      526 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql
--rw-r--r--   0        0        0        6 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/.gitignore
--rw-r--r--   0        0        0      304 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/T_ONLINE_STORE_MAPPING.sql
--rw-r--r--   0        0        0      311 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/T_TILE_FEATURE_MAPPING.sql
--rw-r--r--   0        0        0      228 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/T_TILE_JOB_MONITOR.sql
--rw-r--r--   0        0        0      191 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/T_TILE_MONITOR_SUMMARY.sql
--rw-r--r--   0        0        0      531 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/T_TILE_REGISTRY.sql
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/spark/__init__.py
--rw-r--r--   0        0        0    29690 2023-06-05 04:29:41.147176 featurebyte-0.3.0/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar
--rw-r--r--   0        0        0     2001 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_common.py
--rw-r--r--   0        0        0     5878 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_generate.py
--rw-r--r--   0        0        0     3566 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_generate_entity_tracking.py
--rw-r--r--   0        0        0     9817 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_generate_schedule.py
--rw-r--r--   0        0        0     7297 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_monitor.py
--rw-r--r--   0        0        0     3491 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_registry.py
--rw-r--r--   0        0        0     6139 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/sql/tile_schedule_online_store.py
--rw-r--r--   0        0        0      239 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/storage/__init__.py
--rw-r--r--   0        0        0     4999 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/storage/base.py
--rw-r--r--   0        0        0     3640 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/storage/local.py
--rw-r--r--   0        0        0      415 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/storage/local_temp.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/tile/__init__.py
--rw-r--r--   0        0        0    14347 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/tile/manager.py
--rw-r--r--   0        0        0     2918 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/tile/scheduler.py
--rw-r--r--   0        0        0      411 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/tile/sql_template.py
--rw-r--r--   0        0        0    28505 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/tile/tile_cache.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/__init__.py
--rw-r--r--   0        0        0     1909 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/credential.py
--rw-r--r--   0        0        0     1532 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/messaging.py
--rw-r--r--   0        0        0      534 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/persistent.py
--rw-r--r--   0        0        0        0 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/snowflake/__init__.py
--rw-r--r--   0        0        0      462 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/snowflake/sql.py
--rw-r--r--   0        0        0      765 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/utils/storage.py
--rw-r--r--   0        0        0     1537 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/__init__.py
--rw-r--r--   0        0        0      170 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/enum.py
--rw-r--r--   0        0        0     3873 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/process_store.py
--rw-r--r--   0        0        0     1159 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/progress.py
--rw-r--r--   0        0        0     2502 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/schedulers.py
--rw-r--r--   0        0        0      107 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/start.py
--rw-r--r--   0        0        0      214 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/base.py
--rw-r--r--   0        0        0     4603 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/batch_feature_create.py
--rw-r--r--   0        0        0     3718 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/batch_feature_table.py
--rw-r--r--   0        0        0     2243 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/batch_request_table.py
--rw-r--r--   0        0        0     1795 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/deployment_create_update.py
--rw-r--r--   0        0        0     7130 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/feature_job_setting_analysis.py
--rw-r--r--   0        0        0     3954 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/historical_feature_table.py
--rw-r--r--   0        0        0     4321 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/materialized_table_delete.py
--rw-r--r--   0        0        0     2604 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/mixin.py
--rw-r--r--   0        0        0     2226 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/observation_table.py
--rw-r--r--   0        0        0      626 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/test_task.py
--rw-r--r--   0        0        0     1904 2023-06-05 04:27:45.247716 featurebyte-0.3.0/featurebyte/worker/task/tile_task.py
--rw-r--r--   0        0        0     5407 2023-06-05 04:27:45.251716 featurebyte-0.3.0/featurebyte/worker/task_executor.py
--rw-r--r--   0        0        0     7717 2023-06-05 04:28:21.203564 featurebyte-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    23050 1970-01-01 00:00:00.000000 featurebyte-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-06-08 15:53:14.865277 featurebyte-0.3.1/LICENSE
+-rw-r--r--   0        0        0    19816 2023-06-08 15:53:14.865277 featurebyte-0.3.1/README.md
+-rw-r--r--   0        0        0    14195 2023-06-08 15:53:14.865277 featurebyte-0.3.1/featurebyte/__init__.py
+-rw-r--r--   0        0        0     2017 2023-06-08 15:53:14.865277 featurebyte-0.3.1/featurebyte/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.865277 featurebyte-0.3.1/featurebyte/api/__init__.py
+-rw-r--r--   0        0        0    30557 2023-06-08 15:53:14.865277 featurebyte-0.3.1/featurebyte/api/api_object.py
+-rw-r--r--   0        0        0     3975 2023-06-08 15:53:14.865277 featurebyte-0.3.1/featurebyte/api/api_object_util.py
+-rw-r--r--   0        0        0     4985 2023-06-08 15:53:14.865277 featurebyte-0.3.1/featurebyte/api/asat_aggregator.py
+-rw-r--r--   0        0        0     5521 2023-06-08 15:53:14.865277 featurebyte-0.3.1/featurebyte/api/base_aggregator.py
+-rw-r--r--   0        0        0    37589 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/base_table.py
+-rw-r--r--   0        0        0     4790 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/batch_feature_table.py
+-rw-r--r--   0        0        0     5019 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/batch_request_table.py
+-rw-r--r--   0        0        0    35381 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/catalog.py
+-rw-r--r--   0        0        0     1475 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/catalog_decorator.py
+-rw-r--r--   0        0        0    10842 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/catalog_get_by_id_mixin.py
+-rw-r--r--   0        0        0    11517 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/change_view.py
+-rw-r--r--   0        0        0     6600 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/credential.py
+-rw-r--r--   0        0        0     6540 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/data_source.py
+-rw-r--r--   0        0        0    13660 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/deployment.py
+-rw-r--r--   0        0        0     9699 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/dimension_table.py
+-rw-r--r--   0        0        0     3107 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/dimension_view.py
+-rw-r--r--   0        0        0    12242 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/entity.py
+-rw-r--r--   0        0        0    22561 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/event_table.py
+-rw-r--r--   0        0        0    16044 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/event_view.py
+-rw-r--r--   0        0        0    46149 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/feature.py
+-rw-r--r--   0        0        0    15414 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/feature_group.py
+-rw-r--r--   0        0        0    15001 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/feature_job.py
+-rw-r--r--   0        0        0     8770 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    62689 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/feature_list.py
+-rw-r--r--   0        0        0     4116 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/feature_namespace.py
+-rw-r--r--   0        0        0    10016 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/feature_store.py
+-rw-r--r--   0        0        0     1999 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/feature_util.py
+-rw-r--r--   0        0        0      557 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/feature_validation_util.py
+-rw-r--r--   0        0        0    18206 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/groupby.py
+-rw-r--r--   0        0        0     4927 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/historical_feature_table.py
+-rw-r--r--   0        0        0    16661 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/item_table.py
+-rw-r--r--   0        0        0    11752 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/item_view.py
+-rw-r--r--   0        0        0     2909 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/lag.py
+-rw-r--r--   0        0        0     4909 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/materialized_table.py
+-rw-r--r--   0        0        0     4952 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/observation_table.py
+-rw-r--r--   0        0        0      721 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/periodic_task.py
+-rw-r--r--   0        0        0     8442 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/relationship.py
+-rw-r--r--   0        0        0     3474 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/request_column.py
+-rw-r--r--   0        0        0     5018 2023-06-08 15:53:14.869277 featurebyte-0.3.1/featurebyte/api/savable_api_object.py
+-rw-r--r--   0        0        0    21162 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/scd_table.py
+-rw-r--r--   0        0        0     6023 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/scd_view.py
+-rw-r--r--   0        0        0     3119 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/simple_aggregator.py
+-rw-r--r--   0        0        0    46157 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/source_table.py
+-rw-r--r--   0        0        0     5522 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/table.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/templates/online_serving/__init__.py
+-rw-r--r--   0        0        0      707 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/templates/online_serving/python.tpl
+-rw-r--r--   0        0        0      132 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/templates/online_serving/shell.tpl
+-rw-r--r--   0        0        0    60163 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/view.py
+-rw-r--r--   0        0        0     8368 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/window_aggregator.py
+-rw-r--r--   0        0        0     1607 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/api/window_validator.py
+-rw-r--r--   0        0        0     6870 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/app.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/__init__.py
+-rw-r--r--   0        0        0     3116 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/date_util.py
+-rw-r--r--   0        0        0      956 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/descriptor.py
+-rw-r--r--   0        0        0      636 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/dict_util.py
+-rw-r--r--   0        0        0     2090 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/doc_util.py
+-rw-r--r--   0        0        0      692 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/allowed_classes.py
+-rw-r--r--   0        0        0    16036 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/autodoc_processor.py
+-rw-r--r--   0        0        0     1419 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/constants.py
+-rw-r--r--   0        0        0     4280 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/custom_nav.py
+-rw-r--r--   0        0        0     8560 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/doc_types.py
+-rw-r--r--   0        0        0    43070 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/documentation_layout.py
+-rw-r--r--   0        0        0     7430 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/extract_csv.py
+-rw-r--r--   0        0        0     3479 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/formatters.py
+-rw-r--r--   0        0        0    31657 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/gen_ref_pages_docs_builder.py
+-rw-r--r--   0        0        0      877 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/markdown_extension/extension.py
+-rw-r--r--   0        0        0     5660 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/pydantic_field_docs.py
+-rw-r--r--   0        0        0    16371 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/resource_extractor.py
+-rw-r--r--   0        0        0      519 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/resource_util.py
+-rw-r--r--   0        0        0      200 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/documentation/util.py
+-rw-r--r--   0        0        0     1262 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/env_util.py
+-rw-r--r--   0        0        0     6740 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/formatting_util.py
+-rw-r--r--   0        0        0     3925 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/join_utils.py
+-rw-r--r--   0        0        0     4198 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/model_util.py
+-rw-r--r--   0        0        0      815 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/path_util.py
+-rw-r--r--   0        0        0     1062 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/progress.py
+-rw-r--r--   0        0        0      451 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/singleton.py
+-rw-r--r--   0        0        0     1084 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/tile_util.py
+-rw-r--r--   0        0        0     2629 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/typing.py
+-rw-r--r--   0        0        0    10491 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/utils.py
+-rw-r--r--   0        0        0     4699 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/common/validator.py
+-rw-r--r--   0        0        0    13279 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/config.py
+-rw-r--r--   0        0        0     1366 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/core/accessor/__init__.py
+-rw-r--r--   0        0        0    15412 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/core/accessor/count_dict.py
+-rw-r--r--   0        0        0    23735 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/core/accessor/datetime.py
+-rw-r--r--   0        0        0    10051 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/core/accessor/feature_datetime.py
+-rw-r--r--   0        0        0     8454 2023-06-08 15:53:14.873277 featurebyte-0.3.1/featurebyte/core/accessor/feature_string.py
+-rw-r--r--   0        0        0    15765 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/core/accessor/string.py
+-rw-r--r--   0        0        0     8902 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/core/frame.py
+-rw-r--r--   0        0        0    11843 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/core/generic.py
+-rw-r--r--   0        0        0    16742 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/core/mixin.py
+-rw-r--r--   0        0        0    37956 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/core/series.py
+-rw-r--r--   0        0        0     1484 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/core/timedelta.py
+-rw-r--r--   0        0        0     6393 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/datasets/__init__.py
+-rw-r--r--   0        0        0      697 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/datasets/__main__.py
+-rw-r--r--   0        0        0     5546 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/datasets/app.py
+-rw-r--r--   0        0        0     3125 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/datasets/creditcard.sql
+-rw-r--r--   0        0        0     1154 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/datasets/doctest_grocery.sql
+-rw-r--r--   0        0        0     2200 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/datasets/grocery.sql
+-rw-r--r--   0        0        0     5757 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/datasets/healthcare.sql
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/docker/__init__.py
+-rw-r--r--   0        0        0     4518 2023-06-08 15:53:50.449892 featurebyte-0.3.1/featurebyte/docker/featurebyte.yml
+-rw-r--r--   0        0        0    10343 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/docker/manager.py
+-rw-r--r--   0        0        0     9199 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/enum.py
+-rw-r--r--   0        0        0     9244 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/exception.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/feature_manager/__init__.py
+-rw-r--r--   0        0        0    10392 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/feature_manager/manager.py
+-rw-r--r--   0        0        0     2911 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/feature_manager/model.py
+-rw-r--r--   0        0        0     3997 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/feature_manager/sql_template.py
+-rw-r--r--   0        0        0     3667 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/feature_utility.py
+-rw-r--r--   0        0        0     4145 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/logging.py
+-rw-r--r--   0        0        0     7839 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/migration/__init__.py
+-rw-r--r--   0        0        0      604 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/migration/migration_data_service.py
+-rw-r--r--   0        0        0     1664 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/migration/model.py
+-rw-r--r--   0        0        0     8423 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/migration/run.py
+-rw-r--r--   0        0        0     1442 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/migration/service/__init__.py
+-rw-r--r--   0        0        0     9762 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/migration/service/data_warehouse.py
+-rw-r--r--   0        0        0     9181 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/migration/service/mixin.py
+-rw-r--r--   0        0        0      646 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/__init__.py
+-rw-r--r--   0        0        0    10813 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/base.py
+-rw-r--r--   0        0        0      617 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/batch_feature_table.py
+-rw-r--r--   0        0        0     1726 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/batch_request_table.py
+-rw-r--r--   0        0        0     2377 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/catalog.py
+-rw-r--r--   0        0        0     1572 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/context.py
+-rw-r--r--   0        0        0     8513 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/credential.py
+-rw-r--r--   0        0        0     1333 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/deployment.py
+-rw-r--r--   0        0        0     2026 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/dimension_table.py
+-rw-r--r--   0        0        0     3618 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/entity.py
+-rw-r--r--   0        0        0     3051 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/entity_validation.py
+-rw-r--r--   0        0        0     3551 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/event_table.py
+-rw-r--r--   0        0        0    11926 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/feature.py
+-rw-r--r--   0        0        0     3750 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    21070 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/feature_list.py
+-rw-r--r--   0        0        0     7606 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/feature_store.py
+-rw-r--r--   0        0        0      644 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/historical_feature_table.py
+-rw-r--r--   0        0        0     2919 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/item_table.py
+-rw-r--r--   0        0        0     1620 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/materialized_table.py
+-rw-r--r--   0        0        0     2113 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/observation_table.py
+-rw-r--r--   0        0        0     3738 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/online_store.py
+-rw-r--r--   0        0        0     1433 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/parent_serving.py
+-rw-r--r--   0        0        0     2891 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/periodic_task.py
+-rw-r--r--   0        0        0     1492 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/persistent.py
+-rw-r--r--   0        0        0     1024 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/proxy_table.py
+-rw-r--r--   0        0        0     4330 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/relationship.py
+-rw-r--r--   0        0        0      944 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/relationship_analysis.py
+-rw-r--r--   0        0        0     7865 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/request_input.py
+-rw-r--r--   0        0        0     3554 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/scd_table.py
+-rw-r--r--   0        0        0     1435 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/semantic.py
+-rw-r--r--   0        0        0     1085 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/task.py
+-rw-r--r--   0        0        0     3269 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/models/tile.py
+-rw-r--r--   0        0        0      154 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/persistent/__init__.py
+-rw-r--r--   0        0        0     9396 2023-06-08 15:53:14.877277 featurebyte-0.3.1/featurebyte/persistent/audit.py
+-rw-r--r--   0        0        0    21712 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/persistent/base.py
+-rw-r--r--   0        0        0     9824 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/persistent/mongo.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/__init__.py
+-rw-r--r--   0        0        0     2533 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/algorithm.py
+-rw-r--r--   0        0        0     2988 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/enum.py
+-rw-r--r--   0        0        0    16847 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/graph.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/graph_node/__init__.py
+-rw-r--r--   0        0        0     4592 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/graph_node/base.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/model/__init__.py
+-rw-r--r--   0        0        0      873 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/model/column_info.py
+-rw-r--r--   0        0        0    12700 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/model/common_table.py
+-rw-r--r--   0        0        0     1707 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/model/critical_data_info.py
+-rw-r--r--   0        0        0     6699 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/model/feature_job_setting.py
+-rw-r--r--   0        0        0    19282 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/model/graph.py
+-rw-r--r--   0        0        0    23872 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/model/table.py
+-rw-r--r--   0        0        0     1076 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/__init__.py
+-rw-r--r--   0        0        0     5236 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/agg_func.py
+-rw-r--r--   0        0        0    28374 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/base.py
+-rw-r--r--   0        0        0     5224 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/binary.py
+-rw-r--r--   0        0        0    17953 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/cleaning_operation.py
+-rw-r--r--   0        0        0     7797 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/count_dict.py
+-rw-r--r--   0        0        0     7293 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/date.py
+-rw-r--r--   0        0        0    60575 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/generic.py
+-rw-r--r--   0        0        0    17049 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/input.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/metadata/__init__.py
+-rw-r--r--   0        0        0      873 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/metadata/column.py
+-rw-r--r--   0        0        0    21929 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/metadata/operation.py
+-rw-r--r--   0        0        0    19397 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/metadata/sdk_code.py
+-rw-r--r--   0        0        0       47 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/metadata/templates/sdk_code.tpl
+-rw-r--r--   0        0        0     7393 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/mixin.py
+-rw-r--r--   0        0        0    21084 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/nested.py
+-rw-r--r--   0        0        0     3272 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/request.py
+-rw-r--r--   0        0        0     2054 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/scalar.py
+-rw-r--r--   0        0        0     6696 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/schema.py
+-rw-r--r--   0        0        0     5461 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/string.py
+-rw-r--r--   0        0        0     4824 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/unary.py
+-rw-r--r--   0        0        0     1042 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/node/validator.py
+-rw-r--r--   0        0        0     1050 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/pruning_util.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/sql/__init__.py
+-rw-r--r--   0        0        0    27339 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/sql/adapter.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/__init__.py
+-rw-r--r--   0        0        0     7198 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/asat.py
+-rw-r--r--   0        0        0    16281 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/base.py
+-rw-r--r--   0        0        0     5739 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/item.py
+-rw-r--r--   0        0        0     3801 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/latest.py
+-rw-r--r--   0        0        0     9549 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/lookup.py
+-rw-r--r--   0        0        0     3811 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/request_table.py
+-rw-r--r--   0        0        0    26795 2023-06-08 15:53:14.881277 featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/window.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/__init__.py
+-rw-r--r--   0        0        0     5560 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/aggregate.py
+-rw-r--r--   0        0        0    12647 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/base.py
+-rw-r--r--   0        0        0     2723 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/binary.py
+-rw-r--r--   0        0        0     5740 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/count_dict.py
+-rw-r--r--   0        0        0    10724 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/datetime.py
+-rw-r--r--   0        0        0     7163 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/generic.py
+-rw-r--r--   0        0        0     2409 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/groupby.py
+-rw-r--r--   0        0        0     2593 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/input.py
+-rw-r--r--   0        0        0     1449 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/is_in.py
+-rw-r--r--   0        0        0     6208 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/join.py
+-rw-r--r--   0        0        0     6138 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/join_feature.py
+-rw-r--r--   0        0        0     2291 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/literal.py
+-rw-r--r--   0        0        0      878 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/request.py
+-rw-r--r--   0        0        0     8360 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/string.py
+-rw-r--r--   0        0        0    11741 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/tile.py
+-rw-r--r--   0        0        0     5170 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/track_changes.py
+-rw-r--r--   0        0        0     5157 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/unary.py
+-rw-r--r--   0        0        0     2536 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/ast/util.py
+-rw-r--r--   0        0        0     7070 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/builder.py
+-rw-r--r--   0        0        0     4909 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/common.py
+-rw-r--r--   0        0        0     1704 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/dataframe.py
+-rw-r--r--   0        0        0     1966 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/expression.py
+-rw-r--r--   0        0        0    20348 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/feature_compute.py
+-rw-r--r--   0        0        0    28059 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/feature_historical.py
+-rw-r--r--   0        0        0     3694 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/feature_preview.py
+-rw-r--r--   0        0        0     4449 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/groupby_helper.py
+-rw-r--r--   0        0        0      426 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/interpreter/__init__.py
+-rw-r--r--   0        0        0     3344 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/interpreter/base.py
+-rw-r--r--   0        0        0    27934 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/interpreter/preview.py
+-rw-r--r--   0        0        0     6685 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/interpreter/tile.py
+-rw-r--r--   0        0        0     4027 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/materialisation.py
+-rw-r--r--   0        0        0    17988 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/online_serving.py
+-rw-r--r--   0        0        0      659 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/online_serving_util.py
+-rw-r--r--   0        0        0     5042 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/parent_serving.py
+-rw-r--r--   0        0        0    15948 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/scd_helper.py
+-rw-r--r--   0        0        0    20783 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/specs.py
+-rw-r--r--   0        0        0     2206 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/template.py
+-rw-r--r--   0        0        0    13029 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/tile_compute.py
+-rw-r--r--   0        0        0     3793 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/tile_util.py
+-rw-r--r--   0        0        0     9354 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/sql/tiling.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/transform/__init__.py
+-rw-r--r--   0        0        0     5184 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/transform/base.py
+-rw-r--r--   0        0        0     5201 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/transform/flattening.py
+-rw-r--r--   0        0        0     6716 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/transform/operation_structure.py
+-rw-r--r--   0        0        0    20327 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/transform/pruning.py
+-rw-r--r--   0        0        0    10248 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/transform/reconstruction.py
+-rw-r--r--   0        0        0    13262 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/transform/sdk_code.py
+-rw-r--r--   0        0        0     5951 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/query_graph/util.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/routes/__init__.py
+-rw-r--r--   0        0        0     4367 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/routes/app_container.py
+-rw-r--r--   0        0        0     4340 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/routes/app_container_config.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/routes/batch_feature_table/__init__.py
+-rw-r--r--   0        0        0     4832 2023-06-08 15:53:14.885278 featurebyte-0.3.1/featurebyte/routes/batch_feature_table/api.py
+-rw-r--r--   0        0        0     4616 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/batch_feature_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/batch_request_table/__init__.py
+-rw-r--r--   0        0        0     4860 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/batch_request_table/api.py
+-rw-r--r--   0        0        0     3137 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/batch_request_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/catalog/__init__.py
+-rw-r--r--   0        0        0     4307 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/catalog/api.py
+-rw-r--r--   0        0        0     2524 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/catalog/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/common/__init__.py
+-rw-r--r--   0        0        0    10579 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/common/base.py
+-rw-r--r--   0        0        0     3761 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/common/base_materialized_table.py
+-rw-r--r--   0        0        0     5515 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/common/base_table.py
+-rw-r--r--   0        0        0      886 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/common/schema.py
+-rw-r--r--   0        0        0      400 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/common/util.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/context/__init__.py
+-rw-r--r--   0        0        0     3107 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/context/api.py
+-rw-r--r--   0        0        0     1596 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/context/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/credential/__init__.py
+-rw-r--r--   0        0        0     4605 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/credential/api.py
+-rw-r--r--   0        0        0     3071 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/credential/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/deployment/__init__.py
+-rw-r--r--   0        0        0     5604 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/deployment/api.py
+-rw-r--r--   0        0        0    10416 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/deployment/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/dimension_table/__init__.py
+-rw-r--r--   0        0        0     4181 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/dimension_table/api.py
+-rw-r--r--   0        0        0     1674 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/dimension_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/entity/__init__.py
+-rw-r--r--   0        0        0     5145 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/entity/api.py
+-rw-r--r--   0        0        0     2718 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/entity/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/event_table/__init__.py
+-rw-r--r--   0        0        0     4689 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/event_table/api.py
+-rw-r--r--   0        0        0     1818 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/event_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature/__init__.py
+-rw-r--r--   0        0        0     6378 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature/api.py
+-rw-r--r--   0        0        0    15348 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_job_setting_analysis/__init__.py
+-rw-r--r--   0        0        0     5449 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_job_setting_analysis/api.py
+-rw-r--r--   0        0        0     4703 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_job_setting_analysis/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_list/__init__.py
+-rw-r--r--   0        0        0     7085 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_list/api.py
+-rw-r--r--   0        0        0    13578 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_list/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_list_namespace/__init__.py
+-rw-r--r--   0        0        0     4324 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_list_namespace/api.py
+-rw-r--r--   0        0        0     6989 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_list_namespace/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_namespace/__init__.py
+-rw-r--r--   0        0        0     3960 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_namespace/api.py
+-rw-r--r--   0        0        0     7126 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_namespace/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_store/__init__.py
+-rw-r--r--   0        0        0     7999 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_store/api.py
+-rw-r--r--   0        0        0    12891 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/feature_store/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/historical_feature_table/__init__.py
+-rw-r--r--   0        0        0     5367 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/historical_feature_table/api.py
+-rw-r--r--   0        0        0     5557 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/historical_feature_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/item_table/__init__.py
+-rw-r--r--   0        0        0     3832 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/item_table/api.py
+-rw-r--r--   0        0        0     1514 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/item_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/observation_table/__init__.py
+-rw-r--r--   0        0        0     4768 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/observation_table/api.py
+-rw-r--r--   0        0        0     3157 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/observation_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/periodic_tasks/__init__.py
+-rw-r--r--   0        0        0     1583 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/periodic_tasks/api.py
+-rw-r--r--   0        0        0      540 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/periodic_tasks/controller.py
+-rw-r--r--   0        0        0    16128 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/registry.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/relationship_info/__init__.py
+-rw-r--r--   0        0        0     4202 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/relationship_info/api.py
+-rw-r--r--   0        0        0     4602 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/relationship_info/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/scd_table/__init__.py
+-rw-r--r--   0        0        0     3768 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/scd_table/api.py
+-rw-r--r--   0        0        0     1969 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/scd_table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/semantic/__init__.py
+-rw-r--r--   0        0        0     3733 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/semantic/api.py
+-rw-r--r--   0        0        0     1362 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/semantic/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/table/__init__.py
+-rw-r--r--   0        0        0     1469 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/table/api.py
+-rw-r--r--   0        0        0      464 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/table/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/task/__init__.py
+-rw-r--r--   0        0        0     1045 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/task/api.py
+-rw-r--r--   0        0        0     1837 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/task/controller.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/temp_data/__init__.py
+-rw-r--r--   0        0        0      581 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/temp_data/api.py
+-rw-r--r--   0        0        0     1353 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/routes/temp_data/controller.py
+-rw-r--r--   0        0        0      180 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/schema/__init__.py
+-rw-r--r--   0        0        0     1431 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/schema/batch_feature_table.py
+-rw-r--r--   0        0        0      842 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/schema/batch_request_table.py
+-rw-r--r--   0        0        0     1511 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/schema/catalog.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/schema/common/__init__.py
+-rw-r--r--   0        0        0     1068 2023-06-08 15:53:14.889278 featurebyte-0.3.1/featurebyte/schema/common/base.py
+-rw-r--r--   0        0        0     3662 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/common/operation.py
+-rw-r--r--   0        0        0     1508 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/context.py
+-rw-r--r--   0        0        0     3658 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/credential.py
+-rw-r--r--   0        0        0     1686 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/deployment.py
+-rw-r--r--   0        0        0      981 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/dimension_table.py
+-rw-r--r--   0        0        0     1684 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/entity.py
+-rw-r--r--   0        0        0     2391 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/event_table.py
+-rw-r--r--   0        0        0     7337 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/feature.py
+-rw-r--r--   0        0        0     4664 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0     3758 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/feature_list.py
+-rw-r--r--   0        0        0     1460 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/feature_list_namespace.py
+-rw-r--r--   0        0        0     1965 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/feature_namespace.py
+-rw-r--r--   0        0        0     3589 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/feature_store.py
+-rw-r--r--   0        0        0     1591 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/historical_feature_table.py
+-rw-r--r--   0        0        0    10583 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/info.py
+-rw-r--r--   0        0        0      991 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/item_table.py
+-rw-r--r--   0        0        0      599 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/materialized_table.py
+-rw-r--r--   0        0        0      909 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/observation_table.py
+-rw-r--r--   0        0        0      459 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/periodic_task.py
+-rw-r--r--   0        0        0     1460 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/relationship_info.py
+-rw-r--r--   0        0        0     1190 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/request_table.py
+-rw-r--r--   0        0        0     1376 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/scd_table.py
+-rw-r--r--   0        0        0      914 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/semantic.py
+-rw-r--r--   0        0        0     2415 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/table.py
+-rw-r--r--   0        0        0     1012 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/task.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/__init__.py
+-rw-r--r--   0        0        0      333 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/progress.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/__init__.py
+-rw-r--r--   0        0        0     2829 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/base.py
+-rw-r--r--   0        0        0      520 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/batch_feature_create.py
+-rw-r--r--   0        0        0      610 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/batch_feature_table.py
+-rw-r--r--   0        0        0      602 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/batch_request_table.py
+-rw-r--r--   0        0        0     1382 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/deployment_create_update.py
+-rw-r--r--   0        0        0     1328 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0      725 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/historical_feature_table.py
+-rw-r--r--   0        0        0     1215 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/materialized_table_delete.py
+-rw-r--r--   0        0        0      589 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/observation_table.py
+-rw-r--r--   0        0        0      500 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/test.py
+-rw-r--r--   0        0        0      416 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/schema/worker/task/tile.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/__init__.py
+-rw-r--r--   0        0        0    28027 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/base_document.py
+-rw-r--r--   0        0        0      524 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/base_service.py
+-rw-r--r--   0        0        0     5195 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/base_table_document.py
+-rw-r--r--   0        0        0     1846 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/batch_feature_table.py
+-rw-r--r--   0        0        0     2715 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/batch_request_table.py
+-rw-r--r--   0        0        0     2303 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/catalog.py
+-rw-r--r--   0        0        0     5515 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/context.py
+-rw-r--r--   0        0        0     5558 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/credential.py
+-rw-r--r--   0        0        0     4782 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/default_version_mode.py
+-rw-r--r--   0        0        0    18162 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/deploy.py
+-rw-r--r--   0        0        0      478 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/deployment.py
+-rw-r--r--   0        0        0      674 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/dimension_table.py
+-rw-r--r--   0        0        0     2199 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/entity.py
+-rw-r--r--   0        0        0     7515 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/entity_validation.py
+-rw-r--r--   0        0        0      618 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/event_table.py
+-rw-r--r--   0        0        0    11435 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/feature.py
+-rw-r--r--   0        0        0     3535 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0    10881 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/feature_list.py
+-rw-r--r--   0        0        0      572 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/feature_list_namespace.py
+-rw-r--r--   0        0        0     4048 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/feature_list_status.py
+-rw-r--r--   0        0        0      564 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/feature_namespace.py
+-rw-r--r--   0        0        0    15409 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/feature_readiness.py
+-rw-r--r--   0        0        0      603 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/feature_store.py
+-rw-r--r--   0        0        0    15423 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/feature_store_warehouse.py
+-rw-r--r--   0        0        0     2939 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/historical_feature_table.py
+-rw-r--r--   0        0        0    42750 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/info.py
+-rw-r--r--   0        0        0      604 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/item_table.py
+-rw-r--r--   0        0        0     4788 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/materialized_table.py
+-rw-r--r--   0        0        0     4396 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/mixin.py
+-rw-r--r--   0        0        0     6202 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/observation_table.py
+-rw-r--r--   0        0        0     9257 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/online_enable.py
+-rw-r--r--   0        0        0     4504 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/online_serving.py
+-rw-r--r--   0        0        0     7266 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/parent_serving.py
+-rw-r--r--   0        0        0      437 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/periodic_task.py
+-rw-r--r--   0        0        0    25370 2023-06-08 15:53:14.893278 featurebyte-0.3.1/featurebyte/service/preview.py
+-rw-r--r--   0        0        0     9285 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/relationship.py
+-rw-r--r--   0        0        0     2303 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/relationship_info.py
+-rw-r--r--   0        0        0      590 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/scd_table.py
+-rw-r--r--   0        0        0      600 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/semantic.py
+-rw-r--r--   0        0        0     2703 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/session_manager.py
+-rw-r--r--   0        0        0     7932 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/session_validator.py
+-rw-r--r--   0        0        0     1051 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/table.py
+-rw-r--r--   0        0        0    16758 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/table_columns_info.py
+-rw-r--r--   0        0        0     2241 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/table_status.py
+-rw-r--r--   0        0        0    10862 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/task_manager.py
+-rw-r--r--   0        0        0      779 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/user_service.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/validator/__init__.py
+-rw-r--r--   0        0        0     3704 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/validator/materialized_table_delete.py
+-rw-r--r--   0        0        0    11567 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/validator/production_ready_validator.py
+-rw-r--r--   0        0        0    15798 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/version.py
+-rw-r--r--   0        0        0    14878 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/view_construction.py
+-rw-r--r--   0        0        0     4180 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/service/working_schema.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/__init__.py
+-rw-r--r--   0        0        0    26478 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/base.py
+-rw-r--r--   0        0        0    14634 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/base_spark.py
+-rw-r--r--   0        0        0     5643 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/databricks.py
+-rw-r--r--   0        0        0      434 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/enum.py
+-rw-r--r--   0        0        0     4993 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/hive.py
+-rw-r--r--   0        0        0     5107 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/manager.py
+-rw-r--r--   0        0        0     7592 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/simple_storage.py
+-rw-r--r--   0        0        0    14756 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/snowflake.py
+-rw-r--r--   0        0        0     8393 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/spark.py
+-rw-r--r--   0        0        0     3479 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/session/sqlite.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/__init__.py
+-rw-r--r--   0        0        0     3198 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/base.py
+-rw-r--r--   0        0        0     2743 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/common.py
+-rw-r--r--   0        0        0        6 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/databricks/.gitignore
+-rw-r--r--   0        0        0      957 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql
+-rw-r--r--   0        0        0      476 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_COUNT_DICT_ENTROPY.sql
+-rw-r--r--   0        0        0      171 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT.sql
+-rw-r--r--   0        0        0      610 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql
+-rw-r--r--   0        0        0      177 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_VALUE.sql
+-rw-r--r--   0        0        0      188 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_COUNT_DICT_NUM_UNIQUE.sql
+-rw-r--r--   0        0        0     1491 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_GET_RANK.sql
+-rw-r--r--   0        0        0      397 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_GET_RELATIVE_FREQUENCY.sql
+-rw-r--r--   0        0        0      559 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql
+-rw-r--r--   0        0        0      559 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql
+-rw-r--r--   0        0        0      653 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql
+-rw-r--r--   0        0        0      292 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/T_ONLINE_STORE_MAPPING.sql
+-rw-r--r--   0        0        0      299 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/T_TILE_FEATURE_MAPPING.sql
+-rw-r--r--   0        0        0      212 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/T_TILE_JOB_MONITOR.sql
+-rw-r--r--   0        0        0      153 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/T_TILE_MONITOR_SUMMARY.sql
+-rw-r--r--   0        0        0      526 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql
+-rw-r--r--   0        0        0        6 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/spark/.gitignore
+-rw-r--r--   0        0        0      304 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/spark/T_ONLINE_STORE_MAPPING.sql
+-rw-r--r--   0        0        0      311 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/spark/T_TILE_FEATURE_MAPPING.sql
+-rw-r--r--   0        0        0      228 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/spark/T_TILE_JOB_MONITOR.sql
+-rw-r--r--   0        0        0      191 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/spark/T_TILE_MONITOR_SUMMARY.sql
+-rw-r--r--   0        0        0      531 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/spark/T_TILE_REGISTRY.sql
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/spark/__init__.py
+-rw-r--r--   0        0        0    29690 2023-06-08 15:55:07.262925 featurebyte-0.3.1/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar
+-rw-r--r--   0        0        0     2001 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/tile_common.py
+-rw-r--r--   0        0        0     5878 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/tile_generate.py
+-rw-r--r--   0        0        0     3566 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/tile_generate_entity_tracking.py
+-rw-r--r--   0        0        0     9817 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/tile_generate_schedule.py
+-rw-r--r--   0        0        0     7297 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/tile_monitor.py
+-rw-r--r--   0        0        0     3491 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/tile_registry.py
+-rw-r--r--   0        0        0     6139 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/sql/tile_schedule_online_store.py
+-rw-r--r--   0        0        0      239 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/storage/__init__.py
+-rw-r--r--   0        0        0     4999 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/storage/base.py
+-rw-r--r--   0        0        0     3640 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/storage/local.py
+-rw-r--r--   0        0        0      415 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/storage/local_temp.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/tile/__init__.py
+-rw-r--r--   0        0        0    14347 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/tile/manager.py
+-rw-r--r--   0        0        0     2918 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/tile/scheduler.py
+-rw-r--r--   0        0        0      411 2023-06-08 15:53:14.897278 featurebyte-0.3.1/featurebyte/tile/sql_template.py
+-rw-r--r--   0        0        0    28505 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/tile/tile_cache.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/utils/__init__.py
+-rw-r--r--   0        0        0     1909 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/utils/credential.py
+-rw-r--r--   0        0        0     1532 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/utils/messaging.py
+-rw-r--r--   0        0        0      534 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/utils/persistent.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/utils/snowflake/__init__.py
+-rw-r--r--   0        0        0      462 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/utils/snowflake/sql.py
+-rw-r--r--   0        0        0      765 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/utils/storage.py
+-rw-r--r--   0        0        0     1537 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/enum.py
+-rw-r--r--   0        0        0     3873 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/process_store.py
+-rw-r--r--   0        0        0     1159 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/progress.py
+-rw-r--r--   0        0        0     2502 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/schedulers.py
+-rw-r--r--   0        0        0      107 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/start.py
+-rw-r--r--   0        0        0      214 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/base.py
+-rw-r--r--   0        0        0     4603 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/batch_feature_create.py
+-rw-r--r--   0        0        0     3718 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/batch_feature_table.py
+-rw-r--r--   0        0        0     2243 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/batch_request_table.py
+-rw-r--r--   0        0        0     1795 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/deployment_create_update.py
+-rw-r--r--   0        0        0     7130 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/feature_job_setting_analysis.py
+-rw-r--r--   0        0        0     3954 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/historical_feature_table.py
+-rw-r--r--   0        0        0     4321 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/materialized_table_delete.py
+-rw-r--r--   0        0        0     2604 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/mixin.py
+-rw-r--r--   0        0        0     2226 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/observation_table.py
+-rw-r--r--   0        0        0      626 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/test_task.py
+-rw-r--r--   0        0        0     1904 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task/tile_task.py
+-rw-r--r--   0        0        0     5407 2023-06-08 15:53:14.901278 featurebyte-0.3.1/featurebyte/worker/task_executor.py
+-rw-r--r--   0        0        0     7717 2023-06-08 15:53:47.181841 featurebyte-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    23050 1970-01-01 00:00:00.000000 featurebyte-0.3.1/PKG-INFO
```

### Comparing `featurebyte-0.3.0/LICENSE` & `featurebyte-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/README.md` & `featurebyte-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/__init__.py` & `featurebyte-0.3.1/featurebyte/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/__main__.py` & `featurebyte-0.3.1/featurebyte/__main__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/api_object.py` & `featurebyte-0.3.1/featurebyte/api/api_object.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/api_object_util.py` & `featurebyte-0.3.1/featurebyte/api/api_object_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/asat_aggregator.py` & `featurebyte-0.3.1/featurebyte/api/asat_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/base_aggregator.py` & `featurebyte-0.3.1/featurebyte/api/base_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/base_table.py` & `featurebyte-0.3.1/featurebyte/api/base_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/batch_feature_table.py` & `featurebyte-0.3.1/featurebyte/api/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/batch_request_table.py` & `featurebyte-0.3.1/featurebyte/api/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/catalog.py` & `featurebyte-0.3.1/featurebyte/api/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/catalog_decorator.py` & `featurebyte-0.3.1/featurebyte/api/catalog_decorator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/catalog_get_by_id_mixin.py` & `featurebyte-0.3.1/featurebyte/api/catalog_get_by_id_mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/change_view.py` & `featurebyte-0.3.1/featurebyte/api/change_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/credential.py` & `featurebyte-0.3.1/featurebyte/api/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/data_source.py` & `featurebyte-0.3.1/featurebyte/api/data_source.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/deployment.py` & `featurebyte-0.3.1/featurebyte/api/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/dimension_table.py` & `featurebyte-0.3.1/featurebyte/api/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/dimension_view.py` & `featurebyte-0.3.1/featurebyte/api/dimension_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/entity.py` & `featurebyte-0.3.1/featurebyte/api/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/event_table.py` & `featurebyte-0.3.1/featurebyte/api/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/event_view.py` & `featurebyte-0.3.1/featurebyte/api/event_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/feature.py` & `featurebyte-0.3.1/featurebyte/api/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/feature_group.py` & `featurebyte-0.3.1/featurebyte/api/feature_group.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/feature_job.py` & `featurebyte-0.3.1/featurebyte/api/feature_job.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/feature_job_setting_analysis.py` & `featurebyte-0.3.1/featurebyte/api/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/feature_list.py` & `featurebyte-0.3.1/featurebyte/api/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/feature_namespace.py` & `featurebyte-0.3.1/featurebyte/api/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/feature_store.py` & `featurebyte-0.3.1/featurebyte/api/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/feature_util.py` & `featurebyte-0.3.1/featurebyte/api/feature_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/feature_validation_util.py` & `featurebyte-0.3.1/featurebyte/api/feature_validation_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/groupby.py` & `featurebyte-0.3.1/featurebyte/api/groupby.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/historical_feature_table.py` & `featurebyte-0.3.1/featurebyte/api/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/item_table.py` & `featurebyte-0.3.1/featurebyte/api/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/item_view.py` & `featurebyte-0.3.1/featurebyte/api/item_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/lag.py` & `featurebyte-0.3.1/featurebyte/api/lag.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/materialized_table.py` & `featurebyte-0.3.1/featurebyte/api/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/observation_table.py` & `featurebyte-0.3.1/featurebyte/api/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/periodic_task.py` & `featurebyte-0.3.1/featurebyte/api/periodic_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/relationship.py` & `featurebyte-0.3.1/featurebyte/api/relationship.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/request_column.py` & `featurebyte-0.3.1/featurebyte/api/request_column.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/savable_api_object.py` & `featurebyte-0.3.1/featurebyte/api/savable_api_object.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/scd_table.py` & `featurebyte-0.3.1/featurebyte/api/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/scd_view.py` & `featurebyte-0.3.1/featurebyte/api/scd_view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/simple_aggregator.py` & `featurebyte-0.3.1/featurebyte/api/simple_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/source_table.py` & `featurebyte-0.3.1/featurebyte/api/source_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/table.py` & `featurebyte-0.3.1/featurebyte/api/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/templates/online_serving/python.tpl` & `featurebyte-0.3.1/featurebyte/api/templates/online_serving/python.tpl`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/view.py` & `featurebyte-0.3.1/featurebyte/api/view.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/window_aggregator.py` & `featurebyte-0.3.1/featurebyte/api/window_aggregator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/api/window_validator.py` & `featurebyte-0.3.1/featurebyte/api/window_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/app.py` & `featurebyte-0.3.1/featurebyte/app.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/date_util.py` & `featurebyte-0.3.1/featurebyte/common/date_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/descriptor.py` & `featurebyte-0.3.1/featurebyte/common/descriptor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/dict_util.py` & `featurebyte-0.3.1/featurebyte/common/dict_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/doc_util.py` & `featurebyte-0.3.1/featurebyte/common/doc_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/allowed_classes.py` & `featurebyte-0.3.1/featurebyte/common/documentation/allowed_classes.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/autodoc_processor.py` & `featurebyte-0.3.1/featurebyte/common/documentation/autodoc_processor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/constants.py` & `featurebyte-0.3.1/featurebyte/common/documentation/constants.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/custom_nav.py` & `featurebyte-0.3.1/featurebyte/common/documentation/custom_nav.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/doc_types.py` & `featurebyte-0.3.1/featurebyte/common/documentation/doc_types.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/documentation_layout.py` & `featurebyte-0.3.1/featurebyte/common/documentation/documentation_layout.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/extract_csv.py` & `featurebyte-0.3.1/featurebyte/common/documentation/extract_csv.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/formatters.py` & `featurebyte-0.3.1/featurebyte/common/documentation/formatters.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/gen_ref_pages_docs_builder.py` & `featurebyte-0.3.1/featurebyte/common/documentation/gen_ref_pages_docs_builder.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/markdown_extension/extension.py` & `featurebyte-0.3.1/featurebyte/common/documentation/markdown_extension/extension.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/pydantic_field_docs.py` & `featurebyte-0.3.1/featurebyte/common/documentation/pydantic_field_docs.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/resource_extractor.py` & `featurebyte-0.3.1/featurebyte/common/documentation/resource_extractor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/documentation/resource_util.py` & `featurebyte-0.3.1/featurebyte/common/documentation/resource_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/env_util.py` & `featurebyte-0.3.1/featurebyte/common/env_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/formatting_util.py` & `featurebyte-0.3.1/featurebyte/common/formatting_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/join_utils.py` & `featurebyte-0.3.1/featurebyte/common/join_utils.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/model_util.py` & `featurebyte-0.3.1/featurebyte/common/model_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/path_util.py` & `featurebyte-0.3.1/featurebyte/common/path_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/progress.py` & `featurebyte-0.3.1/featurebyte/common/progress.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/tile_util.py` & `featurebyte-0.3.1/featurebyte/common/tile_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/typing.py` & `featurebyte-0.3.1/featurebyte/common/typing.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/utils.py` & `featurebyte-0.3.1/featurebyte/common/utils.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/common/validator.py` & `featurebyte-0.3.1/featurebyte/common/validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/config.py` & `featurebyte-0.3.1/featurebyte/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 Read configurations from ini file
 """
 from typing import Any, Dict, Iterator, List, Optional, Union, cast
 
 import json
 import os
+import time
 from contextlib import contextmanager
 from http import HTTPStatus
 from pathlib import Path
 
 import requests
 import websocket
 import yaml
 from pydantic import AnyHttpUrl, BaseModel, Field, validator
 from requests import Response
+from websocket import WebSocketConnectionClosedException
 
 from featurebyte.common.doc_util import FBAutoDoc
 from featurebyte.common.utils import get_version
 from featurebyte.enum import StrEnum
 from featurebyte.exception import InvalidSettingsError
 from featurebyte.models.base import get_active_catalog_id
 
@@ -198,16 +200,24 @@
         ----------
         url: str
             URL of FeatureByte websocket service
         access_token: Optional[str]
             Access token to used for authentication
         """
         if access_token:
-            url = f"{url}?token={access_token}"
-        self._ws = websocket.create_connection(url, enable_multithread=True)
+            self._url = f"{url}?token={access_token}"
+        else:
+            self._url = url
+        self._reconnect()
+
+    def _reconnect(self) -> None:
+        """
+        Reconnect websocket connection
+        """
+        self._ws = websocket.create_connection(self._url, enable_multithread=True)
 
     def close(self) -> None:
         """
         Close websocket connection
         """
         self._ws.close()
 
@@ -215,16 +225,29 @@
         """
         Receive message from websocket server as bytes
 
         Returns
         -------
         bytes
             Message
+
+        Raises
+        ------
+        TimeoutError
+            No message received from websocket server
         """
-        return cast(bytes, self._ws.recv())
+        start_time = time.time()
+        # maintain connection for up to 3 minutes without receiving any new message
+        while (time.time() - start_time) < 180:
+            try:
+                return cast(bytes, self._ws.recv())
+            except WebSocketConnectionClosedException:
+                # reconnect on unexpected connection close
+                self._reconnect()
+        raise TimeoutError("No message received from websocket server")
 
     def receive_json(self) -> Optional[Dict[str, Any]]:
         """
         Receive message from websocket server as json
 
         Returns
         -------
@@ -449,15 +472,15 @@
 
         Raises
         ------
         InvalidSettingsError
             Invalid settings
         """
         if self.profile:
-            url = self.profile.api_url.replace("http://", "ws://")
+            url = self.profile.api_url.replace("http://", "ws://").replace("https://", "wss://")
             url = f"{url}/ws/{task_id}"
             websocket_client = WebsocketClient(url=url, access_token=self.profile.api_token)
             try:
                 yield websocket_client
             finally:
                 websocket_client.close()
         else:
```

### Comparing `featurebyte-0.3.0/featurebyte/conftest.py` & `featurebyte-0.3.1/featurebyte/conftest.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/accessor/count_dict.py` & `featurebyte-0.3.1/featurebyte/core/accessor/count_dict.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/accessor/datetime.py` & `featurebyte-0.3.1/featurebyte/core/accessor/datetime.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/accessor/feature_datetime.py` & `featurebyte-0.3.1/featurebyte/core/accessor/feature_datetime.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/accessor/feature_string.py` & `featurebyte-0.3.1/featurebyte/core/accessor/feature_string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/accessor/string.py` & `featurebyte-0.3.1/featurebyte/core/accessor/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/frame.py` & `featurebyte-0.3.1/featurebyte/core/frame.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/generic.py` & `featurebyte-0.3.1/featurebyte/core/generic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/mixin.py` & `featurebyte-0.3.1/featurebyte/core/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/series.py` & `featurebyte-0.3.1/featurebyte/core/series.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/timedelta.py` & `featurebyte-0.3.1/featurebyte/core/timedelta.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/core/util.py` & `featurebyte-0.3.1/featurebyte/core/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/datasets/__main__.py` & `featurebyte-0.3.1/featurebyte/datasets/__main__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/datasets/app.py` & `featurebyte-0.3.1/featurebyte/datasets/app.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/datasets/creditcard.sql` & `featurebyte-0.3.1/featurebyte/datasets/creditcard.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/datasets/doctest_grocery.sql` & `featurebyte-0.3.1/featurebyte/datasets/doctest_grocery.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/datasets/grocery.sql` & `featurebyte-0.3.1/featurebyte/datasets/grocery.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/datasets/healthcare.sql` & `featurebyte-0.3.1/featurebyte/datasets/healthcare.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/docker/featurebyte.yml` & `featurebyte-0.3.1/featurebyte/docker/featurebyte.yml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
       driver: local
   featurebyte-server:
     networks:
       - featurebyte
     hostname: featurebyte-server
     restart: unless-stopped
     container_name: featurebyte-server
-    image: featurebyte/featurebyte-server:0.3.0
+    image: featurebyte/featurebyte-server:0.3.1
     depends_on:
       mongo-rs:
         condition: service_healthy
     ports:
       - "0.0.0.0:8088:8088"
     command: ["bash", "/docker-entrypoint.sh", "server"]
     environment:
@@ -65,15 +65,15 @@
       driver: local
   featurebyte-worker:
     networks:
       - featurebyte
     hostname: featurebyte-worker
     restart: unless-stopped
     container_name: featurebyte-worker
-    image: featurebyte/featurebyte-server:0.3.0
+    image: featurebyte/featurebyte-server:0.3.1
     depends_on:
       mongo-rs:
         condition: service_healthy
       redis:
         condition: service_healthy
     environment:
       - "FEATUREBYTE_HOME=/app/.featurebyte"
```

### Comparing `featurebyte-0.3.0/featurebyte/docker/manager.py` & `featurebyte-0.3.1/featurebyte/docker/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/enum.py` & `featurebyte-0.3.1/featurebyte/enum.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/exception.py` & `featurebyte-0.3.1/featurebyte/exception.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/feature_manager/manager.py` & `featurebyte-0.3.1/featurebyte/feature_manager/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/feature_manager/model.py` & `featurebyte-0.3.1/featurebyte/feature_manager/model.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/feature_manager/sql_template.py` & `featurebyte-0.3.1/featurebyte/feature_manager/sql_template.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/feature_utility.py` & `featurebyte-0.3.1/featurebyte/feature_utility.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/logging.py` & `featurebyte-0.3.1/featurebyte/logging.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/middleware.py` & `featurebyte-0.3.1/featurebyte/middleware.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/migration/migration_data_service.py` & `featurebyte-0.3.1/featurebyte/migration/migration_data_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/migration/model.py` & `featurebyte-0.3.1/featurebyte/migration/model.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/migration/run.py` & `featurebyte-0.3.1/featurebyte/migration/run.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/migration/service/__init__.py` & `featurebyte-0.3.1/featurebyte/migration/service/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/migration/service/data_warehouse.py` & `featurebyte-0.3.1/featurebyte/migration/service/data_warehouse.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/migration/service/mixin.py` & `featurebyte-0.3.1/featurebyte/migration/service/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/__init__.py` & `featurebyte-0.3.1/featurebyte/models/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/base.py` & `featurebyte-0.3.1/featurebyte/models/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/batch_feature_table.py` & `featurebyte-0.3.1/featurebyte/models/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/batch_request_table.py` & `featurebyte-0.3.1/featurebyte/models/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/catalog.py` & `featurebyte-0.3.1/featurebyte/models/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/context.py` & `featurebyte-0.3.1/featurebyte/models/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/credential.py` & `featurebyte-0.3.1/featurebyte/models/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/deployment.py` & `featurebyte-0.3.1/featurebyte/models/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/dimension_table.py` & `featurebyte-0.3.1/featurebyte/models/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/entity.py` & `featurebyte-0.3.1/featurebyte/models/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/entity_validation.py` & `featurebyte-0.3.1/featurebyte/models/entity_validation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/event_table.py` & `featurebyte-0.3.1/featurebyte/models/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/feature.py` & `featurebyte-0.3.1/featurebyte/models/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/feature_job_setting_analysis.py` & `featurebyte-0.3.1/featurebyte/models/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/feature_list.py` & `featurebyte-0.3.1/featurebyte/models/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/feature_store.py` & `featurebyte-0.3.1/featurebyte/models/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/historical_feature_table.py` & `featurebyte-0.3.1/featurebyte/models/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/item_table.py` & `featurebyte-0.3.1/featurebyte/models/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/materialized_table.py` & `featurebyte-0.3.1/featurebyte/models/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/observation_table.py` & `featurebyte-0.3.1/featurebyte/models/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/online_store.py` & `featurebyte-0.3.1/featurebyte/models/online_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/parent_serving.py` & `featurebyte-0.3.1/featurebyte/models/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/periodic_task.py` & `featurebyte-0.3.1/featurebyte/models/periodic_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/persistent.py` & `featurebyte-0.3.1/featurebyte/models/persistent.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/proxy_table.py` & `featurebyte-0.3.1/featurebyte/models/proxy_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/relationship.py` & `featurebyte-0.3.1/featurebyte/models/relationship.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/relationship_analysis.py` & `featurebyte-0.3.1/featurebyte/models/relationship_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/request_input.py` & `featurebyte-0.3.1/featurebyte/models/request_input.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/scd_table.py` & `featurebyte-0.3.1/featurebyte/models/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/semantic.py` & `featurebyte-0.3.1/featurebyte/models/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/task.py` & `featurebyte-0.3.1/featurebyte/models/task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/models/tile.py` & `featurebyte-0.3.1/featurebyte/models/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/persistent/audit.py` & `featurebyte-0.3.1/featurebyte/persistent/audit.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/persistent/base.py` & `featurebyte-0.3.1/featurebyte/persistent/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/persistent/mongo.py` & `featurebyte-0.3.1/featurebyte/persistent/mongo.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/algorithm.py` & `featurebyte-0.3.1/featurebyte/query_graph/algorithm.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/enum.py` & `featurebyte-0.3.1/featurebyte/query_graph/enum.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/graph.py` & `featurebyte-0.3.1/featurebyte/query_graph/graph.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/graph_node/base.py` & `featurebyte-0.3.1/featurebyte/query_graph/graph_node/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/model/column_info.py` & `featurebyte-0.3.1/featurebyte/query_graph/model/column_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/model/common_table.py` & `featurebyte-0.3.1/featurebyte/query_graph/model/common_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/model/critical_data_info.py` & `featurebyte-0.3.1/featurebyte/query_graph/model/critical_data_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/model/feature_job_setting.py` & `featurebyte-0.3.1/featurebyte/query_graph/model/feature_job_setting.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/model/graph.py` & `featurebyte-0.3.1/featurebyte/query_graph/model/graph.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/model/table.py` & `featurebyte-0.3.1/featurebyte/query_graph/model/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/__init__.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/agg_func.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/agg_func.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/base.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/binary.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/binary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/cleaning_operation.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/cleaning_operation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/count_dict.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/count_dict.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/date.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/date.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/generic.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/generic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/input.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/input.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/metadata/column.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/metadata/column.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/metadata/operation.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/metadata/operation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/metadata/sdk_code.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/metadata/sdk_code.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/mixin.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/nested.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/nested.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/request.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/request.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/scalar.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/scalar.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/schema.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/string.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/unary.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/unary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/node/validator.py` & `featurebyte-0.3.1/featurebyte/query_graph/node/validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/pruning_util.py` & `featurebyte-0.3.1/featurebyte/query_graph/pruning_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/adapter.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/adapter.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/asat.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/asat.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/base.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/item.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/item.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/latest.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/latest.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/lookup.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/lookup.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/request_table.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/aggregator/window.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/aggregator/window.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/aggregate.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/aggregate.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/base.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/binary.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/binary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/count_dict.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/count_dict.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/datetime.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/datetime.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/generic.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/generic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/groupby.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/groupby.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/input.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/input.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/is_in.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/is_in.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/join.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/join.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/join_feature.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/join_feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/literal.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/literal.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/request.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/request.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/string.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/string.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/tile.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/track_changes.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/track_changes.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/unary.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/unary.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/ast/util.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/ast/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/builder.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/builder.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/common.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/common.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/dataframe.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/expression.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/expression.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/feature_compute.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/feature_compute.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/feature_historical.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/feature_historical.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/feature_preview.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/feature_preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/groupby_helper.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/groupby_helper.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/base.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/interpreter/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/preview.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/interpreter/preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/interpreter/tile.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/interpreter/tile.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/materialisation.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/materialisation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/online_serving.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/online_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/online_serving_util.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/online_serving_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/parent_serving.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/scd_helper.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/scd_helper.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/specs.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/specs.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/template.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/template.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/tile_compute.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/tile_compute.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/tile_util.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/tile_util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/sql/tiling.py` & `featurebyte-0.3.1/featurebyte/query_graph/sql/tiling.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/transform/base.py` & `featurebyte-0.3.1/featurebyte/query_graph/transform/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/transform/flattening.py` & `featurebyte-0.3.1/featurebyte/query_graph/transform/flattening.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/transform/operation_structure.py` & `featurebyte-0.3.1/featurebyte/query_graph/transform/operation_structure.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/transform/pruning.py` & `featurebyte-0.3.1/featurebyte/query_graph/transform/pruning.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/transform/reconstruction.py` & `featurebyte-0.3.1/featurebyte/query_graph/transform/reconstruction.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/transform/sdk_code.py` & `featurebyte-0.3.1/featurebyte/query_graph/transform/sdk_code.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/query_graph/util.py` & `featurebyte-0.3.1/featurebyte/query_graph/util.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/app_container.py` & `featurebyte-0.3.1/featurebyte/routes/app_container.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/app_container_config.py` & `featurebyte-0.3.1/featurebyte/routes/app_container_config.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/batch_feature_table/api.py` & `featurebyte-0.3.1/featurebyte/routes/batch_feature_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/batch_feature_table/controller.py` & `featurebyte-0.3.1/featurebyte/routes/batch_feature_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/batch_request_table/api.py` & `featurebyte-0.3.1/featurebyte/routes/batch_request_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/batch_request_table/controller.py` & `featurebyte-0.3.1/featurebyte/routes/batch_request_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/catalog/api.py` & `featurebyte-0.3.1/featurebyte/routes/catalog/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/catalog/controller.py` & `featurebyte-0.3.1/featurebyte/routes/catalog/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/common/base.py` & `featurebyte-0.3.1/featurebyte/routes/common/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/common/base_materialized_table.py` & `featurebyte-0.3.1/featurebyte/routes/common/base_materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/common/base_table.py` & `featurebyte-0.3.1/featurebyte/routes/common/base_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/common/schema.py` & `featurebyte-0.3.1/featurebyte/routes/common/schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/context/api.py` & `featurebyte-0.3.1/featurebyte/routes/context/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/context/controller.py` & `featurebyte-0.3.1/featurebyte/routes/context/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/credential/api.py` & `featurebyte-0.3.1/featurebyte/routes/credential/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/credential/controller.py` & `featurebyte-0.3.1/featurebyte/routes/credential/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/deployment/api.py` & `featurebyte-0.3.1/featurebyte/routes/deployment/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/deployment/controller.py` & `featurebyte-0.3.1/featurebyte/routes/deployment/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/dimension_table/api.py` & `featurebyte-0.3.1/featurebyte/routes/dimension_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/dimension_table/controller.py` & `featurebyte-0.3.1/featurebyte/routes/dimension_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/entity/api.py` & `featurebyte-0.3.1/featurebyte/routes/entity/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/entity/controller.py` & `featurebyte-0.3.1/featurebyte/routes/entity/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/event_table/api.py` & `featurebyte-0.3.1/featurebyte/routes/event_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/event_table/controller.py` & `featurebyte-0.3.1/featurebyte/routes/event_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature/api.py` & `featurebyte-0.3.1/featurebyte/routes/feature/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature/controller.py` & `featurebyte-0.3.1/featurebyte/routes/feature/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature_job_setting_analysis/api.py` & `featurebyte-0.3.1/featurebyte/routes/feature_job_setting_analysis/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature_job_setting_analysis/controller.py` & `featurebyte-0.3.1/featurebyte/routes/feature_job_setting_analysis/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature_list/api.py` & `featurebyte-0.3.1/featurebyte/routes/feature_list/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature_list/controller.py` & `featurebyte-0.3.1/featurebyte/routes/feature_list/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature_list_namespace/api.py` & `featurebyte-0.3.1/featurebyte/routes/feature_list_namespace/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature_list_namespace/controller.py` & `featurebyte-0.3.1/featurebyte/routes/feature_list_namespace/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature_namespace/api.py` & `featurebyte-0.3.1/featurebyte/routes/feature_namespace/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature_namespace/controller.py` & `featurebyte-0.3.1/featurebyte/routes/feature_namespace/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature_store/api.py` & `featurebyte-0.3.1/featurebyte/routes/feature_store/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/feature_store/controller.py` & `featurebyte-0.3.1/featurebyte/routes/feature_store/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/historical_feature_table/api.py` & `featurebyte-0.3.1/featurebyte/routes/historical_feature_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/historical_feature_table/controller.py` & `featurebyte-0.3.1/featurebyte/routes/historical_feature_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/item_table/api.py` & `featurebyte-0.3.1/featurebyte/routes/item_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/item_table/controller.py` & `featurebyte-0.3.1/featurebyte/routes/item_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/observation_table/api.py` & `featurebyte-0.3.1/featurebyte/routes/observation_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/observation_table/controller.py` & `featurebyte-0.3.1/featurebyte/routes/observation_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/periodic_tasks/api.py` & `featurebyte-0.3.1/featurebyte/routes/periodic_tasks/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/periodic_tasks/controller.py` & `featurebyte-0.3.1/featurebyte/routes/periodic_tasks/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/registry.py` & `featurebyte-0.3.1/featurebyte/routes/registry.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/relationship_info/api.py` & `featurebyte-0.3.1/featurebyte/routes/relationship_info/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/relationship_info/controller.py` & `featurebyte-0.3.1/featurebyte/routes/relationship_info/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/scd_table/api.py` & `featurebyte-0.3.1/featurebyte/routes/scd_table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/scd_table/controller.py` & `featurebyte-0.3.1/featurebyte/routes/scd_table/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/semantic/api.py` & `featurebyte-0.3.1/featurebyte/routes/semantic/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/semantic/controller.py` & `featurebyte-0.3.1/featurebyte/routes/semantic/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/table/api.py` & `featurebyte-0.3.1/featurebyte/routes/table/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/task/api.py` & `featurebyte-0.3.1/featurebyte/routes/task/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/task/controller.py` & `featurebyte-0.3.1/featurebyte/routes/task/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/temp_data/api.py` & `featurebyte-0.3.1/featurebyte/routes/temp_data/api.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/routes/temp_data/controller.py` & `featurebyte-0.3.1/featurebyte/routes/temp_data/controller.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/batch_feature_table.py` & `featurebyte-0.3.1/featurebyte/schema/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/batch_request_table.py` & `featurebyte-0.3.1/featurebyte/schema/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/catalog.py` & `featurebyte-0.3.1/featurebyte/schema/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/common/base.py` & `featurebyte-0.3.1/featurebyte/schema/common/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/common/operation.py` & `featurebyte-0.3.1/featurebyte/schema/common/operation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/context.py` & `featurebyte-0.3.1/featurebyte/schema/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/credential.py` & `featurebyte-0.3.1/featurebyte/schema/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/deployment.py` & `featurebyte-0.3.1/featurebyte/schema/deployment.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/dimension_table.py` & `featurebyte-0.3.1/featurebyte/schema/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/entity.py` & `featurebyte-0.3.1/featurebyte/schema/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/event_table.py` & `featurebyte-0.3.1/featurebyte/schema/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/feature.py` & `featurebyte-0.3.1/featurebyte/schema/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/feature_job_setting_analysis.py` & `featurebyte-0.3.1/featurebyte/schema/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/feature_list.py` & `featurebyte-0.3.1/featurebyte/schema/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/feature_list_namespace.py` & `featurebyte-0.3.1/featurebyte/schema/feature_list_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/feature_namespace.py` & `featurebyte-0.3.1/featurebyte/schema/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/feature_store.py` & `featurebyte-0.3.1/featurebyte/schema/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/historical_feature_table.py` & `featurebyte-0.3.1/featurebyte/schema/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/info.py` & `featurebyte-0.3.1/featurebyte/schema/info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/item_table.py` & `featurebyte-0.3.1/featurebyte/schema/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/materialized_table.py` & `featurebyte-0.3.1/featurebyte/schema/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/observation_table.py` & `featurebyte-0.3.1/featurebyte/schema/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/relationship_info.py` & `featurebyte-0.3.1/featurebyte/schema/relationship_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/request_table.py` & `featurebyte-0.3.1/featurebyte/schema/request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/scd_table.py` & `featurebyte-0.3.1/featurebyte/schema/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/semantic.py` & `featurebyte-0.3.1/featurebyte/schema/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/table.py` & `featurebyte-0.3.1/featurebyte/schema/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/task.py` & `featurebyte-0.3.1/featurebyte/schema/task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/worker/task/base.py` & `featurebyte-0.3.1/featurebyte/schema/worker/task/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/worker/task/batch_feature_create.py` & `featurebyte-0.3.1/featurebyte/schema/worker/task/batch_feature_create.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/worker/task/batch_feature_table.py` & `featurebyte-0.3.1/featurebyte/schema/worker/task/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/worker/task/batch_request_table.py` & `featurebyte-0.3.1/featurebyte/schema/worker/task/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/worker/task/deployment_create_update.py` & `featurebyte-0.3.1/featurebyte/schema/worker/task/deployment_create_update.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/worker/task/feature_job_setting_analysis.py` & `featurebyte-0.3.1/featurebyte/schema/worker/task/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/worker/task/historical_feature_table.py` & `featurebyte-0.3.1/featurebyte/schema/worker/task/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/worker/task/materialized_table_delete.py` & `featurebyte-0.3.1/featurebyte/schema/worker/task/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/schema/worker/task/observation_table.py` & `featurebyte-0.3.1/featurebyte/schema/worker/task/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/base_document.py` & `featurebyte-0.3.1/featurebyte/service/base_document.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/base_service.py` & `featurebyte-0.3.1/featurebyte/service/base_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/base_table_document.py` & `featurebyte-0.3.1/featurebyte/service/base_table_document.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/batch_feature_table.py` & `featurebyte-0.3.1/featurebyte/service/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/batch_request_table.py` & `featurebyte-0.3.1/featurebyte/service/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/catalog.py` & `featurebyte-0.3.1/featurebyte/service/catalog.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/context.py` & `featurebyte-0.3.1/featurebyte/service/context.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/credential.py` & `featurebyte-0.3.1/featurebyte/service/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/default_version_mode.py` & `featurebyte-0.3.1/featurebyte/service/default_version_mode.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/deploy.py` & `featurebyte-0.3.1/featurebyte/service/deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
                         await self.online_enable_service.update_data_warehouse(
                             updated_feature=updated_feature,
                             online_enabled_before_update=feature.online_enabled,
                             get_credential=get_credential,
                         )
 
                     if update_progress:
-                        percent = 20 + 60 // len(document.feature_ids) * (ind + 1)
+                        percent = 20 + int(60 / len(document.feature_ids) * (ind + 1))
                         update_progress(percent, f"Updated {feature.name}")
 
                 if update_progress:
                     update_progress(80, "Update feature list")
 
                 async with self.persistent.start_transaction():
                     await self._update_feature_list_namespace(
```

### Comparing `featurebyte-0.3.0/featurebyte/service/dimension_table.py` & `featurebyte-0.3.1/featurebyte/service/dimension_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/entity.py` & `featurebyte-0.3.1/featurebyte/service/entity.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/entity_validation.py` & `featurebyte-0.3.1/featurebyte/service/entity_validation.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/event_table.py` & `featurebyte-0.3.1/featurebyte/service/event_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/feature.py` & `featurebyte-0.3.1/featurebyte/service/feature.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/feature_job_setting_analysis.py` & `featurebyte-0.3.1/featurebyte/service/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/feature_list.py` & `featurebyte-0.3.1/featurebyte/service/feature_list.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/feature_list_namespace.py` & `featurebyte-0.3.1/featurebyte/service/feature_list_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/feature_list_status.py` & `featurebyte-0.3.1/featurebyte/service/feature_list_status.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/feature_namespace.py` & `featurebyte-0.3.1/featurebyte/service/feature_namespace.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/feature_readiness.py` & `featurebyte-0.3.1/featurebyte/service/feature_readiness.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/feature_store.py` & `featurebyte-0.3.1/featurebyte/service/feature_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/feature_store_warehouse.py` & `featurebyte-0.3.1/featurebyte/service/feature_store_warehouse.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/historical_feature_table.py` & `featurebyte-0.3.1/featurebyte/service/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/info.py` & `featurebyte-0.3.1/featurebyte/service/info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/item_table.py` & `featurebyte-0.3.1/featurebyte/service/item_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/materialized_table.py` & `featurebyte-0.3.1/featurebyte/service/materialized_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/mixin.py` & `featurebyte-0.3.1/featurebyte/service/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/observation_table.py` & `featurebyte-0.3.1/featurebyte/service/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/online_enable.py` & `featurebyte-0.3.1/featurebyte/service/online_enable.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/online_serving.py` & `featurebyte-0.3.1/featurebyte/service/online_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/parent_serving.py` & `featurebyte-0.3.1/featurebyte/service/parent_serving.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/preview.py` & `featurebyte-0.3.1/featurebyte/service/preview.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/relationship.py` & `featurebyte-0.3.1/featurebyte/service/relationship.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/relationship_info.py` & `featurebyte-0.3.1/featurebyte/service/relationship_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/scd_table.py` & `featurebyte-0.3.1/featurebyte/service/scd_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/semantic.py` & `featurebyte-0.3.1/featurebyte/service/semantic.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/session_manager.py` & `featurebyte-0.3.1/featurebyte/service/session_manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/session_validator.py` & `featurebyte-0.3.1/featurebyte/service/session_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/table.py` & `featurebyte-0.3.1/featurebyte/service/table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/table_columns_info.py` & `featurebyte-0.3.1/featurebyte/service/table_columns_info.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/table_status.py` & `featurebyte-0.3.1/featurebyte/service/table_status.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/task_manager.py` & `featurebyte-0.3.1/featurebyte/service/task_manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/user_service.py` & `featurebyte-0.3.1/featurebyte/service/user_service.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/validator/materialized_table_delete.py` & `featurebyte-0.3.1/featurebyte/service/validator/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/validator/production_ready_validator.py` & `featurebyte-0.3.1/featurebyte/service/validator/production_ready_validator.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/version.py` & `featurebyte-0.3.1/featurebyte/service/version.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/view_construction.py` & `featurebyte-0.3.1/featurebyte/service/view_construction.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/service/working_schema.py` & `featurebyte-0.3.1/featurebyte/service/working_schema.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/session/base.py` & `featurebyte-0.3.1/featurebyte/session/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/session/base_spark.py` & `featurebyte-0.3.1/featurebyte/session/base_spark.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/session/databricks.py` & `featurebyte-0.3.1/featurebyte/session/databricks.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/session/hive.py` & `featurebyte-0.3.1/featurebyte/session/hive.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/session/manager.py` & `featurebyte-0.3.1/featurebyte/session/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/session/simple_storage.py` & `featurebyte-0.3.1/featurebyte/session/simple_storage.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/session/snowflake.py` & `featurebyte-0.3.1/featurebyte/session/snowflake.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/session/spark.py` & `featurebyte-0.3.1/featurebyte/session/spark.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/session/sqlite.py` & `featurebyte-0.3.1/featurebyte/session/sqlite.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/base.py` & `featurebyte-0.3.1/featurebyte/sql/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/common.py` & `featurebyte-0.3.1/featurebyte/sql/common.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql` & `featurebyte-0.3.1/featurebyte/sql/snowflake/F_COUNT_DICT_COSINE_SIMILARITY.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql` & `featurebyte-0.3.1/featurebyte/sql/snowflake/F_COUNT_DICT_MOST_FREQUENT_KEY_VALUE.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/snowflake/F_GET_RANK.sql` & `featurebyte-0.3.1/featurebyte/sql/snowflake/F_GET_RANK.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql` & `featurebyte-0.3.1/featurebyte/sql/snowflake/F_INDEX_TO_TIMESTAMP.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql` & `featurebyte-0.3.1/featurebyte/sql/snowflake/F_TIMESTAMP_TO_INDEX.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql` & `featurebyte-0.3.1/featurebyte/sql/snowflake/F_TIMEZONE_OFFSET_TO_SECOND.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql` & `featurebyte-0.3.1/featurebyte/sql/snowflake/T_TILE_REGISTRY.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/spark/T_TILE_REGISTRY.sql` & `featurebyte-0.3.1/featurebyte/sql/spark/T_TILE_REGISTRY.sql`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar` & `featurebyte-0.3.1/featurebyte/sql/spark/featurebyte-hive-udf-1.0.3-SNAPSHOT-all.jar`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,25 +1,25 @@
 Zip file size: 29690 bytes, number of entries: 23
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-05 04:29 META-INF/
--rw-r--r--  2.0 unx       25 b- defN 23-Jun-05 04:29 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-05 04:29 com/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-05 04:29 com/featurebyte/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-05 04:29 com/featurebyte/hive/
-drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/
--rw-r--r--  2.0 unx     2544 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/ObjectAggregate.class
--rw-r--r--  2.0 unx     3869 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictRelativeFrequency.class
--rw-r--r--  2.0 unx     5593 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictRank.class
--rw-r--r--  2.0 unx      963 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
--rw-r--r--  2.0 unx     3769 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
--rw-r--r--  2.0 unx     2570 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
--rw-r--r--  2.0 unx     2923 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictNumUnique.class
--rw-r--r--  2.0 unx     3796 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictMostFrequent.class
--rw-r--r--  2.0 unx     3721 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictEntropy.class
--rw-r--r--  2.0 unx     5044 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/TimestampToIndex.class
--rw-r--r--  2.0 unx     1070 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/ObjectAggregate$1.class
--rw-r--r--  2.0 unx     2741 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/ObjectDelete.class
--rw-r--r--  2.0 unx     5098 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictUDF.class
--rw-r--r--  2.0 unx     6348 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictCosineSimilarity.class
--rw-r--r--  2.0 unx     5565 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/IndexToTimestamp.class
--rw-r--r--  2.0 unx     3730 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/CountDictMostFrequentValue.class
--rw-r--r--  2.0 unx     5161 b- defN 23-Jun-05 04:29 com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-08 15:54 META-INF/
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-08 15:54 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-08 15:54 com/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-08 15:54 com/featurebyte/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-08 15:54 com/featurebyte/hive/
+drwxr-xr-x  2.0 unx        0 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/
+-rw-r--r--  2.0 unx     5593 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/CountDictRank.class
+-rw-r--r--  2.0 unx     5161 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
+-rw-r--r--  2.0 unx     2544 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/ObjectAggregate.class
+-rw-r--r--  2.0 unx     5098 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/CountDictUDF.class
+-rw-r--r--  2.0 unx     1070 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/ObjectAggregate$1.class
+-rw-r--r--  2.0 unx     6348 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/CountDictCosineSimilarity.class
+-rw-r--r--  2.0 unx     3769 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
+-rw-r--r--  2.0 unx     2570 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
+-rw-r--r--  2.0 unx     2741 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/ObjectDelete.class
+-rw-r--r--  2.0 unx     5565 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/IndexToTimestamp.class
+-rw-r--r--  2.0 unx      963 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
+-rw-r--r--  2.0 unx     5044 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/TimestampToIndex.class
+-rw-r--r--  2.0 unx     3796 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/CountDictMostFrequent.class
+-rw-r--r--  2.0 unx     2923 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/CountDictNumUnique.class
+-rw-r--r--  2.0 unx     3721 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/CountDictEntropy.class
+-rw-r--r--  2.0 unx     3869 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/CountDictRelativeFrequency.class
+-rw-r--r--  2.0 unx     3730 b- defN 23-Jun-08 15:54 com/featurebyte/hive/udf/CountDictMostFrequentValue.class
 23 files, 64530 bytes uncompressed, 25488 bytes compressed:  60.5%
```

#### zipnote «TEMP»/diffoscope_yzl68xzu_/tmprvdbqh2g_.zip

```diff
@@ -12,59 +12,59 @@
 
 Filename: com/featurebyte/hive/
 Comment: 
 
 Filename: com/featurebyte/hive/udf/
 Comment: 
 
+Filename: com/featurebyte/hive/udf/CountDictRank.class
+Comment: 
+
+Filename: com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
+Comment: 
+
 Filename: com/featurebyte/hive/udf/ObjectAggregate.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictRelativeFrequency.class
+Filename: com/featurebyte/hive/udf/CountDictUDF.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictRank.class
+Filename: com/featurebyte/hive/udf/ObjectAggregate$1.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
+Filename: com/featurebyte/hive/udf/CountDictCosineSimilarity.class
 Comment: 
 
 Filename: com/featurebyte/hive/udf/TimezoneOffsetToSecond.class
 Comment: 
 
 Filename: com/featurebyte/hive/udf/CountDictSingleStringArgumentUDF.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictNumUnique.class
+Filename: com/featurebyte/hive/udf/ObjectDelete.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictMostFrequent.class
+Filename: com/featurebyte/hive/udf/IndexToTimestamp.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictEntropy.class
+Filename: com/featurebyte/hive/udf/ObjectAggregate$MapAggregationBuffer.class
 Comment: 
 
 Filename: com/featurebyte/hive/udf/TimestampToIndex.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectAggregate$1.class
-Comment: 
-
-Filename: com/featurebyte/hive/udf/ObjectDelete.class
+Filename: com/featurebyte/hive/udf/CountDictMostFrequent.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictUDF.class
+Filename: com/featurebyte/hive/udf/CountDictNumUnique.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/CountDictCosineSimilarity.class
+Filename: com/featurebyte/hive/udf/CountDictEntropy.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/IndexToTimestamp.class
+Filename: com/featurebyte/hive/udf/CountDictRelativeFrequency.class
 Comment: 
 
 Filename: com/featurebyte/hive/udf/CountDictMostFrequentValue.class
 Comment: 
 
-Filename: com/featurebyte/hive/udf/ObjectAggregate$ObjectAggregatorEvaluator.class
-Comment: 
-
 Zip file comment:
```

### Comparing `featurebyte-0.3.0/featurebyte/sql/tile_common.py` & `featurebyte-0.3.1/featurebyte/sql/tile_common.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/tile_generate.py` & `featurebyte-0.3.1/featurebyte/sql/tile_generate.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/tile_generate_entity_tracking.py` & `featurebyte-0.3.1/featurebyte/sql/tile_generate_entity_tracking.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/tile_generate_schedule.py` & `featurebyte-0.3.1/featurebyte/sql/tile_generate_schedule.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/tile_monitor.py` & `featurebyte-0.3.1/featurebyte/sql/tile_monitor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/tile_registry.py` & `featurebyte-0.3.1/featurebyte/sql/tile_registry.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/sql/tile_schedule_online_store.py` & `featurebyte-0.3.1/featurebyte/sql/tile_schedule_online_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/storage/base.py` & `featurebyte-0.3.1/featurebyte/storage/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/storage/local.py` & `featurebyte-0.3.1/featurebyte/storage/local.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/tile/manager.py` & `featurebyte-0.3.1/featurebyte/tile/manager.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/tile/scheduler.py` & `featurebyte-0.3.1/featurebyte/tile/scheduler.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/tile/tile_cache.py` & `featurebyte-0.3.1/featurebyte/tile/tile_cache.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/utils/credential.py` & `featurebyte-0.3.1/featurebyte/utils/credential.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/utils/messaging.py` & `featurebyte-0.3.1/featurebyte/utils/messaging.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/utils/persistent.py` & `featurebyte-0.3.1/featurebyte/utils/persistent.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/utils/storage.py` & `featurebyte-0.3.1/featurebyte/utils/storage.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/__init__.py` & `featurebyte-0.3.1/featurebyte/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/process_store.py` & `featurebyte-0.3.1/featurebyte/worker/process_store.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/progress.py` & `featurebyte-0.3.1/featurebyte/worker/progress.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/schedulers.py` & `featurebyte-0.3.1/featurebyte/worker/schedulers.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/base.py` & `featurebyte-0.3.1/featurebyte/worker/task/base.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/batch_feature_create.py` & `featurebyte-0.3.1/featurebyte/worker/task/batch_feature_create.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/batch_feature_table.py` & `featurebyte-0.3.1/featurebyte/worker/task/batch_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/batch_request_table.py` & `featurebyte-0.3.1/featurebyte/worker/task/batch_request_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/deployment_create_update.py` & `featurebyte-0.3.1/featurebyte/worker/task/deployment_create_update.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/feature_job_setting_analysis.py` & `featurebyte-0.3.1/featurebyte/worker/task/feature_job_setting_analysis.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/historical_feature_table.py` & `featurebyte-0.3.1/featurebyte/worker/task/historical_feature_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/materialized_table_delete.py` & `featurebyte-0.3.1/featurebyte/worker/task/materialized_table_delete.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/mixin.py` & `featurebyte-0.3.1/featurebyte/worker/task/mixin.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/observation_table.py` & `featurebyte-0.3.1/featurebyte/worker/task/observation_table.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/test_task.py` & `featurebyte-0.3.1/featurebyte/worker/task/test_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task/tile_task.py` & `featurebyte-0.3.1/featurebyte/worker/task/tile_task.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/featurebyte/worker/task_executor.py` & `featurebyte-0.3.1/featurebyte/worker/task_executor.py`

 * *Files identical despite different names*

### Comparing `featurebyte-0.3.0/pyproject.toml` & `featurebyte-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     "featurebyte/sql/spark/*.jar",
 ]
 keywords = []
 license = "Elastic License 2.0"
 name = "featurebyte"
 readme = "README.md"
 repository = "https://github.com/featurebyte/featurebyte"
-version = "0.3.0"
+version = "0.3.1"
 
 [tool.poetry.dependencies]
 PyYAML = "^6.0"
 aiofiles = "^22.1.0"
 aioredis = { version = "^2.0.1", optional = true }
 alive-progress = "^3.1.1"
 asyncache = "^0.3.1"
```

### Comparing `featurebyte-0.3.0/PKG-INFO` & `featurebyte-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurebyte
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python Library for FeatureOps
 Home-page: https://featurebyte.com
 License: Elastic License 2.0
 Author: FeatureByte
 Author-email: it-admin@featurebyte.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

