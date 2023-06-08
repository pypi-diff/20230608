# Comparing `tmp/funboost-21.2-py3-none-any.whl.zip` & `tmp/funboost-23.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 1891829 bytes, number of entries: 224
--rw-rw-rw-  2.0 fat    21054 b- defN 23-May-30 09:43 funboost/__init__.py
+Zip file size: 1903446 bytes, number of entries: 235
+-rw-rw-rw-  2.0 fat     2154 b- defN 23-Jun-05 10:48 funboost/__init__.py
+-rw-rw-rw-  2.0 fat    20378 b- defN 23-Jun-05 04:48 funboost/__init__0000.py
 -rw-rw-rw-  2.0 fat     6154 b- defN 23-May-24 10:24 funboost/constant.py
--rw-rw-rw-  2.0 fat     7332 b- defN 23-May-22 01:23 funboost/funboost_config_deafult.py
--rw-rw-rw-  2.0 fat    14135 b- defN 23-May-30 08:53 funboost/helpers.py
+-rw-rw-rw-  2.0 fat     7358 b- defN 23-Jun-05 04:48 funboost/funboost_config_deafult.py
 -rw-rw-rw-  2.0 fat     9149 b- defN 23-Apr-13 09:47 funboost/set_frame_config.py
 -rw-rw-rw-  2.0 fat     3987 b- defN 23-May-17 08:56 funboost/assist/celery_helper.py
 -rw-rw-rw-  2.0 fat     2089 b- defN 23-May-22 01:31 funboost/assist/dramatiq_helper.py
 -rw-rw-rw-  2.0 fat     1760 b- defN 23-May-24 11:10 funboost/assist/huey_helper.py
 -rw-rw-rw-  2.0 fat     3930 b- defN 22-Sep-17 06:12 funboost/beggar_version_implementation/beggar_redis_consumer.py
 -rw-rw-rw-  2.0 fat      759 b- defN 22-Dec-19 11:45 funboost/concurrent_pool/__init__.py
 -rw-rw-rw-  2.0 fat     3256 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/async_helper.py
@@ -21,16 +21,16 @@
 -rw-rw-rw-  2.0 fat     9317 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/custom_threadpool_executor000.py
 -rw-rw-rw-  2.0 fat      373 b- defN 21-Dec-27 01:40 funboost/concurrent_pool/single_thread_executor.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-24 11:39 funboost/concurrent_pool/backup/__init__.py
 -rw-rw-rw-  2.0 fat     9548 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor0223.py
 -rw-rw-rw-  2.0 fat     9568 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor_back.py
 -rw-rw-rw-  2.0 fat     5728 b- defN 23-Mar-23 05:32 funboost/concurrent_pool/backup/async_pool_executor_janus.py
 -rw-rw-rw-  2.0 fat      126 b- defN 22-Sep-17 06:12 funboost/consumers/__init__.py
--rw-rw-rw-  2.0 fat    96486 b- defN 23-May-18 03:15 funboost/consumers/base_consumer.py
--rw-rw-rw-  2.0 fat     7546 b- defN 23-May-22 01:23 funboost/consumers/celery_consumer.py
+-rw-rw-rw-  2.0 fat    83054 b- defN 23-Jun-05 04:48 funboost/consumers/base_consumer.py
+-rw-rw-rw-  2.0 fat     7574 b- defN 23-Jun-06 01:47 funboost/consumers/celery_consumer.py
 -rw-rw-rw-  2.0 fat     4574 b- defN 23-May-04 06:09 funboost/consumers/celery_consumer000.py
 -rw-rw-rw-  2.0 fat     5877 b- defN 23-Mar-29 02:19 funboost/consumers/confirm_mixin.py
 -rw-rw-rw-  2.0 fat     2144 b- defN 23-May-23 07:08 funboost/consumers/dramatiq_consumer.py
 -rw-rw-rw-  2.0 fat     2025 b- defN 23-May-15 01:33 funboost/consumers/http_consumer.py
 -rw-rw-rw-  2.0 fat     4463 b- defN 22-Sep-17 06:12 funboost/consumers/http_consumer000.py
 -rw-rw-rw-  2.0 fat     1080 b- defN 23-May-04 12:12 funboost/consumers/httpsqs_consumer.py
 -rw-rw-rw-  2.0 fat     1856 b- defN 23-May-24 11:08 funboost/consumers/huey_consumer.py
@@ -62,16 +62,28 @@
 -rw-rw-rw-  2.0 fat     2045 b- defN 23-May-04 12:12 funboost/consumers/tcp_consumer.py
 -rw-rw-rw-  2.0 fat     1340 b- defN 23-May-04 12:12 funboost/consumers/txt_file_consumer.py
 -rw-rw-rw-  2.0 fat     1643 b- defN 23-May-04 12:12 funboost/consumers/udp_consumer.py
 -rw-rw-rw-  2.0 fat     4157 b- defN 23-May-04 12:12 funboost/consumers/zeromq_consumer.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Dec-05 10:31 funboost/contrib/__init__.py
 -rw-rw-rw-  2.0 fat     4680 b- defN 23-May-15 08:24 funboost/contrib/queue2queue.py
 -rw-rw-rw-  2.0 fat     1817 b- defN 23-Mar-22 02:09 funboost/contrib/redis_consume_latest_msg_broker.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 04:48 funboost/core/__init__.py
+-rw-rw-rw-  2.0 fat     4984 b- defN 23-Jun-05 04:48 funboost/core/active_cousumer_info_getter.py
+-rw-rw-rw-  2.0 fat    16419 b- defN 23-Jun-06 02:26 funboost/core/booster.py
+-rw-rw-rw-  2.0 fat      421 b- defN 23-Jun-05 04:48 funboost/core/exit_signal.py
+-rw-rw-rw-  2.0 fat     8875 b- defN 23-Jun-05 04:48 funboost/core/fabric_deploy_helper.py
+-rw-rw-rw-  2.0 fat     1570 b- defN 23-Jun-05 04:48 funboost/core/function_result_status_config.py
+-rw-rw-rw-  2.0 fat     8819 b- defN 23-Jun-05 04:48 funboost/core/function_result_status_saver.py
+-rw-rw-rw-  2.0 fat     1299 b- defN 23-Jun-06 02:26 funboost/core/get_booster.py
+-rw-rw-rw-  2.0 fat      168 b- defN 23-Jun-05 04:48 funboost/core/global_boosters.py
+-rw-rw-rw-  2.0 fat      604 b- defN 23-Jun-05 04:48 funboost/core/helper_funs.py
+-rw-rw-rw-  2.0 fat     7782 b- defN 23-Jun-05 04:48 funboost/core/msg_result_getter.py
+-rw-rw-rw-  2.0 fat     3766 b- defN 23-Jun-05 11:19 funboost/core/muliti_process_enhance.py
 -rw-rw-rw-  2.0 fat      178 b- defN 22-Sep-17 06:12 funboost/factories/__init__.py
--rw-rw-rw-  2.0 fat     8191 b- defN 23-May-29 03:29 funboost/factories/broker_kind__publsiher_consumer_type_map.py
+-rw-rw-rw-  2.0 fat     8420 b- defN 23-May-31 01:38 funboost/factories/broker_kind__publsiher_consumer_type_map.py
 -rw-rw-rw-  2.0 fat      946 b- defN 23-May-29 03:09 funboost/factories/consumer_factory.py
 -rw-rw-rw-  2.0 fat     2281 b- defN 23-May-29 03:09 funboost/factories/publisher_factotry.py
 -rw-rw-rw-  2.0 fat     4841 b- defN 22-Sep-17 06:12 funboost/function_result_web/app.py
 -rw-rw-rw-  2.0 fat     7345 b- defN 23-Mar-08 10:19 funboost/function_result_web/functions.py
 -rw-rw-rw-  2.0 fat     4045 b- defN 22-Feb-21 07:34 funboost/function_result_web/__pycache__/app.cpython-37.pyc
 -rw-rw-rw-  2.0 fat     3921 b- defN 22-Mar-30 13:56 funboost/function_result_web/__pycache__/functions.cpython-37.pyc
 -rw-rw-rw-  2.0 fat     7674 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/assets/css/custom.css
@@ -84,28 +96,27 @@
 -rw-rw-rw-  2.0 fat      546 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/password.png
 -rw-rw-rw-  2.0 fat     2912 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/tick.png
 -rw-rw-rw-  2.0 fat      622 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/images/user.png
 -rw-rw-rw-  2.0 fat    96383 b- defN 21-Dec-27 01:40 funboost/function_result_web/static/js/jquery-1.11.0.min.js
 -rw-rw-rw-  2.0 fat    19501 b- defN 22-Feb-21 12:32 funboost/function_result_web/templates/index.html
 -rw-rw-rw-  2.0 fat     2007 b- defN 21-Dec-27 01:40 funboost/function_result_web/templates/login.html
 -rw-rw-rw-  2.0 fat      131 b- defN 22-Sep-17 06:12 funboost/publishers/__init__.py
--rw-rw-rw-  2.0 fat    15103 b- defN 23-May-15 01:33 funboost/publishers/base_publisher.py
+-rw-rw-rw-  2.0 fat    15047 b- defN 23-Jun-05 04:48 funboost/publishers/base_publisher.py
 -rw-rw-rw-  2.0 fat     3724 b- defN 23-May-15 01:33 funboost/publishers/celery_publisher.py
 -rw-rw-rw-  2.0 fat     3897 b- defN 23-May-04 06:09 funboost/publishers/celery_publisher000.py
 -rw-rw-rw-  2.0 fat     3541 b- defN 23-Mar-23 05:32 funboost/publishers/confluent_kafka_publisher.py
 -rw-rw-rw-  2.0 fat     1410 b- defN 23-May-22 01:23 funboost/publishers/dramatiq_publisher.py
 -rw-rw-rw-  2.0 fat      753 b- defN 23-May-04 11:53 funboost/publishers/http_publisher.py
 -rw-rw-rw-  2.0 fat     2783 b- defN 22-Sep-17 06:12 funboost/publishers/httpsqs_publisher.py
 -rw-rw-rw-  2.0 fat     1101 b- defN 23-May-24 11:08 funboost/publishers/huey_publisher.py
 -rw-rw-rw-  2.0 fat     2160 b- defN 23-Apr-03 10:55 funboost/publishers/kafka_publisher.py
 -rw-rw-rw-  2.0 fat     5321 b- defN 23-May-15 01:33 funboost/publishers/kombu_publisher.py
 -rw-rw-rw-  2.0 fat     1365 b- defN 22-Sep-17 06:12 funboost/publishers/local_python_queue_publisher.py
 -rw-rw-rw-  2.0 fat     1874 b- defN 23-Mar-14 02:56 funboost/publishers/mongomq_publisher.py
 -rw-rw-rw-  2.0 fat     3050 b- defN 22-Sep-17 06:12 funboost/publishers/mqtt_publisher.py
--rw-rw-rw-  2.0 fat     7782 b- defN 23-Mar-31 03:13 funboost/publishers/msg_result_getter.py
 -rw-rw-rw-  2.0 fat     2147 b- defN 23-Apr-28 06:21 funboost/publishers/nameko_publisher.py
 -rw-rw-rw-  2.0 fat      776 b- defN 21-Dec-27 01:40 funboost/publishers/nats_publisher.py
 -rw-rw-rw-  2.0 fat     1302 b- defN 22-Sep-17 06:12 funboost/publishers/nsq_publisher.py
 -rw-rw-rw-  2.0 fat     1095 b- defN 22-Sep-17 06:12 funboost/publishers/peewee_publisher.py
 -rw-rw-rw-  2.0 fat     2540 b- defN 22-Sep-17 06:12 funboost/publishers/persist_queue_publisher.py
 -rw-rw-rw-  2.0 fat     1238 b- defN 23-Apr-13 03:56 funboost/publishers/pulsar_publisher.py
 -rw-rw-rw-  2.0 fat     2725 b- defN 23-Apr-17 07:35 funboost/publishers/rabbitmq_amqpstorm_publisher.py
@@ -121,15 +132,15 @@
 -rw-rw-rw-  2.0 fat     1335 b- defN 23-May-10 08:53 funboost/publishers/tcp_publisher.py
 -rw-rw-rw-  2.0 fat     1380 b- defN 22-Sep-17 08:52 funboost/publishers/txt_file_publisher.py
 -rw-rw-rw-  2.0 fat     1194 b- defN 23-May-04 11:53 funboost/publishers/udp_publisher.py
 -rw-rw-rw-  2.0 fat     1002 b- defN 21-Dec-27 01:40 funboost/publishers/zeromq_publisher.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-22 02:44 funboost/queues/__init__.py
 -rw-rw-rw-  2.0 fat     4944 b- defN 23-May-22 04:27 funboost/queues/peewee_queue.py
 -rw-rw-rw-  2.0 fat    11024 b- defN 23-May-05 02:38 funboost/queues/sqla_queue.py
--rw-rw-rw-  2.0 fat     7307 b- defN 23-May-30 11:07 funboost/timing_job/__init__.py
+-rw-rw-rw-  2.0 fat     7919 b- defN 23-Jun-05 04:56 funboost/timing_job/__init__.py
 -rw-rw-rw-  2.0 fat      418 b- defN 23-Apr-06 06:09 funboost/timing_job/apscheduler_use_mysql_store.py
 -rw-rw-rw-  2.0 fat      876 b- defN 23-May-30 09:38 funboost/timing_job/apscheduler_use_redis_store.py
 -rw-rw-rw-  2.0 fat     1951 b- defN 23-Mar-09 07:27 funboost/utils/__init__.py
 -rw-rw-rw-  2.0 fat     3124 b- defN 21-Dec-27 01:40 funboost/utils/apscheduler_monkey.py
 -rw-rw-rw-  2.0 fat       96 b- defN 23-Jan-29 07:41 funboost/utils/block_exit.py
 -rw-rw-rw-  2.0 fat     9972 b- defN 22-Apr-01 02:17 funboost/utils/bulk_operation.py
 -rw-rw-rw-  2.0 fat     5923 b- defN 21-Dec-27 01:40 funboost/utils/custom_pysnooper.py
@@ -214,13 +225,13 @@
 -rw-rw-rw-  2.0 fat      303 b- defN 23-Mar-13 01:28 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc
 -rw-rw-rw-  2.0 fat      311 b- defN 23-Mar-21 10:43 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc
 -rw-rw-rw-  2.0 fat      909 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/__init__.py
 -rw-rw-rw-  2.0 fat     2243 b- defN 21-Dec-27 01:40 funboost/utils/pysnooper_ydf/pycompat.py
 -rw-rw-rw-  2.0 fat    19131 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/tracer.py
 -rw-rw-rw-  2.0 fat     2753 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/utils.py
 -rw-rw-rw-  2.0 fat     3693 b- defN 23-Mar-23 05:34 funboost/utils/pysnooper_ydf/variables.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-31 01:30 funboost-21.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    26423 b- defN 23-May-31 01:30 funboost-21.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       97 b- defN 23-May-31 01:30 funboost-21.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-31 01:30 funboost-21.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat    24594 b- defN 23-May-31 01:30 funboost-21.2.dist-info/RECORD
-224 files, 3255160 bytes uncompressed, 1850973 bytes compressed:  43.1%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-Jun-08 01:42 funboost-23.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    26423 b- defN 23-Jun-08 01:42 funboost-23.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-08 01:42 funboost-23.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-08 01:42 funboost-23.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat    25590 b- defN 23-Jun-08 01:42 funboost-23.0.dist-info/RECORD
+235 files, 3277831 bytes uncompressed, 1861004 bytes compressed:  43.2%
```

## zipnote {}

```diff
@@ -1,17 +1,17 @@
 Filename: funboost/__init__.py
 Comment: 
 
-Filename: funboost/constant.py
+Filename: funboost/__init__0000.py
 Comment: 
 
-Filename: funboost/funboost_config_deafult.py
+Filename: funboost/constant.py
 Comment: 
 
-Filename: funboost/helpers.py
+Filename: funboost/funboost_config_deafult.py
 Comment: 
 
 Filename: funboost/set_frame_config.py
 Comment: 
 
 Filename: funboost/assist/celery_helper.py
 Comment: 
@@ -195,14 +195,50 @@
 
 Filename: funboost/contrib/queue2queue.py
 Comment: 
 
 Filename: funboost/contrib/redis_consume_latest_msg_broker.py
 Comment: 
 
+Filename: funboost/core/__init__.py
+Comment: 
+
+Filename: funboost/core/active_cousumer_info_getter.py
+Comment: 
+
+Filename: funboost/core/booster.py
+Comment: 
+
+Filename: funboost/core/exit_signal.py
+Comment: 
+
+Filename: funboost/core/fabric_deploy_helper.py
+Comment: 
+
+Filename: funboost/core/function_result_status_config.py
+Comment: 
+
+Filename: funboost/core/function_result_status_saver.py
+Comment: 
+
+Filename: funboost/core/get_booster.py
+Comment: 
+
+Filename: funboost/core/global_boosters.py
+Comment: 
+
+Filename: funboost/core/helper_funs.py
+Comment: 
+
+Filename: funboost/core/msg_result_getter.py
+Comment: 
+
+Filename: funboost/core/muliti_process_enhance.py
+Comment: 
+
 Filename: funboost/factories/__init__.py
 Comment: 
 
 Filename: funboost/factories/broker_kind__publsiher_consumer_type_map.py
 Comment: 
 
 Filename: funboost/factories/consumer_factory.py
@@ -300,17 +336,14 @@
 
 Filename: funboost/publishers/mongomq_publisher.py
 Comment: 
 
 Filename: funboost/publishers/mqtt_publisher.py
 Comment: 
 
-Filename: funboost/publishers/msg_result_getter.py
-Comment: 
-
 Filename: funboost/publishers/nameko_publisher.py
 Comment: 
 
 Filename: funboost/publishers/nats_publisher.py
 Comment: 
 
 Filename: funboost/publishers/nsq_publisher.py
@@ -651,23 +684,23 @@
 
 Filename: funboost/utils/pysnooper_ydf/utils.py
 Comment: 
 
 Filename: funboost/utils/pysnooper_ydf/variables.py
 Comment: 
 
-Filename: funboost-21.2.dist-info/LICENSE
+Filename: funboost-23.0.dist-info/LICENSE
 Comment: 
 
-Filename: funboost-21.2.dist-info/METADATA
+Filename: funboost-23.0.dist-info/METADATA
 Comment: 
 
-Filename: funboost-21.2.dist-info/WHEEL
+Filename: funboost-23.0.dist-info/WHEEL
 Comment: 
 
-Filename: funboost-21.2.dist-info/top_level.txt
+Filename: funboost-23.0.dist-info/top_level.txt
 Comment: 
 
-Filename: funboost-21.2.dist-info/RECORD
+Filename: funboost-23.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## funboost/__init__.py

```diff
@@ -1,329 +1,38 @@
 # noinspection PyUnresolvedReferences
 from funboost.utils.dependency_packages_in_pythonpath import add_to_pythonpath
 
 from funboost.utils import monkey_patches
 from funboost.utils import show_funboost_flag
-import typing
-# noinspection PyUnresolvedReferences
-from functools import update_wrapper, wraps, partial
-import copy
+
 # noinspection PyUnresolvedReferences
 import nb_log
 from funboost.set_frame_config import patch_frame_config, show_frame_config
 from funboost.funboost_config_deafult import BoostDecoratorDefaultParams
-from funboost.helpers import (fabric_deploy, kill_all_remote_tasks,
-                              multi_process_pub_params_list,
-                              run_consumer_with_multi_process, boost_queue__fun_map)
+
+from funboost.core.fabric_deploy_helper import fabric_deploy, kill_all_remote_tasks
 
 from funboost.utils.paramiko_util import ParamikoFolderUploader
+
 from funboost.consumers.base_consumer import (ExceptionForRequeue, ExceptionForRetry, ExceptionForPushToDlxqueue,
                                               AbstractConsumer, ConsumersManager,
                                               FunctionResultStatusPersistanceConfig,
                                               wait_for_possible_has_finish_all_tasks_by_conusmer_list,
-                                              ActiveCousumerProcessInfoGetter, FunctionResultStatus)
+                                              FunctionResultStatus)
+from funboost.core.active_cousumer_info_getter import ActiveCousumerProcessInfoGetter
+from funboost.core.msg_result_getter import HasNotAsyncResult, ResultFromMongo
 from funboost.publishers.base_publisher import (PriorityConsumingControlConfig,
-                                                AbstractPublisher, AsyncResult, HasNotAsyncResult, AioAsyncResult, ResultFromMongo)
+                                                AbstractPublisher, AsyncResult, AioAsyncResult)
 from funboost.factories.broker_kind__publsiher_consumer_type_map import register_custom_broker
 from funboost.factories.publisher_factotry import get_publisher
 from funboost.factories.consumer_factory import get_consumer
 
-
-# noinspection PyUnresolvedReferences
-from funboost.utils import nb_print, patch_print, LogManager, get_logger, LoggerMixin
-from funboost.timing_job import fsdf_background_scheduler, timing_publish_deco,funboost_aps_scheduler
+from funboost.timing_job import fsdf_background_scheduler, timing_publish_deco, funboost_aps_scheduler
 from funboost.constant import BrokerEnum, ConcurrentModeEnum
 
+from funboost.core.booster import boost, Booster
+from funboost.core.get_booster import get_booster
+
+from funboost.core import exit_signal
 
 # 有的包默认没加handlers，原始的日志不漂亮且不可跳转不知道哪里发生的。这里把warnning级别以上的日志默认加上handlers。
 # nb_log.get_logger(name='', log_level_int=30, log_filename='pywarning.log')
-
-
-class IdeAutoCompleteHelper(LoggerMixin):
-    """
-    为了被装饰的消费函数的敲代码时候的被pycharm自动补全而写的类。
-    """
-
-    def __init__(self, consuming_func_decorated: callable):
-        """
-        :param consuming_func_decorated:   传入被boost装饰的函数
-
-        此框架非常非常注重，公有函数、方法、类 的名字和入参在ide开发环境下面的自动提示补全效果，如果不是为了这一点，框架能减少很多重复地方。
-        此类是防止用户调用打错字母或者不知道怎么敲代码不知道有哪些入参。所以才有这个类。
-
-        这个类是个补全类，能够使pycharm自动补全方法名字和入参。可以用，可以不用，用了后在pycharm里面补全效果会起作用。
-
-
-       from funboost import boost, IdeAutoCompleteHelper
-
-       @boost('queue_test_f01', qps=2, broker_kind=3)
-       def f(a, b):
-           print(f'{a} + {b} = {a + b}')
-
-
-       if __name__ == '__main__':
-           f(1000, 2000)
-           IdeAutoCompleteHelper(f).clear()  # f.clear()
-           for i in range(100, 200):
-               f.pub(dict(a=i, b=i * 2))  # f.sub方法是强行用元编程加到f上去的，是运行时状态，pycharm只能补全非运行时态的静态东西。
-               IdeAutoCompleteHelper(f).pub({'a': i * 3, 'b': i * 4})  # 和上面的发布等效，但可以自动补全方法名字和入参。
-               f.push(a=i, b=i * 2)
-               IdeAutoCompleteHelper(f).delay(i * 3,  i * 4)
-
-           IdeAutoCompleteHelper(f).start_consuming_message()  # 和 f.consume()等效
-
-        """
-        self.is_decorated_as_consume_function = consuming_func_decorated.is_decorated_as_consume_function
-        self.consuming_func_decorated = consuming_func_decorated
-
-        self.queue_name = consuming_func_decorated.queue_name
-
-        self.consumer = consuming_func_decorated.consumer  # type: AbstractConsumer
-
-        self.publisher = consuming_func_decorated.publisher  # type: AbstractPublisher
-        self.publish = self.pub = self.apply_async = self.publisher.publish  # type: AbstractPublisher.publish
-        self.push = self.delay = self.publisher.push  # type: AbstractPublisher.push
-        self.clear = self.clear_queue = self.publisher.clear  # type: AbstractPublisher.clear
-        self.get_message_count = self.publisher.get_message_count
-
-        self.start_consuming_message = self.consume = self.start = self.consumer.start_consuming_message
-
-        self.clear_filter_tasks = self.consumer.clear_filter_tasks
-
-        self.wait_for_possible_has_finish_all_tasks = self.consumer.wait_for_possible_has_finish_all_tasks
-
-        self.pause = self.pause_consume = self.consumer.pause_consume
-        self.continue_consume = self.consumer.continue_consume
-
-    def multi_process_consume(self, process_num=1):
-        """超高速多进程消费"""
-        run_consumer_with_multi_process(self.consuming_func_decorated, process_num)
-
-    def multi_process_pub_params_list(self, params_list, process_num=16):
-        """超高速多进程发布，例如先快速发布1000万个任务到中间件，以后慢慢消费"""
-        """
-        用法例如，快速20进程发布1000万任务，充分利用多核加大cpu使用率。
-        @boost('test_queue66c', qps=1/30,broker_kind=BrokerEnum.KAFKA_CONFLUENT)
-        def f(x, y):
-            print(f'函数开始执行时间 {time.strftime("%H:%M:%S")}')
-        if __name__ == '__main__':
-            f.multi_process_pub_params_list([{'x':i,'y':i*3}  for i in range(10000000)],process_num=20)
-            f.consume()
-        """
-        multi_process_pub_params_list(self.consuming_func_decorated, params_list=params_list, process_num=process_num)
-
-    # noinspection PyDefaultArgument
-    def fabric_deploy(self, host, port, user, password,
-                      path_pattern_exluded_tuple=('/.git/', '/.idea/', '/dist/', '/build/'),
-                      file_suffix_tuple_exluded=('.pyc', '.log', '.gz'),
-                      only_upload_within_the_last_modify_time=3650 * 24 * 60 * 60,
-                      file_volume_limit=1000 * 1000, sftp_log_level=20, extra_shell_str='',
-                      invoke_runner_kwargs={'hide': None, 'pty': True, 'warn': False},
-                      python_interpreter='python3',
-                      process_num=1):
-        """
-        入参见 fabric_deploy 函数。这里重复入参是为了代码在pycharm补全提示。
-        """
-        in_kwargs = locals()
-        in_kwargs.pop('self')
-        fabric_deploy(self.consuming_func_decorated, **in_kwargs)
-
-    multi_process_start = multi_process_consume
-
-    def __call__(self, *args, **kwargs):
-        return self.consuming_func_decorated(*args, **kwargs)
-
-
-class _Undefined:
-    pass
-
-
-
-
-
-# import funboost ; funboost.boost_queue__fun_map
-
-def boost(queue_name,
-          *,
-          consumin_function_decorator: typing.Callable = _Undefined,
-          function_timeout: float = _Undefined,
-          concurrent_num: int = _Undefined,
-          specify_concurrent_pool=_Undefined,
-          specify_async_loop=_Undefined,
-          concurrent_mode: int = _Undefined,
-          max_retry_times: int = _Undefined,
-          is_push_to_dlx_queue_when_retry_max_times: bool = _Undefined,
-          log_level: int = _Undefined,
-          is_print_detail_exception: bool = _Undefined,
-          is_show_message_get_from_broker: bool = _Undefined,
-          qps: float = _Undefined,
-          is_using_distributed_frequency_control: bool = _Undefined,
-          msg_expire_senconds: float = _Undefined,
-          is_send_consumer_hearbeat_to_redis: bool = _Undefined,
-          logger_prefix: str = _Undefined,
-          create_logger_file: bool = _Undefined,
-          do_task_filtering: bool = _Undefined,
-          task_filtering_expire_seconds: float = _Undefined,
-          is_do_not_run_by_specify_time_effect: bool = _Undefined,
-          do_not_run_by_specify_time: bool = _Undefined,
-          schedule_tasks_on_main_thread: bool = _Undefined,
-          function_result_status_persistance_conf: FunctionResultStatusPersistanceConfig = _Undefined,
-          user_custom_record_process_info_func: typing.Union[typing.Callable, None] = _Undefined,
-          is_using_rpc_mode: bool = _Undefined,
-          broker_exclusive_config: dict = _Undefined,
-          broker_kind: int = _Undefined,
-          boost_decorator_default_params=BoostDecoratorDefaultParams()
-          ):
-    """
-    funboost.funboost_config_deafult.BoostDecoratorDefaultParams 的值会自动被你项目根目录下的funboost_config.BoostDecoratorDefaultParams的值覆盖，
-    如果boost装饰器不传参，默认使用funboost_config.BoostDecoratorDefaultParams的配置
-
-    入参也可以看文档 https://funboost.readthedocs.io/zh/latest/articles/c3.html   3.3章节。
-
-    # 为了代码提示好，这里重复一次入参意义。被此装饰器装饰的函数f，函数f对象本身自动加了一些方法，例如f.push 、 f.consume等。
-    :param queue_name: 队列名字。
-    :param consumin_function_decorator : 函数的装饰器。因为此框架做参数自动转指点，需要获取精准的入参名称，不支持在消费函数上叠加 @ *args  **kwargs的装饰器，如果想用装饰器可以这里指定。
-    :param function_timeout : 超时秒数，函数运行超过这个时间，则自动杀死函数。为0是不限制。设置后代码性能会变差，非必要不要轻易设置。
-    # 如果设置了qps，并且cocurrent_num是默认的50，会自动开了500并发，由于是采用的智能线程池任务少时候不会真开那么多线程而且会自动缩小线程数量。具体看ThreadPoolExecutorShrinkAble的说明
-    # 由于有很好用的qps控制运行频率和智能扩大缩小的线程池，此框架建议不需要理会和设置并发数量只需要关心qps就行了，框架的并发是自适应并发数量，这一点很强很好用。
-    :param concurrent_num:并发数量
-    :param specify_concurrent_pool:使用指定的线程池（协程池），可以多个消费者共使用一个线程池，不为None时候。threads_num失效
-    :param specify_async_loop:指定的async的loop循环，设置并发模式为async才能起作用。
-    :param concurrent_mode:并发模式，1线程(ConcurrentModeEnum.THREADING) 2gevent(ConcurrentModeEnum.GEVENT)
-                              3eventlet(ConcurrentModeEnum.EVENTLET) 4 asyncio(ConcurrentModeEnum.ASYNC) 5单线程(ConcurrentModeEnum.SINGLE_THREAD)
-    :param max_retry_times: 最大自动重试次数，当函数发生错误，立即自动重试运行n次，对一些特殊不稳定情况会有效果。
-           可以在函数中主动抛出重试的异常ExceptionForRetry，框架也会立即自动重试。
-           主动抛出ExceptionForRequeue异常，则当前 消息会重返中间件，
-           主动抛出 ExceptionForPushToDlxqueue  异常，可以使消息发送到单独的死信队列中，死信队列的名字是 队列名字 + _dlx。
-           。
-    :param is_push_to_dlx_queue_when_retry_max_times : 函数达到最大重试次数仍然没成功，是否发送到死信队列,死信队列的名字是 队列名字 + _dlx。
-    :param log_level:框架的日志级别。logging.DEBUG(10)  logging.DEBUG(10) logging.INFO(20) logging.WARNING(30) logging.ERROR(40) logging.CRITICAL(50)
-    :param is_print_detail_exception:是否打印详细的堆栈错误。为0则打印简略的错误占用控制台屏幕行数少。
-    :param is_show_message_get_from_broker: 从中间件取出消息时候时候打印显示出来
-    :param qps:指定1秒内的函数执行次数，例如可以是小数0.01代表每100秒执行一次，也可以是50代表1秒执行50次.为0则不控频。
-    :param msg_expire_senconds:消息过期时间，为0永不过期，为10则代表，10秒之前发布的任务如果现在才轮到消费则丢弃任务。
-    :param is_using_distributed_frequency_control: 是否使用分布式空频（依赖redis统计消费者数量，然后频率平分），默认只对当前实例化的消费者空频有效。
-            假如实例化了2个qps为10的使用同一队列名的消费者，并且都启动，则每秒运行次数会达到20。如果使用分布式空频则所有消费者加起来的总运行次数是10。
-    :param is_send_consumer_hearbeat_to_redis   是否将发布者的心跳发送到redis，有些功能的实现需要统计活跃消费者。因为有的中间件不是真mq。
-    :param logger_prefix: 日志前缀，可使不同的消费者生成不同的日志前缀
-    :param create_logger_file : 是否创建文件日志
-    :param do_task_filtering :是否执行基于函数参数的任务过滤
-    :param task_filtering_expire_seconds:任务过滤的失效期，为0则永久性过滤任务。例如设置过滤过期时间是1800秒 ，
-           30分钟前发布过1 + 2 的任务，现在仍然执行，
-           如果是30分钟以内发布过这个任务，则不执行1 + 2，现在把这个逻辑集成到框架，一般用于接口价格缓存。
-    :param is_do_not_run_by_specify_time_effect :是否使不运行的时间段生效
-    :param do_not_run_by_specify_time   :不运行的时间段
-    :param schedule_tasks_on_main_thread :直接在主线程调度任务，意味着不能直接在当前主线程同时开启两个消费者。fun.consume()就阻塞了，这之后的代码不会运行
-    :param function_result_status_persistance_conf   :配置。是否保存函数的入参，运行结果和运行状态到mongodb。
-           这一步用于后续的参数追溯，任务统计和web展示，需要安装mongo。
-    :param user_custom_record_process_info_func  提供一个用户自定义的保存消息处理记录到某个地方例如mysql数据库的函数，函数仅仅接受一个入参，入参类型是 FunctionResultStatus，用户可以打印参数
-    :param is_using_rpc_mode 是否使用rpc模式，可以在发布端获取消费端的结果回调，但消耗一定性能，使用async_result.result时候会等待阻塞住当前线程。。
-    :param broker_exclusive_config 加上一个不同种类中间件非通用的配置,不同中间件自身独有的配置，不是所有中间件都兼容的配置，因为框架支持30种消息队列，消息队列不仅仅是一般的先进先出queue这么简单的概念，
-            例如kafka支持消费者组，rabbitmq也支持各种独特概念例如各种ack机制 复杂路由机制，每一种消息队列都有独特的配置参数意义，可以通过这里传递。
-    :param broker_kind:中间件种类，支持30种消息队列。 入参见 BrokerEnum枚举类的属性。
-    :param boost_decorator_default_params: oostDecoratorDefaultParams是
-            @boost装饰器默认的全局入参。如果boost没有亲自指定某个入参，就自动使用funboost_config.py的BoostDecoratorDefaultParams中的配置。
-                    如果你嫌弃每个 boost 装饰器相同入参太多重复了，可以在 funboost_config.py 文件中设置boost装饰器的全局默认值。
-            BoostDecoratorDefaultParams() 实例化时候也可以传递这个boost装饰器任何的入参，BoostDecoratorDefaultParams是个数据类，百度python3.7dataclass的概念，类似。
-
-            funboost.funboost_config_deafult.BoostDecoratorDefaultParams 的值会自动被你项目根目录下的funboost_config.BoostDecoratorDefaultParams的值覆盖
-
-    """
-
-    """
-    这是此框架最重要的一个函数，必须看懂里面的入参有哪些。
-    此函数的入参意义请查看 get_consumer的入参注释。
-
-    本来是这样定义的，def boost(queue_name, **consumer_init_kwargs):
-    为了更好的ide智能补全，重复写全函数入参。
-
-    装饰器方式注册消费任务，如果有人过于喜欢装饰器方式，例如celery 装饰器方式的任务注册，觉得黑科技，那就可以使用这个装饰器。
-    假如你的函数名是f,那么可以调用f.publish或f.pub来发布任务。调用f.start_consuming_message 或 f.consume 或 f.start消费任务。
-    必要时候调用f.publisher.funcxx   和 f.conusmer.funcyy。
-
-
-    装饰器版，使用方式例如：
-    '''
-    @boost('queue_test_f01', qps=0.2, broker_kind=2)
-    def f(a, b):
-        print(a + b)
-
-    for i in range(10, 20):
-        f.pub(dict(a=i, b=i * 2))
-        f.push(i, i * 2)
-    f.consume()
-    # f.multi_process_conusme(8)             # # 这个是新加的方法，细粒度 线程 协程并发 同时叠加8个进程，速度炸裂。主要是无需导入run_consumer_with_multi_process函数。
-    # run_consumer_with_multi_process(f,8)   # 这个是细粒度 线程 协程并发 同时叠加8个进程，速度炸裂。
-    '''
-
-    常规方式，使用方式如下
-    '''
-    def f(a, b):
-        print(a + b)
-
-    consumer = get_consumer('queue_test_f01', consuming_function=f,qps=0.2, broker_kind=2)
-    # 需要手动指定consuming_function入参的值。
-    for i in range(10, 20):
-        consumer.publisher_of_same_queue.publish(dict(a=i, b=i * 2))
-    consumer.start_consuming_message()
-
-    '''
-
-    装饰器版本的 boost 入参 和 get_consumer 入参99%一致，唯一不同的是 装饰器版本加在了函数上自动知道消费函数了，
-    所以不需要传consuming_function参数。
-    """
-    # 装饰器版本能够自动知道消费函数，防止boost按照get_consumer的入参重复传参了consuming_function。
-    consumer_init_params_include_boost_decorator_default_params = copy.copy(locals())
-    consumer_init_params0 = copy.copy(consumer_init_params_include_boost_decorator_default_params)
-    consumer_init_params0.pop('boost_decorator_default_params')
-    consumer_init_params = copy.copy(consumer_init_params0)
-    for k, v in consumer_init_params0.items():
-        if v == _Undefined:
-            # print(k,v,boost_decorator_default_params[k])
-            consumer_init_params[k] = boost_decorator_default_params[k]
-
-    # print(consumer_init_params)
-    def _deco(func) -> IdeAutoCompleteHelper:  # 加这个-> 可以实现pycahrm动态补全
-
-        func.init_params = consumer_init_params
-        consumer = get_consumer(consuming_function=func, **consumer_init_params)
-        func.is_decorated_as_consume_function = True
-        func.consumer = consumer
-        func.queue_name = queue_name
-        # 下面这些连等主要是由于元编程造成的不能再ide下智能补全，参数太长很难手动拼写出来
-
-        func.publisher = consumer.publisher_of_same_queue
-        func.publish = func.pub = func.apply_async = consumer.publisher_of_same_queue.publish
-        func.push = func.delay = consumer.publisher_of_same_queue.push
-        func.multi_process_pub_params_list = partial(multi_process_pub_params_list, func)
-        func.clear = func.clear_queue = consumer.publisher_of_same_queue.clear
-        func.get_message_count = consumer.publisher_of_same_queue.get_message_count
-
-        func.start_consuming_message = func.consume = func.start = consumer.start_consuming_message
-        func.multi_process_start = func.multi_process_consume = partial(run_consumer_with_multi_process, func)
-        # if broker_kind == BrokerEnum.CELERY:   # celery作为消息队列
-        #     from multiprocessing import set_start_method
-        #     set_start_method('spawn', force=True)  # linux上运行需要这样。
-        #     func.consume = partial(func.multi_process_consume, 1)
-
-        func.fabric_deploy = partial(fabric_deploy, func)
-
-        func.clear_filter_tasks = consumer.clear_filter_tasks
-
-        func.wait_for_possible_has_finish_all_tasks = consumer.wait_for_possible_has_finish_all_tasks
-
-        func.pause = func.pause_consume = consumer.pause_consume
-        func.continue_consume = consumer.continue_consume
-
-        boost_queue__fun_map[queue_name] = func
-
-        # @wraps(func)
-        # def __deco(*args, **kwargs):  # 这样函数的id变化了，导致win在装饰器内部开多进程不方便。
-        #     return func(*args, **kwargs)
-        return func
-        # return __deco  # noqa # 两种方式都可以
-        # return update_wrapper(__deco, func)
-
-    return _deco  # noqa
-
-
-task_deco = boost  # 两个装饰器名字都可以。task_deco是原来名字，兼容一下。
```

## funboost/funboost_config_deafult.py

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from pathlib import Path
 import pytz
 from funboost.constant import BrokerEnum, ConcurrentModeEnum
-from funboost.helpers import FunctionResultStatusPersistanceConfig
+from funboost.core.function_result_status_saver import FunctionResultStatusPersistanceConfig
 from funboost.utils.simple_data_class import DataClassBase
 
 '''
 此文件是第一次运行框架自动生成刀项目根目录的，不需要用由户手动创建。
 此文件里面可以写任意python代码。例如 中间件 帐号 密码自己完全可以从apola配置中心获取或者从环境变量获取。
 '''
```

## funboost/consumers/base_consumer.py

```diff
@@ -27,29 +27,26 @@
 from functools import wraps
 import threading
 from threading import Lock, Thread
 import gevent
 import asyncio
 
 from apscheduler.jobstores.redis import RedisJobStore
-from apscheduler.schedulers.background import BackgroundScheduler
 from apscheduler.executors.pool import ThreadPoolExecutor as ApschedulerThreadPoolExecutor
-from apscheduler.events import EVENT_JOB_MISSED
 
 import pymongo
 from pymongo import IndexModel, ReplaceOne
 from pymongo.errors import PyMongoError
 
 import nb_log
 from funboost.concurrent_pool.single_thread_executor import SoloExecutor
-from funboost.helpers import FunctionResultStatusPersistanceConfig, boost_queue__fun_map
-
-from funboost.utils.apscheduler_monkey import patch_run_job as patch_apscheduler_run_job
+from funboost.core.function_result_status_saver import FunctionResultStatusPersistanceConfig, ResultPersistenceHelper, FunctionResultStatus
 
 # noinspection PyUnresolvedReferences
+from funboost.core.helper_funs import _delete_keys_and_return_new_dict, get_publish_time
 from nb_log import get_logger, LoggerLevelSetterMixin, LogManager, nb_print, LoggerMixin, \
     LoggerMixinDefaultWithFileHandler, stdout_write, stderr_write, is_main_process, \
     only_print_on_main_process, nb_log_config_default
 # noinspection PyUnresolvedReferences
 from funboost.concurrent_pool.async_helper import simple_run_in_executor
 from funboost.concurrent_pool.async_pool_executor import AsyncPoolExecutor
 # noinspection PyUnresolvedReferences
@@ -73,190 +70,26 @@
 # noinspection PyUnresolvedReferences
 from funboost.constant import ConcurrentModeEnum, BrokerEnum
 
 
 # patch_apscheduler_run_job()
 
 
-def _delete_keys_and_return_new_dict(dictx: dict, keys: list = None):
-    dict_new = copy.copy(dictx)  # 主要是去掉一级键 publish_time，浅拷贝即可。新的消息已经不是这样了。
-    keys = ['publish_time', 'publish_time_format', 'extra'] if keys is None else keys
-    for dict_key in keys:
-        try:
-            dict_new.pop(dict_key)
-        except KeyError:
-            pass
-    return dict_new
-
-
 class ExceptionForRetry(Exception):
     """为了重试的，抛出错误。只是定义了一个子类，用不用都可以，函数出任何类型错误了框架都会自动重试"""
 
 
 class ExceptionForRequeue(Exception):
     """框架检测到此错误，重新放回当前队列中"""
 
 
 class ExceptionForPushToDlxqueue(Exception):
     """框架检测到ExceptionForPushToDlxqueue错误，发布到死信队列"""
 
 
-def _get_publish_time(paramsx: dict):
-    """
-    原来存放控制参数的位置没想好，建议所有控制参数放到extra键的字典值里面。
-    :param paramsx:
-    :return:
-    """
-    return paramsx.get('extra', {}).get('publish_time', None) or paramsx.get('publish_time', None)
-
-
-class FunctionResultStatus(LoggerMixin, LoggerLevelSetterMixin):
-    host_name = socket.gethostname()
-    host_process = f'{host_name} - {os.getpid()}'
-    script_name_long = sys.argv[0]
-    script_name = script_name_long.split('/')[-1].split('\\')[-1]
-
-    FUNC_RUN_ERROR = 'FUNC_RUN_ERROR'
-
-    def __init__(self, queue_name: str, fucntion_name: str, msg_dict: dict):
-        # print(params)
-        self.queue_name = queue_name
-        self.function = fucntion_name
-        self.msg_dict = msg_dict
-        self.task_id = self.msg_dict.get('extra', {}).get('task_id', '')
-        self.process_id = os.getpid()
-        self.thread_id = threading.get_ident()
-        self.publish_time = publish_time = _get_publish_time(msg_dict)
-        if publish_time:
-            self.publish_time_str = time_util.DatetimeConverter(publish_time).datetime_str
-        function_params = _delete_keys_and_return_new_dict(msg_dict, )
-        self.params = function_params
-        self.params_str = json.dumps(function_params, ensure_ascii=False)
-        self.result = None
-        self.run_times = 0
-        self.exception = None
-        self.time_start = time.time()
-        self.time_cost = None
-        self.time_end = None
-        self.success = False
-        self.total_thread = threading.active_count()
-        self.has_requeue = False
-        self.has_to_dlx_queue = False
-        self.set_log_level(20)
-
-    def get_status_dict(self, without_datetime_obj=False):
-        self.time_end = time.time()
-        self.time_cost = round(self.time_end - self.time_start, 3)
-        item = self.__dict__
-        item['host_name'] = self.host_name
-        item['host_process'] = self.host_process
-        item['script_name'] = self.script_name
-        item['script_name_long'] = self.script_name_long
-        # item.pop('time_start')
-        datetime_str = time_util.DatetimeConverter().datetime_str
-        try:
-            json.dumps(item['result'])  # 不希望存不可json序列化的复杂类型。麻烦。存这种类型的结果是伪需求。
-        except TypeError:
-            item['result'] = str(item['result'])[:1000]
-        item.update({'insert_time_str': datetime_str,
-                     'insert_minutes': datetime_str[:-3],
-                     })
-        if not without_datetime_obj:
-            item.update({'insert_time': datetime.datetime.now(),
-                         'utime': datetime.datetime.utcnow(),
-                         })
-        else:
-            item = _delete_keys_and_return_new_dict(item, ['insert_time', 'utime'])
-        # kw['body']['extra']['task_id']
-        # item['_id'] = self.task_id.split(':')[-1] or str(uuid.uuid4())
-        item['_id'] = self.task_id or str(uuid.uuid4())
-        # self.logger.warning(item['_id'])
-        # self.logger.warning(item)
-        return item
-
-    def __str__(self):
-        return f'''{self.__class__}   {json.dumps(self.get_status_dict(), ensure_ascii=False)}'''
-
-
-class ResultPersistenceHelper(MongoMixin, LoggerMixin):
-    def __init__(self, function_result_status_persistance_conf: FunctionResultStatusPersistanceConfig, queue_name):
-        self.function_result_status_persistance_conf = function_result_status_persistance_conf
-        self._bulk_list = []
-        self._bulk_list_lock = Lock()
-        self._last_bulk_insert_time = 0
-        self._has_start_bulk_insert_thread = False
-        self._queue_name = queue_name
-        if self.function_result_status_persistance_conf.is_save_status:
-            self._create_indexes()
-            # self._mongo_bulk_write_helper = MongoBulkWriteHelper(task_status_col, 100, 2)
-            self.logger.info(f"函数运行状态结果将保存至mongo的 task_status 库的 {queue_name} 集合中，请确认 funboost.py文件中配置的 MONGO_CONNECT_URL")
-
-    def _create_indexes(self):
-        task_status_col = self.get_mongo_collection('task_status', self._queue_name)
-        try:
-            has_creat_index = False
-            index_dict = task_status_col.index_information()
-            if 'insert_time_str_-1' in index_dict:
-                has_creat_index = True
-            old_expire_after_seconds = None
-            for index_name, v in index_dict.items():
-                if index_name == 'utime_1':
-                    old_expire_after_seconds = v['expireAfterSeconds']
-            if has_creat_index is False:
-                # params_str 如果很长，必须使用TEXt或HASHED索引。
-                task_status_col.create_indexes([IndexModel([("insert_time_str", -1)]), IndexModel([("insert_time", -1)]),
-                                                IndexModel([("params_str", pymongo.TEXT)]), IndexModel([("success", 1)])
-                                                ], )
-                task_status_col.create_index([("utime", 1)],  # 这个是过期时间索引。
-                                             expireAfterSeconds=self.function_result_status_persistance_conf.expire_seconds)  # 只保留7天(用户自定义的)。
-            else:
-                if old_expire_after_seconds != self.function_result_status_persistance_conf.expire_seconds:
-                    self.logger.warning(f'过期时间从 {old_expire_after_seconds} 修改为 {self.function_result_status_persistance_conf.expire_seconds} 。。。')
-                    task_status_col.drop_index('utime_1', ),  # 这个不能也设置为True，导致修改过期时间不成功。
-                    task_status_col.create_index([("utime", 1)],
-                                                 expireAfterSeconds=self.function_result_status_persistance_conf.expire_seconds, background=True)  # 只保留7天(用户自定义的)。
-        except pymongo.errors.PyMongoError as e:
-            self.logger.warning(e)
-
-    def save_function_result_to_mongo(self, function_result_status: FunctionResultStatus):
-        if self.function_result_status_persistance_conf.is_save_status:
-            task_status_col = self.get_mongo_collection('task_status', self._queue_name)  # type: pymongo.collection.Collection
-            item = function_result_status.get_status_dict()
-            item2 = copy.copy(item)
-            if not self.function_result_status_persistance_conf.is_save_result:
-                item2['result'] = '不保存结果'
-            if item2['result'] is None:
-                item2['result'] = ''
-            if item2['exception'] is None:
-                item2['exception'] = ''
-            if self.function_result_status_persistance_conf.is_use_bulk_insert:
-                # self._mongo_bulk_write_helper.add_task(InsertOne(item2))  # 自动离散批量聚合方式。
-                with self._bulk_list_lock:
-                    self._bulk_list.append(ReplaceOne({'_id': item2['_id']}, item2, upsert=True))
-                    # if time.time() - self._last_bulk_insert_time > 0.5:
-                    #     self.task_status_col.bulk_write(self._bulk_list, ordered=False)
-                    #     self._bulk_list.clear()
-                    #     self._last_bulk_insert_time = time.time()
-                    if not self._has_start_bulk_insert_thread:
-                        self._has_start_bulk_insert_thread = True
-                        decorators.keep_circulating(time_sleep=0.2, is_display_detail_exception=True, block=False,
-                                                    daemon=False)(self._bulk_insert)()
-                        self.logger.warning(f'启动批量保存函数消费状态 结果到mongo的 线程')
-            else:
-                task_status_col.replace_one({'_id': item2['_id']}, item2, upsert=True)  # 立即实时插入。
-
-    def _bulk_insert(self):
-        with self._bulk_list_lock:
-            if time.time() - self._last_bulk_insert_time > 0.5 and self._bulk_list:
-                task_status_col = self.get_mongo_collection('task_status', self._queue_name)
-                task_status_col.bulk_write(self._bulk_list, ordered=False)
-                self._bulk_list.clear()
-                self._last_bulk_insert_time = time.time()
-
-
 # noinspection PyClassHasNoInit,DuplicatedCode
 class ConsumersManager:
     schedulal_thread_to_be_join = []
     consumers_queue__info_map = dict()
     consumers_queue__consumer_obj_map = dict()
     global_concurrent_mode = None
     schedual_task_always_use_thread = False
@@ -422,45 +255,49 @@
         2、启动 start_consuming_message 启动消费
         3、start_consuming_message 中 调用 _shedual_task 从中间件循环取消息
         4、 _shedual_task 中调用 _submit_task 运行 _run方法，将 任务 添加到并发池中并发运行。
         5、 消费函数执行完成后，运行 _confirm_consume , 确认消费。
         各种中间件的 取消息、确认消费 单独实现，其他逻辑由于采用了模板模式，自动复用代码。
 
         """
-
         self.init_params = copy.copy(locals())
         self.init_params.pop('self')
         self.init_params['broker_kind'] = self.__class__.BROKER_KIND
         self.init_params['consuming_function'] = consuming_function
-
+        # print(999, self.init_params)
         ConsumersManager.consumers_queue__info_map[queue_name] = current_queue__info_dict = copy.copy(self.init_params)
         ConsumersManager.consumers_queue__consumer_obj_map[queue_name] = self
         current_queue__info_dict['consuming_function'] = str(consuming_function)  # consuming_function.__name__
         current_queue__info_dict['specify_async_loop'] = str(specify_async_loop)
         current_queue__info_dict[
             'function_result_status_persistance_conf'] = function_result_status_persistance_conf.to_dict()
         current_queue__info_dict['class_name'] = self.__class__.__name__
         concurrent_name = ConsumersManager.get_concurrent_name_by_concurrent_mode(concurrent_mode)
         current_queue__info_dict['concurrent_mode_name'] = concurrent_name
 
         # 方便点击跳转定位到当前解释器下所有实例化消费者的文件行，点击可跳转到该处。
         # 获取被调用函数在被调用时所处代码行数
         # 直接实例化相应的类和使用工厂模式来实例化相应的类，得到的消费者实际实例化的行是不一样的，希望定位到用户的代码处，而不是定位到工厂模式处。也不要是boost装饰器本身处。
-        line = sys._getframe(0).f_back.f_lineno
-        # 获取被调用函数所在模块文件名
-        file_name = sys._getframe(1).f_code.co_filename
-        if 'consumer_factory.py' in file_name:
-            line = sys._getframe(1).f_back.f_lineno
-            file_name = sys._getframe(2).f_code.co_filename
-        if r'funboost\__init__.py' in file_name or 'funboost/__init__.py' in file_name:
-            line = sys._getframe(2).f_back.f_lineno
-            file_name = sys._getframe(3).f_code.co_filename
-        if r'funboost\helpers.py' in file_name or 'funboost/helpers.py' in file_name:
-            line = sys._getframe(3).f_back.f_lineno
-            file_name = sys._getframe(4).f_code.co_filename
+        # print(consuming_function,dir(consuming_function))
+        # print(dir(consuming_function.__code__))
+        file_name = consuming_function.__code__.co_filename
+        line = consuming_function.__code__.co_firstlineno
+        # line = sys._getframe(2).f_back.f_lineno
+        # # 获取被调用函数所在模块文件名
+        # file_name = sys._getframe(3).f_code.co_filename
+        # print(queue_name,line,file_name)
+        # if 'consumer_factory.py' in file_name:
+        #     line = sys._getframe(2).f_back.f_lineno
+        #     file_name = sys._getframe(3).f_code.co_filename
+        # if r'funboost\__init__.py' in file_name or 'funboost/__init__.py' in file_name:
+        #     line = sys._getframe(3).f_back.f_lineno
+        #     file_name = sys._getframe(4).f_code.co_filename
+        # if r'funboost\helpers.py' in file_name or 'funboost/helpers.py' in file_name:
+        #     line = sys._getframe(4).f_back.f_lineno
+        #     file_name = sys._getframe(5).f_code.co_filename
         current_queue__info_dict['where_to_instantiate'] = f'{file_name}:{line}'
 
         self._queue_name = queue_name
         self.queue_name = queue_name  # 可以换成公有的，免得外部访问有警告。
         if consuming_function is None:
             raise ValueError('必须传 consuming_function 参数')
         self.consuming_function = consuming_function
@@ -714,15 +551,16 @@
         self.logger.warning('启动延时任务sheduler')
 
     logger_apscheduler = nb_log.get_logger('push_for_apscheduler_use_database_store', log_filename='push_for_apscheduler_use_database_store.log')
 
     @classmethod
     def _push_for_apscheduler_use_database_store(cls, queue_name, msg, ):
         cls.logger_apscheduler.debug(f'延时任务用普通消息重新发布到普通队列 {msg}')
-        boost_queue__fun_map[queue_name].publish(msg)
+        from funboost.core.get_booster import get_booster
+        get_booster(queue_name).publish(msg)
 
     @abc.abstractmethod
     def _shedual_task(self):
         """
         每个子类必须实现这个的方法，完成如何从中间件取出消息，并将函数和运行参数添加到工作池。
         :return:
         """
@@ -746,15 +584,15 @@
 
         function_only_params = _delete_keys_and_return_new_dict(kw['body'], )
         if self._get_priority_conf(kw, 'do_task_filtering') and self._redis_filter.check_value_exists(
                 function_only_params):  # 对函数的参数进行检查，过滤已经执行过并且成功的任务。
             self.logger.warning(f'redis的 [{self._redis_filter_key_name}] 键 中 过滤任务 {kw["body"]}')
             self._confirm_consume(kw)
             return
-        publish_time = _get_publish_time(kw['body'])
+        publish_time = get_publish_time(kw['body'])
         msg_expire_senconds_priority = self._get_priority_conf(kw, 'msg_expire_senconds')
         if msg_expire_senconds_priority and time.time() - msg_expire_senconds_priority > publish_time:
             self.logger.warning(
                 f'消息发布时戳是 {publish_time} {kw["body"].get("publish_time_format", "")},距离现在 {round(time.time() - publish_time, 4)} 秒 ,'
                 f'超过了指定的 {msg_expire_senconds_priority} 秒，丢弃任务')
             self._confirm_consume(kw)
             return 0
@@ -1397,85 +1235,7 @@
             self._consumer._stop_flag = 0
 
         pause_flag = self.redis_db_frame.get(self._consumer._redis_key_pause_flag)
         if pause_flag is not None and int(pause_flag) == 1:
             self._consumer._pause_flag = 1
         else:
             self._consumer._pause_flag = 0
-
-
-class ActiveCousumerProcessInfoGetter(RedisMixin, LoggerMixinDefaultWithFileHandler):
-    """
-
-    获取分布式环境中的消费进程信息。
-    使用这里面的4个方法需要相应函数的@boost装饰器设置 is_send_consumer_hearbeat_to_redis=True，这样会自动发送活跃心跳到redis。否则查询不到该函数的消费者进程信息。
-    要想使用消费者进程信息统计功能，用户无论使用何种消息队列中间件类型，用户都必须安装redis，并在 funboost_config.py 中配置好redis链接信息
-    """
-
-    def _get_all_hearbeat_info_by_redis_key_name(self, redis_key):
-        results = self.redis_db_frame.smembers(redis_key)
-        # print(type(results))
-        # print(results)
-        # 如果所有机器所有进程都全部关掉了，就没办法还剩一个线程执行删除了，这里还需要判断一次15秒。
-        active_consumers_processor_info_list = []
-        for result in results:
-            result_dict = json.loads(result)
-            if self.timestamp() - result_dict['hearbeat_timestamp'] < 15:
-                active_consumers_processor_info_list.append(result_dict)
-        return active_consumers_processor_info_list
-
-    def get_all_hearbeat_info_by_queue_name(self, queue_name) -> typing.List[typing.Dict]:
-        """
-        根据队列名查询有哪些活跃的消费者进程
-        返回结果例子：
-        [{
-                "code_filename": "/codes/funboost/test_frame/my/test_consume.py",
-                "computer_ip": "172.16.0.9",
-                "computer_name": "VM_0_9_centos",
-                "consumer_id": 140477437684048,
-                "consumer_uuid": "79473629-b417-4115-b516-4365b3cdf383",
-                "consuming_function": "f2",
-                "hearbeat_datetime_str": "2021-12-27 19:22:04",
-                "hearbeat_timestamp": 1640604124.4643965,
-                "process_id": 9665,
-                "queue_name": "test_queue72c",
-                "start_datetime_str": "2021-12-27 19:21:24",
-                "start_timestamp": 1640604084.0780013
-            }, ...............]
-        """
-        redis_key = f'funboost_hearbeat_queue__dict:{queue_name}'
-        return self._get_all_hearbeat_info_by_redis_key_name(redis_key)
-
-    def get_all_hearbeat_info_by_ip(self, ip=None) -> typing.List[typing.Dict]:
-        """
-        根据机器的ip查询有哪些活跃的消费者进程，ip不传参就查本机ip使用funboost框架运行了哪些消费进程，传参则查询任意机器的消费者进程信息。
-        返回结果的格式和上面的 get_all_hearbeat_dict_by_queue_name 方法相同。
-        """
-        ip = ip or nb_log_config_default.computer_ip
-        redis_key = f'funboost_hearbeat_server__dict:{ip}'
-        return self._get_all_hearbeat_info_by_redis_key_name(redis_key)
-
-    def _get_all_hearbeat_info_partition_by_redis_key_prefix(self, redis_key_prefix):
-        keys = self.redis_db_frame.scan(0, f'{redis_key_prefix}*', 10000)[1]
-        infos_map = {}
-        for key in keys:
-            key = key.decode()
-            infos = self.redis_db_frame.smembers(key)
-            dict_key = key.replace(redis_key_prefix, '')
-            infos_map[dict_key] = []
-            for info_str in infos:
-                info_dict = json.loads(info_str)
-                if self.timestamp() - info_dict['hearbeat_timestamp'] < 15:
-                    infos_map[dict_key].append(info_dict)
-        return infos_map
-
-    def get_all_hearbeat_info_partition_by_queue_name(self) -> typing.Dict[typing.AnyStr, typing.List[typing.Dict]]:
-        """获取所有队列对应的活跃消费者进程信息，按队列名划分,不需要传入队列名，自动扫描redis键。请不要在 funboost_config.py 的redis 指定的db中放太多其他业务的缓存键值对"""
-        infos_map = self._get_all_hearbeat_info_partition_by_redis_key_prefix('funboost_hearbeat_queue__dict:')
-        self.logger.info(f'获取所有队列对应的活跃消费者进程信息，按队列名划分，结果是 {json.dumps(infos_map, indent=4)}')
-        return infos_map
-
-    def get_all_hearbeat_info_partition_by_ip(self) -> typing.Dict[typing.AnyStr, typing.List[typing.Dict]]:
-        """获取所有机器ip对应的活跃消费者进程信息，按机器ip划分,不需要传入机器ip，自动扫描redis键。请不要在 funboost_config.py 的redis 指定的db中放太多其他业务的缓存键值对 """
-        infos_map = self._get_all_hearbeat_info_partition_by_redis_key_prefix('funboost_hearbeat_server__dict:')
-        self.logger.info(f'获取所有机器ip对应的活跃消费者进程信息，按机器ip划分，结果是 {json.dumps(infos_map, indent=4)}')
-        return infos_map
```

## funboost/consumers/celery_consumer.py

```diff
@@ -159,15 +159,15 @@
         # 这就是核心，@boost时候回注册任务路由到celery_app
         @celery_app.task(name=self.queue_name, rate_limit=f'{self._qps}/s', soft_time_limit=self._function_timeout,
                          max_retries=self._max_retry_times,
                          **self.broker_exclusive_config['celery_task_config'])
         def f(*args, **kwargs):
             self.logger.debug(f' 这条消息是 celery 从 {self.queue_name} 队列中取出 ,是由 celery 框架调度 {self.consuming_function.__name__} 函数处理: args:  {args} ,  kwargs: {kwargs}')
             return self.consuming_function(*args, **kwargs)
-
+        self.celery_task = f
         CeleryHelper.concurrent_mode = self._concurrent_mode
 
     def start_consuming_message(self):
         # 不单独每个函数都启动一次celery的worker消费，是把要消费的 queue name放到列表中，CeleryHelper.realy_start_celery_worker 一次性启动多个函数消费。
         CeleryHelper.to_be_start_work_celery_queue_name_set.add(self.queue_name)
         super().start_consuming_message()
```

## funboost/factories/broker_kind__publsiher_consumer_type_map.py

```diff
@@ -83,14 +83,21 @@
 }
 
 for broker_kindx, cls_tuple in broker_kind__publsiher_consumer_type_map.items():
     cls_tuple[1].BROKER_KIND = broker_kindx
 
 
 def register_custom_broker(broker_kind, publisher_class: typing.Type[AbstractPublisher], consumer_class: typing.Type[AbstractConsumer]):
+    """
+    动态注册中间件到框架中， 方便的增加中间件类型或者修改是自定义消费者逻辑。
+    :param broker_kind:
+    :param publisher_class:
+    :param consumer_class:
+    :return:
+    """
     if not issubclass(publisher_class, AbstractPublisher):
         raise TypeError(f'publisher_class 必须是 AbstractPublisher 的子或孙类')
     if not issubclass(consumer_class, AbstractConsumer):
         raise TypeError(f'consumer_class 必须是 AbstractConsumer 的子或孙类')
     broker_kind__publsiher_consumer_type_map[broker_kind] = (publisher_class, consumer_class)
     consumer_class.BROKER_KIND = broker_kind
```

## funboost/publishers/base_publisher.py

```diff
@@ -15,15 +15,15 @@
 import datetime
 import amqpstorm
 from kombu.exceptions import KombuError
 from pikav1.exceptions import AMQPError as PikaAMQPError
 
 from nb_log import LoggerLevelSetterMixin, get_logger, LoggerMixin
 
-from funboost.publishers.msg_result_getter import AsyncResult, AioAsyncResult, HasNotAsyncResult, ResultFromMongo
+from funboost.core.msg_result_getter import AsyncResult, AioAsyncResult
 from funboost.utils import decorators, time_util
 from funboost import funboost_config_deafult
 
 RedisAsyncResult = AsyncResult  # 别名
 RedisAioAsyncResult = AioAsyncResult  # 别名
 
 
@@ -202,19 +202,19 @@
         if 'extra' in msg:
             msg_function_kw.pop('extra')
             raw_extra = msg['extra']
         if self.publish_params_checker:
             self.publish_params_checker.check_params(msg_function_kw)
         task_id = task_id or f'{self._queue_name}_result:{uuid.uuid4()}'
         extra_params = {'task_id': task_id, 'publish_time': round(time.time(), 4),
-                                       'publish_time_format': time.strftime('%Y-%m-%d %H:%M:%S')}
+                        'publish_time_format': time.strftime('%Y-%m-%d %H:%M:%S')}
         if priority_control_config:
             extra_params.update(priority_control_config.to_dict())
         extra_params.update(raw_extra)
-        msg['extra'] =extra_params
+        msg['extra'] = extra_params
         t_start = time.time()
         decorators.handle_exception(retry_times=10, is_throw_error=True, time_sleep=0.1)(
             self.concrete_realization_of_publish)(json.dumps(msg, ensure_ascii=False))
         self.logger.debug(f'向{self._queue_name} 队列，推送消息 耗时{round(time.time() - t_start, 4)}秒  {msg_function_kw}')  # 显示msg太长了。
         with self._lock_for_count:
             self.count_per_minute += 1
             self.publish_msg_num_total += 1
```

## funboost/timing_job/__init__.py

```diff
@@ -13,17 +13,18 @@
 from apscheduler.schedulers.background import BackgroundScheduler
 from apscheduler.jobstores.redis import RedisJobStore
 # noinspection PyProtectedMember
 from apscheduler.schedulers.base import STATE_STOPPED, STATE_RUNNING
 from apscheduler.util import undefined
 import deprecated
 
-from funboost import funboost_config_deafult, boost_queue__fun_map
+from funboost import funboost_config_deafult
 
 from funboost.consumers.base_consumer import AbstractConsumer
+from funboost.core.get_booster import get_booster
 from funboost.publishers.base_publisher import AbstractPublisher
 
 
 def timing_publish_deco(consuming_func_decorated_or_consumer: Union[callable, AbstractConsumer]):
     def _deco(*args, **kwargs):
         if getattr(consuming_func_decorated_or_consumer, 'is_decorated_as_consume_function', False) is True:
             consuming_func_decorated_or_consumer.push(*args, **kwargs)
@@ -31,25 +32,28 @@
             consuming_func_decorated_or_consumer.publisher_of_same_queue.push(*args, **kwargs)
         else:
             raise TypeError('consuming_func_decorated_or_consumer 必须是被 boost 装饰的函数或者consumer类型')
 
     return _deco
 
 
-def _add_push_job(queue_name, *args, **kwargs, ):
-    boost_queue__fun_map[queue_name].push(*args, **kwargs)
+def push_fun_params_to_broker(queue_name: str, *args, **kwargs, ):
+    """
+    *args **kwargs 是消费函数的入参
+    """
+    get_booster(queue_name).push(*args, **kwargs)
 
 
-class FsdfBackgroundScheduler(BackgroundScheduler):
+class FunboostBackgroundScheduler(BackgroundScheduler):
     """
-    自定义的，添加一个方法add_timing_publish_job
+    自定义的， 继承了官方BackgroundScheduler，
+    通过重写 _main_loop ，使得动态修改增加删除定时任务配置更好。
     """
 
-    # noinspection PyShadowingBuiltins
-    @deprecated.deprecated(reason='不使用这种方式，对于job_store为数据库时候需要序列化不好。使用内存和数据库都兼容的添加任务方式: add_push_job')
+    @deprecated.deprecated(reason='以后不要再使用这种方式，对于job_store为数据库时候需要序列化不好。使用内存和数据库都兼容的添加任务方式: add_push_job')
     def add_timing_publish_job(self, func, trigger=None, args=None, kwargs=None, id=None, name=None,
                                misfire_grace_time=undefined, coalesce=undefined, max_instances=undefined,
                                next_run_time=undefined, jobstore='default', executor='default',
                                replace_existing=False, **trigger_args):
         return self.add_job(timing_publish_deco(func), trigger, args, kwargs, id, name,
                             misfire_grace_time, coalesce, max_instances,
                             next_run_time, jobstore, executor,
@@ -74,21 +78,26 @@
         :param executor:
         :param replace_existing:
         :param trigger_args:
         :return:
         """
         # args = args or {}
         # kwargs['queue_name'] = func.queue_name
+
+        """
+        用户如果不使用funboost的 FunboostBackgroundScheduler 类型对象，而是使用原生的apscheduler类型对象，可以scheduler.add_jon(push_fun_params_to_broker,args=(,),kwargs={}) 
+        push_fun_params_to_broker函数入参是消费函数队列的 queue_name 加上 原消费函数的入参
+        """
         if args is None:
             args = (func.queue_name,)
         else:
             args_list = list(args)
             args_list.insert(0, func.queue_name)
             args = tuple(args_list)
-        return self.add_job(_add_push_job, trigger, args, kwargs, id, name,
+        return self.add_job(push_fun_params_to_broker, trigger, args, kwargs, id, name,
                             misfire_grace_time, coalesce, max_instances,
                             next_run_time, jobstore, executor,
                             replace_existing, **trigger_args)
 
     def start(self, paused=False, block_exit=True):
         # def _block_exit():
         #     while True:
@@ -99,15 +108,15 @@
         def _when_exit():
             while 1:
                 # print('阻止退出')
                 time.sleep(100)
 
         if block_exit:
             atexit.register(_when_exit)
-        super(FsdfBackgroundScheduler, self).start(paused=paused, )
+        super().start(paused=paused, )
         # _block_exit()   # python3.9 判断守护线程结束必须主线程在运行，否则结尾
 
     def _main_loop00000(self):
         """
         原来的代码是这，动态添加任务不友好。
         :return:
         """
@@ -129,39 +138,41 @@
         while self.state == STATE_RUNNING:
             if wait_seconds is None:
                 wait_seconds = MAX_WAIT_SECONDS_FOR_NEX_PROCESS_JOBS
             time.sleep(min(wait_seconds, MAX_WAIT_SECONDS_FOR_NEX_PROCESS_JOBS))  # 这个要取最小值，不然例如定时间隔0.1秒运行，不取最小值，不会每隔0.1秒运行。
             wait_seconds = self._process_jobs()
 
 
-FunboostBackgroundScheduler = FsdfBackgroundScheduler
+FsdfBackgroundScheduler = FunboostBackgroundScheduler  # 兼容一下名字，fsdf是 function-scheduling-distributed-framework 老框架名字的缩写
+# funboost_aps_scheduler定时配置基于内存的，不可以跨机器远程动态添加/修改/删除定时任务配置。如果需要动态增删改查定时任务，可以使用funboost_background_scheduler_redis_store
+
 funboost_aps_scheduler = FunboostBackgroundScheduler(timezone=funboost_config_deafult.TIMEZONE, daemon=False, )
-fsdf_background_scheduler = funboost_aps_scheduler  # funboost_aps_scheduler定时配置基于内存的，不可以跨机器远程动态添加/修改/删除定时任务配置。如果需要动态增删改查定时任务，可以使用funboost_background_scheduler_redis_store
+fsdf_background_scheduler = funboost_aps_scheduler  # 兼容一下老名字。
 
 if __name__ == '__main__':
     # 定时运行消费演示
     import datetime
     from funboost import boost, BrokerEnum, fsdf_background_scheduler, timing_publish_deco
 
 
     @boost('queue_test_666', broker_kind=BrokerEnum.LOCAL_PYTHON_QUEUE)
     def consume_func(x, y):
         print(f'{x} + {y} = {x + y}')
 
 
     # 定时每隔3秒执行一次。
     funboost_aps_scheduler.add_push_job(consume_func,
-                                      'interval', id='3_second_job', seconds=3, kwargs={"x": 5, "y": 6})
+                                        'interval', id='3_second_job', seconds=3, kwargs={"x": 5, "y": 6})
 
     # 定时，只执行一次
     funboost_aps_scheduler.add_push_job(consume_func,
-                                      'date', run_date=datetime.datetime(2020, 7, 24, 13, 53, 6), args=(5, 6,))
+                                        'date', run_date=datetime.datetime(2020, 7, 24, 13, 53, 6), args=(5, 6,))
 
     # 定时，每天的11点32分20秒都执行一次。
     funboost_aps_scheduler.add_push_job(consume_func,
-                                                     'cron', day_of_week='*', hour=18, minute=22, second=20, args=(5, 6,))
+                                        'cron', day_of_week='*', hour=18, minute=22, second=20, args=(5, 6,))
 
     # 启动定时
     funboost_aps_scheduler.start()
 
     # 启动消费
     consume_func.consume()
```

## Comparing `funboost/publishers/msg_result_getter.py` & `funboost/core/msg_result_getter.py`

 * *Files identical despite different names*

## Comparing `funboost-21.2.dist-info/LICENSE` & `funboost-23.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `funboost-21.2.dist-info/METADATA` & `funboost-23.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funboost
-Version: 21.2
+Version: 23.0
 Summary: pip install funboost，python全功能分布式函数调度框架,。支持python所有类型的并发模式和一切知名消息队列中间件，python函数加速器，框架包罗万象，一统编程思维，兼容50% python业务场景，适用范围广。只需要一行代码即可分布式执行python一切函数，99%用过funboost的pythoner 感受是 方便 快速 强大，相见恨晚 
 Home-page: https://github.com/ydf0509/funboost
 Author: bfzs
 Author-email: ydf0509@sohu.com
 Maintainer: ydf
 Maintainer-email: ydf0509@sohu.com
 License: BSD License
```

## Comparing `funboost-21.2.dist-info/RECORD` & `funboost-23.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-funboost/__init__.py,sha256=5zaThJG6_jGSf5KyOKDcAscxjy55qAE7Px-FYcNPoO8,21054
+funboost/__init__.py,sha256=CZQbANWNTSr7o7WUTw60sR3Nzs8NS5pzXEb1yCnW0tQ,2154
+funboost/__init__0000.py,sha256=cSzw-ZQqtAAp5_-7eONXQT5fwz_JbZlRjDQPASDLUHk,20378
 funboost/constant.py,sha256=44kHqCwIiab7itJZeu1bk-QSUOy7V0T3etGtfeS3ViM,6154
-funboost/funboost_config_deafult.py,sha256=9TclPwAQvX3GxsMXBKHFxPTKOqWgXD0o6zkl68MoRtQ,7332
-funboost/helpers.py,sha256=0Z5hsNL1iBNr98S71SqHc0AXXW1umhjXMjrrEzDUe5I,14135
+funboost/funboost_config_deafult.py,sha256=CSawbw5Yzkk73wMNOxhxkrkncS-OOSEYismtbK547xA,7358
 funboost/set_frame_config.py,sha256=hz_38C-IXEulYpHQdr1fhsMcdEDCHIsF2la8MkHiIjA,9149
 funboost/assist/celery_helper.py,sha256=iv6gY47nm1agS6E8q8FybhkzWUlYJ8Dej8R1LJCMSiI,3987
 funboost/assist/dramatiq_helper.py,sha256=lRNouO8MyCB_Qj2ppYG4FbMpf-2Aok8QhtGZLH1zWkg,2089
 funboost/assist/huey_helper.py,sha256=VEzMdQDVJJ-ujcOXKw7chrTgvieLz4si3hrjt8gIK38,1760
 funboost/beggar_version_implementation/beggar_redis_consumer.py,sha256=aiucCkj7-GWbLMIWHhevdQrAsxzyc55AL69fue8esYs,3930
 funboost/concurrent_pool/__init__.py,sha256=dGgxgzMSwcXWMexwAnojsML7EMjHAAsmAofNgrxtl2w,759
 funboost/concurrent_pool/async_helper.py,sha256=iyb0Jcjyx-vkUGC_saSUWqN657kcR5K7B-L_SB6cDCE,3256
@@ -20,16 +20,16 @@
 funboost/concurrent_pool/custom_threadpool_executor000.py,sha256=jJLXy3h-bELap6nZA6yLtdozzTWcvCtZ7IY6MTqLEAM,9317
 funboost/concurrent_pool/single_thread_executor.py,sha256=NDWOegh8Nxpb-Bp-lUlj-DONWvepSmA9qepL1yNgdQI,373
 funboost/concurrent_pool/backup/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/concurrent_pool/backup/async_pool_executor0223.py,sha256=iTxxJFk2lu1P9ZAIkBip3euq3oEQ4_qTODy3xUaOecY,9548
 funboost/concurrent_pool/backup/async_pool_executor_back.py,sha256=vIgUUyF4Zb0jIRPWgNPqyO09YEkQP32kkpGBldqm4qA,9568
 funboost/concurrent_pool/backup/async_pool_executor_janus.py,sha256=OHMWJ9l3EYTpPpcrPrGGKd4K0tmQ2PN8HiX0Dta0EOo,5728
 funboost/consumers/__init__.py,sha256=ZXY_6Kut1VYNQiF5aWEgIWobsW1ht9YUP0TdRZRWFqI,126
-funboost/consumers/base_consumer.py,sha256=WOdyiVIKWvhHWbl6H1KVgBEFKeyuGwINoOXvr6RFt_E,96486
-funboost/consumers/celery_consumer.py,sha256=hRDgS384h4vyhZT2ryqRqNT6khA8Kj80Wlb1iW1XKQc,7546
+funboost/consumers/base_consumer.py,sha256=hn61aaexSs2j3kmUFd9ChRASZLozRzfyvuhyPZGUcT4,83054
+funboost/consumers/celery_consumer.py,sha256=6CqorZH5pbxIjVwn5gNzcxSbos5YWT8eYqxYyYjgUcY,7574
 funboost/consumers/celery_consumer000.py,sha256=8SF8ppHIMH-BIAHO0NyJYnSQxe_PcT6hv05e7DySG54,4574
 funboost/consumers/confirm_mixin.py,sha256=H0w07PceU2gGf6X1EXvAB5oD7IavzGv96bQTxm-58sE,5877
 funboost/consumers/dramatiq_consumer.py,sha256=kiHM1wpSZykYDomtSGZ2PlMInCDn_8GOGEHqHUD9m0o,2144
 funboost/consumers/http_consumer.py,sha256=3HF8tsH90fUPX3iOmVid_nqW_7hZCFaL7feOkuAM36U,2025
 funboost/consumers/http_consumer000.py,sha256=NXOSiN1qpLAJfJkuF6SjFpWQ28YxMDULzWCBTNMwYe8,4463
 funboost/consumers/httpsqs_consumer.py,sha256=LICZzovaMVrZsJY4GgLrk3EaHz8f9ZZBLKZtWl3frMc,1080
 funboost/consumers/huey_consumer.py,sha256=_Z2lpfAzvs1HqkSouncN7eH1VfyQJPYNZNgv1FbZj-U,1856
@@ -61,16 +61,28 @@
 funboost/consumers/tcp_consumer.py,sha256=hgjcXOtHyGBDS_h_p0gbOtF__Ba6DS1Chk5P9nc6Its,2045
 funboost/consumers/txt_file_consumer.py,sha256=rd8F7liwUfidk7SXY-qF4Iamx-U1NXJBYsOhOudFyyU,1340
 funboost/consumers/udp_consumer.py,sha256=J-G1ZYktXZ_er_1fg3FdSPVl4V_eEIHZXlBadCNpJmE,1643
 funboost/consumers/zeromq_consumer.py,sha256=7V1RwZKtPDDpjKTKj4GWGuz1AGZ83EBHCnWuYN4ooSM,4157
 funboost/contrib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/contrib/queue2queue.py,sha256=I6e1d2s_TQ_29rbwSs3KuA7Tuj9B905EcJruT287CnM,4680
 funboost/contrib/redis_consume_latest_msg_broker.py,sha256=V-8-pOyotOXNbs2olS7vig-yN1PxRdw_MeLOtpUufJc,1817
+funboost/core/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+funboost/core/active_cousumer_info_getter.py,sha256=VwVRxsApdKqnoBdg1PsHEkyWiOFJMm0_qWIdCFbPOWg,4984
+funboost/core/booster.py,sha256=xNQZt0UXzXdzk77pGiRs4hx_7BMOvLcgJz8bJXdC_6w,16419
+funboost/core/exit_signal.py,sha256=0nlDrtZnaHfYoumRXmXpeveUMvLT1iWoxfrBX2HR5OM,421
+funboost/core/fabric_deploy_helper.py,sha256=yIdWhlJAR1rCpzvcSme-KrU7RwKH8B7tdwHG-q6QH0U,8875
+funboost/core/function_result_status_config.py,sha256=CE7xaGoL7vT2VsLTHvv-EnJE7K83XVWivBimHVmVfnQ,1570
+funboost/core/function_result_status_saver.py,sha256=6dMLpa74t3zsHF20lqfgAdCeRD1yc1oJcw--Usk-A3c,8819
+funboost/core/get_booster.py,sha256=nDD8LXanCb1h07bpgWAD113ct32XT1r6B9l6pTftnrk,1299
+funboost/core/global_boosters.py,sha256=q6-A3-H6RyKAhFofiunpn4XCtFfXumO7mcfLPXXFGX8,168
+funboost/core/helper_funs.py,sha256=hoT3IqsKCxlzF7KosvbWzE1VP4_oONIR8e86O4Phhb4,604
+funboost/core/msg_result_getter.py,sha256=a2ffSE8Rvz1t1KVEt4UxIPsWgcriaHE_Armkac-JrJY,7782
+funboost/core/muliti_process_enhance.py,sha256=ukqVJ2oPkqZvqAD8YgK1HiZRc0UoLqV96Ke0ctU1yEc,3766
 funboost/factories/__init__.py,sha256=s7kKKjR1HU5eMjPD6r5b-SXTVMo1zBp2JjOAtkyt5Yo,178
-funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=iHMW83XCoXZqLx7zgmvAKNakqor-mjaU1q4QPRK_at0,8191
+funboost/factories/broker_kind__publsiher_consumer_type_map.py,sha256=NFfHQHJuxBxg3icnpZD0y_vlKBf8mhQpZ43tf_O6c2s,8420
 funboost/factories/consumer_factory.py,sha256=KFvYkx1a7egtSiTLuVsoRMKLUAotx-QJX1jAI8Xzo3s,946
 funboost/factories/publisher_factotry.py,sha256=Vz66GrCxMt7GV5iqyIXSzZcC_eHF8fj-2kYduzbTTpg,2281
 funboost/function_result_web/app.py,sha256=xUSDBwwDA5wQVWFdFBXj9Y1s7BOh2itUw5pCZl0URMw,4841
 funboost/function_result_web/functions.py,sha256=OIPMxc4jv51qnhBxFGfTZnpMx5p4lQflPoTviDTbJUc,7345
 funboost/function_result_web/__pycache__/app.cpython-37.pyc,sha256=p-jwU7xf31KOJhmhNXqj6J79PTxjMbiTU16gAotpSEw,4045
 funboost/function_result_web/__pycache__/functions.cpython-37.pyc,sha256=KuU8DnYhFpYN0p9rdDXE9mqFuE7eKkcXHCNze3aAdOw,3921
 funboost/function_result_web/static/assets/css/custom.css,sha256=3brvjy2aBOTIXcTUK4NV6dX5wFRqx6K2aLu_jQn63jM,7674
@@ -83,28 +95,27 @@
 funboost/function_result_web/static/images/password.png,sha256=0jRivuQAhWKtkS73p8f_KiLy3D39_flqVTrpFKJPNqk,546
 funboost/function_result_web/static/images/tick.png,sha256=S9dZYN4HQzw7JsWPw3ut1dQp4OTJ_Uh2Qp2KUDF1Jv8,2912
 funboost/function_result_web/static/images/user.png,sha256=HxLjNc83WZzZEscZRdmVhGKlPXNdp_EKmmYxafuyb3g,622
 funboost/function_result_web/static/js/jquery-1.11.0.min.js,sha256=ryQZ3RXgnqkTz-lNEw-YcEhnMuV3ZODwLqOEbyBBRu4,96383
 funboost/function_result_web/templates/index.html,sha256=dWe-JFQhsDpoNjSsBF4P6SJWp_KvHX8EP_yECS5r7_o,19501
 funboost/function_result_web/templates/login.html,sha256=q37dj7O0LeyiV38Zd5P1Qn_qmhjdFomuYTRY1Yk48Bo,2007
 funboost/publishers/__init__.py,sha256=xqBHlvsJQVPfbdvP84G0LHmVB7-pFBS7vDnX1Uo9pVY,131
-funboost/publishers/base_publisher.py,sha256=hFHMGGoPdCBgJ1xVQ2buXnX21e-Hp0AHuzRuNKf5dDw,15103
+funboost/publishers/base_publisher.py,sha256=Pq11w95VVPKQ5D9NEz9a3MuZa2YLplDmAI3F4TQI2OM,15047
 funboost/publishers/celery_publisher.py,sha256=OSNra9kx1_iSOc5WkqMTBkMvICBdRI2Eww1YVtf-eEE,3724
 funboost/publishers/celery_publisher000.py,sha256=ag2s7MzPPrnNdza3u8vcbDJqtiqbQw4lJJzAVuJ6GF0,3897
 funboost/publishers/confluent_kafka_publisher.py,sha256=cpbyWvZ0T_kM62LWeBKRUuEuMkJAKOof97UUMSz6-Dk,3541
 funboost/publishers/dramatiq_publisher.py,sha256=RoZzfvkS5H-XXcmHGBomuvkQRQBlVyiaCdWpgy0LL9o,1410
 funboost/publishers/http_publisher.py,sha256=pS3z_AVqH6h4PAgqB7usihvzLJP5ZzfPKQRMQfHrJHQ,753
 funboost/publishers/httpsqs_publisher.py,sha256=7cf5ijwrbp4smq6ofndrKisruAqG0Wzfo_d_7bnLUk4,2783
 funboost/publishers/huey_publisher.py,sha256=z1CF18YZkQY6lqeoc6tiJkaYsRjRicbhYYeoHSvdD-w,1101
 funboost/publishers/kafka_publisher.py,sha256=cmlJ0mvwq0Ajlth4VQqwnoe6v_bZ4eIz49GgkiJr-ZU,2160
 funboost/publishers/kombu_publisher.py,sha256=TJt24M_Y4x8wjXHFl2hp6z3Dat6rjuA_xGiqA8RbRLg,5321
 funboost/publishers/local_python_queue_publisher.py,sha256=veskMS5tjeneYU9HmrJLXZSK9_UT48NzHzcljjOoy3g,1365
 funboost/publishers/mongomq_publisher.py,sha256=xQr3KMQEKksX4OEvzPlCl8v1VeBHaoZtYw2QujOUyGo,1874
 funboost/publishers/mqtt_publisher.py,sha256=NKVDE5R12QL99IXgRjJtF4phyW8QaXKxHkqW5p_kXr4,3050
-funboost/publishers/msg_result_getter.py,sha256=a2ffSE8Rvz1t1KVEt4UxIPsWgcriaHE_Armkac-JrJY,7782
 funboost/publishers/nameko_publisher.py,sha256=HtR8I_NemyJCO2KL-w8geNMhZcoj06_95QZ8qq1-gog,2147
 funboost/publishers/nats_publisher.py,sha256=hFfaQovij9dm8w-iRN0SgiHHoS_TlrTAjw42dPwCLSA,776
 funboost/publishers/nsq_publisher.py,sha256=Go4UjLd_Vt4JuVtfkmCuuXrmxUXv1y6NaBQJX6s1XUo,1302
 funboost/publishers/peewee_publisher.py,sha256=RsYAqBKf_ZLxkGJeZPWExzG4cpUac7weCeNhcSQ9hZc,1095
 funboost/publishers/persist_queue_publisher.py,sha256=x6qRiR3Ln-jX9KPC5GvBzUzAlmZ0HDjU1KTnILXVJrw,2540
 funboost/publishers/pulsar_publisher.py,sha256=3BqDtywExvTIw1KZWG4kT1uz029uw2YkntLggZ-Ao6A,1238
 funboost/publishers/rabbitmq_amqpstorm_publisher.py,sha256=0o6D7xD8wDalj-FEWfqkZBr_HjyUKRf_CsGOq6_8ygA,2725
@@ -120,15 +131,15 @@
 funboost/publishers/tcp_publisher.py,sha256=qMecOpgVqwTy-VYyevv4mCR6H5bQhCirRbJmcJIaFCE,1335
 funboost/publishers/txt_file_publisher.py,sha256=twTrqRAYnaNmFkXn0nr1xGBjeHCPJStt83voLX3vPao,1380
 funboost/publishers/udp_publisher.py,sha256=TOiKrhmCMjx4teqIgdUwRic0lxyK2cupinafsz--wzY,1194
 funboost/publishers/zeromq_publisher.py,sha256=QCsRDtmgxOdVe2F2z3PwvvkoXv1flmrHWo3Nzsx0X7g,1002
 funboost/queues/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 funboost/queues/peewee_queue.py,sha256=AJlfXWSRK6GdwV8znBZasEum-VFsKHHh3YoUPK_3QVI,4944
 funboost/queues/sqla_queue.py,sha256=PxkMyXHCA_Je7H_p8c81QT7qN8x8Fq6NVmwli7PPhhg,11024
-funboost/timing_job/__init__.py,sha256=NR3UHIKoUKUROrnO6UTLLDNJ4Z66brvDMZRQ-SdvrOw,7307
+funboost/timing_job/__init__.py,sha256=c9w4iakbF9LYqsZqeRKw01UbL80ftoD8HXCAtXOnwxU,7919
 funboost/timing_job/apscheduler_use_mysql_store.py,sha256=zIeK2LETm8m3VX7K6but8YAQOZomfO-P6AKLqeluxys,418
 funboost/timing_job/apscheduler_use_redis_store.py,sha256=zG2QSJYnDm6pgTwbyU3wvtr3GHKhlR9fonc5Fba1F5I,876
 funboost/utils/__init__.py,sha256=9YTXH5jt-_MulaWy5cbIpiJghy-fVQU9Gd1RHSajI94,1951
 funboost/utils/apscheduler_monkey.py,sha256=CcUISbqX6nMWSxr_QjZ26IvvhUk_ojYZWRaKenpsKfE,3124
 funboost/utils/block_exit.py,sha256=BnfxNYo3lnmhk686RAEoc4u3D4RU_iEMMMgu5L8gIuI,96
 funboost/utils/bulk_operation.py,sha256=jty8pvQWCPVUmfqeP6DnilveGc6YGjCMwVbnOAV4eRg,9972
 funboost/utils/custom_pysnooper.py,sha256=7yXLKEMY_JjPRRt0Y0N-wV2CFhILlYNh40Y6uRBUaj8,5923
@@ -213,12 +224,12 @@
 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-37.pyc,sha256=67Zqz4tjErzQSm9FM9mGaY3uMHYOUj3QYKtPqJQvQpE,303
 funboost/utils/dependency_packages_in_pythonpath/func_timeout/__pycache__/py3_raise.cpython-39.pyc,sha256=a1ajayGg3JjQz--IC3-6YQHRFStG9etoieY8mXEdJ6Q,311
 funboost/utils/pysnooper_ydf/__init__.py,sha256=ctbQdJpLVZ5g_PPstj7Xaqcl0sMIgvUGwZXtcogYyHA,909
 funboost/utils/pysnooper_ydf/pycompat.py,sha256=ehsCfjsLdwoK0_o5fwYWDo3WeqCVfHW5lxekrEZxq4Y,2243
 funboost/utils/pysnooper_ydf/tracer.py,sha256=DYxYeRFSH1jXy4OTB5KIAgQm2EHRWEOwq3EXJig7Yrk,19131
 funboost/utils/pysnooper_ydf/utils.py,sha256=evSmGi_Oul7vSP47AJ0DLjFwoCYCfunJZ1mWxAkwPZw,2753
 funboost/utils/pysnooper_ydf/variables.py,sha256=QejRDESBA06KG9OH4sBT4J1M55eaU29EIHg8K_igaXo,3693
-funboost-21.2.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-funboost-21.2.dist-info/METADATA,sha256=9js1hsMskITgusFK5DfwWRLs8Su0dzBJxiCq87XjCWU,26423
-funboost-21.2.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
-funboost-21.2.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
-funboost-21.2.dist-info/RECORD,,
+funboost-23.0.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+funboost-23.0.dist-info/METADATA,sha256=OUxG861Z20n9X1M-h41oPeLXJarDNg65cnBnTK6XYrE,26423
+funboost-23.0.dist-info/WHEEL,sha256=D1Wh14kWDxPnrM-5t_6UCB-UuQNrEODtRa3vF4OsvQY,97
+funboost-23.0.dist-info/top_level.txt,sha256=K8WuKnS6MRcEWxP1NvbmCeujJq6TEfbsB150YROlRw0,9
+funboost-23.0.dist-info/RECORD,,
```

