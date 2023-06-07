# Comparing `tmp/openmsistream-1.5.1.tar.gz` & `tmp/openmsistream-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmsistream-1.5.1.tar", last modified: Tue May 16 17:13:34 2023, max compression
+gzip compressed data, was "openmsistream-1.5.2.tar", last modified: Wed Jun  7 22:48:41 2023, max compression
```

## Comparing `openmsistream-1.5.1.tar` & `openmsistream-1.5.2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.463081 openmsistream-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-16 17:13:25.000000 openmsistream-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-16 17:13:25.000000 openmsistream-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 17:13:34.463081 openmsistream-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-16 17:13:25.000000 openmsistream-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream/data_file_io/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream/data_file_io/actor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_download_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31405 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_upload_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream/data_file_io/entity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file_chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/download_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/reproducer_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/upload_data_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/entity/upload_directory_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/data_file_io/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/kafka_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_file_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test.config
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/prod.config
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test.config
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_encrypted.config
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node/
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/consumer_and_producer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/controlled_message_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/controlled_message_reproducer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19752 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
--rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/producer_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/producible.py
--rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/kafka_wrapper/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/metadata_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/metadata_extraction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/metadata_extraction/metadata_json_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/metadata_extraction/metadata_json_reproducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/s3_buckets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/s3_buckets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/s3_buckets/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/s3_buckets/s3_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/s3_buckets/s3_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/s3_buckets/s3_transfer_stream_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.459081 openmsistream-1.5.1/openmsistream/services/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.463081 openmsistream-1.5.1/openmsistream/services/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/examples/runnable_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/examples/script_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/install_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/linux_service_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/manage_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/service_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/services/windows_service_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.463081 openmsistream-1.5.1/openmsistream/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22077 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/argument_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/controlled_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/controlled_process_multi_threaded.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/controlled_process_single_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/dataclass_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/exception_tracking_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/has_argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/has_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/provision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-16 17:13:25.000000 openmsistream-1.5.1/openmsistream/utilities/runnable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:13:34.455081 openmsistream-1.5.1/openmsistream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 17:13:34.000000 openmsistream-1.5.1/openmsistream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-16 17:13:25.000000 openmsistream-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-16 17:13:34.463081 openmsistream-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-16 17:13:25.000000 openmsistream-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.459239 openmsistream-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-07 22:48:34.000000 openmsistream-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 22:48:34.000000 openmsistream-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-07 22:48:41.459239 openmsistream-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-07 22:48:34.000000 openmsistream-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.455239 openmsistream-1.5.2/openmsistream/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.455239 openmsistream-1.5.2/openmsistream/data_file_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.455239 openmsistream-1.5.2/openmsistream/data_file_io/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_chunk_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_download_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7699 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_stream_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_stream_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18974 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_stream_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31405 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_upload_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.455239 openmsistream-1.5.2/openmsistream/data_file_io/actor/file_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/actor/file_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13916 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16852 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.455239 openmsistream-1.5.2/openmsistream/data_file_io/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/entity/data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/entity/data_file_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/entity/data_file_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/entity/download_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/entity/reproducer_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17892 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/entity/upload_data_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/entity/upload_directory_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/data_file_io/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.455239 openmsistream-1.5.2/openmsistream/kafka_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_file_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.459239 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/local_broker_test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/local_broker_test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/local_broker_test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/prod.config
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/test.config
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/test_encrypted.config
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/test_metadata_rep_consumer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.459239 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/testing_node/
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.seed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.459239 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/testing_node_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.crypto
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.seed
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/consumer_and_producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/controlled_message_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/controlled_message_reproducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19752 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/openmsistream_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16366 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/openmsistream_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/producer_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/producible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9474 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/kafka_wrapper/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.459239 openmsistream-1.5.2/openmsistream/metadata_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/metadata_extraction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/metadata_extraction/metadata_json_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/metadata_extraction/metadata_json_reproducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.459239 openmsistream-1.5.2/openmsistream/s3_buckets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/s3_buckets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/s3_buckets/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/s3_buckets/s3_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/s3_buckets/s3_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/s3_buckets/s3_transfer_stream_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.459239 openmsistream-1.5.2/openmsistream/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.459239 openmsistream-1.5.2/openmsistream/services/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/examples/runnable_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/examples/script_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/install_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/linux_service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/manage_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22467 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/service_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/services/windows_service_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.459239 openmsistream-1.5.2/openmsistream/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22077 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/argument_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/controlled_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/controlled_process_multi_threaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/controlled_process_single_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/dataclass_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/exception_tracking_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/has_argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/has_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/provision_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-07 22:48:34.000000 openmsistream-1.5.2/openmsistream/utilities/runnable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:48:41.455239 openmsistream-1.5.2/openmsistream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-07 22:48:41.000000 openmsistream-1.5.2/openmsistream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-07 22:48:41.000000 openmsistream-1.5.2/openmsistream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:48:41.000000 openmsistream-1.5.2/openmsistream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 22:48:41.000000 openmsistream-1.5.2/openmsistream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-07 22:48:41.000000 openmsistream-1.5.2/openmsistream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 22:48:41.000000 openmsistream-1.5.2/openmsistream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 22:48:34.000000 openmsistream-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 22:48:41.459239 openmsistream-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-07 22:48:34.000000 openmsistream-1.5.2/setup.py
```

### Comparing `openmsistream-1.5.1/LICENSE` & `openmsistream-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/PKG-INFO` & `openmsistream-1.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.1.tar.gz
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.2.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
```

### Comparing `openmsistream-1.5.1/README.md` & `openmsistream-1.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # <div align="center"> OpenMSIStream </div>
-#### <div align="center">***v1.5.1***</div>
+#### <div align="center">***v1.5.2***</div>
 
 #### <div align="center">Maggie Eminizer<sup>1</sup>, Sam Tabrisky<sup>2,3,4</sup>, Amir Sharifzadeh<sup>1</sup>, Christopher DiMarco<sup>4</sup>, Jacob M. Diamond<sup>4,6</sup>, K.T. Ramesh<sup>4</sup>, Todd C. Hufnagel<sup>4,5,6</sup>, Tyrel M. McQueen<sup>4,5,7,8</sup>, David Elbert<sup>1,4</sup></div>
 
  <div align="center"><sup>1</sup> Institute for Data Intensive Engineering and Science (IDIES), The Johns Hopkins University, Baltimore, MD, USA </div>
  <div align="center"><sup>2</sup> Department of Biology, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>3</sup> Department of Computer Science, Dartmouth College, Hanover, NH, USA </div>
  <div align="center"><sup>4</sup> Hopkins Extreme Materials Institute (HEMI), The Johns Hopkins University, Baltimore, MD, USA </div>
```

### Comparing `openmsistream-1.5.1/openmsistream/__init__.py` & `openmsistream-1.5.2/openmsistream/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/__init__.py` & `openmsistream-1.5.2/openmsistream/data_file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_chunk_handlers.py` & `openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_chunk_handlers.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_download_directory.py` & `openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_download_directory.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_handler.py` & `openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_stream_handler.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_processor.py` & `openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_stream_processor.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_stream_reproducer.py` & `openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_stream_reproducer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/actor/data_file_upload_directory.py` & `openmsistream-1.5.2/openmsistream/data_file_io/actor/data_file_upload_directory.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py` & `openmsistream-1.5.2/openmsistream/data_file_io/actor/file_registry/producer_file_registry.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py` & `openmsistream-1.5.2/openmsistream/data_file_io/actor/file_registry/stream_handler_registries.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file.py` & `openmsistream-1.5.2/openmsistream/data_file_io/entity/data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file_chunk.py` & `openmsistream-1.5.2/openmsistream/data_file_io/entity/data_file_chunk.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/entity/data_file_directory.py` & `openmsistream-1.5.2/openmsistream/data_file_io/entity/data_file_directory.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/entity/download_data_file.py` & `openmsistream-1.5.2/openmsistream/data_file_io/entity/download_data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/entity/reproducer_message.py` & `openmsistream-1.5.2/openmsistream/data_file_io/entity/reproducer_message.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/entity/upload_data_file.py` & `openmsistream-1.5.2/openmsistream/data_file_io/entity/upload_data_file.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/entity/upload_directory_event_handler.py` & `openmsistream-1.5.2/openmsistream/data_file_io/entity/upload_directory_event_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,20 @@
                 f"ERROR: {filepath} passed to filepath_should_be_uploaded is not a Path!",
                 exc_type=TypeError,
             )
         # only files count
         if not filepath.is_file():
             return False
         # must be relative to the upload directory
-        if not filepath.is_relative_to(self.__rootdir):
-            return False
+        try:
+            if not filepath.is_relative_to(self.__rootdir):
+                return False
+        except AttributeError:  # "is_relative_to" was added after 3.7
+            if not str(filepath).startswith(str(self.__rootdir)):
+                return False
         # must be outside the logs subdirectory
         if self._logs_subdir in filepath.parents:
             return False
         # name shouldn't start with '.'
         if filepath.name.startswith("."):
             return False
         # must match the given regex
```

### Comparing `openmsistream-1.5.1/openmsistream/data_file_io/utilities.py` & `openmsistream-1.5.2/openmsistream/data_file_io/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/__init__.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_file_parser.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/local_broker_test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/prod.config` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/prod.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test.config` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/test.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_encrypted.config` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/test_encrypted.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/test_encrypted_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/test_s3_transfer.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/testing_node/testing_node.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/config_files/testing_node_2/testing_node_2.config`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/consumer_and_producer_group.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/consumer_and_producer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/consumer_group.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/consumer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/controlled_message_processor.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/controlled_message_processor.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/controlled_message_reproducer.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/controlled_message_reproducer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_consumer.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/openmsistream_consumer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/openmsistream_kafka_crypto.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/openmsistream_producer.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/openmsistream_producer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/producer_group.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/producer_group.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/producible.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/producible.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/serialization.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/serialization.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/kafka_wrapper/utilities.py` & `openmsistream-1.5.2/openmsistream/kafka_wrapper/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/metadata_extraction/metadata_json_message.py` & `openmsistream-1.5.2/openmsistream/metadata_extraction/metadata_json_message.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/metadata_extraction/metadata_json_reproducer.py` & `openmsistream-1.5.2/openmsistream/metadata_extraction/metadata_json_reproducer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/s3_buckets/config_file_parser.py` & `openmsistream-1.5.2/openmsistream/s3_buckets/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/s3_buckets/s3_data_transfer.py` & `openmsistream-1.5.2/openmsistream/s3_buckets/s3_data_transfer.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/s3_buckets/s3_service.py` & `openmsistream-1.5.2/openmsistream/s3_buckets/s3_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/s3_buckets/s3_transfer_stream_processor.py` & `openmsistream-1.5.2/openmsistream/s3_buckets/s3_transfer_stream_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             f"{args.bucket_name} bucket...."
         )
         s3_stream_proc.logger.info(msg)
         n_read, n_processed, n_complete, complete_filenames = s3_stream_proc.make_stream()
         s3_stream_proc.close()
         msg = (
             f"{n_read} total messages were consumed, {n_processed} messages were "
-            f"successfully processed, and {len(complete_filenames)} files were transferred "
+            f"successfully processed, and {n_complete} files were transferred "
             f"to the {args.bucket_name} bucket"
         )
         s3_stream_proc.logger.info(msg)
         if len(complete_filenames) > 0:
             msg = (
                 f'{n_complete} file{" was" if n_complete==1 else "s were"} successfully '
                 f"transferred to the {args.bucket_name} bucket.\nTransferred filepaths "
```

### Comparing `openmsistream-1.5.1/openmsistream/services/config.py` & `openmsistream-1.5.2/openmsistream/services/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,20 @@
         return self.service_dicts
 
     def __init__(self):
         # make the Service dictionaries to use
         self.service_dicts = []
         for script in pkg_resources.iter_entry_points("console_scripts"):
             if script.dist.key == "openmsistream":
-                if script.name in ("InstallService", "ManageService", "ProvisionNode"):
+                if script.name in (
+                    "InstallService",
+                    "ManageService",
+                    "ProvisionNode",
+                    "UploadDataFile",
+                ):
                     continue
                 scriptstr = str(script)
                 cmd = (scriptstr.split())[0]
                 path = ((scriptstr.split())[2].split(":"))[0]
                 funcname = (((scriptstr.split())[2]).split(":"))[1]
                 module = importlib.import_module(path)
                 run_classes = [
```

### Comparing `openmsistream-1.5.1/openmsistream/services/examples/runnable_example.py` & `openmsistream-1.5.2/openmsistream/services/examples/runnable_example.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/services/examples/script_example.py` & `openmsistream-1.5.2/openmsistream/services/examples/script_example.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/services/install_service.py` & `openmsistream-1.5.2/openmsistream/services/install_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/services/linux_service_manager.py` & `openmsistream-1.5.2/openmsistream/services/linux_service_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,22 @@
         Print the status of the daemon
         """
         self.__check_systemd_installed()
         result = run_cmd_in_subprocess(
             ["sudo", "systemctl", "status", f"{self.service_name}.service"],
             logger=self.logger,
         )
-        self.logger.info(f"{self.service_name} status: {result.decode()}")
+        if not result:
+            warnmsg = (
+                f"Failed getting status for service {self.service_name}. "
+                f"Try invoking systemctl status {self.service_name}.service manually."
+            )
+            self.logger.warning(warnmsg)
+        else:
+            self.logger.info(f"{self.service_name} status: {result.decode()}")
 
     def stop_service(self):
         """
         Stop the daemon
         """
         self.logger.info(f"Stopping {self.service_name}...")
         self.__check_systemd_installed()
```

### Comparing `openmsistream-1.5.1/openmsistream/services/manage_service.py` & `openmsistream-1.5.2/openmsistream/services/manage_service.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/services/service_manager_base.py` & `openmsistream-1.5.2/openmsistream/services/service_manager_base.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/services/utilities.py` & `openmsistream-1.5.2/openmsistream/services/utilities.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/services/windows_service_manager.py` & `openmsistream-1.5.2/openmsistream/services/windows_service_manager.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/__init__.py` & `openmsistream-1.5.2/openmsistream/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/argument_parsing.py` & `openmsistream-1.5.2/openmsistream/utilities/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/config.py` & `openmsistream-1.5.2/openmsistream/utilities/config.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/config_file_parser.py` & `openmsistream-1.5.2/openmsistream/utilities/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/controlled_process.py` & `openmsistream-1.5.2/openmsistream/utilities/controlled_process.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/controlled_process_multi_threaded.py` & `openmsistream-1.5.2/openmsistream/utilities/controlled_process_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/controlled_process_single_thread.py` & `openmsistream-1.5.2/openmsistream/utilities/controlled_process_single_thread.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/dataclass_table.py` & `openmsistream-1.5.2/openmsistream/utilities/dataclass_table.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/exception_tracking_thread.py` & `openmsistream-1.5.2/openmsistream/utilities/exception_tracking_thread.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/has_arguments.py` & `openmsistream-1.5.2/openmsistream/utilities/has_arguments.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/logging.py` & `openmsistream-1.5.2/openmsistream/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/misc.py` & `openmsistream-1.5.2/openmsistream/utilities/misc.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/provision_wrapper.py` & `openmsistream-1.5.2/openmsistream/utilities/provision_wrapper.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream/utilities/runnable.py` & `openmsistream-1.5.2/openmsistream/utilities/runnable.py`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream.egg-info/PKG-INFO` & `openmsistream-1.5.2/openmsistream.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openmsistream
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python applications for materials data streaming using Apache Kafka. Developed for Open MSI (NSF DMREF award #1921959)
 Home-page: https://github.com/openmsi/openmsistream
 Author: OpenMSIStream
 Author-email: openmsistream@gmail.com
 License: GNU GPLv3
-Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.1.tar.gz
+Download-URL: https://github.com/openmsi/openmsistream/archive/refs/tags/v1.5.2.tar.gz
 Keywords: data_streaming,stream_processing,apache_kafka,materials,data_science
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
```

### Comparing `openmsistream-1.5.1/openmsistream.egg-info/SOURCES.txt` & `openmsistream-1.5.2/openmsistream.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/openmsistream.egg-info/entry_points.txt` & `openmsistream-1.5.2/openmsistream.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `openmsistream-1.5.1/setup.py` & `openmsistream-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # imports
 import setuptools
 
 # version tag
-version = "1.5.1"
+version = "1.5.2"
 
 long_description = ""
 with open("README.md", "r") as readme:
     for il, line in enumerate(readme.readlines(), start=1):
         if il >= 18:
             long_description += line
```

