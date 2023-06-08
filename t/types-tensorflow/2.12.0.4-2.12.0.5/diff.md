# Comparing `tmp/types-tensorflow-2.12.0.4.tar.gz` & `tmp/types-tensorflow-2.12.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tensorflow-2.12.0.4.tar", last modified: Mon May 22 15:15:42 2023, max compression
+gzip compressed data, was "types-tensorflow-2.12.0.5.tar", last modified: Thu Jun  8 06:19:11 2023, max compression
```

## Comparing `types-tensorflow-2.12.0.4.tar` & `types-tensorflow-2.12.0.5.tar`

### file list

```diff
@@ -1,145 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-22 15:15:41.000000 types-tensorflow-2.12.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 15:15:41.000000 types-tensorflow-2.12.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-22 15:15:41.000000 types-tensorflow-2.12.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.404107 types-tensorflow-2.12.0.4/tensorflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 15:15:41.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/_aliases.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.400107 types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.404107 types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.404107 types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/service/
--rw-r--r--   0 runner    (1001) docker     (123)    78294 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    78920 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.400107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.404107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/example_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/feature_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.408107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/api_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/attr_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22095 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23251 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/full_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/function_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/log_memory_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/node_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/op_def_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/reader_base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/step_stats_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/summary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/variable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    77923 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    26277 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/debug_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28896 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/struct_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    51042 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/
--rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/event_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/test_log_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/data/
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/data/experimental.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/dtypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/experimental/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/feature_column/
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/initializers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.412107 types-tensorflow-2.12.0.4/tensorflow-stubs/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/io/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/io/gfile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/activations.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/constraints.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/initializers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/layers.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/schedules.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/keras/regularizers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/math.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/python/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/python/trackable/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/trackable/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/trackable/autotrackable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/python/trackable/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/sparse.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.404107 types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-22 15:15:08.000000 types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:15:42.416108 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-22 15:15:42.000000 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-05-22 15:15:42.000000 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:15:42.000000 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-22 15:15:42.000000 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 15:15:42.000000 types-tensorflow-2.12.0.4/types_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-08 06:19:09.000000 types-tensorflow-2.12.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 06:19:09.000000 types-tensorflow-2.12.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-08 06:19:09.000000 types-tensorflow-2.12.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.830320 types-tensorflow-2.12.0.5/tensorflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-08 06:19:09.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    16503 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/_aliases.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.830320 types-tensorflow-2.12.0.5/tensorflow-stubs/compiler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.830320 types-tensorflow-2.12.0.5/tensorflow-stubs/compiler/xla/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.830320 types-tensorflow-2.12.0.5/tensorflow-stubs/compiler/xla/service/
+-rw-r--r--   0 runner    (1001) docker     (123)    78294 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    78920 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.830320 types-tensorflow-2.12.0.5/tensorflow-stubs/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.834321 types-tensorflow-2.12.0.5/tensorflow-stubs/core/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/example/example_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/example/feature_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.834321 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/allocation_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/api_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/attr_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/cost_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22095 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/dataset_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/device_attributes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23251 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/full_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13297 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/function_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/kernel_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/log_memory_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12658 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/node_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15381 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/op_def_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/reader_base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/resource_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12381 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/step_stats_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/summary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/tensor_description_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8890 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/variable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.838322 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/cluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    77923 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/data_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26277 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/debug_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28896 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27624 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27163 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/saver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/service_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/struct_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.838322 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    51042 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.838322 types-tensorflow-2.12.0.5/tensorflow-stubs/core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/util/event_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/core/util/test_log_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.838322 types-tensorflow-2.12.0.5/tensorflow-stubs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/data/experimental.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/dtypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.838322 types-tensorflow-2.12.0.5/tensorflow-stubs/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/experimental/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.838322 types-tensorflow-2.12.0.5/tensorflow-stubs/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/initializers.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.838322 types-tensorflow-2.12.0.5/tensorflow-stubs/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/io/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/io/gfile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/activations.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/constraints.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/initializers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/layers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/losses.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/metrics.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/optimizers/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/optimizers/schedules.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/keras/regularizers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/math.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/tensorflow-stubs/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/tensorflow-stubs/python/feature_column/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/feature_column/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/feature_column/feature_column_v2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/tensorflow-stubs/python/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/keras/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/tensorflow-stubs/python/keras/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/tensorflow-stubs/python/trackable/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/trackable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/trackable/autotrackable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/python/trackable/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/sparse.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.830320 types-tensorflow-2.12.0.5/tensorflow-stubs/tsl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/tensorflow-stubs/tsl/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-08 06:18:57.000000 types-tensorflow-2.12.0.5/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 06:19:11.842322 types-tensorflow-2.12.0.5/types_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-08 06:19:11.000000 types-tensorflow-2.12.0.5/types_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5719 2023-06-08 06:19:11.000000 types-tensorflow-2.12.0.5/types_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 06:19:11.000000 types-tensorflow-2.12.0.5/types_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 06:19:11.000000 types-tensorflow-2.12.0.5/types_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 06:19:11.000000 types-tensorflow-2.12.0.5/types_tensorflow.egg-info/top_level.txt
```

### Comparing `types-tensorflow-2.12.0.4/CHANGELOG.md` & `types-tensorflow-2.12.0.5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.12.0.5 (2023-06-08)
+
+Tensorflow losses (#10264)
+
+Co-authored-by: Mehdi Drissi <mdrissi@snapchat.com>
+
 ## 2.12.0.4 (2023-05-22)
 
 Add core tensorflow.data stubs (#10122)
 
 Co-authored-by: Mehdi Drissi <mdrissi@snapchat.com>
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
 Co-authored-by: Jelle Zijlstra <jelle.zijlstra@gmail.com>
```

### Comparing `types-tensorflow-2.12.0.4/PKG-INFO` & `types-tensorflow-2.12.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.12.0.4
+Version: 2.12.0.5
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,13 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `510547ef3c07502faec40cc4c070e2c0dcda7f93`.
+This package was generated from typeshed commit `0fe724dfab58e6cbe1600344a943c11b34247462`.
```

### Comparing `types-tensorflow-2.12.0.4/setup.py` & `types-tensorflow-2.12.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,33 +11,37 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `510547ef3c07502faec40cc4c070e2c0dcda7f93`.
+This package was generated from typeshed commit `0fe724dfab58e6cbe1600344a943c11b34247462`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.12.0.4",
+      version="2.12.0.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-protobuf', 'numpy>=1.20'],
       packages=['tensorflow-stubs'],
-      package_data={'tensorflow-stubs': ['__init__.pyi', '_aliases.pyi', 'compiler/xla/service/hlo_pb2.pyi', 'compiler/xla/xla_data_pb2.pyi', 'core/example/example_parser_configuration_pb2.pyi', 'core/example/example_pb2.pyi', 'core/example/feature_pb2.pyi', 'core/framework/allocation_description_pb2.pyi', 'core/framework/api_def_pb2.pyi', 'core/framework/attr_value_pb2.pyi', 'core/framework/cost_graph_pb2.pyi', 'core/framework/dataset_metadata_pb2.pyi', 'core/framework/dataset_options_pb2.pyi', 'core/framework/device_attributes_pb2.pyi', 'core/framework/full_type_pb2.pyi', 'core/framework/function_pb2.pyi', 'core/framework/graph_pb2.pyi', 'core/framework/graph_transfer_info_pb2.pyi', 'core/framework/kernel_def_pb2.pyi', 'core/framework/log_memory_pb2.pyi', 'core/framework/model_pb2.pyi', 'core/framework/node_def_pb2.pyi', 'core/framework/op_def_pb2.pyi', 'core/framework/reader_base_pb2.pyi', 'core/framework/resource_handle_pb2.pyi', 'core/framework/step_stats_pb2.pyi', 'core/framework/summary_pb2.pyi', 'core/framework/tensor_description_pb2.pyi', 'core/framework/tensor_pb2.pyi', 'core/framework/tensor_shape_pb2.pyi', 'core/framework/tensor_slice_pb2.pyi', 'core/framework/types_pb2.pyi', 'core/framework/variable_pb2.pyi', 'core/framework/versions_pb2.pyi', 'core/protobuf/__init__.pyi', 'core/protobuf/bfc_memory_map_pb2.pyi', 'core/protobuf/cluster_pb2.pyi', 'core/protobuf/composite_tensor_variant_pb2.pyi', 'core/protobuf/config_pb2.pyi', 'core/protobuf/control_flow_pb2.pyi', 'core/protobuf/coordination_config_pb2.pyi', 'core/protobuf/core_platform_payloads_pb2.pyi', 'core/protobuf/data_service_pb2.pyi', 'core/protobuf/debug_event_pb2.pyi', 'core/protobuf/debug_pb2.pyi', 'core/protobuf/device_filters_pb2.pyi', 'core/protobuf/device_properties_pb2.pyi', 'core/protobuf/distributed_runtime_payloads_pb2.pyi', 'core/protobuf/error_codes_pb2.pyi', 'core/protobuf/fingerprint_pb2.pyi', 'core/protobuf/graph_debug_info_pb2.pyi', 'core/protobuf/meta_graph_pb2.pyi', 'core/protobuf/named_tensor_pb2.pyi', 'core/protobuf/queue_runner_pb2.pyi', 'core/protobuf/remote_tensor_handle_pb2.pyi', 'core/protobuf/rewriter_config_pb2.pyi', 'core/protobuf/saved_model_pb2.pyi', 'core/protobuf/saved_object_graph_pb2.pyi', 'core/protobuf/saver_pb2.pyi', 'core/protobuf/service_config_pb2.pyi', 'core/protobuf/snapshot_pb2.pyi', 'core/protobuf/struct_pb2.pyi', 'core/protobuf/tensor_bundle_pb2.pyi', 'core/protobuf/tensorflow_server_pb2.pyi', 'core/protobuf/tpu/compilation_result_pb2.pyi', 'core/protobuf/tpu/dynamic_padding_pb2.pyi', 'core/protobuf/tpu/optimization_parameters_pb2.pyi', 'core/protobuf/tpu/topology_pb2.pyi', 'core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi', 'core/protobuf/trackable_object_graph_pb2.pyi', 'core/protobuf/transport_options_pb2.pyi', 'core/protobuf/verifier_config_pb2.pyi', 'core/util/event_pb2.pyi', 'core/util/memmapped_file_system_pb2.pyi', 'core/util/saved_tensor_slice_pb2.pyi', 'core/util/test_log_pb2.pyi', 'data/__init__.pyi', 'data/experimental.pyi', 'dtypes.pyi', 'experimental/__init__.pyi', 'feature_column/__init__.pyi', 'initializers.pyi', 'io/__init__.pyi', 'io/gfile.pyi', 'keras/__init__.pyi', 'keras/activations.pyi', 'keras/constraints.pyi', 'keras/initializers.pyi', 'keras/layers.pyi', 'keras/optimizers/__init__.pyi', 'keras/optimizers/legacy/__init__.pyi', 'keras/optimizers/schedules.pyi', 'keras/regularizers.pyi', 'math.pyi', 'python/__init__.pyi', 'python/feature_column/__init__.pyi', 'python/feature_column/feature_column_v2.pyi', 'python/feature_column/sequence_feature_column.pyi', 'python/keras/__init__.pyi', 'python/keras/protobuf/projector_config_pb2.pyi', 'python/keras/protobuf/saved_metadata_pb2.pyi', 'python/keras/protobuf/versions_pb2.pyi', 'python/trackable/__init__.pyi', 'python/trackable/autotrackable.pyi', 'python/trackable/base.pyi', 'sparse.pyi', 'tsl/protobuf/error_codes_pb2.pyi', 'tsl/protobuf/histogram_pb2.pyi', 'METADATA.toml']},
+      package_data={'tensorflow-stubs': ['__init__.pyi', '_aliases.pyi', 'compiler/xla/service/hlo_pb2.pyi', 'compiler/xla/xla_data_pb2.pyi', 'core/example/example_parser_configuration_pb2.pyi', 'core/example/example_pb2.pyi', 'core/example/feature_pb2.pyi', 'core/framework/allocation_description_pb2.pyi', 'core/framework/api_def_pb2.pyi', 'core/framework/attr_value_pb2.pyi', 'core/framework/cost_graph_pb2.pyi', 'core/framework/dataset_metadata_pb2.pyi', 'core/framework/dataset_options_pb2.pyi', 'core/framework/device_attributes_pb2.pyi', 'core/framework/full_type_pb2.pyi', 'core/framework/function_pb2.pyi', 'core/framework/graph_pb2.pyi', 'core/framework/graph_transfer_info_pb2.pyi', 'core/framework/kernel_def_pb2.pyi', 'core/framework/log_memory_pb2.pyi', 'core/framework/model_pb2.pyi', 'core/framework/node_def_pb2.pyi', 'core/framework/op_def_pb2.pyi', 'core/framework/reader_base_pb2.pyi', 'core/framework/resource_handle_pb2.pyi', 'core/framework/step_stats_pb2.pyi', 'core/framework/summary_pb2.pyi', 'core/framework/tensor_description_pb2.pyi', 'core/framework/tensor_pb2.pyi', 'core/framework/tensor_shape_pb2.pyi', 'core/framework/tensor_slice_pb2.pyi', 'core/framework/types_pb2.pyi', 'core/framework/variable_pb2.pyi', 'core/framework/versions_pb2.pyi', 'core/protobuf/__init__.pyi', 'core/protobuf/bfc_memory_map_pb2.pyi', 'core/protobuf/cluster_pb2.pyi', 'core/protobuf/composite_tensor_variant_pb2.pyi', 'core/protobuf/config_pb2.pyi', 'core/protobuf/control_flow_pb2.pyi', 'core/protobuf/coordination_config_pb2.pyi', 'core/protobuf/core_platform_payloads_pb2.pyi', 'core/protobuf/data_service_pb2.pyi', 'core/protobuf/debug_event_pb2.pyi', 'core/protobuf/debug_pb2.pyi', 'core/protobuf/device_filters_pb2.pyi', 'core/protobuf/device_properties_pb2.pyi', 'core/protobuf/distributed_runtime_payloads_pb2.pyi', 'core/protobuf/error_codes_pb2.pyi', 'core/protobuf/fingerprint_pb2.pyi', 'core/protobuf/graph_debug_info_pb2.pyi', 'core/protobuf/meta_graph_pb2.pyi', 'core/protobuf/named_tensor_pb2.pyi', 'core/protobuf/queue_runner_pb2.pyi', 'core/protobuf/remote_tensor_handle_pb2.pyi', 'core/protobuf/rewriter_config_pb2.pyi', 'core/protobuf/saved_model_pb2.pyi', 'core/protobuf/saved_object_graph_pb2.pyi', 'core/protobuf/saver_pb2.pyi', 'core/protobuf/service_config_pb2.pyi', 'core/protobuf/snapshot_pb2.pyi', 'core/protobuf/struct_pb2.pyi', 'core/protobuf/tensor_bundle_pb2.pyi', 'core/protobuf/tensorflow_server_pb2.pyi', 'core/protobuf/tpu/compilation_result_pb2.pyi', 'core/protobuf/tpu/dynamic_padding_pb2.pyi', 'core/protobuf/tpu/optimization_parameters_pb2.pyi', 'core/protobuf/tpu/topology_pb2.pyi', 'core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi', 'core/protobuf/trackable_object_graph_pb2.pyi', 'core/protobuf/transport_options_pb2.pyi', 'core/protobuf/verifier_config_pb2.pyi', 'core/util/event_pb2.pyi', 'core/util/memmapped_file_system_pb2.pyi', 'core/util/saved_tensor_slice_pb2.pyi', 'core/util/test_log_pb2.pyi', 'data/__init__.pyi', 'data/experimental.pyi', 'dtypes.pyi', 'experimental/__init__.pyi', 'feature_column/__init__.pyi', 'initializers.pyi', 'io/__init__.pyi', 'io/gfile.pyi', 'keras/__init__.pyi', 'keras/activations.pyi', 'keras/constraints.pyi', 'keras/initializers.pyi', 'keras/layers.pyi', 'keras/losses.pyi', 'keras/metrics.pyi', 'keras/optimizers/__init__.pyi', 'keras/optimizers/legacy/__init__.pyi', 'keras/optimizers/schedules.pyi', 'keras/regularizers.pyi', 'math.pyi', 'python/__init__.pyi', 'python/feature_column/__init__.pyi', 'python/feature_column/feature_column_v2.pyi', 'python/feature_column/sequence_feature_column.pyi', 'python/keras/__init__.pyi', 'python/keras/protobuf/projector_config_pb2.pyi', 'python/keras/protobuf/saved_metadata_pb2.pyi', 'python/keras/protobuf/versions_pb2.pyi', 'python/trackable/__init__.pyi', 'python/trackable/autotrackable.pyi', 'python/trackable/base.pyi', 'sparse.pyi', 'tsl/protobuf/error_codes_pb2.pyi', 'tsl/protobuf/histogram_pb2.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/__init__.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from tensorflow._aliases import ContainerGradients, ContainerTensors, ContainerTensorsLike, Gradients, TensorLike
 from tensorflow.core.protobuf import struct_pb2
 
 # Explicit import of DType is covered by the wildcard, but
 # is necessary to avoid a crash in pytype.
 from tensorflow.dtypes import *
 from tensorflow.dtypes import DType as DType
+from tensorflow.keras import losses as losses
 
 # Most tf.math functions are exported as tf, but sadly not all are.
 from tensorflow.math import (
     abs as abs,
     add as add,
     add_n as add_n,
     argmax as argmax,
```

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/compiler/xla/service/hlo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/compiler/xla/xla_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/example/example_parser_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/example_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/example/example_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/example/feature_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/example/feature_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/allocation_description_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/allocation_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/api_def_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/api_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/attr_value_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/attr_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/cost_graph_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/cost_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/dataset_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/dataset_options_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/dataset_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/device_attributes_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/device_attributes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/full_type_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/full_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/function_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/function_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/graph_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/graph_transfer_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/kernel_def_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/kernel_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/log_memory_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/log_memory_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/model_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/node_def_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/node_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/op_def_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/op_def_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/reader_base_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/reader_base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/resource_handle_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/resource_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/step_stats_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/step_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/summary_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/summary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_description_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/tensor_description_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/tensor_shape_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/types_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/variable_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/variable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/framework/versions_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/framework/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/bfc_memory_map_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/cluster_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/cluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/composite_tensor_variant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/config_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/control_flow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/coordination_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/core_platform_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/data_service_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/data_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/debug_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/debug_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/debug_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/device_filters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/device_properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/distributed_runtime_payloads_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/fingerprint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/graph_debug_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/meta_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/named_tensor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/queue_runner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/remote_tensor_handle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/rewriter_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/saved_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/saved_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/saver_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/saver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/service_config_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/service_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/struct_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/struct_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tensor_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tensorflow_server_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/compilation_result_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/dynamic_padding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/optimization_parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/topology_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/tpu/tpu_embedding_configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/trackable_object_graph_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/transport_options_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/protobuf/verifier_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/event_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/util/event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/util/memmapped_file_system_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/util/saved_tensor_slice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/core/util/test_log_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/core/util/test_log_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/data/__init__.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/data/experimental.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/data/experimental.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/dtypes.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/dtypes.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/feature_column/__init__.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/feature_column/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/io/__init__.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/io/gfile.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/io/gfile.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/constraints.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/keras/constraints.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/initializers.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/keras/initializers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/layers.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/keras/layers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/keras/optimizers/legacy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/optimizers/schedules.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/keras/optimizers/schedules.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/keras/regularizers.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/keras/regularizers.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/math.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/math.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/feature_column_v2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/python/feature_column/feature_column_v2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/python/feature_column/sequence_feature_column.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/python/keras/protobuf/projector_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/python/keras/protobuf/saved_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/python/keras/protobuf/versions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/sparse.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/sparse.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/tsl/protobuf/error_codes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi` & `types-tensorflow-2.12.0.5/tensorflow-stubs/tsl/protobuf/histogram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `types-tensorflow-2.12.0.4/types_tensorflow.egg-info/PKG-INFO` & `types-tensorflow-2.12.0.5/types_tensorflow.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tensorflow
-Version: 2.12.0.4
+Version: 2.12.0.5
 Summary: Typing stubs for tensorflow
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tensorflow.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,13 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tensorflow`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tensorflow. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `510547ef3c07502faec40cc4c070e2c0dcda7f93`.
+This package was generated from typeshed commit `0fe724dfab58e6cbe1600344a943c11b34247462`.
```

### Comparing `types-tensorflow-2.12.0.4/types_tensorflow.egg-info/SOURCES.txt` & `types-tensorflow-2.12.0.5/types_tensorflow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,16 @@
 tensorflow-stubs/io/__init__.pyi
 tensorflow-stubs/io/gfile.pyi
 tensorflow-stubs/keras/__init__.pyi
 tensorflow-stubs/keras/activations.pyi
 tensorflow-stubs/keras/constraints.pyi
 tensorflow-stubs/keras/initializers.pyi
 tensorflow-stubs/keras/layers.pyi
+tensorflow-stubs/keras/losses.pyi
+tensorflow-stubs/keras/metrics.pyi
 tensorflow-stubs/keras/regularizers.pyi
 tensorflow-stubs/keras/optimizers/__init__.pyi
 tensorflow-stubs/keras/optimizers/schedules.pyi
 tensorflow-stubs/keras/optimizers/legacy/__init__.pyi
 tensorflow-stubs/python/__init__.pyi
 tensorflow-stubs/python/feature_column/__init__.pyi
 tensorflow-stubs/python/feature_column/feature_column_v2.pyi
```

