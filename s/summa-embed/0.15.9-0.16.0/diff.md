# Comparing `tmp/summa_embed-0.15.9.tar.gz` & `tmp/summa_embed-0.16.0.tar.gz`

## Comparing `summa_embed-0.15.9.tar` & `summa_embed-0.16.0.tar`

### file list

```diff
@@ -1,106 +1,107 @@
--rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.15.9/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2262 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20      393 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/dag_pb.proto
--rw-r--r--   0      501       20    10419 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7125 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20      407 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/unixfs.proto
--rw-r--r--   0      501       20       96 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2353 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      424 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0     2084 1970-01-01 00:00:00.000000 summa_embed-0.15.9/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20       92 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7087 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5015 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20     1021 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/driver.rs
--rw-r--r--   0      501       20    13794 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    24648 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13833 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    14323 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5038 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     4711 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      163 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20    16401 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1595 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    57848 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     2216 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11274 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7439 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     3093 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8014 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5258 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2421 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     5490 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      450 2023-06-01 08:47:09.000000 summa_embed-0.15.9/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      861 1970-01-01 00:00:00.000000 summa_embed-0.15.9/Cargo.toml
--rw-r--r--   0      501       20      685 2023-06-01 08:47:09.000000 summa_embed-0.15.9/.gitignore
--rwxr-xr-x   0      501       20      347 2023-06-01 08:47:09.000000 summa_embed-0.15.9/build.sh
--rw-r--r--   0      501       20      515 2023-06-01 08:47:09.000000 summa_embed-0.15.9/pyproject.toml
--rw-r--r--   0      501       20       14 2023-06-01 08:47:09.000000 summa_embed-0.15.9/requirements.txt
--rw-r--r--   0      501       20     4398 2023-06-01 08:47:09.000000 summa_embed-0.15.9/src/lib.rs
--rw-r--r--   0      501       20     1082 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/__init__.py
--rw-r--r--   0      501       20        0 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/__init__.py
--rw-r--r--   0      501       20     3124 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/consumer_service_pb2.py
--rw-r--r--   0      501       20     3153 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/consumer_service_pb2.pyi
--rw-r--r--   0      501       20     1336 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/dag_pb_pb2.py
--rw-r--r--   0      501       20     1115 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/dag_pb_pb2.pyi
--rw-r--r--   0      501       20    16689 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/index_service_pb2.py
--rw-r--r--   0      501       20    20021 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/index_service_pb2.pyi
--rw-r--r--   0      501       20    21461 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/query_pb2.py
--rw-r--r--   0      501       20    29410 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/query_pb2.pyi
--rw-r--r--   0      501       20     2214 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/reflection_service_pb2.py
--rw-r--r--   0      501       20     1996 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/reflection_service_pb2.pyi
--rw-r--r--   0      501       20     2012 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/search_service_pb2.py
--rw-r--r--   0      501       20     1903 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/search_service_pb2.pyi
--rw-r--r--   0      501       20     1742 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/unixfs_pb2.py
--rw-r--r--   0      501       20     1653 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/unixfs_pb2.pyi
--rw-r--r--   0      501       20     1041 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/utils_pb2.py
--rw-r--r--   0      501       20      455 2023-06-01 08:47:09.000000 summa_embed-0.15.9/summa_embed/proto/utils_pb2.pyi
--rw-r--r--   0      501       20   102226 2023-06-01 08:47:30.000000 summa_embed-0.15.9/Cargo.lock
--rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.9/PKG-INFO
+-rw-r--r--   0        0        0     2098 1970-01-01 00:00:00.000000 summa_embed-0.16.0/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-08 13:34:47.000000 summa_embed-0.16.0/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20       92 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7181 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5015 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20     1021 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/driver.rs
+-rw-r--r--   0      501       20    13794 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    24071 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13833 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    14323 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5038 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     4711 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      167 2023-06-08 13:34:48.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20    15532 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1687 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    59733 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     4400 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/term_field_mappers.rs
+-rw-r--r--   0      501       20     2216 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11274 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7439 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     3568 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8014 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-06-08 13:34:49.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5474 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-06-08 13:34:50.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      450 2023-06-08 13:34:51.000000 summa_embed-0.16.0/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 summa_embed-0.16.0/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2262 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10469 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7638 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-06-08 13:34:52.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2523 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      394 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-06-08 13:34:53.000000 summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 summa_embed-0.16.0/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-06-08 13:34:51.000000 summa_embed-0.16.0/.gitignore
+-rwxr-xr-x   0      501       20      347 2023-06-08 13:34:51.000000 summa_embed-0.16.0/build.sh
+-rw-r--r--   0      501       20      515 2023-06-08 13:34:51.000000 summa_embed-0.16.0/pyproject.toml
+-rw-r--r--   0      501       20       14 2023-06-08 13:34:51.000000 summa_embed-0.16.0/requirements.txt
+-rw-r--r--   0      501       20     4617 2023-06-08 13:34:52.000000 summa_embed-0.16.0/src/lib.rs
+-rw-r--r--   0      501       20     1559 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/__init__.py
+-rw-r--r--   0      501       20        0 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/__init__.py
+-rw-r--r--   0      501       20     3124 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/consumer_service_pb2.py
+-rw-r--r--   0      501       20     3153 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/consumer_service_pb2.pyi
+-rw-r--r--   0      501       20     1336 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/dag_pb_pb2.py
+-rw-r--r--   0      501       20     1115 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/dag_pb_pb2.pyi
+-rw-r--r--   0      501       20    16903 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/index_service_pb2.py
+-rw-r--r--   0      501       20    20493 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/index_service_pb2.pyi
+-rw-r--r--   0      501       20    23885 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/query_pb2.py
+-rw-r--r--   0      501       20    32310 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/query_pb2.pyi
+-rw-r--r--   0      501       20     2214 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/reflection_service_pb2.py
+-rw-r--r--   0      501       20     1996 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/reflection_service_pb2.pyi
+-rw-r--r--   0      501       20     2012 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/search_service_pb2.py
+-rw-r--r--   0      501       20     1903 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/search_service_pb2.pyi
+-rw-r--r--   0      501       20     1742 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/unixfs_pb2.py
+-rw-r--r--   0      501       20     1653 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/unixfs_pb2.pyi
+-rw-r--r--   0      501       20     1041 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/utils_pb2.py
+-rw-r--r--   0      501       20      455 2023-06-08 13:34:52.000000 summa_embed-0.16.0/summa_embed/proto/utils_pb2.pyi
+-rw-r--r--   0      501       20   101494 2023-06-08 13:37:40.000000 summa_embed-0.16.0/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.16.0/PKG-INFO
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.16.0/local_dependencies/summa-proto/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-proto"
-version = "0.26.0"
+version = "0.27.0"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa search server proto files"
 
 [lib]
 name = "summa_proto"
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.16.0/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/build.rs` & `summa_embed-0.16.0/local_dependencies/summa-proto/build.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.16.0/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.16.0/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.16.0/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
   string index_name = 1;
   // Attach index engine request
   oneof index_engine {
     AttachFileEngineRequest file = 2;
     AttachRemoteEngineRequest remote = 3;
   }
   MergePolicy merge_policy = 10;
+  QueryParserConfig query_parser_config = 11;
 }
 
 // Description of the attached index
 message AttachIndexResponse {
   IndexDescription index = 1;
 }
 
@@ -143,16 +144,14 @@
 }
 
 message IndexAttributes {
   // Timestamp when index has been created
   uint64 created_at = 1;
   // Unique fields of the index. Summa maintains unique constraint on them and uses for deduplicating data
   repeated string unique_fields = 2;
-  // Default fields that are using in `MatchQuery`
-  repeated string default_fields = 3;
   // Multi fields is ones that may have multiple values and processed as lists. All other fields will be forcefully converted to singular value
   repeated string multi_fields = 4;
   // Descriptive field that may be used as name for index when indices are replicating over wire
   optional string default_index_name = 5;
   // Text index description
   optional string description = 6;
   // (Not-used)
@@ -177,14 +176,15 @@
   optional uint32 blocksize = 4;
   // Field for sorting
   optional SortByField sort_by_field = 5;
   // Optional index fields
   IndexAttributes index_attributes = 6;
   // Merge policy
   MergePolicy merge_policy = 20;
+  QueryParserConfig query_parser_config = 21;
 }
 
 message CreateIndexResponse {
   IndexDescription index = 1;
 }
 
 message DeleteDocumentsRequest {
@@ -350,15 +350,16 @@
   oneof config {
     FileEngineConfig file = 1;
     MemoryEngineConfig memory = 2;
     RemoteEngineConfig remote = 3;
   }
   // Merge policy
   MergePolicy merge_policy = 10;
-  map<string, string> field_aliases = 11;
+  QueryParserConfig query_parser_config = 11;
+  map<string, string> field_triggers = 12;
 }
 
 // Description containing `Index` metadata fields
 message IndexDescription {
   string index_name = 1;
   // All index aliases
   repeated string index_aliases = 2;
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.16.0/local_dependencies/summa-proto/proto/query.proto`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,50 @@
 syntax = "proto3";
 package summa.proto;
 
 import "utils.proto";
 
+message FieldMapper {
+  string mapper_name = 1;
+  repeated string fields = 2;
+}
+
+message MatchQueryBooleanShouldMode {};
+message MatchQueryDisjuctionMaxMode {
+  float tie_breaker = 1;
+};
+message ExactMatchesPromoter {
+  uint32 slop = 1;
+  optional float boost = 2;
+}
+enum MissingFieldPolicy {
+  AsUsualTerms = 0;
+  Remove = 1;
+  Fail = 2;
+}
+
+message InflectionConfig {
+  bool derive_plural = 1;
+}
+
+message QueryParserConfig {
+  map<string, string> field_aliases = 1;
+  map<string, float> field_boosts = 2;
+  map<string, FieldMapper> field_mappings = 3;
+  uint32 term_limit = 4;
+  repeated string default_fields = 5;
+  oneof default_mode {
+    MatchQueryBooleanShouldMode boolean_should_mode = 6;
+    MatchQueryDisjuctionMaxMode disjuction_max_mode = 7;
+  }
+  ExactMatchesPromoter exact_matches_promoter = 8;
+  MissingFieldPolicy missing_field_policy = 9;
+  map<string, InflectionConfig> inflection_configs = 10;
+}
+
 message SearchResponse {
   // Time spent inside of `search` handler
   double elapsed_secs = 1;
   // An array of collector outputs
   repeated CollectorOutput collector_outputs = 2;
 }
 
@@ -60,32 +98,17 @@
 }
 
 message RangeQuery {
   string field = 1;
   Range value = 2;
 }
 
-message MatchQueryBooleanShouldMode {};
-message MatchQueryDisjuctionMaxMode {
-  float tie_breaker = 1;
-};
-message ExactMatchesPromoter {
-  uint32 slop = 1;
-  optional float boost = 2;
-}
-
 message MatchQuery {
   string value = 1;
-  repeated string default_fields = 2;
-  oneof default_mode {
-    MatchQueryBooleanShouldMode boolean_should_mode = 3;
-    MatchQueryDisjuctionMaxMode disjuction_max_mode = 4;
-  }
-  map<string, float> field_boosts = 5;
-  ExactMatchesPromoter exact_matches_promoter = 6;
+  optional QueryParserConfig query_parser_config = 2;
 }
 
 message BooleanSubquery {
   Occur occur = 1;
   Query query = 2;
 }
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.16.0/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.16.0/local_dependencies/summa-proto/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,18 @@
 ///     let search_response = search_api_client
 ///         .search(proto::SearchRequest {
 ///             index_queries: vec![proto::IndexQuery {
 ///                 index_alias: "test_index".to_string(),
 ///                 query: Some(proto::Query {
 ///                     query: Some(proto::query::Query::Match(proto::MatchQuery {
 ///                         value: "game of thrones".to_string(),
-///                         default_fields: vec!["title".to_string()],
+///                         query_parser_config: Some(proto::QueryParserConfig {
+///                             default_fields: vec!["title".to_string()],
+///                             ..Default::default()
+///                         }),
 ///                         ..Default::default()
 ///                     })),
 ///                 }),
 ///                 collectors: vec![
 ///                     proto::Collector {
 ///                         collector: Some(proto::collector::Collector::TopDocs(proto::TopDocsCollector {
 ///                             limit: 10,
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.16.0/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.16.0/local_dependencies/summa-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.15.9"
+version = "0.16.0"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
@@ -33,18 +33,19 @@
 itertools = "0.10"
 lru = "0.10.0"
 oneshot = "0.1"
 opentelemetry = { version = "0.19", features = ["metrics", "rt-tokio"], optional = true }
 parking_lot = { version = "0.12", features = ["send_guard"] }
 pest = "2.5"
 pest_derive = "2.5"
+pluralize-rs = "0.1"
 prost = "0.11"
 rand = { version = "0.8", features = ["small_rng"] }
 rayon = "1.6.1"
-safe-regex = "0.2.5"
+regex = "1.8"
 rustc-hash = "1.1.0"
 serde = { version = "1.0", default_features = false, features = ["derive", "std"] }
 serde_bytes = "0.11"
 serde_cbor = "0.11"
 serde_json = { version = "1.0" }
 serde_yaml = { version = "0.8" }
 strfmt = "0.2"
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/LICENSE` & `summa_embed-0.16.0/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 use tantivy::collector::SegmentCollector;
 use tantivy::{DocAddress, DocId, Score, SegmentOrdinal, SegmentReader};
 
 /// `ReservoirSampling` collector collects `k` random documents using `O(k)` memory
 ///
 /// ```rust
 /// use summa_core::collectors::ReservoirSampling;
+/// use summa_core::configs::core::QueryParserConfig;
 /// use tantivy::collector::Count;
 /// use summa_core::components::QueryParser;
 /// use tantivy::schema::{Schema, TEXT};
 /// use tantivy::{doc, Index};
 ///
 /// let mut schema_builder = Schema::builder();
 /// let title = schema_builder.add_text_field("title", TEXT);
@@ -25,15 +26,15 @@
 /// index_writer.add_document(doc!(title => "The Diary of a Young Girl")).unwrap();
 /// assert!(index_writer.commit().is_ok());
 ///
 /// let reader = index.reader().unwrap();
 /// let searcher = reader.searcher();
 ///
 /// // Here comes the important part
-/// let query_parser = QueryParser::for_index(&index, vec!["title".to_string()]).unwrap();
+/// let query_parser = QueryParser::for_index(&index, QueryParserConfig::from_default_fields(vec!["title".to_string()])).unwrap();
 /// let query = query_parser.parse_query("diary").unwrap();
 /// let documents = searcher.search(&query, &ReservoirSampling::with_limit(2)).unwrap();
 ///
 /// assert_eq!(documents.len(), 2);
 /// ```
 pub struct ReservoirSampling {
     limit: usize,
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/driver.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/driver.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::collections::{HashMap, HashSet};
+use std::collections::HashSet;
 use std::fmt::Debug;
 use std::hash::{Hash, Hasher};
 use std::path::Path;
 use std::sync::Arc;
 
 use futures::future::{join_all, try_join_all};
 #[cfg(feature = "metrics")]
@@ -156,21 +156,20 @@
     /// Sets up `IndexHolder`
     pub fn create_holder(
         core_config: &crate::configs::core::Config,
         mut index: Index,
         index_name: Option<&str>,
         index_engine_config: Arc<dyn ConfigProxy<proto::IndexEngineConfig>>,
         merge_policy: Option<proto::MergePolicy>,
-        field_aliases: HashMap<String, String>,
-        read_only: bool,
+        query_parser_config: proto::QueryParserConfig,
         driver: Driver,
     ) -> SummaResult<IndexHolder> {
         register_default_tokenizers(&index);
 
-        index.settings_mut().docstore_compress_dedicated_thread = core_config.dedicated_compression_thread;
+        index.settings_mut().docstore_compress_threads = core_config.doc_store_compress_threads;
         index.set_segment_attributes_merger(Arc::new(SegmentAttributesMergerImpl::<SummaSegmentAttributes>::new()));
 
         let metas = index.load_metas()?;
         let cached_schema = index.schema();
         let cached_index_attributes: Option<IndexAttributes> = metas.index_attributes()?;
         let cached_multi_fields = cached_index_attributes
             .as_ref()
@@ -189,39 +188,33 @@
                 .as_ref()
                 .expect("no attributes")
                 .default_index_name
                 .clone()
                 .expect("no index name")
         });
 
-        let query_parser = ProtoQueryParser::for_index(
-            &index_name,
-            &index,
-            cached_index_attributes.as_ref().map(|a| a.default_fields.clone()).unwrap_or_else(Vec::new),
-            field_aliases,
-        )?;
+        let query_parser = ProtoQueryParser::for_index(&index_name, &index, query_parser_config)?;
         let index_reader = index
             .reader_builder()
             .doc_store_cache_num_blocks(core_config.doc_store_cache_num_blocks)
             .reload_policy(ReloadPolicy::OnCommit)
             .try_into()?;
         index_reader.reload()?;
 
-        let index_writer_holder = match (read_only, &core_config.writer_threads) {
-            (true, _) | (_, None) => None,
-            (_, Some(writer_threads)) => {
-                let merge_policy = Wrapper::from(merge_policy).into();
-                info!(action = "create_index_writer", merge_policy = ?merge_policy, writer_threads = ?writer_threads, writer_heap_size_bytes = core_config.writer_heap_size_bytes);
-                Some(Arc::new(RwLock::new(IndexWriterHolder::create(
-                    &index,
-                    writer_threads.clone(),
-                    core_config.writer_heap_size_bytes as usize,
-                    merge_policy,
-                )?)))
-            }
+        let index_writer_holder = if let Some(writer_threads) = &core_config.writer_threads {
+            let merge_policy = Wrapper::from(merge_policy).into();
+            info!(action = "create_index_writer", merge_policy = ?merge_policy, writer_threads = ?writer_threads, writer_heap_size_bytes = core_config.writer_heap_size_bytes);
+            Some(Arc::new(RwLock::new(IndexWriterHolder::create(
+                &index,
+                writer_threads.clone(),
+                core_config.writer_heap_size_bytes as usize,
+                merge_policy,
+            )?)))
+        } else {
+            None
         };
 
         Ok(IndexHolder {
             index_engine_config,
             index_name,
             index: index.clone(),
             query_parser,
@@ -271,26 +264,26 @@
     }
 
     pub async fn open_remote_index<
         TExternalRequest: ExternalRequest + 'static,
         TExternalRequestGenerator: ExternalRequestGenerator<TExternalRequest> + 'static,
     >(
         remote_engine_config: proto::RemoteEngineConfig,
-        read_only: bool,
+        read_hotcache: bool,
     ) -> SummaResult<Index> {
-        info!(action = "opening_network_directory", config = ?remote_engine_config, read_only = read_only);
+        info!(action = "opening_network_directory", config = ?remote_engine_config, read_hotcache = read_hotcache);
         let network_directory = NetworkDirectory::open(Box::new(TExternalRequestGenerator::new(remote_engine_config.clone())));
         let opstamp = read_opstamp(&network_directory).await?;
         let hotcache_bytes = match network_directory
             .get_network_file_handle(format!("hotcache.{}.bin", opstamp).as_ref())
             .do_read_bytes_async(None)
             .await
         {
             Ok(hotcache_bytes) => {
-                if read_only {
+                if read_hotcache {
                     info!(action = "read_hotcache", len = hotcache_bytes.len());
                     Some(hotcache_bytes)
                 } else {
                     warn!(action = "omit_hotcache");
                     None
                 }
             }
@@ -355,43 +348,35 @@
 
     /// Return internal Tantivy index
     pub fn real_directory(&self) -> &dyn Directory {
         self.index.directory().real_directory()
     }
 
     /// Load term dictionaries into memory
-    pub async fn partial_warmup(&self, load_dictionaries: bool) -> SummaResult<()> {
+    pub async fn partial_warmup<T: AsRef<str>>(&self, load_dictionaries: bool, fields: &[T]) -> SummaResult<()> {
         let searcher = self.index_reader().searcher();
         let mut warm_up_futures = Vec::new();
-        let index_attributes = self.index_attributes();
-        let default_fields = index_attributes
-            .map(|index_attributes| {
-                index_attributes
-                    .default_fields
-                    .iter()
-                    .map(|field_name| self.cached_schema.get_field(field_name))
-                    .collect::<Result<Vec<_>, _>>()
-            })
-            .transpose()?;
-        if let Some(default_fields) = default_fields {
-            for field in default_fields {
-                for segment_reader in searcher.segment_readers() {
-                    let inverted_index = segment_reader.inverted_index_async(field).await?.clone();
-                    if load_dictionaries {
-                        warm_up_futures.push(async move {
-                            let dict = inverted_index.terms();
-                            info!(action = "warming_up_dictionary", index_name = ?self.index_name());
-                            dict.warm_up_dictionary().await
-                        });
-                    }
+        let default_fields = fields
+            .iter()
+            .map(|field_name| self.cached_schema.get_field(field_name.as_ref()))
+            .collect::<Result<Vec<_>, _>>()?;
+        for field in default_fields {
+            for segment_reader in searcher.segment_readers() {
+                let inverted_index = segment_reader.inverted_index_async(field).await?.clone();
+                if load_dictionaries {
+                    warm_up_futures.push(async move {
+                        let dict = inverted_index.terms();
+                        info!(action = "warming_up_dictionary", index_name = ?self.index_name());
+                        dict.warm_up_dictionary().await
+                    });
                 }
             }
-            info!(action = "warming_up");
-            try_join_all(warm_up_futures).await?;
         }
+        info!(action = "warming_up");
+        try_join_all(warm_up_futures).await?;
         Ok(())
     }
 
     /// Load all index files into memory
     pub async fn full_warmup(&self) -> SummaResult<()> {
         let managed_directory = self.index.directory();
         info!(action = "warming_up");
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-use std::collections::HashMap;
 use std::ops::Bound;
 use std::ops::Bound::Unbounded;
 use std::str::FromStr;
 
 use base64::Engine;
 #[cfg(feature = "metrics")]
 use opentelemetry::metrics::Counter;
@@ -13,47 +12,47 @@
 use summa_proto::proto;
 use tantivy::json_utils::{convert_to_fast_value_and_get_term, JsonTermWriter};
 use tantivy::query::{
     AllQuery, BooleanQuery, BoostQuery, DisjunctionMaxQuery, EmptyQuery, MoreLikeThisQuery, Occur, PhraseQuery, Query, RangeQuery, RegexQuery, TermQuery,
 };
 use tantivy::schema::{Field, FieldEntry, FieldType, IndexRecordOption, Schema};
 use tantivy::{DateTime, Index, Score, Term};
-use tracing::{info, warn};
+use tracing::info;
 
 use crate::components::queries::ExistsQuery;
 use crate::components::query_parser::{QueryParser, QueryParserError};
+use crate::configs::core::QueryParserConfig;
 use crate::errors::{Error, SummaResult, ValidationError};
 #[cfg(feature = "metrics")]
 use crate::metrics::ToLabel;
 
 /// Responsible for casting `crate::proto::Query` message to `tantivy::query::Query`
 pub struct ProtoQueryParser {
     index: Index,
     index_name: String,
     cached_schema: Schema,
     // Counters
     #[cfg(feature = "metrics")]
     query_counter: Counter<u64>,
     #[cfg(feature = "metrics")]
     subquery_counter: Counter<u64>,
-    index_default_fields: Vec<String>,
-    field_aliases: HashMap<String, String>,
+    query_parser_config: QueryParserConfig,
 }
 
-pub enum MatchQueryDefaultMode {
+pub enum QueryParserDefaultMode {
     Boolean,
     DisjuctionMax { tie_breaker: Score },
 }
 
-impl From<Option<proto::match_query::DefaultMode>> for MatchQueryDefaultMode {
-    fn from(value: Option<proto::match_query::DefaultMode>) -> Self {
+impl From<Option<proto::query_parser_config::DefaultMode>> for QueryParserDefaultMode {
+    fn from(value: Option<proto::query_parser_config::DefaultMode>) -> Self {
         match value {
-            Some(proto::match_query::DefaultMode::BooleanShouldMode(_)) | None => MatchQueryDefaultMode::Boolean,
-            Some(proto::match_query::DefaultMode::DisjuctionMaxMode(proto::MatchQueryDisjuctionMaxMode { tie_breaker })) => {
-                MatchQueryDefaultMode::DisjuctionMax { tie_breaker }
+            Some(proto::query_parser_config::DefaultMode::BooleanShouldMode(_)) | None => QueryParserDefaultMode::Boolean,
+            Some(proto::query_parser_config::DefaultMode::DisjuctionMaxMode(proto::MatchQueryDisjuctionMaxMode { tie_breaker })) => {
+                QueryParserDefaultMode::DisjuctionMax { tie_breaker }
             }
         }
     }
 }
 
 fn cast_value_to_term(field: Field, full_path: &str, field_type: &FieldType, value: &str) -> SummaResult<Term> {
     Ok(match field_type {
@@ -103,20 +102,15 @@
                 Bound::Excluded(casted_value)
             }
         }
     })
 }
 
 impl ProtoQueryParser {
-    pub fn for_index(
-        index_name: &str,
-        index: &Index,
-        index_default_fields: Vec<String>,
-        field_aliases: HashMap<String, String>,
-    ) -> SummaResult<ProtoQueryParser> {
+    pub fn for_index(index_name: &str, index: &Index, query_parser_config: proto::QueryParserConfig) -> SummaResult<ProtoQueryParser> {
         #[cfg(feature = "metrics")]
         let query_counter = global::meter("summa").u64_counter("query_counter").with_description("Queries counter").init();
         #[cfg(feature = "metrics")]
         let subquery_counter = global::meter("summa")
             .u64_counter("subquery_counter")
             .with_description("Sub-queries counter")
             .init();
@@ -125,21 +119,25 @@
             index: index.clone(),
             index_name: index_name.to_string(),
             cached_schema: index.schema(),
             #[cfg(feature = "metrics")]
             query_counter,
             #[cfg(feature = "metrics")]
             subquery_counter,
-            index_default_fields,
-            field_aliases,
+            query_parser_config: QueryParserConfig(query_parser_config),
         })
     }
 
     pub fn resolve_field_name<'a>(&'a self, field_name: &'a str) -> &str {
-        self.field_aliases.get(field_name).map(|s| s.as_str()).unwrap_or(field_name)
+        self.query_parser_config
+            .0
+            .field_aliases
+            .get(field_name)
+            .map(|s| s.as_str())
+            .unwrap_or(field_name)
     }
 
     #[inline]
     pub(crate) fn field_and_field_entry<'a>(&'a self, field_name: &'a str) -> SummaResult<(Field, &str, &FieldEntry)> {
         match self.cached_schema.find_field(self.resolve_field_name(field_name)) {
             Some((field, full_path)) => {
                 let field_entry = self.cached_schema.get_field_entry(field);
@@ -184,40 +182,21 @@
                     .collect::<SummaResult<Vec<_>>>()?,
                 match disjunction_max_proto.tie_breaker.as_str() {
                     "" => 0.0,
                     s => f32::from_str(s).map_err(|_e| Error::InvalidSyntax(format!("cannot parse {} as f32", disjunction_max_proto.tie_breaker)))?,
                 },
             )),
             proto::query::Query::Match(match_query_proto) => {
-                let default_fields = if !match_query_proto.default_fields.is_empty() {
-                    match_query_proto.default_fields
-                } else {
-                    self.index_default_fields.clone()
-                };
-                if default_fields.is_empty() {
-                    warn!(
-                        action = "missing_default_fields",
-                        hint = "Add `default_fields` to match query, otherwise you match nothing"
-                    )
-                }
-                let mut nested_query_parser = QueryParser::for_index(&self.index, default_fields)?;
-                nested_query_parser.set_default_mode(match_query_proto.default_mode.into());
-
-                if !match_query_proto.field_boosts.is_empty() {
-                    nested_query_parser.set_field_boosts(match_query_proto.field_boosts)
-                }
-
-                if let Some(exact_matches_promoter) = match_query_proto.exact_matches_promoter {
-                    nested_query_parser.set_exact_match_promoter(exact_matches_promoter)
-                }
-
-                if !self.field_aliases.is_empty() {
-                    nested_query_parser.set_field_aliases(self.field_aliases.clone())
-                }
-
+                let nested_query_parser = QueryParser::for_index(
+                    &self.index,
+                    match_query_proto
+                        .query_parser_config
+                        .map(QueryParserConfig)
+                        .unwrap_or_else(|| self.query_parser_config.clone()),
+                )?;
                 match nested_query_parser.parse_query(&match_query_proto.value) {
                     Ok(parsed_query) => {
                         info!(parsed_match_query = ?parsed_query);
                         Ok(parsed_query)
                     }
                     Err(QueryParserError::FieldDoesNotExist(field)) => Err(ValidationError::MissingField(field).into()),
                     Err(e) => Err(Error::InvalidQuerySyntax(Box::new(e), match_query_proto.value.to_owned())),
@@ -308,15 +287,15 @@
             }
             proto::query::Query::Exists(exists_query_proto) => {
                 let (field, full_path, field_entry) = self.field_and_field_entry(&exists_query_proto.field)?;
                 if !field_entry.field_type().is_indexed() {
                     let fni = QueryParserError::FieldNotIndexed(field_entry.name().to_string());
                     return Err(Error::InvalidQuerySyntax(Box::new(fni), exists_query_proto.field.to_string()));
                 }
-                if full_path == "" {
+                if full_path.is_empty() {
                     Box::new(ExistsQuery::new(field))
                 } else {
                     Box::new(TermQuery::new(
                         cast_value_to_term(field, full_path, field_entry.field_type(), "")?,
                         field_entry.field_type().index_record_option().unwrap_or(IndexRecordOption::Basic),
                     ))
                 }
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 quote = _{ "\"" | "'" | "`" | "'" | "“" | "”" | "‘" | "«" | "»" | "„" | "`"}
 star = { "*" }
 statement_sep = _{ WHITE_SPACE | "," | "." | ";" | "!" | "?" | (":" ~ WHITE_SPACE) | "(" | ")" | "/" }
 allowed_chars = _{"_" | "+" | "#" | "-"}
+url_end = _{ WHITE_SPACE | "," }
 
 isbn = @{ "978" ~ ("-"? ~ ASCII_DIGIT){7,10} ~ EOI }
 doi = @{ "10." ~ ASCII_DIGIT{4,9} ~ WHITE_SPACE? ~ "/" ~ WHITE_SPACE? ~ (!WHITE_SPACE ~ ANY)+ }
 wrapped_doi = _{ ("http" ~ "s"? ~ "://")? ~ "doi.org/"? ~ doi }
+// url = _{ ("http" ~ "s"? ~ "://")? ~ (!url_end ~ ANY)+ }
 
 slop = @{ DECIMAL_NUMBER+ }
 boost = { (DECIMAL_NUMBER | ".")+ }
 range = ${ "[" ~ WHITE_SPACE* ~ boundary_word ~ WHITE_SPACE+ ~ ^"to" ~ WHITE_SPACE+ ~ boundary_word ~ WHITE_SPACE* ~ "]" }
 
 field_name = @{ ASCII_ALPHA ~ (ASCII_ALPHANUMERIC | "_" | ".")* }
 word = @{ wrapped_doi | ((LETTER | NUMBER) ~ (LETTER | NUMBER | "_" | "+" | "#" | "-" | "–")*) }
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,38 @@
-use std::collections::{Bound, HashMap};
+use std::collections::Bound;
 use std::ops::Bound::{Included, Unbounded};
 use std::ops::Deref;
 use std::str::FromStr;
 
 use pest::iterators::{Pair, Pairs};
 use pest::Parser;
 use pest_derive::Parser;
-use safe_regex::{regex, Matcher3};
 use summa_proto::proto;
 use tantivy::json_utils::{convert_to_fast_value_and_get_term, JsonTermWriter};
 use tantivy::query::{BooleanQuery, BoostQuery, DisjunctionMaxQuery, EmptyQuery, PhraseQuery, Query, QueryClone, RangeQuery, RegexQuery, TermQuery};
 use tantivy::schema::{FacetParseError, Field, FieldEntry, FieldType, IndexRecordOption, Schema, TextFieldIndexing, Type};
 use tantivy::tokenizer::{TextAnalyzer, TokenizerManager};
 use tantivy::{Index, Term};
-use tantivy_common::HasLen;
 use tantivy_query_grammar::Occur;
 
-use crate::components::query_parser::proto_query_parser::MatchQueryDefaultMode;
+use crate::components::query_parser::proto_query_parser::QueryParserDefaultMode;
+use crate::components::query_parser::term_field_mappers::{DoiIsbnMapper, DoiMapper, IsbnMapper, TermFieldMapper};
+use crate::configs::core::QueryParserConfig;
 use crate::errors::SummaResult;
 use crate::utils::transpose;
 use crate::validators;
 
 #[derive(Parser)]
 #[grammar = "src/components/query_parser/summa_ql.pest"] // relative to src
 struct SummaQlParser;
 
-pub enum MissingFieldPolicy {
-    AsUsualTerms,
-    Remove,
-    Fail,
-}
-
 pub struct QueryParser {
     schema: Schema,
-    default_fields: Vec<Field>,
     tokenizer_manager: TokenizerManager,
-    missing_field_policy: MissingFieldPolicy,
-    limit: usize,
-    field_aliases: HashMap<String, String>,
-    field_boosts: Option<HashMap<String, f32>>,
-    default_mode: MatchQueryDefaultMode,
-    exact_matches_promoter: Option<proto::ExactMatchesPromoter>,
+    query_parser_config: QueryParserConfig,
 }
 
 /// Possible error that may happen when parsing a query.
 #[derive(thiserror::Error, Debug, PartialEq)]
 pub enum QueryParserError {
     /// Error in the query syntax
     #[error("syntax_error: {0}")]
@@ -184,92 +172,103 @@
             return Box::new(EmptyQuery {}) as Box<dyn Query>;
         }
         return Box::new(BooleanQuery::new(subqueries)) as Box<dyn Query>;
     }
     query
 }
 
+pub fn cast_field_to_term(field: &Field, full_path: &str, field_type: &FieldType, value: &str, force_str: bool) -> Term {
+    match field_type {
+        FieldType::Str(_) => Term::from_field_text(*field, value),
+        FieldType::JsonObject(ref json_options) => {
+            let mut term = Term::with_capacity(128);
+            let mut json_term_writer = JsonTermWriter::from_field_and_json_path(*field, full_path, json_options.is_expand_dots_enabled(), &mut term);
+            if force_str {
+                json_term_writer.set_str(value);
+                json_term_writer.term().clone()
+            } else {
+                convert_to_fast_value_and_get_term(&mut json_term_writer, value).unwrap_or_else(|| {
+                    json_term_writer.set_str(value);
+                    json_term_writer.term().clone()
+                })
+            }
+        }
+        _ => unreachable!(),
+    }
+}
+
 type Subqueries = Vec<(Occur, Box<dyn Query>)>;
 
 impl QueryParser {
-    pub fn new(schema: Schema, default_fields: Vec<String>, tokenizer_manager: &TokenizerManager) -> SummaResult<QueryParser> {
-        let default_fields = validators::parse_fields(&schema, &default_fields)?;
+    pub fn new(schema: Schema, query_parser_config: QueryParserConfig, tokenizer_manager: &TokenizerManager) -> SummaResult<QueryParser> {
+        validators::parse_fields(&schema, &query_parser_config.0.default_fields)?;
         Ok(QueryParser {
             schema,
-            default_fields,
             tokenizer_manager: tokenizer_manager.clone(),
-            missing_field_policy: MissingFieldPolicy::Remove,
-            limit: 16,
-            field_aliases: HashMap::new(),
-            field_boosts: None,
-            default_mode: MatchQueryDefaultMode::Boolean,
-            exact_matches_promoter: None,
+            query_parser_config,
         })
     }
 
-    pub fn for_index(index: &Index, default_fields: Vec<String>) -> SummaResult<QueryParser> {
-        QueryParser::new(index.schema(), default_fields, index.tokenizers())
-    }
-
-    pub fn set_field_aliases(&mut self, field_aliases: HashMap<String, String>) {
-        self.field_aliases = field_aliases;
-    }
-
-    pub fn set_field_boosts(&mut self, field_boosts: HashMap<String, f32>) {
-        self.field_boosts = Some(field_boosts);
-    }
-
-    pub fn set_default_mode(&mut self, default_mode: MatchQueryDefaultMode) {
-        self.default_mode = default_mode;
-    }
-
-    pub fn set_missing_field_policy(&mut self, missing_field_policy: MissingFieldPolicy) {
-        self.missing_field_policy = missing_field_policy;
-    }
-
-    pub fn set_exact_match_promoter(&mut self, exact_matches_promoter: proto::ExactMatchesPromoter) {
-        self.exact_matches_promoter = Some(exact_matches_promoter);
+    pub fn for_index(index: &Index, query_parser_config: QueryParserConfig) -> SummaResult<QueryParser> {
+        QueryParser::new(index.schema(), query_parser_config, index.tokenizers())
     }
 
     pub fn resolve_field_name<'a>(&'a self, field_name: &'a str) -> &str {
-        self.field_aliases.get(field_name).map(|s| s.as_str()).unwrap_or(field_name)
+        self.query_parser_config
+            .0
+            .field_aliases
+            .get(field_name)
+            .map(|s| s.as_str())
+            .unwrap_or(field_name)
     }
 
     fn get_text_analyzer(&self, field_entry: &FieldEntry, option: &TextFieldIndexing) -> Result<TextAnalyzer, QueryParserError> {
         self.tokenizer_manager
             .get(option.tokenizer())
             .ok_or_else(|| QueryParserError::UnknownTokenizer {
                 field: field_entry.name().to_string(),
                 tokenizer: option.tokenizer().to_string(),
             })
     }
 
-    fn default_fields_term(&self, term: Pair<Rule>, boost: Option<f32>) -> Result<Box<dyn Query>, QueryParserError> {
-        let term = term.into_inner().next().expect("grammar failure");
-        let occur = self.parse_occur(&term);
-        let pre_term = term.into_inner().next().expect("grammar failure");
+    fn default_field_queries(&self, term: Pair<Rule>, boost: Option<f32>) -> Result<Box<dyn Query>, QueryParserError> {
+        let (occur, term) = match term.as_rule() {
+            Rule::field_name => (Occur::Should, term),
+            _ => {
+                let term = term.into_inner().next().expect("grammar failure");
+                let occur = self.parse_occur(&term);
+                let pre_term = term.into_inner().next().expect("grammar failure");
+                (occur, pre_term.clone())
+            }
+        };
+
         let default_field_queries = self
+            .query_parser_config
+            .0
             .default_fields
             .iter()
-            .map(|field| self.parse_pre_term(field, "", pre_term.clone(), boost))
+            .map(|field| {
+                let (field, full_path) = self.schema.find_field(field).expect("inconsistent state");
+                self.parse_pre_term(&field, full_path, term.clone(), boost)
+            })
             .collect::<Result<Vec<_>, _>>()?;
 
         Ok(match occur {
             Occur::Should => {
                 let default_field_queries = default_field_queries.into_iter().flatten();
-                match self.default_mode {
-                    MatchQueryDefaultMode::Boolean => Box::new(BooleanQuery::new(default_field_queries.map(|q| (occur, q)).collect())) as Box<dyn Query>,
-                    MatchQueryDefaultMode::DisjuctionMax { tie_breaker } => {
+                match QueryParserDefaultMode::from(self.query_parser_config.0.default_mode.clone()) {
+                    QueryParserDefaultMode::Boolean => Box::new(BooleanQuery::new(default_field_queries.map(|q| (occur, q)).collect())) as Box<dyn Query>,
+                    QueryParserDefaultMode::DisjuctionMax { tie_breaker } => {
                         Box::new(DisjunctionMaxQuery::with_tie_breaker(default_field_queries.collect(), tie_breaker)) as Box<dyn Query>
                     }
                 }
             }
             Occur::MustNot => Box::new(BooleanQuery::new(default_field_queries.into_iter().flatten().map(|q| (occur, q)).collect())) as Box<dyn Query>,
             Occur::Must => {
-                if self.default_fields.len() == 1 {
+                if self.query_parser_config.0.default_fields.len() == 1 {
                     Box::new(BooleanQuery::new(
                         default_field_queries.into_iter().flatten().map(|q| (Occur::Must, q)).collect(),
                     )) as Box<dyn Query>
                 } else {
                     let transposed_default_field_queries = transpose(default_field_queries);
                     Box::new(BooleanQuery::new(
                         transposed_default_field_queries
@@ -328,39 +327,37 @@
             return Err(QueryParserError::NonJsonFieldWithPath(format!(
                 "{}.{}",
                 field_entry.name().to_string(),
                 full_path
             )));
         }
 
-        let boost = multiply_boosts(self.field_boosts.as_ref().and_then(|boosts| boosts.get(field_entry.name()).cloned()), boost);
+        if !(field_type.is_indexed() || matches!(pre_term.as_rule(), Rule::range) && field_type.is_fast()) {
+            return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
+        }
+
+        let boost = multiply_boosts(self.query_parser_config.0.field_boosts.get(field_entry.name()).copied(), boost);
 
         if matches!(pre_term.as_rule(), Rule::range) {
             return Ok(vec![boost_query(Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>, boost)]);
         }
 
         return match *field_type {
             FieldType::U64(_) => match pre_term.as_rule() {
                 Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                 Rule::phrase | Rule::word => {
-                    if !field_type.is_indexed() {
-                        return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
-                    }
                     let val: u64 = u64::from_str(pre_term.as_str())?;
                     let query = Box::new(TermQuery::new(Term::from_field_u64(*field, val), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                     Ok(vec![boost_query(query, boost)])
                 }
                 _ => unreachable!(),
             },
             FieldType::I64(_) => match pre_term.as_rule() {
                 Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                 Rule::phrase | Rule::word => {
-                    if !field_type.is_indexed() {
-                        return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
-                    }
                     let val: i64 = i64::from_str(pre_term.as_str())?;
                     let query = Box::new(TermQuery::new(Term::from_field_i64(*field, val), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                     Ok(vec![boost_query(query, boost)])
                 }
                 _ => unreachable!(),
             },
             FieldType::F64(_) => match pre_term.as_rule() {
@@ -374,17 +371,14 @@
                     Ok(vec![boost_query(query, boost)])
                 }
                 _ => unreachable!(),
             },
             FieldType::Bool(_) => match pre_term.as_rule() {
                 Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                 Rule::phrase | Rule::word => {
-                    if !field_type.is_indexed() {
-                        return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
-                    }
                     let val: bool = bool::from_str(pre_term.as_str())?;
                     let query = Box::new(TermQuery::new(Term::from_field_bool(*field, val), IndexRecordOption::WithFreqs)) as Box<dyn Query>;
                     Ok(vec![boost_query(query, boost)])
                 }
                 _ => unreachable!(),
             },
             FieldType::Str(_) | FieldType::JsonObject(_) => {
@@ -394,79 +388,98 @@
                     json_options.get_text_indexing_options().expect("unreachable")
                 } else {
                     unreachable!()
                 };
 
                 match pre_term.as_rule() {
                     Rule::word | Rule::field_name => {
-                        if !field_type.is_indexed() {
-                            return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
-                        }
-
                         let mut token_stream = self.get_text_analyzer(field_entry, indexing)?.token_stream(pre_term.as_str());
                         let mut queries = Vec::new();
-
                         token_stream.process(&mut |token| {
-                            let term = match field_type {
-                                FieldType::Str(_) => Term::from_field_text(*field, &token.text),
-                                FieldType::JsonObject(ref json_options) => {
-                                    let mut term = Term::with_capacity(128);
-                                    let mut json_term_writer =
-                                        JsonTermWriter::from_field_and_json_path(*field, full_path, json_options.is_expand_dots_enabled(), &mut term);
-                                    convert_to_fast_value_and_get_term(&mut json_term_writer, &token.text).unwrap_or_else(|| {
-                                        json_term_writer.set_str(&token.text);
-                                        json_term_writer.term().clone()
-                                    })
+                            let term = cast_field_to_term(field, full_path, field_type, &token.text, false);
+                            let inflection_config = self
+                                .query_parser_config
+                                .0
+                                .inflection_configs
+                                .get(field_entry.name())
+                                .cloned()
+                                .unwrap_or_default();
+                            if inflection_config.derive_plural {
+                                let is_singular = pluralize_rs::is_singular(&token.text);
+                                let is_plural = pluralize_rs::is_plural(&token.text);
+                                let other_token = if is_singular {
+                                    Some(pluralize_rs::to_plural(&token.text))
+                                } else if is_plural {
+                                    Some(pluralize_rs::to_singular(&token.text))
+                                } else {
+                                    None
+                                };
+                                if let Some(other_token) = other_token {
+                                    let other_term = cast_field_to_term(field, full_path, field_type, &other_token, false);
+                                    let disjunction_query = DisjunctionMaxQuery::new(vec![
+                                        Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>,
+                                        Box::new(TermQuery::new(other_term, IndexRecordOption::WithFreqs)) as Box<dyn Query>,
+                                    ]);
+                                    queries.push(boost_query(Box::new(disjunction_query) as Box<dyn Query>, boost))
                                 }
-                                _ => unreachable!(),
-                            };
-                            let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
-                            queries.push(boost_query(query, boost));
+                            } else {
+                                let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
+                                queries.push(boost_query(query, boost));
+                            }
                         });
-
                         Ok(queries)
                     }
                     Rule::phrase => {
-                        if !field_type.is_indexed() {
-                            return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
-                        }
-
                         let mut phrase_pairs = pre_term.into_inner();
                         let words = match phrase_pairs.next() {
                             None => return Ok(vec![]),
                             Some(words) => words,
                         };
-                        let slop = phrase_pairs
-                            .next()
-                            .map(|v| match v.as_str() {
-                                "" => 0,
-                                _ => u32::from_str(v.as_str()).expect("cannot parse"),
-                            })
-                            .unwrap_or(0);
-                        let terms = self.parse_words(*field, indexing, words.as_str())?;
-                        if terms.len() <= 1 {
-                            return Ok(terms
-                                .into_iter()
-                                .map(|(_, term)| {
+
+                        match field_type {
+                            FieldType::JsonObject(_) => {
+                                let mut token_stream = self.get_text_analyzer(field_entry, indexing)?.token_stream(words.as_str());
+                                let mut queries = Vec::new();
+
+                                token_stream.process(&mut |token| {
+                                    let term = cast_field_to_term(field, full_path, field_type, &token.text, true);
                                     let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
-                                    boost_query(query, boost)
-                                })
-                                .collect());
-                        }
-                        if !indexing.index_option().has_positions() {
-                            return Err(QueryParserError::FieldDoesNotHavePositionsIndexed(field_entry.name().to_string()));
+                                    queries.push(boost_query(query, boost));
+                                });
+
+                                Ok(queries)
+                            }
+                            _ => {
+                                let slop = phrase_pairs
+                                    .next()
+                                    .map(|v| match v.as_str() {
+                                        "" => 0,
+                                        _ => u32::from_str(v.as_str()).expect("cannot parse"),
+                                    })
+                                    .unwrap_or(0);
+                                let terms = self.parse_words(*field, indexing, words.as_str())?;
+                                if terms.len() <= 1 {
+                                    return Ok(terms
+                                        .into_iter()
+                                        .map(|(_, term)| {
+                                            let query = Box::new(TermQuery::new(term, IndexRecordOption::WithFreqs)) as Box<dyn Query>;
+                                            boost_query(query, boost)
+                                        })
+                                        .collect());
+                                }
+                                if !indexing.index_option().has_positions() {
+                                    return Err(QueryParserError::FieldDoesNotHavePositionsIndexed(field_entry.name().to_string()));
+                                }
+                                let query = Box::new(PhraseQuery::new_with_offset_and_slop(terms, slop)) as Box<dyn Query>;
+                                return Ok(vec![boost_query(query, boost)]);
+                            }
                         }
-                        let query = Box::new(PhraseQuery::new_with_offset_and_slop(terms, slop)) as Box<dyn Query>;
-                        return Ok(vec![boost_query(query, boost)]);
                     }
                     Rule::range => Ok(vec![Box::new(self.parse_range(pre_term, field)?) as Box<dyn Query>]),
                     Rule::regex => {
-                        if !field_type.is_indexed() {
-                            return Err(QueryParserError::FieldNotIndexed(field_entry.name().to_string()));
-                        }
                         let query = Box::new(
                             RegexQuery::from_pattern(pre_term.clone().into_inner().next().expect("grammar failure").as_str(), *field)
                                 .map_err(|_| QueryParserError::Syntax(pre_term.as_str().to_string()))?,
                         ) as Box<dyn Query>;
                         return Ok(vec![boost_query(query, boost)]);
                     }
                     _ => unreachable!(),
@@ -577,150 +590,114 @@
                 }
                 _ => return None,
             }
         }
         (!terms.is_empty()).then(|| terms.join(" "))
     }
 
-    fn parse_isbn(&self, isbn: &str) -> Result<Box<dyn Query>, QueryParserError> {
-        if let Ok(isbns_fields) = self.schema.get_field("isbns") {
-            Ok(Box::new(TermQuery::new(
-                Term::from_field_text(isbns_fields, &isbn.replace('-', "")),
-                IndexRecordOption::Basic,
-            )) as Box<dyn Query>)
-        } else {
-            Ok(Box::new(EmptyQuery) as Box<dyn Query>)
-        }
-    }
-
-    fn parse_doi(&self, doi: &str) -> Result<Box<dyn Query>, QueryParserError> {
-        if let Ok(doi_field) = self.schema.get_field("doi") {
-            // ToDo: use more general approach, i.e. use doi tokenizer
-            let mut term_queries = vec![];
-            let mut boost_original_match = None;
-            let lowercased_doi = doi.to_lowercase();
-            // ToDo: compile statically
-            let matcher: Matcher3<_> = regex!(br"(10.[0-9]+)/((?:cbo)?(?:(?:978[0-9]{10})|(?:978[0-9]{13})|(?:978[-0-9]+)))(.*)");
-            if let Some((prefix, isbn, tail)) = matcher.match_slices(lowercased_doi.as_ref()) {
-                let isbn = unsafe { std::str::from_utf8_unchecked(isbn) };
-                let corrected_isbn = isbn.replace('-', "").replace("cbo", "");
-                if (corrected_isbn.len() == 10 || corrected_isbn.len() == 13) && !prefix.is_empty() {
-                    if !tail.is_empty() {
-                        term_queries.push((
-                            Occur::Should,
-                            Box::new(TermQuery::new(
-                                Term::from_field_text(doi_field, &format!("{}/{}", unsafe { std::str::from_utf8_unchecked(prefix) }, isbn)),
-                                IndexRecordOption::Basic,
-                            )) as Box<dyn Query>,
-                        ));
-                    }
-                    if let Ok(isbns_field) = self.schema.get_field("isbns") {
-                        term_queries.push((
-                            Occur::Should,
-                            Box::new(TermQuery::new(Term::from_field_text(isbns_field, &corrected_isbn), IndexRecordOption::Basic)) as Box<dyn Query>,
-                        ));
-                        boost_original_match = Some(3.0);
-                    }
-                }
-            }
-            if let Some(boost) = boost_original_match {
-                term_queries.push((
-                    Occur::Should,
-                    Box::new(BoostQuery::new(
-                        Box::new(TermQuery::new(Term::from_field_text(doi_field, &lowercased_doi), IndexRecordOption::Basic)) as Box<dyn Query>,
-                        boost,
-                    )) as Box<dyn Query>,
-                ))
-            } else {
-                term_queries.push((
-                    Occur::Should,
-                    Box::new(TermQuery::new(Term::from_field_text(doi_field, &lowercased_doi), IndexRecordOption::Basic)) as Box<dyn Query>,
-                ));
-            }
-            Ok(Box::new(BooleanQuery::new(term_queries)) as Box<dyn Query>)
-        } else {
-            Ok(Box::new(EmptyQuery) as Box<dyn Query>)
-        }
-    }
-
     fn parse_statement(&self, pair: Pair<Rule>) -> Result<Box<dyn Query>, QueryParserError> {
         let mut statement_pairs = pair.into_inner();
         let isbn_doi_or_search_group_or_term = statement_pairs.next().expect("grammar failure");
         let statement_boost = statement_pairs.next().map(|boost| f32::from_str(boost.as_str()).expect("grammar failure"));
         let statement_result = match isbn_doi_or_search_group_or_term.as_rule() {
             Rule::search_group => {
                 let mut search_group = isbn_doi_or_search_group_or_term.into_inner();
                 let field_name = search_group.next().expect("grammar failure");
                 let grouping_or_term = search_group.next().expect("grammar failure");
                 match grouping_or_term.as_rule() {
                     Rule::grouping => {
                         let mut intermediate_results = vec![];
-                        match self.schema.get_field(self.resolve_field_name(field_name.as_str())) {
-                            Ok(field) => {
+                        match self.schema.find_field(self.resolve_field_name(field_name.as_str())) {
+                            Some((field, full_path)) => {
                                 for term in grouping_or_term.into_inner() {
-                                    intermediate_results.push(self.parse_term(term, &field, "", statement_boost)?);
+                                    intermediate_results.push(self.parse_term(term, &field, full_path, statement_boost)?);
                                 }
                             }
-                            Err(tantivy::TantivyError::FieldNotFound(_)) => match self.missing_field_policy {
-                                MissingFieldPolicy::AsUsualTerms => {
-                                    intermediate_results.push(self.default_fields_term(field_name, statement_boost)?);
+                            None => match proto::MissingFieldPolicy::from_i32(self.query_parser_config.0.missing_field_policy) {
+                                Some(proto::MissingFieldPolicy::AsUsualTerms) => {
+                                    intermediate_results.push(self.default_field_queries(field_name, statement_boost)?);
                                     for term in grouping_or_term.into_inner() {
-                                        intermediate_results.push(self.default_fields_term(term, statement_boost)?)
+                                        intermediate_results.push(self.default_field_queries(term, statement_boost)?)
                                     }
                                 }
-                                MissingFieldPolicy::Remove => return Ok(Box::new(EmptyQuery {})),
-                                MissingFieldPolicy::Fail => return Err(QueryParserError::FieldDoesNotExist(field_name.as_str().to_string())),
+                                Some(proto::MissingFieldPolicy::Remove) => return Ok(Box::new(EmptyQuery {})),
+                                Some(proto::MissingFieldPolicy::Fail) => return Err(QueryParserError::FieldDoesNotExist(field_name.as_str().to_string())),
+                                _ => unreachable!(),
                             },
-                            _ => unreachable!(),
                         }
                         Ok(Box::new(BooleanQuery::new(intermediate_results.into_iter().map(|q| (Occur::Should, q)).collect())) as Box<dyn Query>)
                     }
                     Rule::term => match self.schema.find_field(self.resolve_field_name(field_name.as_str())) {
                         Some((field, full_path)) => self.parse_term(grouping_or_term, &field, full_path, statement_boost),
-                        None => match self.missing_field_policy {
-                            MissingFieldPolicy::AsUsualTerms => Ok(Box::new(BooleanQuery::new(vec![
-                                (Occur::Should, self.default_fields_term(field_name, statement_boost)?),
-                                (Occur::Should, self.default_fields_term(grouping_or_term, statement_boost)?),
+                        None => match proto::MissingFieldPolicy::from_i32(self.query_parser_config.0.missing_field_policy) {
+                            Some(proto::MissingFieldPolicy::AsUsualTerms) => Ok(Box::new(BooleanQuery::new(vec![
+                                (Occur::Should, self.default_field_queries(field_name, statement_boost)?),
+                                (Occur::Should, self.default_field_queries(grouping_or_term, statement_boost)?),
                             ])) as Box<dyn Query>),
-                            MissingFieldPolicy::Remove => Ok(Box::new(EmptyQuery {}) as Box<dyn Query>),
-                            MissingFieldPolicy::Fail => Err(QueryParserError::FieldDoesNotExist(field_name.as_str().to_string())),
+                            Some(proto::MissingFieldPolicy::Remove) => Ok(Box::new(EmptyQuery {}) as Box<dyn Query>),
+                            Some(proto::MissingFieldPolicy::Fail) => Err(QueryParserError::FieldDoesNotExist(field_name.as_str().to_string())),
+                            _ => unreachable!(),
                         },
                     },
                     _ => unreachable!(),
                 }
             }
-            Rule::doi => self.parse_doi(isbn_doi_or_search_group_or_term.as_str()),
-            Rule::isbn => self.parse_isbn(isbn_doi_or_search_group_or_term.as_str()),
-            Rule::term => self.default_fields_term(isbn_doi_or_search_group_or_term, statement_boost),
+            Rule::doi => {
+                let mut queries = vec![];
+                let doi_mapper = Box::new(DoiMapper::new(self.schema.clone(), vec!["doi".to_string()])) as Box<dyn TermFieldMapper>;
+                let doi_isbn_mapper = Box::new(DoiIsbnMapper::new(self.schema.clone(), vec!["metadata.isbns".to_string()])) as Box<dyn TermFieldMapper>;
+
+                for mapper in &[doi_mapper, doi_isbn_mapper] {
+                    if let Some(query) = mapper.map(isbn_doi_or_search_group_or_term.as_str()) {
+                        queries.push((Occur::Should, query));
+                    }
+                }
+                Ok(Box::new(BooleanQuery::new(queries)) as Box<dyn Query>)
+            }
+            Rule::isbn => {
+                let mut queries = vec![];
+                let isbn_mapper = Box::new(IsbnMapper::new(self.schema.clone(), vec!["metadata.isbns".to_string()])) as Box<dyn TermFieldMapper>;
+
+                for mapper in &[isbn_mapper] {
+                    if let Some(query) = mapper.map(isbn_doi_or_search_group_or_term.as_str()) {
+                        queries.push((Occur::Should, query));
+                    }
+                }
+                Ok(Box::new(BooleanQuery::new(queries)) as Box<dyn Query>)
+            }
+            Rule::term => self.default_field_queries(isbn_doi_or_search_group_or_term, statement_boost),
             e => panic!("{e:?}"),
         }?;
         Ok(statement_result)
     }
 
     fn parse_statements(&self, pairs: Pairs<Rule>) -> Result<Box<dyn Query>, QueryParserError> {
         let mut subqueries = Subqueries::new();
 
         for pair in pairs.clone() {
             let parsed_queries = self.parse_statement(pair)?;
             subqueries.push((Occur::Should, parsed_queries));
         }
 
-        if let Some(exact_matches_promoter) = &self.exact_matches_promoter {
+        if let Some(exact_matches_promoter) = &self.query_parser_config.0.exact_matches_promoter {
             if let Some(top_level_phrase) = self.extract_top_level_phrase(pairs) {
                 subqueries.extend(
-                    self.default_fields
+                    self.query_parser_config
+                        .0
+                        .default_fields
                         .iter()
                         .filter_map(|field| {
-                            let field_entry = self.schema.get_field_entry(*field);
-                            let field_boost = self.field_boosts.as_ref().and_then(|boosts| boosts.get(field_entry.name()).cloned());
+                            let field = self.schema.get_field(field).expect("no field");
+                            let field_entry = self.schema.get_field_entry(field);
+                            let field_boost = self.query_parser_config.0.field_boosts.get(field_entry.name()).copied();
                             if let FieldType::Str(ref str_option) = field_entry.field_type() {
                                 let Some(option) = str_option.get_indexing_options() else {
                                     return None
                                 };
-                                let terms = match self.parse_words(*field, option, &top_level_phrase) {
+                                let terms = match self.parse_words(field, option, &top_level_phrase) {
                                     Ok(terms) => terms,
                                     Err(err) => return Some(Err(err)),
                                 };
                                 (terms.len() > 1 && option.index_option().has_positions()).then(|| {
                                     let query = Box::new(PhraseQuery::new_with_offset_and_slop(terms, exact_matches_promoter.slop)) as Box<dyn Query>;
                                     Ok(boost_query(query, multiply_boosts(exact_matches_promoter.boost, field_boost)))
                                 })
@@ -730,42 +707,48 @@
                         })
                         .collect::<Result<Vec<_>, _>>()?
                         .into_iter()
                         .map(|q| (Occur::Should, q)),
                 )
             }
         }
-        Ok(Box::new(BooleanQuery::new(subqueries.into_iter().take(self.limit).collect())) as Box<dyn Query>)
+        Ok(Box::new(BooleanQuery::new(subqueries.into_iter().take(self.query_parser_config.term_limit()).collect())) as Box<dyn Query>)
     }
 
     pub fn parse_query(&self, query: &str) -> Result<Box<dyn Query>, QueryParserError> {
         let pairs = SummaQlParser::parse(Rule::main, query).map_err(Box::new)?;
         Ok(reduce_empty_queries(reduce_should_clause(self.parse_statements(pairs)?)))
     }
 }
 
 #[cfg(test)]
 mod tests {
+    use std::collections::HashMap;
+
     use tantivy::schema::{TextOptions, INDEXED, STRING, TEXT};
     use tantivy::tokenizer::{LowerCaser, RemoveLongFilter};
 
     use super::*;
     use crate::components::SummaTokenizer;
 
     fn create_query_parser() -> QueryParser {
         let tokenizer_manager = TokenizerManager::default();
         let mut schema_builder = Schema::builder();
         schema_builder.add_text_field("title", TEXT);
         schema_builder.add_text_field("body", TEXT);
         schema_builder.add_i64_field("timestamp", INDEXED);
         schema_builder.add_text_field("doi", STRING);
         schema_builder.add_text_field("isbns", STRING);
+        schema_builder.add_json_field("metadata", TEXT);
         let schema = schema_builder.build();
-        let default_fields = vec!["title".to_string()];
-        QueryParser::new(schema, default_fields, &tokenizer_manager).expect("cannot create parser")
+        let query_parser_config = QueryParserConfig(proto::QueryParserConfig {
+            default_fields: vec!["title".to_string()],
+            ..Default::default()
+        });
+        QueryParser::new(schema, query_parser_config, &tokenizer_manager).expect("cannot create parser")
     }
 
     fn create_complex_query_parser() -> QueryParser {
         let tokenizer_manager = TokenizerManager::default();
         tokenizer_manager.register(
             "summa",
             TextAnalyzer::builder(SummaTokenizer)
@@ -782,17 +765,21 @@
         schema_builder.add_text_field("title", text_options);
         schema_builder.add_text_field("body", TEXT);
         schema_builder.add_text_field("authors", TEXT);
         schema_builder.add_text_field("language", TEXT);
         schema_builder.add_i64_field("timestamp", INDEXED);
         schema_builder.add_text_field("doi", STRING);
         schema_builder.add_text_field("isbns", STRING);
+        schema_builder.add_json_field("metadata", TEXT);
         let schema = schema_builder.build();
-        let default_fields = vec!["title".to_string(), "body".to_string()];
-        QueryParser::new(schema, default_fields, &tokenizer_manager).expect("cannot create parser")
+        let query_parser_config = QueryParserConfig(proto::QueryParserConfig {
+            default_fields: vec!["title".to_string(), "body".to_string()],
+            ..Default::default()
+        });
+        QueryParser::new(schema, query_parser_config, &tokenizer_manager).expect("cannot create parser")
     }
 
     #[test]
     pub fn test_parser_base() {
         let query_parser = create_query_parser();
         let query = query_parser.parse_query("search engine");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, TermQuery(Term(field=0, type=Str, \"engine\")))] })");
@@ -826,15 +813,15 @@
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("title:search engine")),
             "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, TermQuery(Term(field=0, type=Str, \"engine\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("not_field:search engine")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"engine\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"not\"))), (Should, TermQuery(Term(field=0, type=Str, \"field\"))), (Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, TermQuery(Term(field=0, type=Str, \"engine\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("doi:10.0000/abcd.0123 ")),
             "Ok(TermQuery(Term(field=3, type=Str, \"10.0000/abcd.0123\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("doi:https://doi.org/10.0000/abcd.0123")),
@@ -844,30 +831,30 @@
             format!("{:?}", query_parser.parse_query("doi:doi.org/10.0000/abcd.0123")),
             "Ok(TermQuery(Term(field=3, type=Str, \"doi.org/10.0000/abcd.0123\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("10.0000/978123")),
             "Ok(TermQuery(Term(field=3, type=Str, \"10.0000/978123\")))"
         );
-        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/9781234567890")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=4, type=Str, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(field=3, type=Str, \"10.0000/9781234567890\")), boost=3))] })");
-        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/978-12345-6789-0")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=4, type=Str, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(field=3, type=Str, \"10.0000/978-12345-6789-0\")), boost=3))] })");
-        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/978-12345-6789-0.ch11")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=3, type=Str, \"10.0000/978-12345-6789-0\"))), (Should, TermQuery(Term(field=4, type=Str, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(field=3, type=Str, \"10.0000/978-12345-6789-0.ch11\")), boost=3))] })");
-        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/cbo978-12345-6789-0.ch11")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=3, type=Str, \"10.0000/cbo978-12345-6789-0\"))), (Should, TermQuery(Term(field=4, type=Str, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(field=3, type=Str, \"10.0000/cbo978-12345-6789-0.ch11\")), boost=3))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/9781234567890")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=3, type=Str, \"10.0000/9781234567890\"))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=Str, \"9781234567890\")))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/978-12345-6789-0")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=3, type=Str, \"10.0000/978-12345-6789-0\"))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=Str, \"9781234567890\")))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/978-12345-6789-0.ch11")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=3, type=Str, \"10.0000/978-12345-6789-0.ch11\"))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=Str, \"9781234567890\")))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/cbo978-12345-6789-0.ch11")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=3, type=Str, \"10.0000/cbo978-12345-6789-0.ch11\"))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=Str, \"9781234567890\")))] })");
         assert_eq!(
             format!("{:?}", query_parser.parse_query("978-12345-6789-0")),
-            "Ok(TermQuery(Term(field=4, type=Str, \"9781234567890\")))"
+            "Ok(TermQuery(Term(field=5, type=Json, path=isbns, type=Str, \"9781234567890\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("9781234567890")),
-            "Ok(TermQuery(Term(field=4, type=Str, \"9781234567890\")))"
+            "Ok(TermQuery(Term(field=5, type=Json, path=isbns, type=Str, \"9781234567890\")))"
         );
         assert_eq!(format!("{:?}", query_parser.parse_query("97812-34-5678-909")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"97812\"))), (Should, TermQuery(Term(field=0, type=Str, \"34\"))), (Should, TermQuery(Term(field=0, type=Str, \"5678\"))), (Should, TermQuery(Term(field=0, type=Str, \"909\")))] })");
         assert_eq!(
-            format!("{:?}", query_parser.parse_query("isbns:97812-34-5678-90")),
-            "Ok(TermQuery(Term(field=4, type=Str, \"97812-34-5678-90\")))"
+            format!("{:?}", query_parser.parse_query("metadata.isbns:97812-34-5678-90")),
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=5, type=Json, path=isbns, type=U64, 97812))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=U64, 34))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=U64, 5678))), (Should, TermQuery(Term(field=5, type=Json, path=isbns, type=U64, 90)))] })"
         );
         assert_eq!(format!("{:?}", query_parser.parse_query("123 97812-34-5678-909")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"123\"))), (Should, TermQuery(Term(field=0, type=Str, \"97812\"))), (Should, TermQuery(Term(field=0, type=Str, \"34\"))), (Should, TermQuery(Term(field=0, type=Str, \"5678\"))), (Should, TermQuery(Term(field=0, type=Str, \"909\")))] })");
         assert_eq!(
             format!("{:?}", query_parser.parse_query("10.0000/cbo123")),
             "Ok(TermQuery(Term(field=3, type=Str, \"10.0000/cbo123\")))"
         );
         assert_eq!(
@@ -977,14 +964,27 @@
         assert_eq!(
             format!("{:?}", query_parser.parse_query("body:/поисковые.*/")),
             "Ok(RegexQuery { regex: Regex(\"поисковые.*\")\n, field: Field(1) })"
         );
     }
 
     #[test]
+    pub fn test_json() {
+        let query_parser = create_query_parser();
+        assert_eq!(
+            format!("{:?}", query_parser.parse_query("metadata.a:1")),
+            "Ok(TermQuery(Term(field=5, type=Json, path=a, type=U64, 1)))"
+        );
+        assert_eq!(
+            format!("{:?}", query_parser.parse_query("metadata.a:\"1\"")),
+            "Ok(TermQuery(Term(field=5, type=Json, path=a, type=Str, \"1\")))"
+        );
+    }
+
+    #[test]
     pub fn test_plus_minus() {
         let query_parser = create_query_parser();
         assert_eq!(
             format!("{:?}", query_parser.parse_query("body:+search -engine")),
             "Ok(BooleanQuery { subqueries: [(Must, TermQuery(Term(field=1, type=Str, \"search\"))), (MustNot, TermQuery(Term(field=0, type=Str, \"engine\")))] })"
         );
         assert_eq!(
@@ -1049,17 +1049,27 @@
         let query = query_parser.parse_query("timestamp:(-[1100 to 1200] [ 1000 to 2000 ] -1500 +3000)");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(MustNot, RangeQuery { field: \"timestamp\", value_type: I64, lower_bound: Included([128, 0, 0, 0, 0, 0, 4, 76]), upper_bound: Included([128, 0, 0, 0, 0, 0, 4, 176]), limit: None }), (Should, RangeQuery { field: \"timestamp\", value_type: I64, lower_bound: Included([128, 0, 0, 0, 0, 0, 3, 232]), upper_bound: Included([128, 0, 0, 0, 0, 0, 7, 208]), limit: None }), (MustNot, TermQuery(Term(field=2, type=I64, 1500))), (Must, TermQuery(Term(field=2, type=I64, 3000)))] })");
     }
 
     #[test]
     pub fn test_exact_phrase_promoter() {
         let mut query_parser = create_query_parser();
-        query_parser.set_exact_match_promoter(proto::ExactMatchesPromoter { slop: 3, boost: Some(2.0) });
+        query_parser.query_parser_config.0.exact_matches_promoter = Some(proto::ExactMatchesPromoter { slop: 3, boost: Some(2.0) });
         let query = query_parser.parse_query("old school holy-wood");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"old\"))), (Should, TermQuery(Term(field=0, type=Str, \"school\"))), (Should, TermQuery(Term(field=0, type=Str, \"holy\"))), (Should, TermQuery(Term(field=0, type=Str, \"wood\"))), (Should, Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"old\")), (1, Term(field=0, type=Str, \"school\")), (2, Term(field=0, type=Str, \"holy\")), (3, Term(field=0, type=Str, \"wood\"))], slop: 3 }, boost=2))] })");
         let query = query_parser.parse_query("old^2.0 school");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, Boost(query=TermQuery(Term(field=0, type=Str, \"old\")), boost=2)), (Should, TermQuery(Term(field=0, type=Str, \"school\")))] })");
-        query_parser.set_field_boosts(HashMap::from_iter(vec![("title".to_string(), 3.0)].into_iter()));
+        query_parser.query_parser_config.0.field_boosts = HashMap::from_iter(vec![("title".to_string(), 3.0)]);
         let query = query_parser.parse_query("old school");
         assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, Boost(query=TermQuery(Term(field=0, type=Str, \"old\")), boost=3)), (Should, Boost(query=TermQuery(Term(field=0, type=Str, \"school\")), boost=3)), (Should, Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"old\")), (1, Term(field=0, type=Str, \"school\"))], slop: 3 }, boost=6))] })");
     }
+
+    #[test]
+    pub fn test_inflection() {
+        let mut query_parser = create_query_parser();
+        let mut inflection_configs = HashMap::new();
+        inflection_configs.insert("title".to_string(), proto::InflectionConfig { derive_plural: true });
+        query_parser.query_parser_config.0.inflection_configs = inflection_configs;
+        let query = query_parser.parse_query("search engine");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"search\")), TermQuery(Term(field=0, type=Str, \"searches\"))], tie_breaker: 0.0 }), (Should, DisjunctionMaxQuery { disjuncts: [TermQuery(Term(field=0, type=Str, \"engine\")), TermQuery(Term(field=0, type=Str, \"engines\"))], tie_breaker: 0.0 })] })");
+    }
 }
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/configs/core.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 use std::collections::HashMap;
 use std::default::Default;
 
 use serde::{Deserialize, Serialize};
+use summa_proto::proto;
 use summa_proto::proto::IndexEngineConfig;
 
 use crate::errors::{BuilderError, SummaResult, ValidationError};
 
-fn return_true() -> bool {
-    true
+fn return_1() -> usize {
+    1
 }
 fn return_100() -> usize {
     100
 }
 
 #[derive(Clone, Debug, Serialize, Deserialize)]
 #[serde(rename_all = "snake_case")]
@@ -32,17 +33,17 @@
 #[derive(Builder, Clone, Debug, Serialize, Deserialize)]
 #[builder(default, build_fn(error = "BuilderError"))]
 pub struct Config {
     #[serde(default = "HashMap::new")]
     pub aliases: HashMap<String, String>,
     #[builder(default = "None")]
     pub autocommit_interval_ms: Option<u64>,
-    #[builder(default = "true")]
-    #[serde(default = "return_true")]
-    pub dedicated_compression_thread: bool,
+    #[builder(default = "1")]
+    #[serde(default = "return_1")]
+    pub doc_store_compress_threads: usize,
     #[builder(default = "100")]
     #[serde(default = "return_100")]
     pub doc_store_cache_num_blocks: usize,
     #[serde(default = "HashMap::new")]
     pub indices: HashMap<String, IndexEngineConfig>,
     #[builder(default = "1024 * 1024 * 1024")]
     pub writer_heap_size_bytes: u64,
@@ -51,15 +52,15 @@
 }
 
 impl Default for Config {
     fn default() -> Self {
         Config {
             aliases: HashMap::new(),
             autocommit_interval_ms: None,
-            dedicated_compression_thread: true,
+            doc_store_compress_threads: 1,
             indices: HashMap::new(),
             writer_heap_size_bytes: 1024 * 1024 * 1024,
             writer_threads: Some(WriterThreads::N(1)),
             doc_store_cache_num_blocks: 100,
         }
     }
 }
@@ -96,7 +97,25 @@
     /// Delete all aliases listed in `index_aliases`
     pub fn delete_index_aliases(&mut self, index_aliases: &Vec<String>) {
         for alias in index_aliases {
             self.aliases.remove(alias);
         }
     }
 }
+
+#[derive(Clone)]
+pub struct QueryParserConfig(pub proto::QueryParserConfig);
+impl QueryParserConfig {
+    pub fn from_default_fields(default_fields: Vec<String>) -> Self {
+        QueryParserConfig(proto::QueryParserConfig {
+            default_fields,
+            ..Default::default()
+        })
+    }
+    pub fn term_limit(&self) -> usize {
+        if self.0.term_limit > 0 {
+            self.0.term_limit as usize
+        } else {
+            16
+        }
+    }
+}
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/aggregation.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/aggregation.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     }
 }
 
 impl TryFrom<Wrapper<proto::aggregation::Aggregation>> for Aggregation {
     type Error = Error;
 
     fn try_from(aggregation: Wrapper<proto::aggregation::Aggregation>) -> Result<Self, Error> {
-        Ok(serde_json::from_str(&serde_json::to_string(&aggregation.into_inner()).unwrap()).unwrap())
+        Ok(serde_json::from_str(&serde_json::to_string(&aggregation.into_inner())?)?)
     }
 }
 
 impl From<AggregationResult> for Wrapper<proto::AggregationResult> {
     fn from(aggregation_result: AggregationResult) -> Self {
         Wrapper::from(proto::AggregationResult {
             aggregation_result: Some(match aggregation_result {
```

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.16.0/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/Cargo.toml` & `summa_embed-0.16.0/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "summa-embed-py"
-version = "0.15.9"
+version = "0.16.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
 [dependencies]
 futures = "0.3"
 prost = "0.11"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
-pythonize = "0.18"
+pyo3-log = "0.8"
 serde_json = "1.0"
-summa-core = { version = "0.15.9", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.16.0", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.15.9/.gitignore` & `summa_embed-0.16.0/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/pyproject.toml` & `summa_embed-0.16.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/src/lib.rs` & `summa_embed-0.16.0/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-use std::collections::HashMap;
+extern crate core;
+
 use std::sync::Arc;
 
 use futures::future::join_all;
 use prost::Message;
 use pyo3::exceptions::PyOSError;
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
-use pythonize::pythonize;
 use summa_core::components::{Driver, IndexHolder};
 use summa_core::configs::{ConfigProxy, DirectProxy};
 use summa_core::directories::DefaultExternalRequestGenerator;
 use summa_core::hyper_external_request::HyperExternalRequest;
 use summa_proto::proto;
 use tantivy::IndexBuilder;
 
@@ -31,20 +31,26 @@
 #[pyclass]
 #[derive(Clone)]
 struct IndexRegistry {
     index_registry: summa_core::components::IndexRegistry,
     core_config: Arc<dyn ConfigProxy<summa_core::configs::core::Config>>,
 }
 
+impl Default for IndexRegistry {
+    fn default() -> Self {
+        Self::new()
+    }
+}
+
 #[pymethods]
 impl IndexRegistry {
     #[new]
     pub fn new() -> Self {
         let core_config = summa_core::configs::core::ConfigBuilder::default()
-            .dedicated_compression_thread(false)
+            .doc_store_compress_threads(1)
             .writer_threads(None)
             .build()
             .expect("cannot build");
         let core_config = Arc::new(DirectProxy::new(core_config)) as Arc<dyn ConfigProxy<_>>;
         IndexRegistry {
             index_registry: summa_core::components::IndexRegistry::new(&core_config),
             core_config,
@@ -66,47 +72,48 @@
                     DefaultExternalRequestGenerator<HyperExternalRequest>,
                 >(remote_engine_config.clone(), true)
                 .await
                 .unwrap(),
                 _ => unimplemented!(),
             };
             let core_config = this.core_config.read().await.get().clone();
-            let index_holder = tokio::task::spawn_blocking(move || {
-                IndexHolder::create_holder(
-                    &core_config,
-                    index,
-                    index_name.as_deref(),
-                    Arc::new(DirectProxy::new(index_engine_config)),
-                    None,
-                    HashMap::new(),
-                    true,
-                    Driver::current_tokio(),
-                )
-            })
-            .await
-            .unwrap()
+            let query_parser_config = index_engine_config.query_parser_config.as_ref().cloned().unwrap_or_default();
+            let index_holder = IndexHolder::create_holder(
+                &core_config,
+                index,
+                index_name.as_deref(),
+                Arc::new(DirectProxy::new(index_engine_config)),
+                None,
+                query_parser_config,
+                Driver::current_tokio(),
+            )
             .unwrap();
-            let index_attributes = index_holder.index_attributes().cloned();
+            let index_attributes = index_holder.index_attributes().cloned().unwrap();
             this.index_registry.add(index_holder).await.unwrap();
-            Ok(Python::with_gil(|py| pythonize(py, &index_attributes).unwrap()))
+            Ok(Python::with_gil(|py| index_attributes.encode_to_vec().as_slice().into_py(py)))
         })
     }
 
     fn search<'a>(&'a self, py: Python<'a>, index_queries: &PyBytes) -> PyResult<&'a PyAny> {
         let search_request = proto::SearchRequest::decode(index_queries.as_bytes()).unwrap();
         let this = self.clone();
         pyo3_asyncio::tokio::future_into_py(py, async move {
             let futures = this.index_registry.search_futures(search_request.index_queries).unwrap();
             let extraction_results = join_all(futures).await.into_iter().map(|r| r.expect("cannot receive")).collect::<Vec<_>>();
             let result = this.index_registry.finalize_extraction(extraction_results).await.unwrap();
-            Ok(Python::with_gil(|py| pythonize(py, &result).unwrap()))
+            let search_response = proto::SearchResponse {
+                elapsed_secs: 0.0,
+                collector_outputs: result,
+            };
+            Ok(Python::with_gil(|py| search_response.encode_to_vec().as_slice().into_py(py)))
         })
     }
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
 #[pyo3(name = "summa_embed_bin")]
 fn summa_embed_bin(_py: Python, m: &PyModule) -> PyResult<()> {
+    pyo3_log::init();
     m.add_class::<IndexRegistry>()?;
     Ok(())
 }
```

### Comparing `summa_embed-0.15.9/summa_embed/__init__.py` & `summa_embed-0.16.0/summa_embed/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 from typing import Dict, Optional
 
 from izihawa_utils.pb_to_json import ParseDict
 
-from .proto import index_service_pb2, search_service_pb2
+from .proto import index_service_pb2, query_pb2, search_service_pb2
 from .summa_embed_bin import IndexRegistry as IndexRegistryBin
 
 
 class IndexRegistry:
     def __init__(self):
         self.index_registry = IndexRegistryBin()
 
-    def add(self, index_config, index_name: Optional[str] = None):
+    async def add(self, index_config, index_name: Optional[str] = None) -> index_service_pb2.IndexAttributes:
         parsed_index_config = index_service_pb2.IndexEngineConfig()
         ParseDict(index_config, parsed_index_config)
-        return self.index_registry.add(parsed_index_config.SerializeToString(), index_name=index_name)
+        index_attributes_bytes = await self.index_registry.add(
+            parsed_index_config.SerializeToString(),
+            index_name=index_name,
+        )
+        index_attributes = index_service_pb2.IndexAttributes()
+        index_attributes.ParseFromString(index_attributes_bytes)
+        return index_attributes
 
-    def search(self, index_queries):
+    async def search(self, index_queries) -> query_pb2.SearchResponse:
         search_request = search_service_pb2.SearchRequest()
         for index_query in index_queries:
             if isinstance(index_query, Dict):
                 dict_index_query = index_query
                 index_query = search_service_pb2.IndexQuery()
                 ParseDict(dict_index_query, index_query)
             search_request.index_queries.append(index_query)
-        return self.index_registry.search(search_request.SerializeToString())
+        search_response_bytes = await self.index_registry.search(search_request.SerializeToString())
+        search_response = query_pb2.SearchResponse()
+        search_response.ParseFromString(search_response_bytes)
+        return search_response
```

### Comparing `summa_embed-0.15.9/summa_embed/proto/consumer_service_pb2.py` & `summa_embed-0.16.0/summa_embed/proto/consumer_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/summa_embed/proto/consumer_service_pb2.pyi` & `summa_embed-0.16.0/summa_embed/proto/consumer_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/summa_embed/proto/dag_pb_pb2.py` & `summa_embed-0.16.0/summa_embed/proto/dag_pb_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/summa_embed/proto/dag_pb_pb2.pyi` & `summa_embed-0.16.0/summa_embed/proto/dag_pb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/summa_embed/proto/index_service_pb2.py` & `summa_embed-0.16.0/summa_embed/proto/index_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,137 +11,137 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from . import query_pb2 as query__pb2
 from . import utils_pb2 as utils__pb2
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13index_service.proto\x12\x0bsumma.proto\x1a\x0bquery.proto\x1a\x0butils.proto\"3\n\nPrimaryKey\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03i64\x18\x02 \x01(\x03H\x00\x42\x07\n\x05value\"\x7f\n\x0bMergePolicy\x12*\n\x03log\x18\x0b \x01(\x0b\x32\x1b.summa.proto.LogMergePolicyH\x00\x12\x34\n\x08temporal\x18\x0c \x01(\x0b\x32 .summa.proto.TemporalMergePolicyH\x00\x42\x0e\n\x0cmerge_policy\"\x19\n\x17\x41ttachFileEngineRequest\"L\n\x19\x41ttachRemoteEngineRequest\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfig\"\xd8\x01\n\x12\x41ttachIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x02 \x01(\x0b\x32$.summa.proto.AttachFileEngineRequestH\x00\x12\x38\n\x06remote\x18\x03 \x01(\x0b\x32&.summa.proto.AttachRemoteEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x0e\n\x0cindex_engine\"C\n\x13\x41ttachIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"(\n\x12\x43ommitIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"+\n\x13\x43ommitIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\"L\n\x14\x43opyDocumentsRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\"G\n\x15\x43opyDocumentsResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x18\n\x10\x63opied_documents\x18\x02 \x01(\r\"\xff\x01\n\x10\x43opyIndexRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\x12\x34\n\x04\x66ile\x18\x03 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x04 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\x06 \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x15\n\x13target_index_engine\"A\n\x11\x43opyIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"?\n\x0bSortByField\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05order\x18\x02 \x01(\x0e\x32\x12.summa.proto.Order\"\x19\n\x17\x43reateFileEngineRequest\"\x1b\n\x19\x43reateMemoryEngineRequest\"\xa0\x02\n\x0fIndexAttributes\x12\x12\n\ncreated_at\x18\x01 \x01(\x04\x12\x15\n\runique_fields\x18\x02 \x03(\t\x12\x16\n\x0e\x64\x65\x66\x61ult_fields\x18\x03 \x03(\t\x12\x14\n\x0cmulti_fields\x18\x04 \x03(\t\x12\x1f\n\x12\x64\x65\x66\x61ult_index_name\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x10\x64\x65\x66\x61ult_snippets\x18\x07 \x03(\t\x12\x38\n\x11\x63onflict_strategy\x18\x08 \x01(\x0e\x32\x1d.summa.proto.ConflictStrategyB\x15\n\x13_default_index_nameB\x0e\n\x0c_description\"\xbd\x03\n\x12\x43reateIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x07 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x08 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12-\n\x0b\x63ompression\x18\x03 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x16\n\tblocksize\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x34\n\rsort_by_field\x18\x05 \x01(\x0b\x32\x18.summa.proto.SortByFieldH\x02\x88\x01\x01\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\x12.\n\x0cmerge_policy\x18\x14 \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x0e\n\x0cindex_engineB\x0c\n\n_blocksizeB\x10\n\x0e_sort_by_field\"C\n\x13\x43reateIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"O\n\x16\x44\x65leteDocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"4\n\x17\x44\x65leteDocumentsResponse\x12\x19\n\x11\x64\x65leted_documents\x18\x01 \x01(\x04\"(\n\x12\x44\x65leteIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"1\n\x13\x44\x65leteIndexResponse\x12\x1a\n\x12\x64\x65leted_index_name\x18\x01 \x01(\t\"\x1a\n\x18GetIndicesAliasesRequest\"\xa7\x01\n\x19GetIndicesAliasesResponse\x12S\n\x0findices_aliases\x18\x01 \x03(\x0b\x32:.summa.proto.GetIndicesAliasesResponse.IndicesAliasesEntry\x1a\x35\n\x13IndicesAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"%\n\x0fGetIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"@\n\x10GetIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"\x13\n\x11GetIndicesRequest\")\n\x12GetIndicesResponse\x12\x13\n\x0bindex_names\x18\x01 \x03(\t\"C\n\x1aIndexDocumentStreamRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x11\n\tdocuments\x18\x02 \x03(\x0c\"^\n\x1bIndexDocumentStreamResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x14\n\x0csuccess_docs\x18\x02 \x01(\x04\x12\x13\n\x0b\x66\x61iled_docs\x18\x03 \x01(\x04\"<\n\x14IndexDocumentRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocument\x18\x02 \x01(\x0c\"\x17\n\x15IndexDocumentResponse\"?\n\x14MergeSegmentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x13\n\x0bsegment_ids\x18\x02 \x03(\t\"?\n\x15MergeSegmentsResponse\x12\x17\n\nsegment_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_segment_id\"?\n\x14SetIndexAliasRequest\x12\x13\n\x0bindex_alias\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"G\n\x15SetIndexAliasResponse\x12\x1b\n\x0eold_index_name\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x11\n\x0f_old_index_name\"6\n\x10\x44ocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"%\n\x11\x44ocumentsResponse\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\"C\n\x12VacuumIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x19\n\x11\x65xcluded_segments\x18\x02 \x03(\t\"0\n\x13VacuumIndexResponse\x12\x19\n\x11\x66reed_space_bytes\x18\x01 \x01(\x04\"9\n\x12WarmupIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0f\n\x07is_full\x18\x02 \x01(\x08\"+\n\x13WarmupIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\" \n\x10\x46ileEngineConfig\x12\x0c\n\x04path\x18\x01 \x01(\t\"$\n\x12MemoryEngineConfig\x12\x0e\n\x06schema\x18\x01 \x01(\t\"!\n\x0b\x43\x61\x63heConfig\x12\x12\n\ncache_size\x18\x01 \x01(\x04\"\x9a\x02\n\x12RemoteEngineConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x14\n\x0curl_template\x18\x02 \x01(\t\x12N\n\x10headers_template\x18\x03 \x03(\x0b\x32\x34.summa.proto.RemoteEngineConfig.HeadersTemplateEntry\x12.\n\x0c\x63\x61\x63he_config\x18\x04 \x01(\x0b\x32\x18.summa.proto.CacheConfig\x12\x17\n\ntimeout_ms\x18\x05 \x01(\rH\x00\x88\x01\x01\x1a\x36\n\x14HeadersTemplateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\r\n\x0b_timeout_ms\"#\n\x0eLogMergePolicy\x12\x11\n\tis_frozen\x18\x01 \x01(\x08\"4\n\x13TemporalMergePolicy\x12\x1d\n\x15merge_older_then_secs\x18\x01 \x01(\x04\"\xe0\x02\n\x11IndexEngineConfig\x12-\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x1d.summa.proto.FileEngineConfigH\x00\x12\x31\n\x06memory\x18\x02 \x01(\x0b\x32\x1f.summa.proto.MemoryEngineConfigH\x00\x12\x31\n\x06remote\x18\x03 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfigH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12G\n\rfield_aliases\x18\x0b \x03(\x0b\x32\x30.summa.proto.IndexEngineConfig.FieldAliasesEntry\x1a\x33\n\x11\x46ieldAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x08\n\x06\x63onfig\"\xec\x01\n\x10IndexDescription\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x15\n\rindex_aliases\x18\x02 \x03(\t\x12\x34\n\x0cindex_engine\x18\x03 \x01(\x0b\x32\x1e.summa.proto.IndexEngineConfig\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12-\n\x0b\x63ompression\x18\x05 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\"*\n\x16IndexDocumentOperation\x12\x10\n\x08\x64ocument\x18\x01 \x01(\x0c\"\\\n\x0eIndexOperation\x12=\n\x0eindex_document\x18\x02 \x01(\x0b\x32#.summa.proto.IndexDocumentOperationH\x00\x42\x0b\n\toperation*R\n\x10\x43onflictStrategy\x12\x0e\n\nDO_NOTHING\x10\x00\x12\x14\n\x10OVERWRITE_ALWAYS\x10\x01\x12\r\n\tOVERWRITE\x10\x02\x12\t\n\x05MERGE\x10\x03*|\n\x0b\x43ompression\x12\x08\n\x04None\x10\x00\x12\n\n\x06\x42rotli\x10\x01\x12\x07\n\x03Lz4\x10\x02\x12\n\n\x06Snappy\x10\x03\x12\x08\n\x04Zstd\x10\x04\x12\t\n\x05Zstd7\x10\x05\x12\t\n\x05Zstd9\x10\x06\x12\n\n\x06Zstd14\x10\x07\x12\n\n\x06Zstd19\x10\x08\x12\n\n\x06Zstd22\x10\t2\xeb\x0b\n\x08IndexApi\x12S\n\x0c\x61ttach_index\x12\x1f.summa.proto.AttachIndexRequest\x1a .summa.proto.AttachIndexResponse\"\x00\x12S\n\x0c\x63ommit_index\x12\x1f.summa.proto.CommitIndexRequest\x1a .summa.proto.CommitIndexResponse\"\x00\x12Y\n\x0e\x63opy_documents\x12!.summa.proto.CopyDocumentsRequest\x1a\".summa.proto.CopyDocumentsResponse\"\x00\x12S\n\x0c\x63reate_index\x12\x1f.summa.proto.CreateIndexRequest\x1a .summa.proto.CreateIndexResponse\"\x00\x12M\n\ncopy_index\x12\x1d.summa.proto.CopyIndexRequest\x1a\x1e.summa.proto.CopyIndexResponse\"\x00\x12_\n\x10\x64\x65lete_documents\x12#.summa.proto.DeleteDocumentsRequest\x1a$.summa.proto.DeleteDocumentsResponse\"\x00\x12S\n\x0c\x64\x65lete_index\x12\x1f.summa.proto.DeleteIndexRequest\x1a .summa.proto.DeleteIndexResponse\"\x00\x12N\n\tdocuments\x12\x1d.summa.proto.DocumentsRequest\x1a\x1e.summa.proto.DocumentsResponse\"\x00\x30\x01\x12\x66\n\x13get_indices_aliases\x12%.summa.proto.GetIndicesAliasesRequest\x1a&.summa.proto.GetIndicesAliasesResponse\"\x00\x12J\n\tget_index\x12\x1c.summa.proto.GetIndexRequest\x1a\x1d.summa.proto.GetIndexResponse\"\x00\x12P\n\x0bget_indices\x12\x1e.summa.proto.GetIndicesRequest\x1a\x1f.summa.proto.GetIndicesResponse\"\x00\x12n\n\x15index_document_stream\x12\'.summa.proto.IndexDocumentStreamRequest\x1a(.summa.proto.IndexDocumentStreamResponse\"\x00(\x01\x12Y\n\x0eindex_document\x12!.summa.proto.IndexDocumentRequest\x1a\".summa.proto.IndexDocumentResponse\"\x00\x12Y\n\x0emerge_segments\x12!.summa.proto.MergeSegmentsRequest\x1a\".summa.proto.MergeSegmentsResponse\"\x00\x12Z\n\x0fset_index_alias\x12!.summa.proto.SetIndexAliasRequest\x1a\".summa.proto.SetIndexAliasResponse\"\x00\x12S\n\x0cvacuum_index\x12\x1f.summa.proto.VacuumIndexRequest\x1a .summa.proto.VacuumIndexResponse\"\x00\x12S\n\x0cwarmup_index\x12\x1f.summa.proto.WarmupIndexRequest\x1a .summa.proto.WarmupIndexResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13index_service.proto\x12\x0bsumma.proto\x1a\x0bquery.proto\x1a\x0butils.proto\"3\n\nPrimaryKey\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03i64\x18\x02 \x01(\x03H\x00\x42\x07\n\x05value\"\x7f\n\x0bMergePolicy\x12*\n\x03log\x18\x0b \x01(\x0b\x32\x1b.summa.proto.LogMergePolicyH\x00\x12\x34\n\x08temporal\x18\x0c \x01(\x0b\x32 .summa.proto.TemporalMergePolicyH\x00\x42\x0e\n\x0cmerge_policy\"\x19\n\x17\x41ttachFileEngineRequest\"L\n\x19\x41ttachRemoteEngineRequest\x12/\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfig\"\x95\x02\n\x12\x41ttachIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x02 \x01(\x0b\x32$.summa.proto.AttachFileEngineRequestH\x00\x12\x38\n\x06remote\x18\x03 \x01(\x0b\x32&.summa.proto.AttachRemoteEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12;\n\x13query_parser_config\x18\x0b \x01(\x0b\x32\x1e.summa.proto.QueryParserConfigB\x0e\n\x0cindex_engine\"C\n\x13\x41ttachIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"(\n\x12\x43ommitIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"+\n\x13\x43ommitIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\"L\n\x14\x43opyDocumentsRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\"G\n\x15\x43opyDocumentsResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x18\n\x10\x63opied_documents\x18\x02 \x01(\r\"\xff\x01\n\x10\x43opyIndexRequest\x12\x19\n\x11source_index_name\x18\x01 \x01(\t\x12\x19\n\x11target_index_name\x18\x02 \x01(\t\x12\x34\n\x04\x66ile\x18\x03 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x04 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12.\n\x0cmerge_policy\x18\x06 \x01(\x0b\x32\x18.summa.proto.MergePolicyB\x15\n\x13target_index_engine\"A\n\x11\x43opyIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"?\n\x0bSortByField\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05order\x18\x02 \x01(\x0e\x32\x12.summa.proto.Order\"\x19\n\x17\x43reateFileEngineRequest\"\x1b\n\x19\x43reateMemoryEngineRequest\"\x88\x02\n\x0fIndexAttributes\x12\x12\n\ncreated_at\x18\x01 \x01(\x04\x12\x15\n\runique_fields\x18\x02 \x03(\t\x12\x14\n\x0cmulti_fields\x18\x04 \x03(\t\x12\x1f\n\x12\x64\x65\x66\x61ult_index_name\x18\x05 \x01(\tH\x00\x88\x01\x01\x12\x18\n\x0b\x64\x65scription\x18\x06 \x01(\tH\x01\x88\x01\x01\x12\x18\n\x10\x64\x65\x66\x61ult_snippets\x18\x07 \x03(\t\x12\x38\n\x11\x63onflict_strategy\x18\x08 \x01(\x0e\x32\x1d.summa.proto.ConflictStrategyB\x15\n\x13_default_index_nameB\x0e\n\x0c_description\"\xfa\x03\n\x12\x43reateIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x34\n\x04\x66ile\x18\x07 \x01(\x0b\x32$.summa.proto.CreateFileEngineRequestH\x00\x12\x38\n\x06memory\x18\x08 \x01(\x0b\x32&.summa.proto.CreateMemoryEngineRequestH\x00\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12-\n\x0b\x63ompression\x18\x03 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x16\n\tblocksize\x18\x04 \x01(\rH\x01\x88\x01\x01\x12\x34\n\rsort_by_field\x18\x05 \x01(\x0b\x32\x18.summa.proto.SortByFieldH\x02\x88\x01\x01\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\x12.\n\x0cmerge_policy\x18\x14 \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12;\n\x13query_parser_config\x18\x15 \x01(\x0b\x32\x1e.summa.proto.QueryParserConfigB\x0e\n\x0cindex_engineB\x0c\n\n_blocksizeB\x10\n\x0e_sort_by_field\"C\n\x13\x43reateIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"O\n\x16\x44\x65leteDocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"4\n\x17\x44\x65leteDocumentsResponse\x12\x19\n\x11\x64\x65leted_documents\x18\x01 \x01(\x04\"(\n\x12\x44\x65leteIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"1\n\x13\x44\x65leteIndexResponse\x12\x1a\n\x12\x64\x65leted_index_name\x18\x01 \x01(\t\"\x1a\n\x18GetIndicesAliasesRequest\"\xa7\x01\n\x19GetIndicesAliasesResponse\x12S\n\x0findices_aliases\x18\x01 \x03(\x0b\x32:.summa.proto.GetIndicesAliasesResponse.IndicesAliasesEntry\x1a\x35\n\x13IndicesAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"%\n\x0fGetIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\"@\n\x10GetIndexResponse\x12,\n\x05index\x18\x01 \x01(\x0b\x32\x1d.summa.proto.IndexDescription\"\x13\n\x11GetIndicesRequest\")\n\x12GetIndicesResponse\x12\x13\n\x0bindex_names\x18\x01 \x03(\t\"C\n\x1aIndexDocumentStreamRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x11\n\tdocuments\x18\x02 \x03(\x0c\"^\n\x1bIndexDocumentStreamResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x14\n\x0csuccess_docs\x18\x02 \x01(\x04\x12\x13\n\x0b\x66\x61iled_docs\x18\x03 \x01(\x04\"<\n\x14IndexDocumentRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocument\x18\x02 \x01(\x0c\"\x17\n\x15IndexDocumentResponse\"?\n\x14MergeSegmentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x13\n\x0bsegment_ids\x18\x02 \x03(\t\"?\n\x15MergeSegmentsResponse\x12\x17\n\nsegment_id\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_segment_id\"?\n\x14SetIndexAliasRequest\x12\x13\n\x0bindex_alias\x18\x01 \x01(\t\x12\x12\n\nindex_name\x18\x02 \x01(\t\"G\n\x15SetIndexAliasResponse\x12\x1b\n\x0eold_index_name\x18\x01 \x01(\tH\x00\x88\x01\x01\x42\x11\n\x0f_old_index_name\"6\n\x10\x44ocumentsRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"%\n\x11\x44ocumentsResponse\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\"C\n\x12VacuumIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x19\n\x11\x65xcluded_segments\x18\x02 \x03(\t\"0\n\x13VacuumIndexResponse\x12\x19\n\x11\x66reed_space_bytes\x18\x01 \x01(\x04\"9\n\x12WarmupIndexRequest\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x0f\n\x07is_full\x18\x02 \x01(\x08\"+\n\x13WarmupIndexResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\" \n\x10\x46ileEngineConfig\x12\x0c\n\x04path\x18\x01 \x01(\t\"$\n\x12MemoryEngineConfig\x12\x0e\n\x06schema\x18\x01 \x01(\t\"!\n\x0b\x43\x61\x63heConfig\x12\x12\n\ncache_size\x18\x01 \x01(\x04\"\x9a\x02\n\x12RemoteEngineConfig\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\x14\n\x0curl_template\x18\x02 \x01(\t\x12N\n\x10headers_template\x18\x03 \x03(\x0b\x32\x34.summa.proto.RemoteEngineConfig.HeadersTemplateEntry\x12.\n\x0c\x63\x61\x63he_config\x18\x04 \x01(\x0b\x32\x18.summa.proto.CacheConfig\x12\x17\n\ntimeout_ms\x18\x05 \x01(\rH\x00\x88\x01\x01\x1a\x36\n\x14HeadersTemplateEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\r\n\x0b_timeout_ms\"#\n\x0eLogMergePolicy\x12\x11\n\tis_frozen\x18\x01 \x01(\x08\"4\n\x13TemporalMergePolicy\x12\x1d\n\x15merge_older_then_secs\x18\x01 \x01(\x04\"\xa0\x03\n\x11IndexEngineConfig\x12-\n\x04\x66ile\x18\x01 \x01(\x0b\x32\x1d.summa.proto.FileEngineConfigH\x00\x12\x31\n\x06memory\x18\x02 \x01(\x0b\x32\x1f.summa.proto.MemoryEngineConfigH\x00\x12\x31\n\x06remote\x18\x03 \x01(\x0b\x32\x1f.summa.proto.RemoteEngineConfigH\x00\x12.\n\x0cmerge_policy\x18\n \x01(\x0b\x32\x18.summa.proto.MergePolicy\x12;\n\x13query_parser_config\x18\x0b \x01(\x0b\x32\x1e.summa.proto.QueryParserConfig\x12I\n\x0e\x66ield_triggers\x18\x0c \x03(\x0b\x32\x31.summa.proto.IndexEngineConfig.FieldTriggersEntry\x1a\x34\n\x12\x46ieldTriggersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x08\n\x06\x63onfig\"\xec\x01\n\x10IndexDescription\x12\x12\n\nindex_name\x18\x01 \x01(\t\x12\x15\n\rindex_aliases\x18\x02 \x03(\t\x12\x34\n\x0cindex_engine\x18\x03 \x01(\x0b\x32\x1e.summa.proto.IndexEngineConfig\x12\x10\n\x08num_docs\x18\x04 \x01(\x04\x12-\n\x0b\x63ompression\x18\x05 \x01(\x0e\x32\x18.summa.proto.Compression\x12\x36\n\x10index_attributes\x18\x06 \x01(\x0b\x32\x1c.summa.proto.IndexAttributes\"*\n\x16IndexDocumentOperation\x12\x10\n\x08\x64ocument\x18\x01 \x01(\x0c\"\\\n\x0eIndexOperation\x12=\n\x0eindex_document\x18\x02 \x01(\x0b\x32#.summa.proto.IndexDocumentOperationH\x00\x42\x0b\n\toperation*R\n\x10\x43onflictStrategy\x12\x0e\n\nDO_NOTHING\x10\x00\x12\x14\n\x10OVERWRITE_ALWAYS\x10\x01\x12\r\n\tOVERWRITE\x10\x02\x12\t\n\x05MERGE\x10\x03*|\n\x0b\x43ompression\x12\x08\n\x04None\x10\x00\x12\n\n\x06\x42rotli\x10\x01\x12\x07\n\x03Lz4\x10\x02\x12\n\n\x06Snappy\x10\x03\x12\x08\n\x04Zstd\x10\x04\x12\t\n\x05Zstd7\x10\x05\x12\t\n\x05Zstd9\x10\x06\x12\n\n\x06Zstd14\x10\x07\x12\n\n\x06Zstd19\x10\x08\x12\n\n\x06Zstd22\x10\t2\xeb\x0b\n\x08IndexApi\x12S\n\x0c\x61ttach_index\x12\x1f.summa.proto.AttachIndexRequest\x1a .summa.proto.AttachIndexResponse\"\x00\x12S\n\x0c\x63ommit_index\x12\x1f.summa.proto.CommitIndexRequest\x1a .summa.proto.CommitIndexResponse\"\x00\x12Y\n\x0e\x63opy_documents\x12!.summa.proto.CopyDocumentsRequest\x1a\".summa.proto.CopyDocumentsResponse\"\x00\x12S\n\x0c\x63reate_index\x12\x1f.summa.proto.CreateIndexRequest\x1a .summa.proto.CreateIndexResponse\"\x00\x12M\n\ncopy_index\x12\x1d.summa.proto.CopyIndexRequest\x1a\x1e.summa.proto.CopyIndexResponse\"\x00\x12_\n\x10\x64\x65lete_documents\x12#.summa.proto.DeleteDocumentsRequest\x1a$.summa.proto.DeleteDocumentsResponse\"\x00\x12S\n\x0c\x64\x65lete_index\x12\x1f.summa.proto.DeleteIndexRequest\x1a .summa.proto.DeleteIndexResponse\"\x00\x12N\n\tdocuments\x12\x1d.summa.proto.DocumentsRequest\x1a\x1e.summa.proto.DocumentsResponse\"\x00\x30\x01\x12\x66\n\x13get_indices_aliases\x12%.summa.proto.GetIndicesAliasesRequest\x1a&.summa.proto.GetIndicesAliasesResponse\"\x00\x12J\n\tget_index\x12\x1c.summa.proto.GetIndexRequest\x1a\x1d.summa.proto.GetIndexResponse\"\x00\x12P\n\x0bget_indices\x12\x1e.summa.proto.GetIndicesRequest\x1a\x1f.summa.proto.GetIndicesResponse\"\x00\x12n\n\x15index_document_stream\x12\'.summa.proto.IndexDocumentStreamRequest\x1a(.summa.proto.IndexDocumentStreamResponse\"\x00(\x01\x12Y\n\x0eindex_document\x12!.summa.proto.IndexDocumentRequest\x1a\".summa.proto.IndexDocumentResponse\"\x00\x12Y\n\x0emerge_segments\x12!.summa.proto.MergeSegmentsRequest\x1a\".summa.proto.MergeSegmentsResponse\"\x00\x12Z\n\x0fset_index_alias\x12!.summa.proto.SetIndexAliasRequest\x1a\".summa.proto.SetIndexAliasResponse\"\x00\x12S\n\x0cvacuum_index\x12\x1f.summa.proto.VacuumIndexRequest\x1a .summa.proto.VacuumIndexResponse\"\x00\x12S\n\x0cwarmup_index\x12\x1f.summa.proto.WarmupIndexRequest\x1a .summa.proto.WarmupIndexResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'index_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._options = None
   _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_options = b'8\001'
   _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._options = None
   _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_options = b'8\001'
-  _INDEXENGINECONFIG_FIELDALIASESENTRY._options = None
-  _INDEXENGINECONFIG_FIELDALIASESENTRY._serialized_options = b'8\001'
-  _CONFLICTSTRATEGY._serialized_start=4777
-  _CONFLICTSTRATEGY._serialized_end=4859
-  _COMPRESSION._serialized_start=4861
-  _COMPRESSION._serialized_end=4985
+  _INDEXENGINECONFIG_FIELDTRIGGERSENTRY._options = None
+  _INDEXENGINECONFIG_FIELDTRIGGERSENTRY._serialized_options = b'8\001'
+  _CONFLICTSTRATEGY._serialized_start=4939
+  _CONFLICTSTRATEGY._serialized_end=5021
+  _COMPRESSION._serialized_start=5023
+  _COMPRESSION._serialized_end=5147
   _PRIMARYKEY._serialized_start=62
   _PRIMARYKEY._serialized_end=113
   _MERGEPOLICY._serialized_start=115
   _MERGEPOLICY._serialized_end=242
   _ATTACHFILEENGINEREQUEST._serialized_start=244
   _ATTACHFILEENGINEREQUEST._serialized_end=269
   _ATTACHREMOTEENGINEREQUEST._serialized_start=271
   _ATTACHREMOTEENGINEREQUEST._serialized_end=347
   _ATTACHINDEXREQUEST._serialized_start=350
-  _ATTACHINDEXREQUEST._serialized_end=566
-  _ATTACHINDEXRESPONSE._serialized_start=568
-  _ATTACHINDEXRESPONSE._serialized_end=635
-  _COMMITINDEXREQUEST._serialized_start=637
-  _COMMITINDEXREQUEST._serialized_end=677
-  _COMMITINDEXRESPONSE._serialized_start=679
-  _COMMITINDEXRESPONSE._serialized_end=722
-  _COPYDOCUMENTSREQUEST._serialized_start=724
-  _COPYDOCUMENTSREQUEST._serialized_end=800
-  _COPYDOCUMENTSRESPONSE._serialized_start=802
-  _COPYDOCUMENTSRESPONSE._serialized_end=873
-  _COPYINDEXREQUEST._serialized_start=876
-  _COPYINDEXREQUEST._serialized_end=1131
-  _COPYINDEXRESPONSE._serialized_start=1133
-  _COPYINDEXRESPONSE._serialized_end=1198
-  _SORTBYFIELD._serialized_start=1200
-  _SORTBYFIELD._serialized_end=1263
-  _CREATEFILEENGINEREQUEST._serialized_start=1265
-  _CREATEFILEENGINEREQUEST._serialized_end=1290
-  _CREATEMEMORYENGINEREQUEST._serialized_start=1292
-  _CREATEMEMORYENGINEREQUEST._serialized_end=1319
-  _INDEXATTRIBUTES._serialized_start=1322
-  _INDEXATTRIBUTES._serialized_end=1610
-  _CREATEINDEXREQUEST._serialized_start=1613
-  _CREATEINDEXREQUEST._serialized_end=2058
-  _CREATEINDEXRESPONSE._serialized_start=2060
-  _CREATEINDEXRESPONSE._serialized_end=2127
-  _DELETEDOCUMENTSREQUEST._serialized_start=2129
-  _DELETEDOCUMENTSREQUEST._serialized_end=2208
-  _DELETEDOCUMENTSRESPONSE._serialized_start=2210
-  _DELETEDOCUMENTSRESPONSE._serialized_end=2262
-  _DELETEINDEXREQUEST._serialized_start=2264
-  _DELETEINDEXREQUEST._serialized_end=2304
-  _DELETEINDEXRESPONSE._serialized_start=2306
-  _DELETEINDEXRESPONSE._serialized_end=2355
-  _GETINDICESALIASESREQUEST._serialized_start=2357
-  _GETINDICESALIASESREQUEST._serialized_end=2383
-  _GETINDICESALIASESRESPONSE._serialized_start=2386
-  _GETINDICESALIASESRESPONSE._serialized_end=2553
-  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_start=2500
-  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_end=2553
-  _GETINDEXREQUEST._serialized_start=2555
-  _GETINDEXREQUEST._serialized_end=2592
-  _GETINDEXRESPONSE._serialized_start=2594
-  _GETINDEXRESPONSE._serialized_end=2658
-  _GETINDICESREQUEST._serialized_start=2660
-  _GETINDICESREQUEST._serialized_end=2679
-  _GETINDICESRESPONSE._serialized_start=2681
-  _GETINDICESRESPONSE._serialized_end=2722
-  _INDEXDOCUMENTSTREAMREQUEST._serialized_start=2724
-  _INDEXDOCUMENTSTREAMREQUEST._serialized_end=2791
-  _INDEXDOCUMENTSTREAMRESPONSE._serialized_start=2793
-  _INDEXDOCUMENTSTREAMRESPONSE._serialized_end=2887
-  _INDEXDOCUMENTREQUEST._serialized_start=2889
-  _INDEXDOCUMENTREQUEST._serialized_end=2949
-  _INDEXDOCUMENTRESPONSE._serialized_start=2951
-  _INDEXDOCUMENTRESPONSE._serialized_end=2974
-  _MERGESEGMENTSREQUEST._serialized_start=2976
-  _MERGESEGMENTSREQUEST._serialized_end=3039
-  _MERGESEGMENTSRESPONSE._serialized_start=3041
-  _MERGESEGMENTSRESPONSE._serialized_end=3104
-  _SETINDEXALIASREQUEST._serialized_start=3106
-  _SETINDEXALIASREQUEST._serialized_end=3169
-  _SETINDEXALIASRESPONSE._serialized_start=3171
-  _SETINDEXALIASRESPONSE._serialized_end=3242
-  _DOCUMENTSREQUEST._serialized_start=3244
-  _DOCUMENTSREQUEST._serialized_end=3298
-  _DOCUMENTSRESPONSE._serialized_start=3300
-  _DOCUMENTSRESPONSE._serialized_end=3337
-  _VACUUMINDEXREQUEST._serialized_start=3339
-  _VACUUMINDEXREQUEST._serialized_end=3406
-  _VACUUMINDEXRESPONSE._serialized_start=3408
-  _VACUUMINDEXRESPONSE._serialized_end=3456
-  _WARMUPINDEXREQUEST._serialized_start=3458
-  _WARMUPINDEXREQUEST._serialized_end=3515
-  _WARMUPINDEXRESPONSE._serialized_start=3517
-  _WARMUPINDEXRESPONSE._serialized_end=3560
-  _FILEENGINECONFIG._serialized_start=3562
-  _FILEENGINECONFIG._serialized_end=3594
-  _MEMORYENGINECONFIG._serialized_start=3596
-  _MEMORYENGINECONFIG._serialized_end=3632
-  _CACHECONFIG._serialized_start=3634
-  _CACHECONFIG._serialized_end=3667
-  _REMOTEENGINECONFIG._serialized_start=3670
-  _REMOTEENGINECONFIG._serialized_end=3952
-  _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_start=3883
-  _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_end=3937
-  _LOGMERGEPOLICY._serialized_start=3954
-  _LOGMERGEPOLICY._serialized_end=3989
-  _TEMPORALMERGEPOLICY._serialized_start=3991
-  _TEMPORALMERGEPOLICY._serialized_end=4043
-  _INDEXENGINECONFIG._serialized_start=4046
-  _INDEXENGINECONFIG._serialized_end=4398
-  _INDEXENGINECONFIG_FIELDALIASESENTRY._serialized_start=4337
-  _INDEXENGINECONFIG_FIELDALIASESENTRY._serialized_end=4388
-  _INDEXDESCRIPTION._serialized_start=4401
-  _INDEXDESCRIPTION._serialized_end=4637
-  _INDEXDOCUMENTOPERATION._serialized_start=4639
-  _INDEXDOCUMENTOPERATION._serialized_end=4681
-  _INDEXOPERATION._serialized_start=4683
-  _INDEXOPERATION._serialized_end=4775
-  _INDEXAPI._serialized_start=4988
-  _INDEXAPI._serialized_end=6503
+  _ATTACHINDEXREQUEST._serialized_end=627
+  _ATTACHINDEXRESPONSE._serialized_start=629
+  _ATTACHINDEXRESPONSE._serialized_end=696
+  _COMMITINDEXREQUEST._serialized_start=698
+  _COMMITINDEXREQUEST._serialized_end=738
+  _COMMITINDEXRESPONSE._serialized_start=740
+  _COMMITINDEXRESPONSE._serialized_end=783
+  _COPYDOCUMENTSREQUEST._serialized_start=785
+  _COPYDOCUMENTSREQUEST._serialized_end=861
+  _COPYDOCUMENTSRESPONSE._serialized_start=863
+  _COPYDOCUMENTSRESPONSE._serialized_end=934
+  _COPYINDEXREQUEST._serialized_start=937
+  _COPYINDEXREQUEST._serialized_end=1192
+  _COPYINDEXRESPONSE._serialized_start=1194
+  _COPYINDEXRESPONSE._serialized_end=1259
+  _SORTBYFIELD._serialized_start=1261
+  _SORTBYFIELD._serialized_end=1324
+  _CREATEFILEENGINEREQUEST._serialized_start=1326
+  _CREATEFILEENGINEREQUEST._serialized_end=1351
+  _CREATEMEMORYENGINEREQUEST._serialized_start=1353
+  _CREATEMEMORYENGINEREQUEST._serialized_end=1380
+  _INDEXATTRIBUTES._serialized_start=1383
+  _INDEXATTRIBUTES._serialized_end=1647
+  _CREATEINDEXREQUEST._serialized_start=1650
+  _CREATEINDEXREQUEST._serialized_end=2156
+  _CREATEINDEXRESPONSE._serialized_start=2158
+  _CREATEINDEXRESPONSE._serialized_end=2225
+  _DELETEDOCUMENTSREQUEST._serialized_start=2227
+  _DELETEDOCUMENTSREQUEST._serialized_end=2306
+  _DELETEDOCUMENTSRESPONSE._serialized_start=2308
+  _DELETEDOCUMENTSRESPONSE._serialized_end=2360
+  _DELETEINDEXREQUEST._serialized_start=2362
+  _DELETEINDEXREQUEST._serialized_end=2402
+  _DELETEINDEXRESPONSE._serialized_start=2404
+  _DELETEINDEXRESPONSE._serialized_end=2453
+  _GETINDICESALIASESREQUEST._serialized_start=2455
+  _GETINDICESALIASESREQUEST._serialized_end=2481
+  _GETINDICESALIASESRESPONSE._serialized_start=2484
+  _GETINDICESALIASESRESPONSE._serialized_end=2651
+  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_start=2598
+  _GETINDICESALIASESRESPONSE_INDICESALIASESENTRY._serialized_end=2651
+  _GETINDEXREQUEST._serialized_start=2653
+  _GETINDEXREQUEST._serialized_end=2690
+  _GETINDEXRESPONSE._serialized_start=2692
+  _GETINDEXRESPONSE._serialized_end=2756
+  _GETINDICESREQUEST._serialized_start=2758
+  _GETINDICESREQUEST._serialized_end=2777
+  _GETINDICESRESPONSE._serialized_start=2779
+  _GETINDICESRESPONSE._serialized_end=2820
+  _INDEXDOCUMENTSTREAMREQUEST._serialized_start=2822
+  _INDEXDOCUMENTSTREAMREQUEST._serialized_end=2889
+  _INDEXDOCUMENTSTREAMRESPONSE._serialized_start=2891
+  _INDEXDOCUMENTSTREAMRESPONSE._serialized_end=2985
+  _INDEXDOCUMENTREQUEST._serialized_start=2987
+  _INDEXDOCUMENTREQUEST._serialized_end=3047
+  _INDEXDOCUMENTRESPONSE._serialized_start=3049
+  _INDEXDOCUMENTRESPONSE._serialized_end=3072
+  _MERGESEGMENTSREQUEST._serialized_start=3074
+  _MERGESEGMENTSREQUEST._serialized_end=3137
+  _MERGESEGMENTSRESPONSE._serialized_start=3139
+  _MERGESEGMENTSRESPONSE._serialized_end=3202
+  _SETINDEXALIASREQUEST._serialized_start=3204
+  _SETINDEXALIASREQUEST._serialized_end=3267
+  _SETINDEXALIASRESPONSE._serialized_start=3269
+  _SETINDEXALIASRESPONSE._serialized_end=3340
+  _DOCUMENTSREQUEST._serialized_start=3342
+  _DOCUMENTSREQUEST._serialized_end=3396
+  _DOCUMENTSRESPONSE._serialized_start=3398
+  _DOCUMENTSRESPONSE._serialized_end=3435
+  _VACUUMINDEXREQUEST._serialized_start=3437
+  _VACUUMINDEXREQUEST._serialized_end=3504
+  _VACUUMINDEXRESPONSE._serialized_start=3506
+  _VACUUMINDEXRESPONSE._serialized_end=3554
+  _WARMUPINDEXREQUEST._serialized_start=3556
+  _WARMUPINDEXREQUEST._serialized_end=3613
+  _WARMUPINDEXRESPONSE._serialized_start=3615
+  _WARMUPINDEXRESPONSE._serialized_end=3658
+  _FILEENGINECONFIG._serialized_start=3660
+  _FILEENGINECONFIG._serialized_end=3692
+  _MEMORYENGINECONFIG._serialized_start=3694
+  _MEMORYENGINECONFIG._serialized_end=3730
+  _CACHECONFIG._serialized_start=3732
+  _CACHECONFIG._serialized_end=3765
+  _REMOTEENGINECONFIG._serialized_start=3768
+  _REMOTEENGINECONFIG._serialized_end=4050
+  _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_start=3981
+  _REMOTEENGINECONFIG_HEADERSTEMPLATEENTRY._serialized_end=4035
+  _LOGMERGEPOLICY._serialized_start=4052
+  _LOGMERGEPOLICY._serialized_end=4087
+  _TEMPORALMERGEPOLICY._serialized_start=4089
+  _TEMPORALMERGEPOLICY._serialized_end=4141
+  _INDEXENGINECONFIG._serialized_start=4144
+  _INDEXENGINECONFIG._serialized_end=4560
+  _INDEXENGINECONFIG_FIELDTRIGGERSENTRY._serialized_start=4498
+  _INDEXENGINECONFIG_FIELDTRIGGERSENTRY._serialized_end=4550
+  _INDEXDESCRIPTION._serialized_start=4563
+  _INDEXDESCRIPTION._serialized_end=4799
+  _INDEXDOCUMENTOPERATION._serialized_start=4801
+  _INDEXDOCUMENTOPERATION._serialized_end=4843
+  _INDEXOPERATION._serialized_start=4845
+  _INDEXOPERATION._serialized_end=4937
+  _INDEXAPI._serialized_start=5150
+  _INDEXAPI._serialized_end=6665
 # @@protoc_insertion_point(module_scope)
```

### Comparing `summa_embed-0.15.9/summa_embed/proto/index_service_pb2.pyi` & `summa_embed-0.16.0/summa_embed/proto/index_service_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -28,24 +28,26 @@
 Zstd9: Compression
 
 class AttachFileEngineRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class AttachIndexRequest(_message.Message):
-    __slots__ = ["file", "index_name", "merge_policy", "remote"]
+    __slots__ = ["file", "index_name", "merge_policy", "query_parser_config", "remote"]
     FILE_FIELD_NUMBER: _ClassVar[int]
     INDEX_NAME_FIELD_NUMBER: _ClassVar[int]
     MERGE_POLICY_FIELD_NUMBER: _ClassVar[int]
+    QUERY_PARSER_CONFIG_FIELD_NUMBER: _ClassVar[int]
     REMOTE_FIELD_NUMBER: _ClassVar[int]
     file: AttachFileEngineRequest
     index_name: str
     merge_policy: MergePolicy
+    query_parser_config: _query_pb2.QueryParserConfig
     remote: AttachRemoteEngineRequest
-    def __init__(self, index_name: _Optional[str] = ..., file: _Optional[_Union[AttachFileEngineRequest, _Mapping]] = ..., remote: _Optional[_Union[AttachRemoteEngineRequest, _Mapping]] = ..., merge_policy: _Optional[_Union[MergePolicy, _Mapping]] = ...) -> None: ...
+    def __init__(self, index_name: _Optional[str] = ..., file: _Optional[_Union[AttachFileEngineRequest, _Mapping]] = ..., remote: _Optional[_Union[AttachRemoteEngineRequest, _Mapping]] = ..., merge_policy: _Optional[_Union[MergePolicy, _Mapping]] = ..., query_parser_config: _Optional[_Union[_query_pb2.QueryParserConfig, _Mapping]] = ...) -> None: ...
 
 class AttachIndexResponse(_message.Message):
     __slots__ = ["index"]
     INDEX_FIELD_NUMBER: _ClassVar[int]
     index: IndexDescription
     def __init__(self, index: _Optional[_Union[IndexDescription, _Mapping]] = ...) -> None: ...
 
@@ -110,34 +112,36 @@
     def __init__(self, index: _Optional[_Union[IndexDescription, _Mapping]] = ...) -> None: ...
 
 class CreateFileEngineRequest(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class CreateIndexRequest(_message.Message):
-    __slots__ = ["blocksize", "compression", "file", "index_attributes", "index_name", "memory", "merge_policy", "schema", "sort_by_field"]
+    __slots__ = ["blocksize", "compression", "file", "index_attributes", "index_name", "memory", "merge_policy", "query_parser_config", "schema", "sort_by_field"]
     BLOCKSIZE_FIELD_NUMBER: _ClassVar[int]
     COMPRESSION_FIELD_NUMBER: _ClassVar[int]
     FILE_FIELD_NUMBER: _ClassVar[int]
     INDEX_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
     INDEX_NAME_FIELD_NUMBER: _ClassVar[int]
     MEMORY_FIELD_NUMBER: _ClassVar[int]
     MERGE_POLICY_FIELD_NUMBER: _ClassVar[int]
+    QUERY_PARSER_CONFIG_FIELD_NUMBER: _ClassVar[int]
     SCHEMA_FIELD_NUMBER: _ClassVar[int]
     SORT_BY_FIELD_FIELD_NUMBER: _ClassVar[int]
     blocksize: int
     compression: Compression
     file: CreateFileEngineRequest
     index_attributes: IndexAttributes
     index_name: str
     memory: CreateMemoryEngineRequest
     merge_policy: MergePolicy
+    query_parser_config: _query_pb2.QueryParserConfig
     schema: str
     sort_by_field: SortByField
-    def __init__(self, index_name: _Optional[str] = ..., file: _Optional[_Union[CreateFileEngineRequest, _Mapping]] = ..., memory: _Optional[_Union[CreateMemoryEngineRequest, _Mapping]] = ..., schema: _Optional[str] = ..., compression: _Optional[_Union[Compression, str]] = ..., blocksize: _Optional[int] = ..., sort_by_field: _Optional[_Union[SortByField, _Mapping]] = ..., index_attributes: _Optional[_Union[IndexAttributes, _Mapping]] = ..., merge_policy: _Optional[_Union[MergePolicy, _Mapping]] = ...) -> None: ...
+    def __init__(self, index_name: _Optional[str] = ..., file: _Optional[_Union[CreateFileEngineRequest, _Mapping]] = ..., memory: _Optional[_Union[CreateMemoryEngineRequest, _Mapping]] = ..., schema: _Optional[str] = ..., compression: _Optional[_Union[Compression, str]] = ..., blocksize: _Optional[int] = ..., sort_by_field: _Optional[_Union[SortByField, _Mapping]] = ..., index_attributes: _Optional[_Union[IndexAttributes, _Mapping]] = ..., merge_policy: _Optional[_Union[MergePolicy, _Mapping]] = ..., query_parser_config: _Optional[_Union[_query_pb2.QueryParserConfig, _Mapping]] = ...) -> None: ...
 
 class CreateIndexResponse(_message.Message):
     __slots__ = ["index"]
     INDEX_FIELD_NUMBER: _ClassVar[int]
     index: IndexDescription
     def __init__(self, index: _Optional[_Union[IndexDescription, _Mapping]] = ...) -> None: ...
 
@@ -227,32 +231,30 @@
 class GetIndicesResponse(_message.Message):
     __slots__ = ["index_names"]
     INDEX_NAMES_FIELD_NUMBER: _ClassVar[int]
     index_names: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, index_names: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class IndexAttributes(_message.Message):
-    __slots__ = ["conflict_strategy", "created_at", "default_fields", "default_index_name", "default_snippets", "description", "multi_fields", "unique_fields"]
+    __slots__ = ["conflict_strategy", "created_at", "default_index_name", "default_snippets", "description", "multi_fields", "unique_fields"]
     CONFLICT_STRATEGY_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    DEFAULT_FIELDS_FIELD_NUMBER: _ClassVar[int]
     DEFAULT_INDEX_NAME_FIELD_NUMBER: _ClassVar[int]
     DEFAULT_SNIPPETS_FIELD_NUMBER: _ClassVar[int]
     DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     MULTI_FIELDS_FIELD_NUMBER: _ClassVar[int]
     UNIQUE_FIELDS_FIELD_NUMBER: _ClassVar[int]
     conflict_strategy: ConflictStrategy
     created_at: int
-    default_fields: _containers.RepeatedScalarFieldContainer[str]
     default_index_name: str
     default_snippets: _containers.RepeatedScalarFieldContainer[str]
     description: str
     multi_fields: _containers.RepeatedScalarFieldContainer[str]
     unique_fields: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, created_at: _Optional[int] = ..., unique_fields: _Optional[_Iterable[str]] = ..., default_fields: _Optional[_Iterable[str]] = ..., multi_fields: _Optional[_Iterable[str]] = ..., default_index_name: _Optional[str] = ..., description: _Optional[str] = ..., default_snippets: _Optional[_Iterable[str]] = ..., conflict_strategy: _Optional[_Union[ConflictStrategy, str]] = ...) -> None: ...
+    def __init__(self, created_at: _Optional[int] = ..., unique_fields: _Optional[_Iterable[str]] = ..., multi_fields: _Optional[_Iterable[str]] = ..., default_index_name: _Optional[str] = ..., description: _Optional[str] = ..., default_snippets: _Optional[_Iterable[str]] = ..., conflict_strategy: _Optional[_Union[ConflictStrategy, str]] = ...) -> None: ...
 
 class IndexDescription(_message.Message):
     __slots__ = ["compression", "index_aliases", "index_attributes", "index_engine", "index_name", "num_docs"]
     COMPRESSION_FIELD_NUMBER: _ClassVar[int]
     INDEX_ALIASES_FIELD_NUMBER: _ClassVar[int]
     INDEX_ATTRIBUTES_FIELD_NUMBER: _ClassVar[int]
     INDEX_ENGINE_FIELD_NUMBER: _ClassVar[int]
@@ -299,33 +301,35 @@
     SUCCESS_DOCS_FIELD_NUMBER: _ClassVar[int]
     elapsed_secs: float
     failed_docs: int
     success_docs: int
     def __init__(self, elapsed_secs: _Optional[float] = ..., success_docs: _Optional[int] = ..., failed_docs: _Optional[int] = ...) -> None: ...
 
 class IndexEngineConfig(_message.Message):
-    __slots__ = ["field_aliases", "file", "memory", "merge_policy", "remote"]
-    class FieldAliasesEntry(_message.Message):
+    __slots__ = ["field_triggers", "file", "memory", "merge_policy", "query_parser_config", "remote"]
+    class FieldTriggersEntry(_message.Message):
         __slots__ = ["key", "value"]
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
-    FIELD_ALIASES_FIELD_NUMBER: _ClassVar[int]
+    FIELD_TRIGGERS_FIELD_NUMBER: _ClassVar[int]
     FILE_FIELD_NUMBER: _ClassVar[int]
     MEMORY_FIELD_NUMBER: _ClassVar[int]
     MERGE_POLICY_FIELD_NUMBER: _ClassVar[int]
+    QUERY_PARSER_CONFIG_FIELD_NUMBER: _ClassVar[int]
     REMOTE_FIELD_NUMBER: _ClassVar[int]
-    field_aliases: _containers.ScalarMap[str, str]
+    field_triggers: _containers.ScalarMap[str, str]
     file: FileEngineConfig
     memory: MemoryEngineConfig
     merge_policy: MergePolicy
+    query_parser_config: _query_pb2.QueryParserConfig
     remote: RemoteEngineConfig
-    def __init__(self, file: _Optional[_Union[FileEngineConfig, _Mapping]] = ..., memory: _Optional[_Union[MemoryEngineConfig, _Mapping]] = ..., remote: _Optional[_Union[RemoteEngineConfig, _Mapping]] = ..., merge_policy: _Optional[_Union[MergePolicy, _Mapping]] = ..., field_aliases: _Optional[_Mapping[str, str]] = ...) -> None: ...
+    def __init__(self, file: _Optional[_Union[FileEngineConfig, _Mapping]] = ..., memory: _Optional[_Union[MemoryEngineConfig, _Mapping]] = ..., remote: _Optional[_Union[RemoteEngineConfig, _Mapping]] = ..., merge_policy: _Optional[_Union[MergePolicy, _Mapping]] = ..., query_parser_config: _Optional[_Union[_query_pb2.QueryParserConfig, _Mapping]] = ..., field_triggers: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
 class IndexOperation(_message.Message):
     __slots__ = ["index_document"]
     INDEX_DOCUMENT_FIELD_NUMBER: _ClassVar[int]
     index_document: IndexDocumentOperation
     def __init__(self, index_document: _Optional[_Union[IndexDocumentOperation, _Mapping]] = ...) -> None: ...
```

### Comparing `summa_embed-0.15.9/summa_embed/proto/query_pb2.py` & `summa_embed-0.16.0/summa_embed/proto/query_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,29 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from . import utils_pb2 as utils__pb2
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bquery.proto\x12\x0bsumma.proto\x1a\x0butils.proto\"_\n\x0eSearchResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x37\n\x11\x63ollector_outputs\x18\x02 \x03(\x0b\x32\x1c.summa.proto.CollectorOutput\"\xad\x04\n\x05Query\x12,\n\x07\x62oolean\x18\x01 \x01(\x0b\x32\x19.summa.proto.BooleanQueryH\x00\x12(\n\x05match\x18\x02 \x01(\x0b\x32\x17.summa.proto.MatchQueryH\x00\x12(\n\x05regex\x18\x03 \x01(\x0b\x32\x17.summa.proto.RegexQueryH\x00\x12&\n\x04term\x18\x04 \x01(\x0b\x32\x16.summa.proto.TermQueryH\x00\x12*\n\x06phrase\x18\x05 \x01(\x0b\x32\x18.summa.proto.PhraseQueryH\x00\x12(\n\x05range\x18\x06 \x01(\x0b\x32\x17.summa.proto.RangeQueryH\x00\x12$\n\x03\x61ll\x18\x07 \x01(\x0b\x32\x15.summa.proto.AllQueryH\x00\x12\x38\n\x0emore_like_this\x18\x08 \x01(\x0b\x32\x1e.summa.proto.MoreLikeThisQueryH\x00\x12(\n\x05\x62oost\x18\t \x01(\x0b\x32\x17.summa.proto.BoostQueryH\x00\x12;\n\x0f\x64isjunction_max\x18\n \x01(\x0b\x32 .summa.proto.DisjunctionMaxQueryH\x00\x12(\n\x05\x65mpty\x18\x0b \x01(\x0b\x32\x17.summa.proto.EmptyQueryH\x00\x12*\n\x06\x65xists\x18\x0c \x01(\x0b\x32\x18.summa.proto.ExistsQueryH\x00\x42\x07\n\x05query\"\n\n\x08\x41llQuery\"\x0c\n\nEmptyQuery\">\n\nBoostQuery\x12!\n\x05query\x18\x01 \x01(\x0b\x32\x12.summa.proto.Query\x12\r\n\x05score\x18\x02 \x01(\t\"Q\n\x13\x44isjunctionMaxQuery\x12%\n\tdisjuncts\x18\x01 \x03(\x0b\x32\x12.summa.proto.Query\x12\x13\n\x0btie_breaker\x18\x02 \x01(\t\"\x91\x03\n\x11MoreLikeThisQuery\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12\x1e\n\x11min_doc_frequency\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x1e\n\x11max_doc_frequency\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x1f\n\x12min_term_frequency\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x1c\n\x0fmax_query_terms\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12\x1c\n\x0fmin_word_length\x18\x06 \x01(\x04H\x04\x88\x01\x01\x12\x1c\n\x0fmax_word_length\x18\x07 \x01(\x04H\x05\x88\x01\x01\x12\x12\n\x05\x62oost\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x12\n\nstop_words\x18\t \x03(\tB\x14\n\x12_min_doc_frequencyB\x14\n\x12_max_doc_frequencyB\x15\n\x13_min_term_frequencyB\x12\n\x10_max_query_termsB\x12\n\x10_min_word_lengthB\x12\n\x10_max_word_lengthB\x08\n\x06_boost\"9\n\x0bPhraseQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04slop\x18\x03 \x01(\r\">\n\nRangeQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.summa.proto.Range\"\x1d\n\x1bMatchQueryBooleanShouldMode\"2\n\x1bMatchQueryDisjuctionMaxMode\x12\x13\n\x0btie_breaker\x18\x01 \x01(\x02\"B\n\x14\x45xactMatchesPromoter\x12\x0c\n\x04slop\x18\x01 \x01(\r\x12\x12\n\x05\x62oost\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\x08\n\x06_boost\"\x8c\x03\n\nMatchQuery\x12\r\n\x05value\x18\x01 \x01(\t\x12\x16\n\x0e\x64\x65\x66\x61ult_fields\x18\x02 \x03(\t\x12G\n\x13\x62oolean_should_mode\x18\x03 \x01(\x0b\x32(.summa.proto.MatchQueryBooleanShouldModeH\x00\x12G\n\x13\x64isjuction_max_mode\x18\x04 \x01(\x0b\x32(.summa.proto.MatchQueryDisjuctionMaxModeH\x00\x12>\n\x0c\x66ield_boosts\x18\x05 \x03(\x0b\x32(.summa.proto.MatchQuery.FieldBoostsEntry\x12\x41\n\x16\x65xact_matches_promoter\x18\x06 \x01(\x0b\x32!.summa.proto.ExactMatchesPromoter\x1a\x32\n\x10\x46ieldBoostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x42\x0e\n\x0c\x64\x65\x66\x61ult_mode\"W\n\x0f\x42ooleanSubquery\x12!\n\x05occur\x18\x01 \x01(\x0e\x32\x12.summa.proto.Occur\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"@\n\x0c\x42ooleanQuery\x12\x30\n\nsubqueries\x18\x01 \x03(\x0b\x32\x1c.summa.proto.BooleanSubquery\"*\n\nRegexQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\")\n\tTermQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x1c\n\x0b\x45xistsQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"\x80\x01\n\x0b\x41ggregation\x12\x30\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x1e.summa.proto.BucketAggregationH\x00\x12\x30\n\x06metric\x18\x02 \x01(\x0b\x32\x1e.summa.proto.MetricAggregationH\x00\x42\r\n\x0b\x61ggregation\"\xd7\x02\n\x11\x42ucketAggregation\x12.\n\x05range\x18\x01 \x01(\x0b\x32\x1d.summa.proto.RangeAggregationH\x00\x12\x36\n\thistogram\x18\x02 \x01(\x0b\x32!.summa.proto.HistogramAggregationH\x00\x12.\n\x05terms\x18\x03 \x01(\x0b\x32\x1d.summa.proto.TermsAggregationH\x00\x12K\n\x0fsub_aggregation\x18\x04 \x03(\x0b\x32\x32.summa.proto.BucketAggregation.SubAggregationEntry\x1aO\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.Aggregation:\x02\x38\x01\x42\x0c\n\nbucket_agg\"U\n\x10RangeAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x32\n\x06ranges\x18\x02 \x03(\x0b\x32\".summa.proto.RangeAggregationRange\"e\n\x15RangeAggregationRange\x12\x11\n\x04\x66rom\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02to\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03key\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x07\n\x05_fromB\x05\n\x03_toB\x06\n\x04_key\"\x9d\x02\n\x14HistogramAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x10\n\x08interval\x18\x02 \x01(\x01\x12\x13\n\x06offset\x18\x03 \x01(\x01H\x00\x88\x01\x01\x12\x1a\n\rmin_doc_count\x18\x04 \x01(\x04H\x01\x88\x01\x01\x12\x36\n\x0bhard_bounds\x18\x05 \x01(\x0b\x32\x1c.summa.proto.HistogramBoundsH\x02\x88\x01\x01\x12:\n\x0f\x65xtended_bounds\x18\x06 \x01(\x0b\x32\x1c.summa.proto.HistogramBoundsH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x10\n\x0e_min_doc_countB\x0e\n\x0c_hard_boundsB\x12\n\x10_extended_bounds\"+\n\x0fHistogramBounds\x12\x0b\n\x03min\x18\x01 \x01(\x01\x12\x0b\n\x03max\x18\x02 \x01(\x01\"\xbd\x02\n\x10TermsAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x11\n\x04size\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x17\n\nsplit_size\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x19\n\x0csegment_size\x18\x04 \x01(\rH\x02\x88\x01\x01\x12&\n\x19show_term_doc_count_error\x18\x05 \x01(\x08H\x03\x88\x01\x01\x12\x1a\n\rmin_doc_count\x18\x06 \x01(\x04H\x04\x88\x01\x01\x12,\n\x05order\x18\x07 \x01(\x0b\x32\x18.summa.proto.CustomOrderH\x05\x88\x01\x01\x42\x07\n\x05_sizeB\r\n\x0b_split_sizeB\x0f\n\r_segment_sizeB\x1c\n\x1a_show_term_doc_count_errorB\x10\n\x0e_min_doc_countB\x08\n\x06_order\"\xa3\x01\n\x0b\x43ustomOrder\x12!\n\x03key\x18\x01 \x01(\x0b\x32\x12.summa.proto.EmptyH\x00\x12#\n\x05\x63ount\x18\x02 \x01(\x0b\x32\x12.summa.proto.EmptyH\x00\x12\x19\n\x0fsub_aggregation\x18\x03 \x01(\tH\x00\x12!\n\x05order\x18\x04 \x01(\x0e\x32\x12.summa.proto.OrderB\x0e\n\x0corder_target\"\x8d\x01\n\x11MetricAggregation\x12\x32\n\x07\x61verage\x18\x01 \x01(\x0b\x32\x1f.summa.proto.AverageAggregationH\x00\x12.\n\x05stats\x18\x02 \x01(\x0b\x32\x1d.summa.proto.StatsAggregationH\x00\x42\x14\n\x12metric_aggregation\"#\n\x12\x41verageAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"!\n\x10StatsAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"\xdd\x01\n\x0b\x42ucketEntry\x12\x1d\n\x03key\x18\x01 \x01(\x0b\x32\x10.summa.proto.Key\x12\x11\n\tdoc_count\x18\x02 \x01(\x04\x12\x45\n\x0fsub_aggregation\x18\x03 \x03(\x0b\x32,.summa.proto.BucketEntry.SubAggregationEntry\x1aU\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\"*\n\x03Key\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03\x66\x36\x34\x18\x02 \x01(\x01H\x00\x42\x05\n\x03key\"U\n\x05Range\x12\x0c\n\x04left\x18\x01 \x01(\t\x12\r\n\x05right\x18\x02 \x01(\t\x12\x16\n\x0eincluding_left\x18\x03 \x01(\x08\x12\x17\n\x0fincluding_right\x18\x04 \x01(\x08\"\x9b\x02\n\x10RangeBucketEntry\x12\x1d\n\x03key\x18\x01 \x01(\x0b\x32\x10.summa.proto.Key\x12\x11\n\tdoc_count\x18\x02 \x01(\x04\x12J\n\x0fsub_aggregation\x18\x03 \x03(\x0b\x32\x31.summa.proto.RangeBucketEntry.SubAggregationEntry\x12\x11\n\x04\x66rom\x18\x04 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02to\x18\x05 \x01(\x01H\x01\x88\x01\x01\x1aU\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\x42\x07\n\x05_fromB\x05\n\x03_to\":\n\x05Score\x12\x13\n\tf64_score\x18\x01 \x01(\x01H\x00\x12\x13\n\tu64_score\x18\x02 \x01(\x04H\x00\x42\x07\n\x05score\"%\n\tHighlight\x12\x0c\n\x04\x66rom\x18\x01 \x01(\r\x12\n\n\x02to\x18\x02 \x01(\r\"U\n\x07Snippet\x12\x10\n\x08\x66ragment\x18\x01 \x01(\x0c\x12*\n\nhighlights\x18\x02 \x03(\x0b\x32\x16.summa.proto.Highlight\x12\x0c\n\x04html\x18\x03 \x01(\t\"\xf0\x01\n\x0eScoredDocument\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12!\n\x05score\x18\x02 \x01(\x0b\x32\x12.summa.proto.Score\x12\x10\n\x08position\x18\x03 \x01(\r\x12;\n\x08snippets\x18\x04 \x03(\x0b\x32).summa.proto.ScoredDocument.SnippetsEntry\x12\x13\n\x0bindex_alias\x18\x05 \x01(\t\x1a\x45\n\rSnippetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.summa.proto.Snippet:\x02\x38\x01\";\n\x06Scorer\x12\x13\n\teval_expr\x18\x01 \x01(\tH\x00\x12\x12\n\x08order_by\x18\x02 \x01(\tH\x00\x42\x08\n\x06scorer\"\xa8\x02\n\tCollector\x12\x31\n\x08top_docs\x18\x01 \x01(\x0b\x32\x1d.summa.proto.TopDocsCollectorH\x00\x12\x45\n\x12reservoir_sampling\x18\x02 \x01(\x0b\x32\'.summa.proto.ReservoirSamplingCollectorH\x00\x12,\n\x05\x63ount\x18\x03 \x01(\x0b\x32\x1b.summa.proto.CountCollectorH\x00\x12,\n\x05\x66\x61\x63\x65t\x18\x04 \x01(\x0b\x32\x1b.summa.proto.FacetCollectorH\x00\x12\x38\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32!.summa.proto.AggregationCollectorH\x00\x42\x0b\n\tcollector\"\x89\x02\n\x0f\x43ollectorOutput\x12:\n\tdocuments\x18\x01 \x01(\x0b\x32%.summa.proto.DocumentsCollectorOutputH\x00\x12\x32\n\x05\x63ount\x18\x03 \x01(\x0b\x32!.summa.proto.CountCollectorOutputH\x00\x12\x32\n\x05\x66\x61\x63\x65t\x18\x04 \x01(\x0b\x32!.summa.proto.FacetCollectorOutputH\x00\x12>\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32\'.summa.proto.AggregationCollectorOutputH\x00\x42\x12\n\x10\x63ollector_output\"\x10\n\x0e\x43ountCollector\"%\n\x14\x43ountCollectorOutput\x12\r\n\x05\x63ount\x18\x01 \x01(\r\"/\n\x0e\x46\x61\x63\x65tCollector\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x0e\n\x06\x66\x61\x63\x65ts\x18\x02 \x03(\t\"\x94\x01\n\x14\x46\x61\x63\x65tCollectorOutput\x12H\n\x0c\x66\x61\x63\x65t_counts\x18\x01 \x03(\x0b\x32\x32.summa.proto.FacetCollectorOutput.FacetCountsEntry\x1a\x32\n\x10\x46\x61\x63\x65tCountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\";\n\x1aReservoirSamplingCollector\x12\r\n\x05limit\x18\x01 \x01(\r\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"Z\n\x0eRandomDocument\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12!\n\x05score\x18\x02 \x01(\x0b\x32\x12.summa.proto.Score\x12\x13\n\x0bindex_alias\x18\x03 \x01(\t\"R\n ReservoirSamplingCollectorOutput\x12.\n\tdocuments\x18\x01 \x03(\x0b\x32\x1b.summa.proto.RandomDocument\"\x8a\x02\n\x10TopDocsCollector\x12\r\n\x05limit\x18\x01 \x01(\r\x12\x0e\n\x06offset\x18\x02 \x01(\r\x12(\n\x06scorer\x18\x03 \x01(\x0b\x32\x13.summa.proto.ScorerH\x00\x88\x01\x01\x12J\n\x0fsnippet_configs\x18\x04 \x03(\x0b\x32\x31.summa.proto.TopDocsCollector.SnippetConfigsEntry\x12\x0f\n\x07\x65xplain\x18\x05 \x01(\x08\x12\x0e\n\x06\x66ields\x18\x06 \x03(\t\x1a\x35\n\x13SnippetConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\x42\t\n\x07_scorer\"c\n\x18\x44ocumentsCollectorOutput\x12\x35\n\x10scored_documents\x18\x01 \x03(\x0b\x32\x1b.summa.proto.ScoredDocument\x12\x10\n\x08has_next\x18\x02 \x01(\x08\"\xb0\x01\n\x14\x41ggregationCollector\x12I\n\x0c\x61ggregations\x18\x01 \x03(\x0b\x32\x33.summa.proto.AggregationCollector.AggregationsEntry\x1aM\n\x11\x41ggregationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.Aggregation:\x02\x38\x01\"\xd5\x01\n\x1a\x41ggregationCollectorOutput\x12\\\n\x13\x61ggregation_results\x18\x01 \x03(\x0b\x32?.summa.proto.AggregationCollectorOutput.AggregationResultsEntry\x1aY\n\x17\x41ggregationResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\"\x83\x01\n\x11\x41ggregationResult\x12+\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x19.summa.proto.BucketResultH\x00\x12+\n\x06metric\x18\x02 \x01(\x0b\x32\x19.summa.proto.MetricResultH\x00\x42\x14\n\x12\x61ggregation_result\"\xa8\x01\n\x0c\x42ucketResult\x12)\n\x05range\x18\x01 \x01(\x0b\x32\x18.summa.proto.RangeResultH\x00\x12\x31\n\thistogram\x18\x02 \x01(\x0b\x32\x1c.summa.proto.HistogramResultH\x00\x12)\n\x05terms\x18\x03 \x01(\x0b\x32\x18.summa.proto.TermsResultH\x00\x42\x0f\n\rbucket_result\"=\n\x0bRangeResult\x12.\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x1d.summa.proto.RangeBucketEntry\"<\n\x0fHistogramResult\x12)\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x18.summa.proto.BucketEntry\"\x9f\x01\n\x0bTermsResult\x12)\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x18.summa.proto.BucketEntry\x12\x1b\n\x13sum_other_doc_count\x18\x02 \x01(\x04\x12(\n\x1b\x64oc_count_error_upper_bound\x18\x03 \x01(\x04H\x00\x88\x01\x01\x42\x1e\n\x1c_doc_count_error_upper_bound\"\x84\x01\n\x0cMetricResult\x12\x38\n\rsingle_metric\x18\x01 \x01(\x0b\x32\x1f.summa.proto.SingleMetricResultH\x00\x12)\n\x05stats\x18\x02 \x01(\x0b\x32\x18.summa.proto.StatsResultH\x00\x42\x0f\n\rmetric_result\"2\n\x12SingleMetricResult\x12\x12\n\x05value\x18\x01 \x01(\x01H\x00\x88\x01\x01\x42\x08\n\x06_value\"w\n\x0bStatsResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\x12\x0b\n\x03sum\x18\x02 \x01(\x01\x12\x10\n\x03min\x18\x03 \x01(\x01H\x00\x88\x01\x01\x12\x10\n\x03max\x18\x04 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03\x61vg\x18\x05 \x01(\x01H\x02\x88\x01\x01\x42\x06\n\x04_minB\x06\n\x04_maxB\x06\n\x04_avg*+\n\x05Occur\x12\n\n\x06should\x10\x00\x12\x08\n\x04must\x10\x01\x12\x0c\n\x08must_not\x10\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0bquery.proto\x12\x0bsumma.proto\x1a\x0butils.proto\"2\n\x0b\x46ieldMapper\x12\x13\n\x0bmapper_name\x18\x01 \x01(\t\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"\x1d\n\x1bMatchQueryBooleanShouldMode\"2\n\x1bMatchQueryDisjuctionMaxMode\x12\x13\n\x0btie_breaker\x18\x01 \x01(\x02\"B\n\x14\x45xactMatchesPromoter\x12\x0c\n\x04slop\x18\x01 \x01(\r\x12\x12\n\x05\x62oost\x18\x02 \x01(\x02H\x00\x88\x01\x01\x42\x08\n\x06_boost\")\n\x10InflectionConfig\x12\x15\n\rderive_plural\x18\x01 \x01(\x08\"\xa3\x07\n\x11QueryParserConfig\x12G\n\rfield_aliases\x18\x01 \x03(\x0b\x32\x30.summa.proto.QueryParserConfig.FieldAliasesEntry\x12\x45\n\x0c\x66ield_boosts\x18\x02 \x03(\x0b\x32/.summa.proto.QueryParserConfig.FieldBoostsEntry\x12I\n\x0e\x66ield_mappings\x18\x03 \x03(\x0b\x32\x31.summa.proto.QueryParserConfig.FieldMappingsEntry\x12\x12\n\nterm_limit\x18\x04 \x01(\r\x12\x16\n\x0e\x64\x65\x66\x61ult_fields\x18\x05 \x03(\t\x12G\n\x13\x62oolean_should_mode\x18\x06 \x01(\x0b\x32(.summa.proto.MatchQueryBooleanShouldModeH\x00\x12G\n\x13\x64isjuction_max_mode\x18\x07 \x01(\x0b\x32(.summa.proto.MatchQueryDisjuctionMaxModeH\x00\x12\x41\n\x16\x65xact_matches_promoter\x18\x08 \x01(\x0b\x32!.summa.proto.ExactMatchesPromoter\x12=\n\x14missing_field_policy\x18\t \x01(\x0e\x32\x1f.summa.proto.MissingFieldPolicy\x12Q\n\x12inflection_configs\x18\n \x03(\x0b\x32\x35.summa.proto.QueryParserConfig.InflectionConfigsEntry\x1a\x33\n\x11\x46ieldAliasesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x1a\x32\n\x10\x46ieldBoostsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1aN\n\x12\x46ieldMappingsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.FieldMapper:\x02\x38\x01\x1aW\n\x16InflectionConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x1d.summa.proto.InflectionConfig:\x02\x38\x01\x42\x0e\n\x0c\x64\x65\x66\x61ult_mode\"_\n\x0eSearchResponse\x12\x14\n\x0c\x65lapsed_secs\x18\x01 \x01(\x01\x12\x37\n\x11\x63ollector_outputs\x18\x02 \x03(\x0b\x32\x1c.summa.proto.CollectorOutput\"\xad\x04\n\x05Query\x12,\n\x07\x62oolean\x18\x01 \x01(\x0b\x32\x19.summa.proto.BooleanQueryH\x00\x12(\n\x05match\x18\x02 \x01(\x0b\x32\x17.summa.proto.MatchQueryH\x00\x12(\n\x05regex\x18\x03 \x01(\x0b\x32\x17.summa.proto.RegexQueryH\x00\x12&\n\x04term\x18\x04 \x01(\x0b\x32\x16.summa.proto.TermQueryH\x00\x12*\n\x06phrase\x18\x05 \x01(\x0b\x32\x18.summa.proto.PhraseQueryH\x00\x12(\n\x05range\x18\x06 \x01(\x0b\x32\x17.summa.proto.RangeQueryH\x00\x12$\n\x03\x61ll\x18\x07 \x01(\x0b\x32\x15.summa.proto.AllQueryH\x00\x12\x38\n\x0emore_like_this\x18\x08 \x01(\x0b\x32\x1e.summa.proto.MoreLikeThisQueryH\x00\x12(\n\x05\x62oost\x18\t \x01(\x0b\x32\x17.summa.proto.BoostQueryH\x00\x12;\n\x0f\x64isjunction_max\x18\n \x01(\x0b\x32 .summa.proto.DisjunctionMaxQueryH\x00\x12(\n\x05\x65mpty\x18\x0b \x01(\x0b\x32\x17.summa.proto.EmptyQueryH\x00\x12*\n\x06\x65xists\x18\x0c \x01(\x0b\x32\x18.summa.proto.ExistsQueryH\x00\x42\x07\n\x05query\"\n\n\x08\x41llQuery\"\x0c\n\nEmptyQuery\">\n\nBoostQuery\x12!\n\x05query\x18\x01 \x01(\x0b\x32\x12.summa.proto.Query\x12\r\n\x05score\x18\x02 \x01(\t\"Q\n\x13\x44isjunctionMaxQuery\x12%\n\tdisjuncts\x18\x01 \x03(\x0b\x32\x12.summa.proto.Query\x12\x13\n\x0btie_breaker\x18\x02 \x01(\t\"\x91\x03\n\x11MoreLikeThisQuery\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12\x1e\n\x11min_doc_frequency\x18\x02 \x01(\x04H\x00\x88\x01\x01\x12\x1e\n\x11max_doc_frequency\x18\x03 \x01(\x04H\x01\x88\x01\x01\x12\x1f\n\x12min_term_frequency\x18\x04 \x01(\x04H\x02\x88\x01\x01\x12\x1c\n\x0fmax_query_terms\x18\x05 \x01(\x04H\x03\x88\x01\x01\x12\x1c\n\x0fmin_word_length\x18\x06 \x01(\x04H\x04\x88\x01\x01\x12\x1c\n\x0fmax_word_length\x18\x07 \x01(\x04H\x05\x88\x01\x01\x12\x12\n\x05\x62oost\x18\x08 \x01(\tH\x06\x88\x01\x01\x12\x12\n\nstop_words\x18\t \x03(\tB\x14\n\x12_min_doc_frequencyB\x14\n\x12_max_doc_frequencyB\x15\n\x13_min_term_frequencyB\x12\n\x10_max_query_termsB\x12\n\x10_min_word_lengthB\x12\n\x10_max_word_lengthB\x08\n\x06_boost\"9\n\x0bPhraseQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\x12\x0c\n\x04slop\x18\x03 \x01(\r\">\n\nRangeQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12!\n\x05value\x18\x02 \x01(\x0b\x32\x12.summa.proto.Range\"u\n\nMatchQuery\x12\r\n\x05value\x18\x01 \x01(\t\x12@\n\x13query_parser_config\x18\x02 \x01(\x0b\x32\x1e.summa.proto.QueryParserConfigH\x00\x88\x01\x01\x42\x16\n\x14_query_parser_config\"W\n\x0f\x42ooleanSubquery\x12!\n\x05occur\x18\x01 \x01(\x0e\x32\x12.summa.proto.Occur\x12!\n\x05query\x18\x02 \x01(\x0b\x32\x12.summa.proto.Query\"@\n\x0c\x42ooleanQuery\x12\x30\n\nsubqueries\x18\x01 \x03(\x0b\x32\x1c.summa.proto.BooleanSubquery\"*\n\nRegexQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\")\n\tTermQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\x1c\n\x0b\x45xistsQuery\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"\x80\x01\n\x0b\x41ggregation\x12\x30\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x1e.summa.proto.BucketAggregationH\x00\x12\x30\n\x06metric\x18\x02 \x01(\x0b\x32\x1e.summa.proto.MetricAggregationH\x00\x42\r\n\x0b\x61ggregation\"\xd7\x02\n\x11\x42ucketAggregation\x12.\n\x05range\x18\x01 \x01(\x0b\x32\x1d.summa.proto.RangeAggregationH\x00\x12\x36\n\thistogram\x18\x02 \x01(\x0b\x32!.summa.proto.HistogramAggregationH\x00\x12.\n\x05terms\x18\x03 \x01(\x0b\x32\x1d.summa.proto.TermsAggregationH\x00\x12K\n\x0fsub_aggregation\x18\x04 \x03(\x0b\x32\x32.summa.proto.BucketAggregation.SubAggregationEntry\x1aO\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.Aggregation:\x02\x38\x01\x42\x0c\n\nbucket_agg\"U\n\x10RangeAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x32\n\x06ranges\x18\x02 \x03(\x0b\x32\".summa.proto.RangeAggregationRange\"e\n\x15RangeAggregationRange\x12\x11\n\x04\x66rom\x18\x01 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02to\x18\x02 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03key\x18\x03 \x01(\tH\x02\x88\x01\x01\x42\x07\n\x05_fromB\x05\n\x03_toB\x06\n\x04_key\"\x9d\x02\n\x14HistogramAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x10\n\x08interval\x18\x02 \x01(\x01\x12\x13\n\x06offset\x18\x03 \x01(\x01H\x00\x88\x01\x01\x12\x1a\n\rmin_doc_count\x18\x04 \x01(\x04H\x01\x88\x01\x01\x12\x36\n\x0bhard_bounds\x18\x05 \x01(\x0b\x32\x1c.summa.proto.HistogramBoundsH\x02\x88\x01\x01\x12:\n\x0f\x65xtended_bounds\x18\x06 \x01(\x0b\x32\x1c.summa.proto.HistogramBoundsH\x03\x88\x01\x01\x42\t\n\x07_offsetB\x10\n\x0e_min_doc_countB\x0e\n\x0c_hard_boundsB\x12\n\x10_extended_bounds\"+\n\x0fHistogramBounds\x12\x0b\n\x03min\x18\x01 \x01(\x01\x12\x0b\n\x03max\x18\x02 \x01(\x01\"\xbd\x02\n\x10TermsAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x11\n\x04size\x18\x02 \x01(\rH\x00\x88\x01\x01\x12\x17\n\nsplit_size\x18\x03 \x01(\rH\x01\x88\x01\x01\x12\x19\n\x0csegment_size\x18\x04 \x01(\rH\x02\x88\x01\x01\x12&\n\x19show_term_doc_count_error\x18\x05 \x01(\x08H\x03\x88\x01\x01\x12\x1a\n\rmin_doc_count\x18\x06 \x01(\x04H\x04\x88\x01\x01\x12,\n\x05order\x18\x07 \x01(\x0b\x32\x18.summa.proto.CustomOrderH\x05\x88\x01\x01\x42\x07\n\x05_sizeB\r\n\x0b_split_sizeB\x0f\n\r_segment_sizeB\x1c\n\x1a_show_term_doc_count_errorB\x10\n\x0e_min_doc_countB\x08\n\x06_order\"\xa3\x01\n\x0b\x43ustomOrder\x12!\n\x03key\x18\x01 \x01(\x0b\x32\x12.summa.proto.EmptyH\x00\x12#\n\x05\x63ount\x18\x02 \x01(\x0b\x32\x12.summa.proto.EmptyH\x00\x12\x19\n\x0fsub_aggregation\x18\x03 \x01(\tH\x00\x12!\n\x05order\x18\x04 \x01(\x0e\x32\x12.summa.proto.OrderB\x0e\n\x0corder_target\"\x8d\x01\n\x11MetricAggregation\x12\x32\n\x07\x61verage\x18\x01 \x01(\x0b\x32\x1f.summa.proto.AverageAggregationH\x00\x12.\n\x05stats\x18\x02 \x01(\x0b\x32\x1d.summa.proto.StatsAggregationH\x00\x42\x14\n\x12metric_aggregation\"#\n\x12\x41verageAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"!\n\x10StatsAggregation\x12\r\n\x05\x66ield\x18\x01 \x01(\t\"\xdd\x01\n\x0b\x42ucketEntry\x12\x1d\n\x03key\x18\x01 \x01(\x0b\x32\x10.summa.proto.Key\x12\x11\n\tdoc_count\x18\x02 \x01(\x04\x12\x45\n\x0fsub_aggregation\x18\x03 \x03(\x0b\x32,.summa.proto.BucketEntry.SubAggregationEntry\x1aU\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\"*\n\x03Key\x12\r\n\x03str\x18\x01 \x01(\tH\x00\x12\r\n\x03\x66\x36\x34\x18\x02 \x01(\x01H\x00\x42\x05\n\x03key\"U\n\x05Range\x12\x0c\n\x04left\x18\x01 \x01(\t\x12\r\n\x05right\x18\x02 \x01(\t\x12\x16\n\x0eincluding_left\x18\x03 \x01(\x08\x12\x17\n\x0fincluding_right\x18\x04 \x01(\x08\"\x9b\x02\n\x10RangeBucketEntry\x12\x1d\n\x03key\x18\x01 \x01(\x0b\x32\x10.summa.proto.Key\x12\x11\n\tdoc_count\x18\x02 \x01(\x04\x12J\n\x0fsub_aggregation\x18\x03 \x03(\x0b\x32\x31.summa.proto.RangeBucketEntry.SubAggregationEntry\x12\x11\n\x04\x66rom\x18\x04 \x01(\x01H\x00\x88\x01\x01\x12\x0f\n\x02to\x18\x05 \x01(\x01H\x01\x88\x01\x01\x1aU\n\x13SubAggregationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\x42\x07\n\x05_fromB\x05\n\x03_to\":\n\x05Score\x12\x13\n\tf64_score\x18\x01 \x01(\x01H\x00\x12\x13\n\tu64_score\x18\x02 \x01(\x04H\x00\x42\x07\n\x05score\"%\n\tHighlight\x12\x0c\n\x04\x66rom\x18\x01 \x01(\r\x12\n\n\x02to\x18\x02 \x01(\r\"U\n\x07Snippet\x12\x10\n\x08\x66ragment\x18\x01 \x01(\x0c\x12*\n\nhighlights\x18\x02 \x03(\x0b\x32\x16.summa.proto.Highlight\x12\x0c\n\x04html\x18\x03 \x01(\t\"\xf0\x01\n\x0eScoredDocument\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12!\n\x05score\x18\x02 \x01(\x0b\x32\x12.summa.proto.Score\x12\x10\n\x08position\x18\x03 \x01(\r\x12;\n\x08snippets\x18\x04 \x03(\x0b\x32).summa.proto.ScoredDocument.SnippetsEntry\x12\x13\n\x0bindex_alias\x18\x05 \x01(\t\x1a\x45\n\rSnippetsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.summa.proto.Snippet:\x02\x38\x01\";\n\x06Scorer\x12\x13\n\teval_expr\x18\x01 \x01(\tH\x00\x12\x12\n\x08order_by\x18\x02 \x01(\tH\x00\x42\x08\n\x06scorer\"\xa8\x02\n\tCollector\x12\x31\n\x08top_docs\x18\x01 \x01(\x0b\x32\x1d.summa.proto.TopDocsCollectorH\x00\x12\x45\n\x12reservoir_sampling\x18\x02 \x01(\x0b\x32\'.summa.proto.ReservoirSamplingCollectorH\x00\x12,\n\x05\x63ount\x18\x03 \x01(\x0b\x32\x1b.summa.proto.CountCollectorH\x00\x12,\n\x05\x66\x61\x63\x65t\x18\x04 \x01(\x0b\x32\x1b.summa.proto.FacetCollectorH\x00\x12\x38\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32!.summa.proto.AggregationCollectorH\x00\x42\x0b\n\tcollector\"\x89\x02\n\x0f\x43ollectorOutput\x12:\n\tdocuments\x18\x01 \x01(\x0b\x32%.summa.proto.DocumentsCollectorOutputH\x00\x12\x32\n\x05\x63ount\x18\x03 \x01(\x0b\x32!.summa.proto.CountCollectorOutputH\x00\x12\x32\n\x05\x66\x61\x63\x65t\x18\x04 \x01(\x0b\x32!.summa.proto.FacetCollectorOutputH\x00\x12>\n\x0b\x61ggregation\x18\x05 \x01(\x0b\x32\'.summa.proto.AggregationCollectorOutputH\x00\x42\x12\n\x10\x63ollector_output\"\x10\n\x0e\x43ountCollector\"%\n\x14\x43ountCollectorOutput\x12\r\n\x05\x63ount\x18\x01 \x01(\r\"/\n\x0e\x46\x61\x63\x65tCollector\x12\r\n\x05\x66ield\x18\x01 \x01(\t\x12\x0e\n\x06\x66\x61\x63\x65ts\x18\x02 \x03(\t\"\x94\x01\n\x14\x46\x61\x63\x65tCollectorOutput\x12H\n\x0c\x66\x61\x63\x65t_counts\x18\x01 \x03(\x0b\x32\x32.summa.proto.FacetCollectorOutput.FacetCountsEntry\x1a\x32\n\x10\x46\x61\x63\x65tCountsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x04:\x02\x38\x01\";\n\x1aReservoirSamplingCollector\x12\r\n\x05limit\x18\x01 \x01(\r\x12\x0e\n\x06\x66ields\x18\x02 \x03(\t\"Z\n\x0eRandomDocument\x12\x10\n\x08\x64ocument\x18\x01 \x01(\t\x12!\n\x05score\x18\x02 \x01(\x0b\x32\x12.summa.proto.Score\x12\x13\n\x0bindex_alias\x18\x03 \x01(\t\"R\n ReservoirSamplingCollectorOutput\x12.\n\tdocuments\x18\x01 \x03(\x0b\x32\x1b.summa.proto.RandomDocument\"\x8a\x02\n\x10TopDocsCollector\x12\r\n\x05limit\x18\x01 \x01(\r\x12\x0e\n\x06offset\x18\x02 \x01(\r\x12(\n\x06scorer\x18\x03 \x01(\x0b\x32\x13.summa.proto.ScorerH\x00\x88\x01\x01\x12J\n\x0fsnippet_configs\x18\x04 \x03(\x0b\x32\x31.summa.proto.TopDocsCollector.SnippetConfigsEntry\x12\x0f\n\x07\x65xplain\x18\x05 \x01(\x08\x12\x0e\n\x06\x66ields\x18\x06 \x03(\t\x1a\x35\n\x13SnippetConfigsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\x42\t\n\x07_scorer\"c\n\x18\x44ocumentsCollectorOutput\x12\x35\n\x10scored_documents\x18\x01 \x03(\x0b\x32\x1b.summa.proto.ScoredDocument\x12\x10\n\x08has_next\x18\x02 \x01(\x08\"\xb0\x01\n\x14\x41ggregationCollector\x12I\n\x0c\x61ggregations\x18\x01 \x03(\x0b\x32\x33.summa.proto.AggregationCollector.AggregationsEntry\x1aM\n\x11\x41ggregationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.summa.proto.Aggregation:\x02\x38\x01\"\xd5\x01\n\x1a\x41ggregationCollectorOutput\x12\\\n\x13\x61ggregation_results\x18\x01 \x03(\x0b\x32?.summa.proto.AggregationCollectorOutput.AggregationResultsEntry\x1aY\n\x17\x41ggregationResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x1e.summa.proto.AggregationResult:\x02\x38\x01\"\x83\x01\n\x11\x41ggregationResult\x12+\n\x06\x62ucket\x18\x01 \x01(\x0b\x32\x19.summa.proto.BucketResultH\x00\x12+\n\x06metric\x18\x02 \x01(\x0b\x32\x19.summa.proto.MetricResultH\x00\x42\x14\n\x12\x61ggregation_result\"\xa8\x01\n\x0c\x42ucketResult\x12)\n\x05range\x18\x01 \x01(\x0b\x32\x18.summa.proto.RangeResultH\x00\x12\x31\n\thistogram\x18\x02 \x01(\x0b\x32\x1c.summa.proto.HistogramResultH\x00\x12)\n\x05terms\x18\x03 \x01(\x0b\x32\x18.summa.proto.TermsResultH\x00\x42\x0f\n\rbucket_result\"=\n\x0bRangeResult\x12.\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x1d.summa.proto.RangeBucketEntry\"<\n\x0fHistogramResult\x12)\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x18.summa.proto.BucketEntry\"\x9f\x01\n\x0bTermsResult\x12)\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\x18.summa.proto.BucketEntry\x12\x1b\n\x13sum_other_doc_count\x18\x02 \x01(\x04\x12(\n\x1b\x64oc_count_error_upper_bound\x18\x03 \x01(\x04H\x00\x88\x01\x01\x42\x1e\n\x1c_doc_count_error_upper_bound\"\x84\x01\n\x0cMetricResult\x12\x38\n\rsingle_metric\x18\x01 \x01(\x0b\x32\x1f.summa.proto.SingleMetricResultH\x00\x12)\n\x05stats\x18\x02 \x01(\x0b\x32\x18.summa.proto.StatsResultH\x00\x42\x0f\n\rmetric_result\"2\n\x12SingleMetricResult\x12\x12\n\x05value\x18\x01 \x01(\x01H\x00\x88\x01\x01\x42\x08\n\x06_value\"w\n\x0bStatsResult\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\x12\x0b\n\x03sum\x18\x02 \x01(\x01\x12\x10\n\x03min\x18\x03 \x01(\x01H\x00\x88\x01\x01\x12\x10\n\x03max\x18\x04 \x01(\x01H\x01\x88\x01\x01\x12\x10\n\x03\x61vg\x18\x05 \x01(\x01H\x02\x88\x01\x01\x42\x06\n\x04_minB\x06\n\x04_maxB\x06\n\x04_avg*<\n\x12MissingFieldPolicy\x12\x10\n\x0c\x41sUsualTerms\x10\x00\x12\n\n\x06Remove\x10\x01\x12\x08\n\x04\x46\x61il\x10\x02*+\n\x05Occur\x12\n\n\x06should\x10\x00\x12\x08\n\x04must\x10\x01\x12\x0c\n\x08must_not\x10\x02\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'query_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _MATCHQUERY_FIELDBOOSTSENTRY._options = None
-  _MATCHQUERY_FIELDBOOSTSENTRY._serialized_options = b'8\001'
+  _QUERYPARSERCONFIG_FIELDALIASESENTRY._options = None
+  _QUERYPARSERCONFIG_FIELDALIASESENTRY._serialized_options = b'8\001'
+  _QUERYPARSERCONFIG_FIELDBOOSTSENTRY._options = None
+  _QUERYPARSERCONFIG_FIELDBOOSTSENTRY._serialized_options = b'8\001'
+  _QUERYPARSERCONFIG_FIELDMAPPINGSENTRY._options = None
+  _QUERYPARSERCONFIG_FIELDMAPPINGSENTRY._serialized_options = b'8\001'
+  _QUERYPARSERCONFIG_INFLECTIONCONFIGSENTRY._options = None
+  _QUERYPARSERCONFIG_INFLECTIONCONFIGSENTRY._serialized_options = b'8\001'
   _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._options = None
   _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._serialized_options = b'8\001'
   _BUCKETENTRY_SUBAGGREGATIONENTRY._options = None
   _BUCKETENTRY_SUBAGGREGATIONENTRY._serialized_options = b'8\001'
   _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._options = None
   _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._serialized_options = b'8\001'
   _SCOREDDOCUMENT_SNIPPETSENTRY._options = None
@@ -35,146 +41,160 @@
   _FACETCOLLECTOROUTPUT_FACETCOUNTSENTRY._serialized_options = b'8\001'
   _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._options = None
   _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._serialized_options = b'8\001'
   _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._options = None
   _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._serialized_options = b'8\001'
   _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._options = None
   _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._serialized_options = b'8\001'
-  _OCCUR._serialized_start=7779
-  _OCCUR._serialized_end=7822
-  _SEARCHRESPONSE._serialized_start=41
-  _SEARCHRESPONSE._serialized_end=136
-  _QUERY._serialized_start=139
-  _QUERY._serialized_end=696
-  _ALLQUERY._serialized_start=698
-  _ALLQUERY._serialized_end=708
-  _EMPTYQUERY._serialized_start=710
-  _EMPTYQUERY._serialized_end=722
-  _BOOSTQUERY._serialized_start=724
-  _BOOSTQUERY._serialized_end=786
-  _DISJUNCTIONMAXQUERY._serialized_start=788
-  _DISJUNCTIONMAXQUERY._serialized_end=869
-  _MORELIKETHISQUERY._serialized_start=872
-  _MORELIKETHISQUERY._serialized_end=1273
-  _PHRASEQUERY._serialized_start=1275
-  _PHRASEQUERY._serialized_end=1332
-  _RANGEQUERY._serialized_start=1334
-  _RANGEQUERY._serialized_end=1396
-  _MATCHQUERYBOOLEANSHOULDMODE._serialized_start=1398
-  _MATCHQUERYBOOLEANSHOULDMODE._serialized_end=1427
-  _MATCHQUERYDISJUCTIONMAXMODE._serialized_start=1429
-  _MATCHQUERYDISJUCTIONMAXMODE._serialized_end=1479
-  _EXACTMATCHESPROMOTER._serialized_start=1481
-  _EXACTMATCHESPROMOTER._serialized_end=1547
-  _MATCHQUERY._serialized_start=1550
-  _MATCHQUERY._serialized_end=1946
-  _MATCHQUERY_FIELDBOOSTSENTRY._serialized_start=1880
-  _MATCHQUERY_FIELDBOOSTSENTRY._serialized_end=1930
-  _BOOLEANSUBQUERY._serialized_start=1948
-  _BOOLEANSUBQUERY._serialized_end=2035
-  _BOOLEANQUERY._serialized_start=2037
-  _BOOLEANQUERY._serialized_end=2101
-  _REGEXQUERY._serialized_start=2103
-  _REGEXQUERY._serialized_end=2145
-  _TERMQUERY._serialized_start=2147
-  _TERMQUERY._serialized_end=2188
-  _EXISTSQUERY._serialized_start=2190
-  _EXISTSQUERY._serialized_end=2218
-  _AGGREGATION._serialized_start=2221
-  _AGGREGATION._serialized_end=2349
-  _BUCKETAGGREGATION._serialized_start=2352
-  _BUCKETAGGREGATION._serialized_end=2695
-  _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._serialized_start=2602
-  _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._serialized_end=2681
-  _RANGEAGGREGATION._serialized_start=2697
-  _RANGEAGGREGATION._serialized_end=2782
-  _RANGEAGGREGATIONRANGE._serialized_start=2784
-  _RANGEAGGREGATIONRANGE._serialized_end=2885
-  _HISTOGRAMAGGREGATION._serialized_start=2888
-  _HISTOGRAMAGGREGATION._serialized_end=3173
-  _HISTOGRAMBOUNDS._serialized_start=3175
-  _HISTOGRAMBOUNDS._serialized_end=3218
-  _TERMSAGGREGATION._serialized_start=3221
-  _TERMSAGGREGATION._serialized_end=3538
-  _CUSTOMORDER._serialized_start=3541
-  _CUSTOMORDER._serialized_end=3704
-  _METRICAGGREGATION._serialized_start=3707
-  _METRICAGGREGATION._serialized_end=3848
-  _AVERAGEAGGREGATION._serialized_start=3850
-  _AVERAGEAGGREGATION._serialized_end=3885
-  _STATSAGGREGATION._serialized_start=3887
-  _STATSAGGREGATION._serialized_end=3920
-  _BUCKETENTRY._serialized_start=3923
-  _BUCKETENTRY._serialized_end=4144
-  _BUCKETENTRY_SUBAGGREGATIONENTRY._serialized_start=4059
-  _BUCKETENTRY_SUBAGGREGATIONENTRY._serialized_end=4144
-  _KEY._serialized_start=4146
-  _KEY._serialized_end=4188
-  _RANGE._serialized_start=4190
-  _RANGE._serialized_end=4275
-  _RANGEBUCKETENTRY._serialized_start=4278
-  _RANGEBUCKETENTRY._serialized_end=4561
-  _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._serialized_start=4059
-  _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._serialized_end=4144
-  _SCORE._serialized_start=4563
-  _SCORE._serialized_end=4621
-  _HIGHLIGHT._serialized_start=4623
-  _HIGHLIGHT._serialized_end=4660
-  _SNIPPET._serialized_start=4662
-  _SNIPPET._serialized_end=4747
-  _SCOREDDOCUMENT._serialized_start=4750
-  _SCOREDDOCUMENT._serialized_end=4990
-  _SCOREDDOCUMENT_SNIPPETSENTRY._serialized_start=4921
-  _SCOREDDOCUMENT_SNIPPETSENTRY._serialized_end=4990
-  _SCORER._serialized_start=4992
-  _SCORER._serialized_end=5051
-  _COLLECTOR._serialized_start=5054
-  _COLLECTOR._serialized_end=5350
-  _COLLECTOROUTPUT._serialized_start=5353
-  _COLLECTOROUTPUT._serialized_end=5618
-  _COUNTCOLLECTOR._serialized_start=5620
-  _COUNTCOLLECTOR._serialized_end=5636
-  _COUNTCOLLECTOROUTPUT._serialized_start=5638
-  _COUNTCOLLECTOROUTPUT._serialized_end=5675
-  _FACETCOLLECTOR._serialized_start=5677
-  _FACETCOLLECTOR._serialized_end=5724
-  _FACETCOLLECTOROUTPUT._serialized_start=5727
-  _FACETCOLLECTOROUTPUT._serialized_end=5875
-  _FACETCOLLECTOROUTPUT_FACETCOUNTSENTRY._serialized_start=5825
-  _FACETCOLLECTOROUTPUT_FACETCOUNTSENTRY._serialized_end=5875
-  _RESERVOIRSAMPLINGCOLLECTOR._serialized_start=5877
-  _RESERVOIRSAMPLINGCOLLECTOR._serialized_end=5936
-  _RANDOMDOCUMENT._serialized_start=5938
-  _RANDOMDOCUMENT._serialized_end=6028
-  _RESERVOIRSAMPLINGCOLLECTOROUTPUT._serialized_start=6030
-  _RESERVOIRSAMPLINGCOLLECTOROUTPUT._serialized_end=6112
-  _TOPDOCSCOLLECTOR._serialized_start=6115
-  _TOPDOCSCOLLECTOR._serialized_end=6381
-  _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._serialized_start=6317
-  _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._serialized_end=6370
-  _DOCUMENTSCOLLECTOROUTPUT._serialized_start=6383
-  _DOCUMENTSCOLLECTOROUTPUT._serialized_end=6482
-  _AGGREGATIONCOLLECTOR._serialized_start=6485
-  _AGGREGATIONCOLLECTOR._serialized_end=6661
-  _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._serialized_start=6584
-  _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._serialized_end=6661
-  _AGGREGATIONCOLLECTOROUTPUT._serialized_start=6664
-  _AGGREGATIONCOLLECTOROUTPUT._serialized_end=6877
-  _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._serialized_start=6788
-  _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._serialized_end=6877
-  _AGGREGATIONRESULT._serialized_start=6880
-  _AGGREGATIONRESULT._serialized_end=7011
-  _BUCKETRESULT._serialized_start=7014
-  _BUCKETRESULT._serialized_end=7182
-  _RANGERESULT._serialized_start=7184
-  _RANGERESULT._serialized_end=7245
-  _HISTOGRAMRESULT._serialized_start=7247
-  _HISTOGRAMRESULT._serialized_end=7307
-  _TERMSRESULT._serialized_start=7310
-  _TERMSRESULT._serialized_end=7469
-  _METRICRESULT._serialized_start=7472
-  _METRICRESULT._serialized_end=7604
-  _SINGLEMETRICRESULT._serialized_start=7606
-  _SINGLEMETRICRESULT._serialized_end=7656
-  _STATSRESULT._serialized_start=7658
-  _STATSRESULT._serialized_end=7777
+  _MISSINGFIELDPOLICY._serialized_start=8528
+  _MISSINGFIELDPOLICY._serialized_end=8588
+  _OCCUR._serialized_start=8590
+  _OCCUR._serialized_end=8633
+  _FIELDMAPPER._serialized_start=41
+  _FIELDMAPPER._serialized_end=91
+  _MATCHQUERYBOOLEANSHOULDMODE._serialized_start=93
+  _MATCHQUERYBOOLEANSHOULDMODE._serialized_end=122
+  _MATCHQUERYDISJUCTIONMAXMODE._serialized_start=124
+  _MATCHQUERYDISJUCTIONMAXMODE._serialized_end=174
+  _EXACTMATCHESPROMOTER._serialized_start=176
+  _EXACTMATCHESPROMOTER._serialized_end=242
+  _INFLECTIONCONFIG._serialized_start=244
+  _INFLECTIONCONFIG._serialized_end=285
+  _QUERYPARSERCONFIG._serialized_start=288
+  _QUERYPARSERCONFIG._serialized_end=1219
+  _QUERYPARSERCONFIG_FIELDALIASESENTRY._serialized_start=931
+  _QUERYPARSERCONFIG_FIELDALIASESENTRY._serialized_end=982
+  _QUERYPARSERCONFIG_FIELDBOOSTSENTRY._serialized_start=984
+  _QUERYPARSERCONFIG_FIELDBOOSTSENTRY._serialized_end=1034
+  _QUERYPARSERCONFIG_FIELDMAPPINGSENTRY._serialized_start=1036
+  _QUERYPARSERCONFIG_FIELDMAPPINGSENTRY._serialized_end=1114
+  _QUERYPARSERCONFIG_INFLECTIONCONFIGSENTRY._serialized_start=1116
+  _QUERYPARSERCONFIG_INFLECTIONCONFIGSENTRY._serialized_end=1203
+  _SEARCHRESPONSE._serialized_start=1221
+  _SEARCHRESPONSE._serialized_end=1316
+  _QUERY._serialized_start=1319
+  _QUERY._serialized_end=1876
+  _ALLQUERY._serialized_start=1878
+  _ALLQUERY._serialized_end=1888
+  _EMPTYQUERY._serialized_start=1890
+  _EMPTYQUERY._serialized_end=1902
+  _BOOSTQUERY._serialized_start=1904
+  _BOOSTQUERY._serialized_end=1966
+  _DISJUNCTIONMAXQUERY._serialized_start=1968
+  _DISJUNCTIONMAXQUERY._serialized_end=2049
+  _MORELIKETHISQUERY._serialized_start=2052
+  _MORELIKETHISQUERY._serialized_end=2453
+  _PHRASEQUERY._serialized_start=2455
+  _PHRASEQUERY._serialized_end=2512
+  _RANGEQUERY._serialized_start=2514
+  _RANGEQUERY._serialized_end=2576
+  _MATCHQUERY._serialized_start=2578
+  _MATCHQUERY._serialized_end=2695
+  _BOOLEANSUBQUERY._serialized_start=2697
+  _BOOLEANSUBQUERY._serialized_end=2784
+  _BOOLEANQUERY._serialized_start=2786
+  _BOOLEANQUERY._serialized_end=2850
+  _REGEXQUERY._serialized_start=2852
+  _REGEXQUERY._serialized_end=2894
+  _TERMQUERY._serialized_start=2896
+  _TERMQUERY._serialized_end=2937
+  _EXISTSQUERY._serialized_start=2939
+  _EXISTSQUERY._serialized_end=2967
+  _AGGREGATION._serialized_start=2970
+  _AGGREGATION._serialized_end=3098
+  _BUCKETAGGREGATION._serialized_start=3101
+  _BUCKETAGGREGATION._serialized_end=3444
+  _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._serialized_start=3351
+  _BUCKETAGGREGATION_SUBAGGREGATIONENTRY._serialized_end=3430
+  _RANGEAGGREGATION._serialized_start=3446
+  _RANGEAGGREGATION._serialized_end=3531
+  _RANGEAGGREGATIONRANGE._serialized_start=3533
+  _RANGEAGGREGATIONRANGE._serialized_end=3634
+  _HISTOGRAMAGGREGATION._serialized_start=3637
+  _HISTOGRAMAGGREGATION._serialized_end=3922
+  _HISTOGRAMBOUNDS._serialized_start=3924
+  _HISTOGRAMBOUNDS._serialized_end=3967
+  _TERMSAGGREGATION._serialized_start=3970
+  _TERMSAGGREGATION._serialized_end=4287
+  _CUSTOMORDER._serialized_start=4290
+  _CUSTOMORDER._serialized_end=4453
+  _METRICAGGREGATION._serialized_start=4456
+  _METRICAGGREGATION._serialized_end=4597
+  _AVERAGEAGGREGATION._serialized_start=4599
+  _AVERAGEAGGREGATION._serialized_end=4634
+  _STATSAGGREGATION._serialized_start=4636
+  _STATSAGGREGATION._serialized_end=4669
+  _BUCKETENTRY._serialized_start=4672
+  _BUCKETENTRY._serialized_end=4893
+  _BUCKETENTRY_SUBAGGREGATIONENTRY._serialized_start=4808
+  _BUCKETENTRY_SUBAGGREGATIONENTRY._serialized_end=4893
+  _KEY._serialized_start=4895
+  _KEY._serialized_end=4937
+  _RANGE._serialized_start=4939
+  _RANGE._serialized_end=5024
+  _RANGEBUCKETENTRY._serialized_start=5027
+  _RANGEBUCKETENTRY._serialized_end=5310
+  _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._serialized_start=4808
+  _RANGEBUCKETENTRY_SUBAGGREGATIONENTRY._serialized_end=4893
+  _SCORE._serialized_start=5312
+  _SCORE._serialized_end=5370
+  _HIGHLIGHT._serialized_start=5372
+  _HIGHLIGHT._serialized_end=5409
+  _SNIPPET._serialized_start=5411
+  _SNIPPET._serialized_end=5496
+  _SCOREDDOCUMENT._serialized_start=5499
+  _SCOREDDOCUMENT._serialized_end=5739
+  _SCOREDDOCUMENT_SNIPPETSENTRY._serialized_start=5670
+  _SCOREDDOCUMENT_SNIPPETSENTRY._serialized_end=5739
+  _SCORER._serialized_start=5741
+  _SCORER._serialized_end=5800
+  _COLLECTOR._serialized_start=5803
+  _COLLECTOR._serialized_end=6099
+  _COLLECTOROUTPUT._serialized_start=6102
+  _COLLECTOROUTPUT._serialized_end=6367
+  _COUNTCOLLECTOR._serialized_start=6369
+  _COUNTCOLLECTOR._serialized_end=6385
+  _COUNTCOLLECTOROUTPUT._serialized_start=6387
+  _COUNTCOLLECTOROUTPUT._serialized_end=6424
+  _FACETCOLLECTOR._serialized_start=6426
+  _FACETCOLLECTOR._serialized_end=6473
+  _FACETCOLLECTOROUTPUT._serialized_start=6476
+  _FACETCOLLECTOROUTPUT._serialized_end=6624
+  _FACETCOLLECTOROUTPUT_FACETCOUNTSENTRY._serialized_start=6574
+  _FACETCOLLECTOROUTPUT_FACETCOUNTSENTRY._serialized_end=6624
+  _RESERVOIRSAMPLINGCOLLECTOR._serialized_start=6626
+  _RESERVOIRSAMPLINGCOLLECTOR._serialized_end=6685
+  _RANDOMDOCUMENT._serialized_start=6687
+  _RANDOMDOCUMENT._serialized_end=6777
+  _RESERVOIRSAMPLINGCOLLECTOROUTPUT._serialized_start=6779
+  _RESERVOIRSAMPLINGCOLLECTOROUTPUT._serialized_end=6861
+  _TOPDOCSCOLLECTOR._serialized_start=6864
+  _TOPDOCSCOLLECTOR._serialized_end=7130
+  _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._serialized_start=7066
+  _TOPDOCSCOLLECTOR_SNIPPETCONFIGSENTRY._serialized_end=7119
+  _DOCUMENTSCOLLECTOROUTPUT._serialized_start=7132
+  _DOCUMENTSCOLLECTOROUTPUT._serialized_end=7231
+  _AGGREGATIONCOLLECTOR._serialized_start=7234
+  _AGGREGATIONCOLLECTOR._serialized_end=7410
+  _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._serialized_start=7333
+  _AGGREGATIONCOLLECTOR_AGGREGATIONSENTRY._serialized_end=7410
+  _AGGREGATIONCOLLECTOROUTPUT._serialized_start=7413
+  _AGGREGATIONCOLLECTOROUTPUT._serialized_end=7626
+  _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._serialized_start=7537
+  _AGGREGATIONCOLLECTOROUTPUT_AGGREGATIONRESULTSENTRY._serialized_end=7626
+  _AGGREGATIONRESULT._serialized_start=7629
+  _AGGREGATIONRESULT._serialized_end=7760
+  _BUCKETRESULT._serialized_start=7763
+  _BUCKETRESULT._serialized_end=7931
+  _RANGERESULT._serialized_start=7933
+  _RANGERESULT._serialized_end=7994
+  _HISTOGRAMRESULT._serialized_start=7996
+  _HISTOGRAMRESULT._serialized_end=8056
+  _TERMSRESULT._serialized_start=8059
+  _TERMSRESULT._serialized_end=8218
+  _METRICRESULT._serialized_start=8221
+  _METRICRESULT._serialized_end=8353
+  _SINGLEMETRICRESULT._serialized_start=8355
+  _SINGLEMETRICRESULT._serialized_end=8405
+  _STATSRESULT._serialized_start=8407
+  _STATSRESULT._serialized_end=8526
 # @@protoc_insertion_point(module_scope)
```

### Comparing `summa_embed-0.15.9/summa_embed/proto/query_pb2.pyi` & `summa_embed-0.16.0/summa_embed/proto/query_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 
 import utils_pb2 as _utils_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 
+AsUsualTerms: MissingFieldPolicy
 DESCRIPTOR: _descriptor.FileDescriptor
+Fail: MissingFieldPolicy
+Remove: MissingFieldPolicy
 must: Occur
 must_not: Occur
 should: Occur
 
 class Aggregation(_message.Message):
     __slots__ = ["bucket", "metric"]
     BUCKET_FIELD_NUMBER: _ClassVar[int]
@@ -234,14 +237,22 @@
         key: str
         value: int
         def __init__(self, key: _Optional[str] = ..., value: _Optional[int] = ...) -> None: ...
     FACET_COUNTS_FIELD_NUMBER: _ClassVar[int]
     facet_counts: _containers.ScalarMap[str, int]
     def __init__(self, facet_counts: _Optional[_Mapping[str, int]] = ...) -> None: ...
 
+class FieldMapper(_message.Message):
+    __slots__ = ["fields", "mapper_name"]
+    FIELDS_FIELD_NUMBER: _ClassVar[int]
+    MAPPER_NAME_FIELD_NUMBER: _ClassVar[int]
+    fields: _containers.RepeatedScalarFieldContainer[str]
+    mapper_name: str
+    def __init__(self, mapper_name: _Optional[str] = ..., fields: _Optional[_Iterable[str]] = ...) -> None: ...
+
 class Highlight(_message.Message):
     __slots__ = ["to"]
     FROM_FIELD_NUMBER: _ClassVar[int]
     TO_FIELD_NUMBER: _ClassVar[int]
     to: int
     def __init__(self, to: _Optional[int] = ..., **kwargs) -> None: ...
 
@@ -271,44 +282,35 @@
 
 class HistogramResult(_message.Message):
     __slots__ = ["buckets"]
     BUCKETS_FIELD_NUMBER: _ClassVar[int]
     buckets: _containers.RepeatedCompositeFieldContainer[BucketEntry]
     def __init__(self, buckets: _Optional[_Iterable[_Union[BucketEntry, _Mapping]]] = ...) -> None: ...
 
+class InflectionConfig(_message.Message):
+    __slots__ = ["derive_plural"]
+    DERIVE_PLURAL_FIELD_NUMBER: _ClassVar[int]
+    derive_plural: bool
+    def __init__(self, derive_plural: bool = ...) -> None: ...
+
 class Key(_message.Message):
     __slots__ = ["f64", "str"]
     F64_FIELD_NUMBER: _ClassVar[int]
     STR_FIELD_NUMBER: _ClassVar[int]
     f64: float
     str: str
     def __init__(self, str: _Optional[str] = ..., f64: _Optional[float] = ...) -> None: ...
 
 class MatchQuery(_message.Message):
-    __slots__ = ["boolean_should_mode", "default_fields", "disjuction_max_mode", "exact_matches_promoter", "field_boosts", "value"]
-    class FieldBoostsEntry(_message.Message):
-        __slots__ = ["key", "value"]
-        KEY_FIELD_NUMBER: _ClassVar[int]
-        VALUE_FIELD_NUMBER: _ClassVar[int]
-        key: str
-        value: float
-        def __init__(self, key: _Optional[str] = ..., value: _Optional[float] = ...) -> None: ...
-    BOOLEAN_SHOULD_MODE_FIELD_NUMBER: _ClassVar[int]
-    DEFAULT_FIELDS_FIELD_NUMBER: _ClassVar[int]
-    DISJUCTION_MAX_MODE_FIELD_NUMBER: _ClassVar[int]
-    EXACT_MATCHES_PROMOTER_FIELD_NUMBER: _ClassVar[int]
-    FIELD_BOOSTS_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["query_parser_config", "value"]
+    QUERY_PARSER_CONFIG_FIELD_NUMBER: _ClassVar[int]
     VALUE_FIELD_NUMBER: _ClassVar[int]
-    boolean_should_mode: MatchQueryBooleanShouldMode
-    default_fields: _containers.RepeatedScalarFieldContainer[str]
-    disjuction_max_mode: MatchQueryDisjuctionMaxMode
-    exact_matches_promoter: ExactMatchesPromoter
-    field_boosts: _containers.ScalarMap[str, float]
+    query_parser_config: QueryParserConfig
     value: str
-    def __init__(self, value: _Optional[str] = ..., default_fields: _Optional[_Iterable[str]] = ..., boolean_should_mode: _Optional[_Union[MatchQueryBooleanShouldMode, _Mapping]] = ..., disjuction_max_mode: _Optional[_Union[MatchQueryDisjuctionMaxMode, _Mapping]] = ..., field_boosts: _Optional[_Mapping[str, float]] = ..., exact_matches_promoter: _Optional[_Union[ExactMatchesPromoter, _Mapping]] = ...) -> None: ...
+    def __init__(self, value: _Optional[str] = ..., query_parser_config: _Optional[_Union[QueryParserConfig, _Mapping]] = ...) -> None: ...
 
 class MatchQueryBooleanShouldMode(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class MatchQueryDisjuctionMaxMode(_message.Message):
     __slots__ = ["tie_breaker"]
@@ -388,14 +390,66 @@
     more_like_this: MoreLikeThisQuery
     phrase: PhraseQuery
     range: RangeQuery
     regex: RegexQuery
     term: TermQuery
     def __init__(self, boolean: _Optional[_Union[BooleanQuery, _Mapping]] = ..., match: _Optional[_Union[MatchQuery, _Mapping]] = ..., regex: _Optional[_Union[RegexQuery, _Mapping]] = ..., term: _Optional[_Union[TermQuery, _Mapping]] = ..., phrase: _Optional[_Union[PhraseQuery, _Mapping]] = ..., range: _Optional[_Union[RangeQuery, _Mapping]] = ..., all: _Optional[_Union[AllQuery, _Mapping]] = ..., more_like_this: _Optional[_Union[MoreLikeThisQuery, _Mapping]] = ..., boost: _Optional[_Union[BoostQuery, _Mapping]] = ..., disjunction_max: _Optional[_Union[DisjunctionMaxQuery, _Mapping]] = ..., empty: _Optional[_Union[EmptyQuery, _Mapping]] = ..., exists: _Optional[_Union[ExistsQuery, _Mapping]] = ...) -> None: ...
 
+class QueryParserConfig(_message.Message):
+    __slots__ = ["boolean_should_mode", "default_fields", "disjuction_max_mode", "exact_matches_promoter", "field_aliases", "field_boosts", "field_mappings", "inflection_configs", "missing_field_policy", "term_limit"]
+    class FieldAliasesEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    class FieldBoostsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: float
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[float] = ...) -> None: ...
+    class FieldMappingsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: FieldMapper
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[FieldMapper, _Mapping]] = ...) -> None: ...
+    class InflectionConfigsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: InflectionConfig
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[InflectionConfig, _Mapping]] = ...) -> None: ...
+    BOOLEAN_SHOULD_MODE_FIELD_NUMBER: _ClassVar[int]
+    DEFAULT_FIELDS_FIELD_NUMBER: _ClassVar[int]
+    DISJUCTION_MAX_MODE_FIELD_NUMBER: _ClassVar[int]
+    EXACT_MATCHES_PROMOTER_FIELD_NUMBER: _ClassVar[int]
+    FIELD_ALIASES_FIELD_NUMBER: _ClassVar[int]
+    FIELD_BOOSTS_FIELD_NUMBER: _ClassVar[int]
+    FIELD_MAPPINGS_FIELD_NUMBER: _ClassVar[int]
+    INFLECTION_CONFIGS_FIELD_NUMBER: _ClassVar[int]
+    MISSING_FIELD_POLICY_FIELD_NUMBER: _ClassVar[int]
+    TERM_LIMIT_FIELD_NUMBER: _ClassVar[int]
+    boolean_should_mode: MatchQueryBooleanShouldMode
+    default_fields: _containers.RepeatedScalarFieldContainer[str]
+    disjuction_max_mode: MatchQueryDisjuctionMaxMode
+    exact_matches_promoter: ExactMatchesPromoter
+    field_aliases: _containers.ScalarMap[str, str]
+    field_boosts: _containers.ScalarMap[str, float]
+    field_mappings: _containers.MessageMap[str, FieldMapper]
+    inflection_configs: _containers.MessageMap[str, InflectionConfig]
+    missing_field_policy: MissingFieldPolicy
+    term_limit: int
+    def __init__(self, field_aliases: _Optional[_Mapping[str, str]] = ..., field_boosts: _Optional[_Mapping[str, float]] = ..., field_mappings: _Optional[_Mapping[str, FieldMapper]] = ..., term_limit: _Optional[int] = ..., default_fields: _Optional[_Iterable[str]] = ..., boolean_should_mode: _Optional[_Union[MatchQueryBooleanShouldMode, _Mapping]] = ..., disjuction_max_mode: _Optional[_Union[MatchQueryDisjuctionMaxMode, _Mapping]] = ..., exact_matches_promoter: _Optional[_Union[ExactMatchesPromoter, _Mapping]] = ..., missing_field_policy: _Optional[_Union[MissingFieldPolicy, str]] = ..., inflection_configs: _Optional[_Mapping[str, InflectionConfig]] = ...) -> None: ...
+
 class RandomDocument(_message.Message):
     __slots__ = ["document", "index_alias", "score"]
     DOCUMENT_FIELD_NUMBER: _ClassVar[int]
     INDEX_ALIAS_FIELD_NUMBER: _ClassVar[int]
     SCORE_FIELD_NUMBER: _ClassVar[int]
     document: str
     index_alias: str
@@ -623,9 +677,12 @@
     fields: _containers.RepeatedScalarFieldContainer[str]
     limit: int
     offset: int
     scorer: Scorer
     snippet_configs: _containers.ScalarMap[str, int]
     def __init__(self, limit: _Optional[int] = ..., offset: _Optional[int] = ..., scorer: _Optional[_Union[Scorer, _Mapping]] = ..., snippet_configs: _Optional[_Mapping[str, int]] = ..., explain: bool = ..., fields: _Optional[_Iterable[str]] = ...) -> None: ...
 
+class MissingFieldPolicy(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
+
 class Occur(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
```

### Comparing `summa_embed-0.15.9/summa_embed/proto/reflection_service_pb2.py` & `summa_embed-0.16.0/summa_embed/proto/reflection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/summa_embed/proto/reflection_service_pb2.pyi` & `summa_embed-0.16.0/summa_embed/proto/reflection_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/summa_embed/proto/search_service_pb2.py` & `summa_embed-0.16.0/summa_embed/proto/search_service_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/summa_embed/proto/search_service_pb2.pyi` & `summa_embed-0.16.0/summa_embed/proto/search_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/summa_embed/proto/unixfs_pb2.py` & `summa_embed-0.16.0/summa_embed/proto/unixfs_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/summa_embed/proto/unixfs_pb2.pyi` & `summa_embed-0.16.0/summa_embed/proto/unixfs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/summa_embed/proto/utils_pb2.py` & `summa_embed-0.16.0/summa_embed/proto/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `summa_embed-0.15.9/Cargo.lock` & `summa_embed-0.16.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
  "cfg-if",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
 version = "0.3.2"
@@ -367,26 +367,26 @@
  "multihash 0.18.1",
  "serde",
  "unsigned-varint",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.0"
+version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93aae7a4192245f70fe75dd9157fc7b4a5bf53e88d30bd4396f7d8f9284d5acc"
+checksum = "401a4694d2bf92537b6867d94de48c4842089645fdcdf6c71865b175d836e9c2"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.0"
+version = "4.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f423e341edefb78c9caba2d9c7f7687d0e72e89df3ce3394554754393ac3990"
+checksum = "72394f3339a76daf211e57d4bcb374410f3965dcc606dd0e03738c7888766980"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "once_cell",
  "strsim",
@@ -591,15 +591,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
 dependencies = [
  "cfg-if",
  "hashbrown 0.12.3",
  "lock_api",
  "once_cell",
- "parking_lot_core 0.9.7",
+ "parking_lot_core 0.9.8",
 ]
 
 [[package]]
 name = "data-encoding"
 version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
@@ -711,15 +711,15 @@
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
 name = "examples"
 version = "0.0.0"
 dependencies = [
  "serde_json",
- "summa-proto 0.26.0",
+ "summa-proto 0.27.0",
  "tokio",
  "tonic 0.9.2",
 ]
 
 [[package]]
 name = "fail"
 version = "0.5.1"
@@ -978,17 +978,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -1235,15 +1235,15 @@
  "minicbor",
  "multihash 0.18.1",
  "prost",
  "rayon",
  "rust-unixfs",
  "serde_json",
  "sled",
- "summa-proto 0.26.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "summa-proto 0.26.0",
  "unsigned-varint",
 ]
 
 [[package]]
 name = "ipfs-hamt-directory-py"
 version = "0.1.1"
 dependencies = [
@@ -1339,17 +1339,17 @@
 name = "levenshtein_automata"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2cdeb66e45e9f36bfad5bbdb4d2384e70936afbee843c6f6543f0c551ebb25"
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "libipld"
 version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a20e38e0ad9a2fd600476691fa0780421931a198279985e398a3a0851903e1b2"
 dependencies = [
@@ -1457,23 +1457,29 @@
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "lockfree-object-pool"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee33defb27b106378a6efcfcde4dda6226dfdac8ba7a2904f5bc93363cb88557"
+
+[[package]]
 name = "log"
 version = "0.4.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
 
 [[package]]
 name = "loom"
@@ -1743,32 +1749,32 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.2"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oneshot"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc22d22931513428ea6cc089e942d38600e3d00976eef8c86de6b8a3aadec6eb"
 dependencies = [
  "loom",
 ]
 
 [[package]]
 name = "openssl"
-version = "0.10.53"
+version = "0.10.54"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12df40a956736488b7b44fe79fe12d4f245bb5b3f5a1f6095e499760015be392"
+checksum = "69b3f656a17a6cbc115b5c7a40c616947d213ba182135b014d6051b73ab6f019"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
@@ -1888,15 +1894,15 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "ownedbytes"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "parking_lot"
 version = "0.11.2"
@@ -1911,15 +1917,15 @@
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core 0.9.7",
+ "parking_lot_core 0.9.8",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
@@ -1930,23 +1936,23 @@
  "redox_syscall 0.2.16",
  "smallvec",
  "winapi",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall 0.2.16",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "path-absolutize"
 version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43eb3595c63a214e1b37b44f44b0a84900ef7ae0b4c5efce59e123d246d7a0de"
@@ -1967,17 +1973,17 @@
 name = "pathdiff"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8835116a5c179084a830efb3adc117ab007512b535bc1a21c991d3b32a6b44dd"
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pest"
 version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e68e84bfb01f0507134eac1e9b410a12ba379d064eab48c50ba4ce329a527b70"
 dependencies = [
@@ -2064,14 +2070,25 @@
 [[package]]
 name = "pkg-config"
 version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
+name = "pluralize-rs"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "003d04a126ec3708d3aa5721101e3554ac224fd2e764f381063d4e64ee6c53ef"
+dependencies = [
+ "lazy_static",
+ "regex",
+ "voca_rs",
+]
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "prettyplease"
@@ -2115,17 +2132,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "prometheus"
 version = "0.13.3"
@@ -2311,14 +2328,25 @@
 checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
+name = "pyo3-log"
+version = "0.8.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c94ff6535a6bae58d7d0b85e60d4c53f7f84d0d0aa35d6a28c3f3e70bfe51444"
+dependencies = [
+ "arc-swap",
+ "log",
+ "pyo3",
+]
+
+[[package]]
 name = "pyo3-macros"
 version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
@@ -2334,24 +2362,14 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
-name = "pythonize"
-version = "0.18.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a0e1bbcd2a3856284bf4f4ef09ccb1157e9467847792754556f153ea3fe6b42"
-dependencies = [
- "pyo3",
- "serde",
-]
-
-[[package]]
 name = "quick-protobuf"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d6da84cc204722a989e01ba2f6e1e276e190f22263d0cb6ce8526fcdb0d2e1f"
 dependencies = [
  "byteorder",
 ]
@@ -2506,18 +2524,20 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.3"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
+ "aho-corasick",
+ "memchr",
  "regex-syntax 0.7.2",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2629,61 +2649,14 @@
 [[package]]
 name = "ryu"
 version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
-name = "safe-proc-macro2"
-version = "1.0.36"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "814c536dcd27acf03296c618dab7ad62d28e70abd7ba41d3f34a2ce707a2c666"
-dependencies = [
- "unicode-xid",
-]
-
-[[package]]
-name = "safe-quote"
-version = "1.0.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77e530f7831f3feafcd5f1aae406ac205dd998436b4007c8e80f03eca78a88f7"
-dependencies = [
- "safe-proc-macro2",
-]
-
-[[package]]
-name = "safe-regex"
-version = "0.2.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a15289bf322e0673d52756a18194167f2378ec1a15fe884af6e2d2cb934822b0"
-dependencies = [
- "safe-regex-macro",
-]
-
-[[package]]
-name = "safe-regex-compiler"
-version = "0.2.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fba76fae590a2aa665279deb1f57b5098cbace01a0c5e60e262fcf55f7c51542"
-dependencies = [
- "safe-proc-macro2",
- "safe-quote",
-]
-
-[[package]]
-name = "safe-regex-macro"
-version = "0.2.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96c2e96b5c03f158d1b16ba79af515137795f4ad4e8de3f790518aae91f1d127"
-dependencies = [
- "safe-proc-macro2",
- "safe-regex-compiler",
-]
-
-[[package]]
 name = "schannel"
 version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
 dependencies = [
  "windows-sys 0.42.0",
 ]
@@ -2721,17 +2694,17 @@
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.5.0"
@@ -2760,17 +2733,17 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
@@ -2899,28 +2872,38 @@
 [[package]]
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
 
 [[package]]
+name = "stfu8"
+version = "0.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1310970b29733b601839578f8ba24991a97057dbedc4ac0decea835474054ee7"
+dependencies = [
+ "lazy_static",
+ "regex",
+]
+
+[[package]]
 name = "strfmt"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a8348af2d9fc3258c8733b8d9d8db2e56f54b2363a4b5b81585c7875ed65e65"
 
 [[package]]
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.15.9"
+version = "0.16.0"
 dependencies = [
  "anyhow",
  "async-trait",
  "base64 0.21.2",
  "bytes",
  "config",
  "derive_builder",
@@ -2934,86 +2917,87 @@
  "lru",
  "matches",
  "oneshot",
  "opentelemetry",
  "parking_lot 0.12.1",
  "pest",
  "pest_derive",
+ "pluralize-rs",
  "prost",
  "rand 0.8.5",
  "rayon",
+ "regex",
  "rustc-hash",
- "safe-regex",
  "serde",
  "serde_bytes",
  "serde_cbor",
  "serde_json",
  "serde_yaml",
  "strfmt",
- "summa-proto 0.26.0",
+ "summa-proto 0.27.0",
  "take_mut",
  "tantivy",
  "tantivy-common",
  "tantivy-query-grammar",
  "thiserror",
  "time",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.15.9"
+version = "0.16.0"
 dependencies = [
  "futures",
  "prost",
  "pyo3",
  "pyo3-asyncio",
- "pythonize",
+ "pyo3-log",
  "serde_json",
  "summa-core",
- "summa-proto 0.26.0",
+ "summa-proto 0.27.0",
  "tantivy",
  "tokio",
 ]
 
 [[package]]
 name = "summa-proto"
 version = "0.26.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "11800e4c382bb5e8b6756e4fcaeb37a966e75f9c9796912e5066799587d81d00"
 dependencies = [
  "prost",
  "prost-build",
  "prost-types",
  "protoc-bin-vendored",
  "serde",
- "tokio",
- "tonic 0.9.2",
- "tonic-build 0.9.2",
- "tonic-reflection 0.9.2",
+ "tonic 0.8.3",
+ "tonic-build 0.8.4",
+ "tonic-reflection 0.6.0",
 ]
 
 [[package]]
 name = "summa-proto"
-version = "0.26.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11800e4c382bb5e8b6756e4fcaeb37a966e75f9c9796912e5066799587d81d00"
+version = "0.27.0"
 dependencies = [
  "prost",
  "prost-build",
  "prost-types",
  "protoc-bin-vendored",
  "serde",
- "tonic 0.8.3",
- "tonic-build 0.8.4",
- "tonic-reflection 0.6.0",
+ "tokio",
+ "tonic 0.9.2",
+ "tonic-build 0.9.2",
+ "tonic-reflection 0.9.2",
 ]
 
 [[package]]
 name = "summa-server"
-version = "0.15.0"
+version = "0.16.0"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "clap",
  "config",
  "derive_builder",
@@ -3033,15 +3017,15 @@
  "rdkafka",
  "rlimit",
  "serde",
  "serde_derive",
  "serde_json",
  "serde_yaml",
  "summa-core",
- "summa-proto 0.26.0",
+ "summa-proto 0.27.0",
  "take_mut",
  "tantivy",
  "tantivy-fst",
  "tempdir",
  "thiserror",
  "tikv-jemallocator",
  "time",
@@ -3058,28 +3042,29 @@
  "tracing-appender",
  "tracing-futures",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "summa-wasm"
-version = "0.123.0"
+version = "0.123.8"
 dependencies = [
  "async-trait",
  "console_error_panic_hook",
  "futures",
  "getrandom",
  "instant",
  "js-sys",
  "parking_lot 0.12.1",
+ "prost",
  "serde",
  "serde-wasm-bindgen",
  "strfmt",
  "summa-core",
- "summa-proto 0.26.0",
+ "summa-proto 0.27.0",
  "tantivy",
  "thiserror",
  "tokio",
  "tracing",
  "tracing-wasm",
  "wasm-bindgen",
  "wasm-bindgen-futures",
@@ -3131,15 +3116,15 @@
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "tantivy"
 version = "0.19.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
 dependencies = [
  "aho-corasick",
  "arc-swap",
  "async-trait",
  "base64 0.21.2",
  "bitpacking",
  "byteorder",
@@ -3152,14 +3137,15 @@
  "fs4",
  "futures",
  "futures-util",
  "htmlescape",
  "itertools",
  "izihawa-fst",
  "levenshtein_automata",
+ "lockfree-object-pool",
  "log",
  "lru",
  "measure_time",
  "memmap2",
  "murmurhash32",
  "num_cpus",
  "once_cell",
@@ -3187,38 +3173,38 @@
  "winapi",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-bitpacker"
 version = "0.3.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
 dependencies = [
  "bitpacking",
 ]
 
 [[package]]
 name = "tantivy-columnar"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
 dependencies = [
  "fastdivide",
  "fnv",
  "itertools",
  "serde",
  "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-sstable",
  "tantivy-stacker",
 ]
 
 [[package]]
 name = "tantivy-common"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
 dependencies = [
  "async-trait",
  "byteorder",
  "ownedbytes",
  "serde",
  "time",
 ]
@@ -3233,44 +3219,44 @@
  "regex-syntax 0.6.29",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "tantivy-query-grammar"
 version = "0.19.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
 dependencies = [
  "combine",
  "once_cell",
  "regex",
 ]
 
 [[package]]
 name = "tantivy-sstable"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
 dependencies = [
  "izihawa-fst",
  "tantivy-common",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-stacker"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
 dependencies = [
  "murmurhash32",
  "tantivy-common",
 ]
 
 [[package]]
 name = "tantivy-tokenizer-api"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#312aeb060eea5fae9e4b152f45b301f6939c5520"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#358298c7973b6e668113468b4c02577f8d835b38"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
@@ -3291,23 +3277,24 @@
 dependencies = [
  "rand 0.4.6",
  "remove_dir_all",
 ]
 
 [[package]]
 name = "tempfile"
-version = "3.5.0"
+version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
+checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
+ "autocfg",
  "cfg-if",
  "fastrand",
  "redox_syscall 0.3.5",
  "rustix",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "thiserror"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
@@ -3354,17 +3341,17 @@
 dependencies = [
  "libc",
  "tikv-jemalloc-sys",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.21"
+version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "itoa",
  "js-sys",
  "serde",
  "time-core",
  "time-macros",
 ]
@@ -3784,14 +3771,20 @@
 [[package]]
 name = "unicode-ident"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
+name = "unicode-segmentation"
+version = "1.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+
+[[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
 name = "unindent"
@@ -3848,14 +3841,25 @@
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
+name = "voca_rs"
+version = "1.15.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3e44efbf25e32768d5ecd22244feacc3d3b3eca72d318f5ef0a4764c2c158e18"
+dependencies = [
+ "regex",
+ "stfu8",
+ "unicode-segmentation",
+]
+
+[[package]]
 name = "want"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ce8a968cb1cd110d136ff8b819a556d6fb6d919363c61534f6860c7eb172ba0"
 dependencies = [
  "log",
  "try-lock",
@@ -3978,15 +3982,15 @@
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
@@ -3998,43 +4002,19 @@
  "windows_x86_64_gnu 0.42.2",
  "windows_x86_64_gnullvm 0.42.2",
  "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets 0.42.2",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets 0.48.0",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
-dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
```

