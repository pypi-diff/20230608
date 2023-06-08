# Comparing `tmp/fabric_cf-1.5.0b3.tar.gz` & `tmp/fabric_cf-1.5.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric_cf-1.5.0b3.tar", last modified: Thu May 11 16:37:50 2023, max compression
+gzip compressed data, was "fabric_cf-1.5.0b4.tar", last modified: Thu Jun  8 15:00:41 2023, max compression
```

## Comparing `fabric_cf-1.5.0b3.tar` & `fabric_cf-1.5.0b4.tar`

### file list

```diff
@@ -1,517 +1,525 @@
--rw-r--r--   0        0        0     2035 2023-05-11 16:37:35.592130 fabric_cf-1.5.0b3/.gitignore
--rw-r--r--   0        0        0      851 2023-05-11 16:32:26.699200 fabric_cf-1.5.0b3/Dockerfile-auth
--rw-r--r--   0        0        0      769 2023-05-11 16:32:36.872162 fabric_cf-1.5.0b3/Dockerfile-broker
--rw-r--r--   0        0        0     1037 2023-05-11 16:32:57.016934 fabric_cf-1.5.0b3/Dockerfile-cf
--rw-r--r--   0        0        0      787 2023-05-11 16:32:47.114231 fabric_cf-1.5.0b3/Dockerfile-orchestrator
--rw-r--r--   0        0        0     1071 2023-04-03 14:50:53.535054 fabric_cf-1.5.0b3/LICENSE
--rw-r--r--   0        0        0     2046 2023-04-03 14:50:53.535620 fabric_cf-1.5.0b3/README.md
--rwxr-xr-x   0        0        0       74 2023-04-03 14:50:53.535840 fabric_cf-1.5.0b3/authority.sh
--rwxr-xr-x   0        0        0       79 2023-04-03 14:50:53.535996 fabric_cf-1.5.0b3/broker.sh
--rw-r--r--   0        0        0      947 2023-04-03 14:50:53.536169 fabric_cf-1.5.0b3/cleanup_old_schema_from_schema_registry.sh
--rw-r--r--   0        0        0     2861 2023-04-03 19:02:18.268979 fabric_cf-1.5.0b3/docker-compose-kafka.yaml
--rw-r--r--   0        0        0     1560 2023-04-03 14:50:53.536634 fabric_cf-1.5.0b3/docker-compose-no-ssl-kafka.yaml
--rw-r--r--   0        0        0    10757 2023-04-03 19:05:05.566974 fabric_cf-1.5.0b3/docker-compose-test.yaml
--rwxr-xr-x   0        0        0       45 2023-04-03 14:50:53.536998 fabric_cf-1.5.0b3/docker-entrypoint.sh
--rw-r--r--   0        0        0      350 2023-04-03 14:50:53.537353 fabric_cf-1.5.0b3/env.template
--rw-r--r--   0        0        0     1135 2023-04-03 17:25:25.716942 fabric_cf-1.5.0b3/env.template.test
--rw-r--r--   0        0        0    16609 2023-04-03 14:50:53.537818 fabric_cf-1.5.0b3/fabricNo.AnyActorNoPolicy.xml
--rw-r--r--   0        0        0     6343 2023-04-03 14:50:53.538166 fabric_cf-1.5.0b3/fabric_cf/Design.md
--rw-r--r--   0        0        0       24 2023-05-11 16:34:38.443594 fabric_cf-1.5.0b3/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.538462 fabric_cf-1.5.0b3/fabric_cf/actor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.538776 fabric_cf-1.5.0b3/fabric_cf/actor/boot/__init__.py
--rw-r--r--   0        0        0    15281 2023-04-03 14:50:53.539116 fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration.py
--rw-r--r--   0        0        0     1268 2023-04-03 14:50:53.539529 fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_exception.py
--rw-r--r--   0        0        0     2509 2023-04-03 14:50:53.539906 fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_loader.py
--rw-r--r--   0        0        0    23003 2023-05-11 15:20:50.246839 fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_processor.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.540419 fabric_cf-1.5.0b3/fabric_cf/actor/boot/inventory/__init__.py
--rw-r--r--   0        0        0     4969 2023-04-03 14:50:53.540687 fabric_cf-1.5.0b3/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.540852 fabric_cf-1.5.0b3/fabric_cf/actor/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.541039 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/__init__.py
--rw-r--r--   0        0        0     4907 2023-04-03 14:50:53.541250 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_container.py
--rw-r--r--   0        0        0     1530 2023-04-03 14:50:53.541590 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_event.py
--rw-r--r--   0        0        0     2176 2023-04-03 14:50:53.541925 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_identity.py
--rw-r--r--   0        0        0     1991 2023-04-03 14:50:53.542388 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_management_object.py
--rw-r--r--   0        0        0    21765 2023-04-03 14:50:53.542778 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_mixin.py
--rw-r--r--   0        0        0     1918 2023-04-03 14:50:53.543106 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_proxy.py
--rw-r--r--   0        0        0     1323 2023-04-03 14:50:53.543429 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_runnable.py
--rw-r--r--   0        0        0     4497 2023-04-03 14:50:53.543679 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority.py
--rw-r--r--   0        0        0     8736 2023-04-03 14:50:53.543930 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_policy.py
--rw-r--r--   0        0        0     3299 2023-04-03 14:50:53.544153 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_proxy.py
--rw-r--r--   0        0        0     3367 2023-04-03 14:50:53.545583 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_reservation.py
--rw-r--r--   0        0        0     6071 2023-04-03 14:50:53.545879 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_base_plugin.py
--rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.546104 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_mixin.py
--rw-r--r--   0        0        0     1492 2023-04-03 14:50:53.546359 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py
--rw-r--r--   0        0        0     3690 2023-04-03 14:50:53.546566 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_proxy.py
--rw-r--r--   0        0        0     4012 2023-04-03 14:50:53.546780 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_reservation.py
--rw-r--r--   0        0        0     2442 2023-04-03 14:50:53.547038 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_callback_proxy.py
--rw-r--r--   0        0        0     9216 2023-04-03 14:50:53.547299 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_actor.py
--rw-r--r--   0        0        0     6215 2023-04-11 13:18:18.781604 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_actor_management_object.py
--rw-r--r--   0        0        0     2640 2023-04-03 14:50:53.547942 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_callback_proxy.py
--rw-r--r--   0        0        0     5802 2023-04-03 14:50:53.548385 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_policy.py
--rw-r--r--   0        0        0     7724 2023-04-03 14:50:53.548730 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_reservation.py
--rw-r--r--   0        0        0     1936 2023-04-03 14:50:53.548982 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_component.py
--rw-r--r--   0        0        0     9833 2023-04-03 14:50:53.549228 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_concrete_set.py
--rw-r--r--   0        0        0     2729 2023-04-03 14:50:53.549801 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_container_clock.py
--rw-r--r--   0        0        0     3976 2023-04-03 14:50:53.550228 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_container_database.py
--rw-r--r--   0        0        0     3367 2023-04-03 14:50:53.550497 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller.py
--rw-r--r--   0        0        0     2423 2023-04-03 14:50:53.550710 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py
--rw-r--r--   0        0        0     2787 2023-04-03 14:50:53.550900 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_policy.py
--rw-r--r--   0        0        0     5715 2023-04-03 14:50:53.551118 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_reservation.py
--rw-r--r--   0        0        0    10332 2023-05-11 15:20:50.247543 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_database.py
--rw-r--r--   0        0        0    11026 2023-04-03 14:50:53.551566 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_delegation.py
--rw-r--r--   0        0        0     1867 2023-04-03 14:50:53.551767 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_event.py
--rw-r--r--   0        0        0     1943 2023-04-03 14:50:53.552014 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_management_object.py
--rw-r--r--   0        0        0     9044 2023-04-03 14:50:53.552250 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_actor.py
--rw-r--r--   0        0        0     2534 2023-04-03 14:50:53.552486 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_authority.py
--rw-r--r--   0        0        0     1452 2023-04-03 14:50:53.552674 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py
--rw-r--r--   0        0        0     6191 2023-04-03 14:50:53.552834 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py
--rw-r--r--   0        0        0     5041 2023-04-03 14:50:53.553039 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_container.py
--rw-r--r--   0        0        0     2317 2023-04-03 14:50:53.553242 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py
--rw-r--r--   0        0        0     5014 2023-04-03 14:50:53.553457 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py
--rw-r--r--   0        0        0    11147 2023-04-03 14:50:53.553629 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_policy.py
--rw-r--r--   0        0        0     2304 2023-04-03 14:50:53.553847 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_proxy.py
--rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.554059 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_proxy_factory.py
--rw-r--r--   0        0        0     1658 2023-04-03 14:50:53.554593 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_query_response_handler.py
--rw-r--r--   0        0        0    14096 2023-04-03 14:50:53.554880 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_mixin.py
--rw-r--r--   0        0        0     9388 2023-04-03 14:50:53.555129 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_resources.py
--rw-r--r--   0        0        0     5581 2023-04-03 14:50:53.555376 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_status.py
--rw-r--r--   0        0        0     8963 2023-04-03 14:50:53.555582 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_resource_control.py
--rw-r--r--   0        0        0     1336 2023-04-03 14:50:53.555785 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_response_handler.py
--rw-r--r--   0        0        0     2246 2023-04-03 14:50:53.556014 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_rpc_request_state.py
--rw-r--r--   0        0        0     5634 2023-04-03 14:50:53.556345 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_actor.py
--rw-r--r--   0        0        0     6415 2023-04-03 14:50:53.556589 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_policy.py
--rw-r--r--   0        0        0     4846 2023-04-03 14:50:53.556782 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_reservation.py
--rw-r--r--   0        0        0    13280 2023-04-03 14:50:53.557016 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_slice.py
--rw-r--r--   0        0        0     3227 2023-04-03 14:50:53.557270 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_substrate.py
--rw-r--r--   0        0        0     2225 2023-04-03 14:50:53.557477 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_substrate_database.py
--rw-r--r--   0        0        0     2943 2023-04-03 14:50:53.557727 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_tick.py
--rw-r--r--   0        0        0     6121 2023-04-03 14:50:53.557931 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_ticker.py
--rw-r--r--   0        0        0     1590 2023-04-03 14:50:53.558112 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_timer_queue.py
--rw-r--r--   0        0        0     1387 2023-04-03 14:50:53.558344 fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_timer_task.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.558543 fabric_cf-1.5.0b3/fabric_cf/actor/core/common/__init__.py
--rw-r--r--   0        0        0    12749 2023-04-03 14:50:53.558881 fabric_cf-1.5.0b3/fabric_cf/actor/core/common/constants.py
--rw-r--r--   0        0        0     3254 2023-04-03 14:50:53.559144 fabric_cf-1.5.0b3/fabric_cf/actor/core/common/event_logger.py
--rw-r--r--   0        0        0     5517 2023-04-03 14:50:53.559364 fabric_cf-1.5.0b3/fabric_cf/actor/core/common/exceptions.py
--rw-r--r--   0        0        0     6108 2023-04-03 14:50:53.559599 fabric_cf-1.5.0b3/fabric_cf/actor/core/common/resource_config.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.559841 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/__init__.py
--rw-r--r--   0        0        0    24564 2023-04-03 14:50:53.560251 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/container.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.560471 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/db/__init__.py
--rw-r--r--   0        0        0     8667 2023-05-11 15:20:50.248592 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/db/container_database.py
--rw-r--r--   0        0        0    19263 2023-04-03 14:50:53.561010 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/globals.py
--rw-r--r--   0        0        0     7053 2023-04-03 14:50:53.561272 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/maintenance.py
--rw-r--r--   0        0        0     5472 2023-04-03 14:50:53.561525 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/message_service.py
--rw-r--r--   0        0        0     1508 2023-04-03 14:50:53.561724 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/protocol_descriptor.py
--rw-r--r--   0        0        0    13005 2023-04-03 14:50:53.562081 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/remote_actor_cache.py
--rw-r--r--   0        0        0     8040 2023-04-03 14:50:53.562299 fabric_cf-1.5.0b3/fabric_cf/actor/core/container/rpc_producer.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.562481 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/__init__.py
--rw-r--r--   0        0        0    35633 2023-05-11 15:20:50.249090 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/actor.py
--rw-r--r--   0        0        0     1975 2023-04-03 14:50:53.563319 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/actor_identity.py
--rw-r--r--   0        0        0    14656 2023-04-03 14:50:53.563570 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/authority.py
--rw-r--r--   0        0        0     4845 2023-04-03 14:50:53.563854 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/authority_policy.py
--rw-r--r--   0        0        0    20313 2023-04-03 14:50:53.564180 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/broker.py
--rw-r--r--   0        0        0     5914 2023-04-03 14:50:53.565067 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/broker_policy.py
--rw-r--r--   0        0        0    19290 2023-05-11 15:20:50.249428 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/controller.py
--rw-r--r--   0        0        0     8604 2023-05-11 15:20:50.249865 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/event_processor.py
--rw-r--r--   0        0        0     5467 2023-04-03 14:50:53.565861 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/inventory_slice_manager.py
--rw-r--r--   0        0        0     6171 2023-04-03 14:50:53.566145 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/policy.py
--rw-r--r--   0        0        0     2042 2023-04-03 14:50:53.566366 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/rpc_request_state.py
--rw-r--r--   0        0        0     8688 2023-04-03 14:50:53.566587 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/ticket.py
--rw-r--r--   0        0        0    15442 2023-05-11 15:20:50.250153 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/unit.py
--rw-r--r--   0        0        0    13263 2023-04-03 14:50:53.567022 fabric_cf-1.5.0b3/fabric_cf/actor/core/core/unit_set.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.567201 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/__init__.py
--rw-r--r--   0        0        0    10969 2023-04-03 14:50:53.567422 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/broker_delegation.py
--rw-r--r--   0        0        0     1874 2023-04-03 14:50:53.567633 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/broker_delegation_factory.py
--rw-r--r--   0        0        0    16897 2023-04-03 14:50:53.567918 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/delegation.py
--rw-r--r--   0        0        0     1825 2023-04-03 14:50:53.568190 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/delegation_factory.py
--rw-r--r--   0        0        0     5364 2023-04-03 14:50:53.568399 fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/resource_ticket.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.568570 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/__init__.py
--rw-r--r--   0        0        0    27428 2023-04-03 14:50:53.568871 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/authority_reservation.py
--rw-r--r--   0        0        0     3384 2023-04-03 14:50:53.569249 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/broker_query_model_publisher.py
--rw-r--r--   0        0        0    26805 2023-04-03 14:50:53.569537 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/broker_reservation.py
--rw-r--r--   0        0        0     2992 2023-04-03 14:50:53.569880 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/claim_timeout.py
--rw-r--r--   0        0        0     4396 2023-04-03 14:50:53.570217 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/failed_rpc.py
--rw-r--r--   0        0        0     3639 2023-04-03 14:50:53.570449 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/failed_rpc_event.py
--rw-r--r--   0        0        0     2668 2023-04-03 14:50:53.570827 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py
--rw-r--r--   0        0        0     2708 2023-04-03 14:50:53.571106 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_failed_rpc.py
--rw-r--r--   0        0        0     2105 2023-04-03 14:50:53.571543 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_query_rpc.py
--rw-r--r--   0        0        0     2703 2023-04-03 14:50:53.571750 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py
--rw-r--r--   0        0        0     4158 2023-04-03 14:50:53.571968 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_rpc.py
--rw-r--r--   0        0        0    10748 2023-05-11 15:20:50.250399 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_rpc_event.py
--rw-r--r--   0        0        0    63706 2023-05-11 15:20:50.282572 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel.py
--rw-r--r--   0        0        0     3314 2023-04-03 14:50:53.572703 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel_tick.py
--rw-r--r--   0        0        0    55548 2023-05-11 15:20:50.250916 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel_wrapper.py
--rw-r--r--   0        0        0     2363 2023-04-03 14:50:53.573675 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/predecessor_state.py
--rw-r--r--   0        0        0     2860 2023-04-03 14:50:53.573873 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/query_timeout.py
--rw-r--r--   0        0        0     1404 2023-04-03 14:50:53.574038 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/request_types.py
--rw-r--r--   0        0        0    24493 2023-04-03 14:51:26.321598 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation.py
--rw-r--r--   0        0        0    89315 2023-05-11 15:20:50.251560 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_client.py
--rw-r--r--   0        0        0     9994 2023-04-03 14:50:53.575366 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_server.py
--rw-r--r--   0        0        0     3263 2023-04-03 14:50:53.575644 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_states.py
--rw-r--r--   0        0        0    20888 2023-04-03 14:50:53.575901 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/resource_set.py
--rw-r--r--   0        0        0     1614 2023-04-03 14:50:53.576176 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/retry_rpc.py
--rw-r--r--   0        0        0     1899 2023-04-03 14:50:53.576398 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/retry_rpc_event.py
--rw-r--r--   0        0        0     4128 2023-04-03 14:50:53.576854 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_executor.py
--rw-r--r--   0        0        0    31229 2023-05-11 15:20:50.251975 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_manager.py
--rw-r--r--   0        0        0     1772 2023-04-03 14:50:53.577467 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_manager_singleton.py
--rw-r--r--   0        0        0     3579 2023-04-03 14:50:53.577700 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_request.py
--rw-r--r--   0        0        0     1620 2023-04-03 14:50:53.577956 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_request_type.py
--rw-r--r--   0        0        0     1340 2023-04-03 14:50:53.578168 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/sequence_comparison_codes.py
--rw-r--r--   0        0        0    12284 2023-04-03 14:50:53.578451 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice.py
--rw-r--r--   0        0        0    12613 2023-05-11 16:31:49.234715 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice_state_machine.py
--rw-r--r--   0        0        0     8319 2023-04-03 14:50:53.578901 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice_table.py
--rw-r--r--   0        0        0     6527 2023-04-03 14:50:53.579044 fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/tick.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.579204 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/__init__.py
--rw-r--r--   0        0        0    37415 2023-05-11 15:20:50.252308 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/actor_management_object.py
--rw-r--r--   0        0        0     8431 2023-04-03 14:50:53.579975 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/authority_management_object.py
--rw-r--r--   0        0        0     6903 2023-04-11 13:18:18.767746 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/broker_management_object.py
--rw-r--r--   0        0        0    27727 2023-05-11 15:22:36.518505 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/client_actor_management_object_helper.py
--rw-r--r--   0        0        0     9605 2023-04-03 14:50:53.580935 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/container_management_object.py
--rw-r--r--   0        0        0     8973 2023-04-11 13:18:18.771385 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/controller_management_object.py
--rw-r--r--   0        0        0    13007 2023-04-03 14:50:53.581333 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/converter.py
--rw-r--r--   0        0        0     1624 2023-04-03 14:50:53.581543 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/error.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.581729 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/__init__.py
--rw-r--r--   0        0        0    10194 2023-04-03 14:50:53.582040 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_actor.py
--rw-r--r--   0        0        0     3509 2023-04-03 14:50:53.582317 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_authority.py
--rw-r--r--   0        0        0     8200 2023-05-11 15:20:50.252529 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_broker.py
--rw-r--r--   0        0        0     4483 2023-04-03 14:50:53.583057 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_container.py
--rw-r--r--   0        0        0     5300 2023-04-03 14:50:53.583248 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_controller.py
--rw-r--r--   0        0        0     5462 2023-04-03 14:50:53.583439 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py
--rw-r--r--   0        0        0     6960 2023-05-11 16:31:49.235814 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_proxy.py
--rw-r--r--   0        0        0     5730 2023-04-03 14:50:53.583847 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.584078 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/__init__.py
--rw-r--r--   0        0        0    24550 2023-04-03 14:50:53.584410 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py
--rw-r--r--   0        0        0     5715 2023-04-03 14:50:53.584691 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py
--rw-r--r--   0        0        0     5797 2023-04-03 14:50:53.585104 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py
--rw-r--r--   0        0        0    15846 2023-04-03 14:50:53.585409 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py
--rw-r--r--   0        0        0     4008 2023-04-03 14:50:53.585584 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py
--rw-r--r--   0        0        0     8228 2023-04-03 14:50:53.585867 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py
--rw-r--r--   0        0        0     2148 2023-04-03 14:50:53.586169 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_service.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.586361 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/__init__.py
--rw-r--r--   0        0        0    10935 2023-04-03 14:50:53.586634 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_actor.py
--rw-r--r--   0        0        0     3902 2023-04-03 14:50:53.586852 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_authority.py
--rw-r--r--   0        0        0     8391 2023-04-03 14:50:53.587036 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_broker.py
--rw-r--r--   0        0        0    10119 2023-04-03 14:50:53.587201 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_container.py
--rw-r--r--   0        0        0     9395 2023-04-03 14:50:53.587383 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_controller.py
--rw-r--r--   0        0        0     2855 2023-04-03 14:50:53.587571 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_proxy.py
--rw-r--r--   0        0        0     8655 2023-04-03 14:50:53.587724 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_server_actor.py
--rw-r--r--   0        0        0     7217 2023-04-03 14:50:53.588020 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_object.py
--rw-r--r--   0        0        0     7841 2023-04-03 14:50:53.588258 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_object_manager.py
--rw-r--r--   0        0        0     4972 2023-04-03 14:50:53.588521 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_utils.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.588706 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/__init__.py
--rw-r--r--   0        0        0     1604 2023-04-03 14:50:53.588914 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/client_mng.py
--rw-r--r--   0        0        0     1570 2023-04-03 14:50:53.589110 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/event_mng.py
--rw-r--r--   0        0        0     1802 2023-04-03 14:50:53.589285 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py
--rw-r--r--   0        0        0     1741 2023-04-03 14:50:53.589460 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/result_client_mng.py
--rw-r--r--   0        0        0     1554 2023-04-03 14:50:53.589750 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/result_event_mng.py
--rw-r--r--   0        0        0     1904 2023-04-03 14:50:53.590017 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py
--rw-r--r--   0        0        0    15777 2023-04-03 14:50:53.590202 fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/server_actor_management_object.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.590369 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/__init__.py
--rw-r--r--   0        0        0     7756 2023-04-03 14:50:53.590739 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/base_plugin.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.590945 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/__init__.py
--rw-r--r--   0        0        0    31456 2023-05-11 15:20:50.253712 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/actor_database.py
--rw-r--r--   0        0        0     2624 2023-05-11 15:20:50.254268 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/client_database.py
--rw-r--r--   0        0        0     3792 2023-05-11 15:20:50.254603 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/server_actor_database.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.591940 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/__init__.py
--rw-r--r--   0        0        0    12823 2023-04-03 14:50:53.592182 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py
--rw-r--r--   0        0        0     2831 2023-04-03 14:50:53.592374 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/config_token.py
--rw-r--r--   0        0        0     2286 2023-04-03 14:50:53.592660 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py
--rw-r--r--   0        0        0     7114 2023-05-11 15:20:50.254849 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/handler_processor.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.593035 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/__init__.py
--rw-r--r--   0        0        0     3612 2023-04-03 14:50:53.593263 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/authority_substrate.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.593460 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/db/__init__.py
--rw-r--r--   0        0        0     4365 2023-05-11 15:20:50.255164 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py
--rw-r--r--   0        0        0    14268 2023-04-03 14:50:53.594012 fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.594246 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/__init__.py
--rw-r--r--   0        0        0    28295 2023-04-03 14:50:53.594548 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/authority_calendar_policy.py
--rw-r--r--   0        0        0     8891 2023-04-03 14:50:53.595030 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/broker_calendar_policy.py
--rw-r--r--   0        0        0    63111 2023-04-03 14:50:53.595571 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/broker_simpler_units_policy.py
--rw-r--r--   0        0        0    19840 2023-05-11 15:20:50.255474 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_calendar_policy.py
--rw-r--r--   0        0        0     9815 2023-05-11 15:20:50.255764 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_simple_policy.py
--rw-r--r--   0        0        0     9546 2023-05-11 15:20:50.255972 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_ticket_review_policy.py
--rw-r--r--   0        0        0     1814 2023-04-03 14:50:53.596494 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/fifo_queue.py
--rw-r--r--   0        0        0     2981 2023-04-03 14:50:53.596828 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/inventory.py
--rw-r--r--   0        0        0     2785 2023-04-03 14:50:53.597031 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/inventory_for_type.py
--rw-r--r--   0        0        0    14499 2023-04-03 14:50:53.597231 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_node_control.py
--rw-r--r--   0        0        0    28363 2023-04-03 14:50:53.597532 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_node_inventory.py
--rw-r--r--   0        0        0     5435 2023-04-03 14:50:53.597856 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_service_control.py
--rw-r--r--   0        0        0    22745 2023-04-03 14:50:53.598106 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_service_inventory.py
--rw-r--r--   0        0        0     2032 2023-04-03 14:50:53.598641 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/queue_wrapper.py
--rw-r--r--   0        0        0     5157 2023-04-03 14:50:53.598857 fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/resource_control.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.599020 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/__init__.py
--rw-r--r--   0        0        0     1821 2023-04-03 14:50:53.599277 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/actor_location.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.599432 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/__init__.py
--rw-r--r--   0        0        0     7798 2023-04-03 14:50:53.599583 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py
--rw-r--r--   0        0        0     9013 2023-04-03 14:50:53.599758 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py
--rw-r--r--   0        0        0     6686 2023-04-03 14:50:53.599942 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py
--rw-r--r--   0        0        0     4809 2023-04-03 14:50:53.600099 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py
--rw-r--r--   0        0        0     8466 2023-04-03 14:50:53.600393 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_retun.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.600601 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/__init__.py
--rw-r--r--   0        0        0    11710 2023-04-03 14:50:53.600939 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/actor_service.py
--rw-r--r--   0        0        0     6931 2023-04-03 14:50:53.601111 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/authority_service.py
--rw-r--r--   0        0        0     8218 2023-04-03 14:50:53.601343 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/broker_service.py
--rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.601562 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/controller_service.py
--rw-r--r--   0        0        0    15551 2023-04-03 14:50:53.601817 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/translate.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.601999 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/__init__.py
--rw-r--r--   0        0        0     4525 2023-04-03 14:50:53.602224 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_authority.py
--rw-r--r--   0        0        0     5726 2023-04-03 14:50:53.602562 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_broker.py
--rw-r--r--   0        0        0     6896 2023-04-03 14:50:53.603120 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_proxy.py
--rw-r--r--   0        0        0     2868 2023-04-03 14:50:53.604580 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_proxy_factory.py
--rw-r--r--   0        0        0     6397 2023-04-03 14:50:53.605005 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_return.py
--rw-r--r--   0        0        0     8303 2023-04-03 14:50:53.605283 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/proxy.py
--rw-r--r--   0        0        0     3013 2023-04-03 14:50:53.605545 fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/proxy_factory.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.605762 fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/__init__.py
--rw-r--r--   0        0        0     7672 2023-04-03 14:50:53.605950 fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/actor_registry.py
--rw-r--r--   0        0        0     2177 2023-04-03 14:50:53.606181 fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/callback_registry.py
--rw-r--r--   0        0        0     4926 2023-04-03 14:50:53.606408 fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/peer_registry.py
--rw-r--r--   0        0        0     3912 2023-04-03 14:50:53.606565 fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/proxy_registry.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.606740 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/__init__.py
--rw-r--r--   0        0        0     7165 2023-04-03 14:50:53.606931 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/actor_clock.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.607146 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/__init__.py
--rw-r--r--   0        0        0     8224 2023-04-03 14:50:53.607463 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/authority_calendar.py
--rw-r--r--   0        0        0     1667 2023-04-03 14:50:53.607755 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/base_calendar.py
--rw-r--r--   0        0        0    11573 2023-04-03 14:50:53.607991 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/broker_calendar.py
--rw-r--r--   0        0        0     9733 2023-04-03 14:50:53.608213 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/client_calendar.py
--rw-r--r--   0        0        0     5239 2023-04-03 14:50:53.608505 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/controller_calendar.py
--rw-r--r--   0        0        0     2550 2023-04-03 14:50:53.608738 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/source_calendar.py
--rw-r--r--   0        0        0    15769 2023-04-03 14:50:53.609015 fabric_cf-1.5.0b3/fabric_cf/actor/core/time/term.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.609215 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/__init__.py
--rw-r--r--   0        0        0     2213 2023-04-03 14:50:53.609476 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/bids.py
--rw-r--r--   0        0        0     2905 2023-04-03 14:50:53.609992 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/client.py
--rw-r--r--   0        0        0     2063 2023-04-03 14:50:53.610294 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/graceful_interrupt_handler.py
--rw-r--r--   0        0        0     2163 2023-04-03 14:50:53.610582 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/id.py
--rw-r--r--   0        0        0     1488 2023-04-03 14:50:53.610758 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/iterable_queue.py
--rw-r--r--   0        0        0     2263 2023-04-03 14:50:53.611043 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/kernel_timer.py
--rw-r--r--   0        0        0     2905 2023-04-03 14:50:53.611261 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/log_helper.py
--rw-r--r--   0        0        0     2238 2023-04-03 14:50:53.611511 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/notice.py
--rw-r--r--   0        0        0     1999 2023-04-03 14:50:53.611700 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reflection_utils.py
--rw-r--r--   0        0        0     8380 2023-04-03 14:50:53.612072 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_holdings.py
--rw-r--r--   0        0        0     8864 2023-04-03 14:50:53.612305 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_list.py
--rw-r--r--   0        0        0     6700 2023-05-11 15:20:50.256475 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_set.py
--rw-r--r--   0        0        0     3144 2023-04-03 14:50:53.612687 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_state.py
--rw-r--r--   0        0        0     2250 2023-04-03 14:50:53.612855 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/resource_type.py
--rw-r--r--   0        0        0     1690 2023-04-03 14:50:53.613024 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/rpc_exception.py
--rw-r--r--   0        0        0     4440 2023-04-03 14:50:53.613195 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/update_data.py
--rw-r--r--   0        0        0     4188 2023-04-03 14:50:53.613384 fabric_cf-1.5.0b3/fabric_cf/actor/core/util/utils.py
--rw-r--r--   0        0        0     7474 2023-04-03 14:50:53.613876 fabric_cf-1.5.0b3/fabric_cf/actor/db/__init__.py
--rw-r--r--   0        0        0    58450 2023-05-11 15:20:50.257173 fabric_cf-1.5.0b3/fabric_cf/actor/db/psql_database.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.614689 fabric_cf-1.5.0b3/fabric_cf/actor/fim/__init__.py
--rw-r--r--   0        0        0     6326 2023-05-11 15:20:50.257526 fabric_cf-1.5.0b3/fabric_cf/actor/fim/asm_update_thread.py
--rw-r--r--   0        0        0    28243 2023-05-11 15:20:50.258048 fabric_cf-1.5.0b3/fabric_cf/actor/fim/fim_helper.py
--rw-r--r--   0        0        0        1 2023-04-03 14:50:53.616623 fabric_cf-1.5.0b3/fabric_cf/actor/fim/plugins/__init__.py
--rw-r--r--   0        0        0        1 2023-04-03 14:50:53.616848 fabric_cf-1.5.0b3/fabric_cf/actor/fim/plugins/broker/__init__.py
--rw-r--r--   0        0        0    23622 2023-04-03 14:50:53.617119 fabric_cf-1.5.0b3/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.617325 fabric_cf-1.5.0b3/fabric_cf/actor/handlers/__init__.py
--rw-r--r--   0        0        0     2842 2023-04-03 14:50:53.617552 fabric_cf-1.5.0b3/fabric_cf/actor/handlers/handler_base.py
--rw-r--r--   0        0        0     9305 2023-04-03 14:50:53.617730 fabric_cf-1.5.0b3/fabric_cf/actor/handlers/no_op_handler.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.617898 fabric_cf-1.5.0b3/fabric_cf/actor/security/__init__.py
--rw-r--r--   0        0        0     4348 2023-04-03 14:50:53.618115 fabric_cf-1.5.0b3/fabric_cf/actor/security/access_checker.py
--rw-r--r--   0        0        0     2955 2023-04-03 14:50:53.618313 fabric_cf-1.5.0b3/fabric_cf/actor/security/auth_token.py
--rw-r--r--   0        0        0     3983 2023-05-11 15:20:50.258526 fabric_cf-1.5.0b3/fabric_cf/actor/security/fabric_token.py
--rw-r--r--   0        0        0     8635 2023-04-03 14:50:53.618697 fabric_cf-1.5.0b3/fabric_cf/actor/security/pdp_auth.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.618864 fabric_cf-1.5.0b3/fabric_cf/actor/test/__init__.py
--rw-r--r--   0        0        0    10932 2023-04-04 13:01:29.470229 fabric_cf-1.5.0b3/fabric_cf/actor/test/base_test_case.py
--rw-r--r--   0        0        0     4679 2023-04-03 14:50:53.619270 fabric_cf-1.5.0b3/fabric_cf/actor/test/client_callback_helper.py
--rw-r--r--   0        0        0     4639 2023-04-05 14:49:38.077013 fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.jenkins.yaml
--rw-r--r--   0        0        0     4305 2023-04-04 15:28:06.631503 fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.orchestrator.yaml
--rw-r--r--   0        0        0     4696 2023-04-05 17:47:55.443819 fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.test.yaml
--rw-r--r--   0        0        0     5376 2023-04-03 14:50:53.620212 fabric_cf-1.5.0b3/fabric_cf/actor/test/controller_callback_helper.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.620415 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.620599 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/container/__init__.py
--rw-r--r--   0        0        0     2815 2023-04-04 13:02:25.891866 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/container/container_database_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.621040 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/core/__init__.py
--rw-r--r--   0        0        0     4091 2023-04-04 13:02:48.136107 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/core/unit_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.621493 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/kernel/__init__.py
--rw-r--r--   0        0        0    21480 2023-04-04 15:12:06.450576 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/kernel/kernel_test.py
--rw-r--r--   0        0        0     3378 2023-04-04 15:11:51.860496 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/kernel/tick_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.624033 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/__init__.py
--rw-r--r--   0        0        0     3176 2023-04-04 15:15:43.466105 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/actor_database_test.py
--rw-r--r--   0        0        0     4729 2023-04-04 17:23:55.100076 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py
--rw-r--r--   0        0        0     1963 2023-04-03 14:50:53.624564 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/authority_substrate_test.py
--rw-r--r--   0        0        0     3263 2023-04-03 14:50:53.624725 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/substrate_database_test.py
--rw-r--r--   0        0        0     2280 2023-04-04 15:15:47.470348 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/substrate_test_base.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.625348 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/__init__.py
--rw-r--r--   0        0        0    21995 2023-04-04 17:23:55.095211 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py
--rw-r--r--   0        0        0    23678 2023-04-04 17:23:55.075259 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py
--rw-r--r--   0        0        0     4515 2023-04-04 17:23:55.081745 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py
--rw-r--r--   0        0        0     1561 2023-04-03 14:50:53.626668 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py
--rw-r--r--   0        0        0     8437 2023-04-03 14:50:53.626899 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_test_wrapper.py
--rw-r--r--   0        0        0     7719 2023-04-04 17:23:55.088766 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py
--rw-r--r--   0        0        0     1586 2023-04-03 14:50:53.627291 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.627471 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/__init__.py
--rw-r--r--   0        0        0     3786 2023-04-03 14:50:53.627666 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/actor_clock_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.627830 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/calendar/__init__.py
--rw-r--r--   0        0        0     4290 2023-04-03 14:50:53.628007 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py
--rw-r--r--   0        0        0     2225 2023-04-03 14:50:53.628189 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py
--rw-r--r--   0        0        0    14887 2023-04-03 14:50:53.628405 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/term_test.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.628584 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/util/__init__.py
--rw-r--r--   0        0        0     8041 2023-04-03 14:50:53.628792 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/util/reservation_holdings_test.py
--rw-r--r--   0        0        0     5072 2023-04-03 14:50:53.628930 fabric_cf-1.5.0b3/fabric_cf/actor/test/core/util/reservation_list_test.py
--rw-r--r--   0        0        0     3738 2023-04-03 14:50:53.629079 fabric_cf-1.5.0b3/fabric_cf/actor/test/dummy_authority_proxy.py
--rw-r--r--   0        0        0     1953 2023-04-03 14:50:53.629248 fabric_cf-1.5.0b3/fabric_cf/actor/test/dummy_proxy.py
--rw-r--r--   0        0        0     2498 2023-04-04 16:00:31.265177 fabric_cf-1.5.0b3/fabric_cf/actor/test/fim_test_helper.py
--rw-r--r--   0        0        0       92 2023-04-03 15:02:26.648185 fabric_cf-1.5.0b3/fabric_cf/actor/test/schema/key.avsc
--rw-r--r--   0        0        0    27389 2023-04-03 15:02:26.648701 fabric_cf-1.5.0b3/fabric_cf/actor/test/schema/message.avsc
--rw-r--r--   0        0        0     4532 2023-04-03 15:21:18.938300 fabric_cf-1.5.0b3/fabric_cf/actor/test/test_abqm.py
--rw-r--r--   0        0        0     1892 2023-04-03 14:50:53.630509 fabric_cf-1.5.0b3/fabric_cf/actor/test/test_actor.py
--rw-r--r--   0        0        0     1249 2023-04-03 14:50:53.630745 fabric_cf-1.5.0b3/fabric_cf/actor/test/test_exception.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.630912 fabric_cf-1.5.0b3/fabric_cf/aits/__init__.py
--rw-r--r--   0        0        0     4826 2023-04-05 16:57:12.446895 fabric_cf-1.5.0b3/fabric_cf/aits/config/config.broker.yaml
--rw-r--r--   0        0        0     4808 2023-04-05 16:57:36.798748 fabric_cf-1.5.0b3/fabric_cf/aits/config/config.netam.yaml
--rw-r--r--   0        0        0     4414 2023-04-05 16:57:45.775270 fabric_cf-1.5.0b3/fabric_cf/aits/config/config.orchestrator.yaml
--rw-r--r--   0        0        0     4788 2023-04-05 16:57:55.683500 fabric_cf-1.5.0b3/fabric_cf/aits/config/config.siteam.yaml
--rw-r--r--   0        0        0    49220 2023-04-07 14:15:47.763078 fabric_cf-1.5.0b3/fabric_cf/aits/integration_test.py
--rw-r--r--   0        0        0     7393 2023-04-06 18:22:24.720925 fabric_cf-1.5.0b3/fabric_cf/aits/kafka_processor.py
--rw-r--r--   0        0        0     8633 2023-04-06 18:12:27.261323 fabric_cf-1.5.0b3/fabric_cf/aits/manage_helper.py
--rw-r--r--   0        0        0     8339 2023-04-06 16:21:40.377393 fabric_cf-1.5.0b3/fabric_cf/aits/orchestrator_helper.py
--rw-r--r--   0        0        0    16256 2023-04-03 14:50:53.634161 fabric_cf-1.5.0b3/fabric_cf/authority/Readme.md
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.634241 fabric_cf-1.5.0b3/fabric_cf/authority/__init__.py
--rw-r--r--   0        0        0     2164 2023-04-03 14:50:53.634418 fabric_cf-1.5.0b3/fabric_cf/authority/__main__.py
--rw-r--r--   0        0        0    32973 2023-04-03 14:50:53.634699 fabric_cf-1.5.0b3/fabric_cf/authority/am-yes.xml
--rw-r--r--   0        0        0     4936 2023-04-03 14:50:53.634941 fabric_cf-1.5.0b3/fabric_cf/authority/config.al2s.am.yaml
--rw-r--r--   0        0        0     5030 2023-04-03 14:50:53.635111 fabric_cf-1.5.0b3/fabric_cf/authority/config.net.am.yaml
--rw-r--r--   0        0        0     5402 2023-04-03 14:50:53.635298 fabric_cf-1.5.0b3/fabric_cf/authority/config.site.am.geni.yaml
--rw-r--r--   0        0        0     4896 2023-04-03 14:50:53.635465 fabric_cf-1.5.0b3/fabric_cf/authority/config.site.am.yaml
--rw-r--r--   0        0        0     3427 2023-05-11 16:23:44.688550 fabric_cf-1.5.0b3/fabric_cf/authority/docker-compose.geni.yml
--rw-r--r--   0        0        0     3336 2023-05-11 16:23:58.379562 fabric_cf-1.5.0b3/fabric_cf/authority/docker-compose.yml
--rw-r--r--   0        0        0     1188 2023-05-11 16:24:05.923091 fabric_cf-1.5.0b3/fabric_cf/authority/env.template
--rw-r--r--   0        0        0    16080 2023-04-03 14:50:53.636162 fabric_cf-1.5.0b3/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml
--rw-r--r--   0        0        0     1588 2023-04-03 14:50:53.636606 fabric_cf-1.5.0b3/fabric_cf/authority/net_handler_config.yml
--rw-r--r--   0        0        0     1523 2023-04-03 14:50:53.636812 fabric_cf-1.5.0b3/fabric_cf/authority/oess_handler_config.yml
--rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.636998 fabric_cf-1.5.0b3/fabric_cf/authority/pdp.xml
--rwxr-xr-x   0        0        0     2446 2023-04-03 14:50:53.637179 fabric_cf-1.5.0b3/fabric_cf/authority/setup.sh
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.637346 fabric_cf-1.5.0b3/fabric_cf/authority/test/__init__.py
--rw-r--r--   0        0        0     2463 2023-04-03 14:50:53.637572 fabric_cf-1.5.0b3/fabric_cf/authority/test/al2s_am.py
--rw-r--r--   0        0        0     2459 2023-04-03 14:50:53.637740 fabric_cf-1.5.0b3/fabric_cf/authority/test/net_am.py
--rw-r--r--   0        0        0     2456 2023-04-03 14:50:53.637876 fabric_cf-1.5.0b3/fabric_cf/authority/test/site_am.py
--rw-r--r--   0        0        0     2461 2023-04-03 14:50:53.638045 fabric_cf-1.5.0b3/fabric_cf/authority/test/site_am_geni.py
--rw-r--r--   0        0        0     4729 2023-04-03 14:50:53.638234 fabric_cf-1.5.0b3/fabric_cf/authority/test/test-al2sam.yaml
--rw-r--r--   0        0        0     4839 2023-04-05 17:18:17.956714 fabric_cf-1.5.0b3/fabric_cf/authority/test/test-netam.yaml
--rw-r--r--   0        0        0     5071 2023-04-03 14:50:53.638536 fabric_cf-1.5.0b3/fabric_cf/authority/test/test.geni.yaml
--rw-r--r--   0        0        0     4685 2023-04-05 17:18:17.952345 fabric_cf-1.5.0b3/fabric_cf/authority/test/test.yaml
--rw-r--r--   0        0        0     2779 2023-05-11 15:20:50.260288 fabric_cf-1.5.0b3/fabric_cf/authority/vm_handler_config.yml
--rw-r--r--   0        0        0     1448 2023-04-03 14:50:53.639031 fabric_cf-1.5.0b3/fabric_cf/authority/vnic_net_handler_config.yml
--rw-r--r--   0        0        0    14262 2023-04-03 14:50:53.639328 fabric_cf-1.5.0b3/fabric_cf/broker/Readme.md
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.639412 fabric_cf-1.5.0b3/fabric_cf/broker/__init__.py
--rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.639603 fabric_cf-1.5.0b3/fabric_cf/broker/__main__.py
--rw-r--r--   0        0        0    27944 2023-04-03 14:50:53.639781 fabric_cf-1.5.0b3/fabric_cf/broker/broker-yes.xml
--rw-r--r--   0        0        0     5035 2023-04-03 14:50:53.640005 fabric_cf-1.5.0b3/fabric_cf/broker/config.broker.yaml
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.640163 fabric_cf-1.5.0b3/fabric_cf/broker/core/__init__.py
--rw-r--r--   0        0        0     3314 2023-04-03 14:50:53.640348 fabric_cf-1.5.0b3/fabric_cf/broker/core/broker_kernel.py
--rw-r--r--   0        0        0     3135 2023-05-11 16:25:29.197878 fabric_cf-1.5.0b3/fabric_cf/broker/docker-compose.yml
--rw-r--r--   0        0        0     1192 2023-05-11 16:25:51.672782 fabric_cf-1.5.0b3/fabric_cf/broker/env.template
--rw-r--r--   0        0        0    16080 2023-04-03 14:50:53.640954 fabric_cf-1.5.0b3/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml
--rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.641105 fabric_cf-1.5.0b3/fabric_cf/broker/pdp.xml
--rwxr-xr-x   0        0        0     2239 2023-04-03 14:50:53.641257 fabric_cf-1.5.0b3/fabric_cf/broker/setup.sh
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.641487 fabric_cf-1.5.0b3/fabric_cf/broker/test/__init__.py
--rw-r--r--   0        0        0     2507 2023-04-03 14:50:53.641689 fabric_cf-1.5.0b3/fabric_cf/broker/test/broker.py
--rw-r--r--   0        0        0     5042 2023-04-05 17:51:02.224321 fabric_cf-1.5.0b3/fabric_cf/broker/test/test.yaml
--rw-r--r--   0        0        0    20305 2023-05-11 15:20:50.261921 fabric_cf-1.5.0b3/fabric_cf/orchestrator/README.md
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.642384 fabric_cf-1.5.0b3/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0     3355 2023-05-11 15:20:50.262402 fabric_cf-1.5.0b3/fabric_cf/orchestrator/__main__.py
--rw-r--r--   0        0        0     1757 2023-04-03 14:50:53.642803 fabric_cf-1.5.0b3/fabric_cf/orchestrator/certs/fullchain.pem
--rw-r--r--   0        0        0     3272 2023-04-03 14:50:53.642965 fabric_cf-1.5.0b3/fabric_cf/orchestrator/certs/privkey.pem
--rw-r--r--   0        0        0     4859 2023-05-11 16:31:49.236795 fabric_cf-1.5.0b3/fabric_cf/orchestrator/config.orchestrator.yaml
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.643278 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/__init__.py
--rw-r--r--   0        0        0     2917 2023-04-03 14:50:53.643501 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/active_status_checker.py
--rw-r--r--   0        0        0     3050 2023-04-03 14:50:53.643707 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/bqm_wrapper.py
--rw-r--r--   0        0        0     1556 2023-04-03 14:50:53.643947 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/exceptions.py
--rw-r--r--   0        0        0     1884 2023-04-03 14:50:53.644155 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/i_status_update_callback.py
--rw-r--r--   0        0        0    39097 2023-05-11 15:20:50.264144 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_handler.py
--rw-r--r--   0        0        0     5389 2023-04-03 14:50:53.644692 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_kernel.py
--rw-r--r--   0        0        0    34864 2023-04-03 14:50:53.645078 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py
--rw-r--r--   0        0        0     3581 2023-04-03 14:50:53.645306 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_converter.py
--rw-r--r--   0        0        0     4880 2023-04-03 14:50:53.645464 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_status_update.py
--rw-r--r--   0        0        0     7876 2023-04-03 14:50:53.645708 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_status_update_thread.py
--rw-r--r--   0        0        0     6179 2023-04-03 14:50:53.645975 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/response_builder.py
--rw-r--r--   0        0        0     8722 2023-04-11 15:09:36.158110 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/slice_defer_thread.py
--rw-r--r--   0        0        0     1972 2023-04-03 14:50:53.646372 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/status_checker.py
--rw-r--r--   0        0        0     1581 2023-04-03 14:50:53.646556 fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/watch_entry.py
--rw-r--r--   0        0        0     3501 2023-05-11 16:25:29.205244 fabric_cf-1.5.0b3/fabric_cf/orchestrator/docker-compose.yml
--rw-r--r--   0        0        0     1198 2023-05-11 16:25:39.495582 fabric_cf-1.5.0b3/fabric_cf/orchestrator/env.template
--rw-r--r--   0        0        0    72323 2023-04-03 14:50:53.647218 fabric_cf-1.5.0b3/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml
--rw-r--r--   0        0        0     1626 2023-04-03 14:50:53.647500 fabric_cf-1.5.0b3/fabric_cf/orchestrator/nginx/default.conf
--rw-r--r--   0        0        0    46956 2023-05-11 15:20:50.265345 fabric_cf-1.5.0b3/fabric_cf/orchestrator/openapi.json
--rw-r--r--   0        0        0    30829 2023-04-03 14:50:53.648266 fabric_cf-1.5.0b3/fabric_cf/orchestrator/orchestrator-yes.xml
--rw-r--r--   0        0        0     1548 2023-04-03 14:50:53.648514 fabric_cf-1.5.0b3/fabric_cf/orchestrator/pdp.xml
--rwxr-xr-x   0        0        0     2284 2023-04-03 14:50:53.648696 fabric_cf-1.5.0b3/fabric_cf/orchestrator/setup.sh
--rw-r--r--   0        0        0      430 2023-04-03 14:50:53.648991 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/__init__.py
--rw-r--r--   0        0        0      392 2023-04-03 14:50:53.649220 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/__main__.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.649376 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/__init__.py
--rw-r--r--   0        0        0      311 2023-04-03 14:50:53.649537 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/authorization_controller.py
--rw-r--r--   0        0        0     1241 2023-04-03 14:50:53.649770 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py
--rw-r--r--   0        0        0     5510 2023-05-11 15:20:50.265817 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py
--rw-r--r--   0        0        0      860 2023-04-03 14:50:53.650215 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py
--rw-r--r--   0        0        0      305 2023-04-03 14:50:53.650408 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/version_controller.py
--rw-r--r--   0        0        0      631 2023-04-03 14:50:53.650559 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/encoder.py
--rw-r--r--   0        0        0     2275 2023-04-03 14:50:53.650868 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/__init__.py
--rw-r--r--   0        0        0     1889 2023-04-03 14:50:53.651022 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/base_model_.py
--rw-r--r--   0        0        0     1628 2023-04-03 14:50:53.651195 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/resource.py
--rw-r--r--   0        0        0     3564 2023-04-03 14:50:53.651368 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/resources.py
--rw-r--r--   0        0        0     7311 2023-04-03 14:50:53.651598 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slice.py
--rw-r--r--   0        0        0     3616 2023-04-03 14:50:53.651786 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slice_details.py
--rw-r--r--   0        0        0     5251 2023-04-03 14:50:53.651992 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slices.py
--rw-r--r--   0        0        0     8995 2023-04-03 14:50:53.652138 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/sliver.py
--rw-r--r--   0        0        0     5301 2023-04-03 14:50:53.652316 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slivers.py
--rw-r--r--   0        0        0     3896 2023-04-03 14:50:53.652450 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     2464 2023-04-03 14:50:53.652610 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     4929 2023-04-03 14:50:53.652747 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     2870 2023-04-03 14:50:53.652914 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py
--rw-r--r--   0        0        0     1983 2023-04-03 14:50:53.653092 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py
--rw-r--r--   0        0        0     4503 2023-04-03 14:50:53.653265 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     3984 2023-04-03 14:50:53.653436 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py
--rw-r--r--   0        0        0     2512 2023-04-03 14:50:53.653613 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     3879 2023-04-03 14:50:53.653846 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py
--rw-r--r--   0        0        0     2461 2023-04-03 14:50:53.654001 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     3846 2023-04-03 14:50:53.654159 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py
--rw-r--r--   0        0        0     2446 2023-04-03 14:50:53.654361 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     4233 2023-04-03 14:50:53.654697 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     2635 2023-04-03 14:50:53.654868 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3540 2023-04-03 14:50:53.655073 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/version.py
--rw-r--r--   0        0        0     2536 2023-04-03 14:50:53.655253 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/version_data.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.655440 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/__init__.py
--rw-r--r--   0        0        0     1355 2023-04-03 14:50:53.655618 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py
--rw-r--r--   0        0        0     1941 2023-05-11 15:20:50.266214 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/constants.py
--rw-r--r--   0        0        0     5537 2023-04-03 14:50:53.655976 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/cors_response.py
--rw-r--r--   0        0        0     4321 2023-04-03 14:50:53.656175 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/resources_controller.py
--rw-r--r--   0        0        0    15207 2023-05-11 15:20:50.266552 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/slices_controller.py
--rw-r--r--   0        0        0     4449 2023-04-03 14:50:53.656622 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py
--rw-r--r--   0        0        0     2530 2023-04-03 14:50:53.656817 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/utils.py
--rw-r--r--   0        0        0     2632 2023-04-05 17:52:22.168825 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/version_controller.py
--rw-r--r--   0        0        0    34085 2023-05-11 15:20:50.266865 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml
--rw-r--r--   0        0        0      438 2023-04-03 14:50:53.657698 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/__init__.py
--rw-r--r--   0        0        0     2094 2023-04-03 14:50:53.658010 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py
--rw-r--r--   0        0        0     5143 2023-05-11 15:20:50.267349 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py
--rw-r--r--   0        0        0     1903 2023-04-03 14:50:53.658437 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py
--rw-r--r--   0        0        0      855 2023-04-03 14:50:53.658595 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py
--rw-r--r--   0        0        0      809 2023-04-03 14:50:53.658764 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/type_util.py
--rw-r--r--   0        0        0     3452 2023-04-03 14:50:53.658932 fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/util.py
--rw-r--r--   0        0        0        0 2023-04-03 14:50:53.659106 fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/__init__.py
--rw-r--r--   0        0        0     3542 2023-04-03 14:50:53.659281 fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/orchestrator.py
--rwxr-xr-x   0        0        0       78 2023-04-03 14:50:53.659409 fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/test.sh
--rw-r--r--   0        0        0     4453 2023-04-05 17:51:26.470070 fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/test.yaml
--rwxr-xr-x   0        0        0     2900 2023-04-03 14:50:53.659782 fabric_cf-1.5.0b3/fabric_cf/orchestrator/update_swagger_stub.sh
--rw-r--r--   0        0        0    18177 2023-04-03 14:50:53.660187 fabric_cf-1.5.0b3/images/am-pod.png
--rw-r--r--   0        0        0    74927 2023-04-03 14:50:53.660890 fabric_cf-1.5.0b3/images/am.png
--rw-r--r--   0        0        0    18471 2023-04-03 14:50:53.661225 fabric_cf-1.5.0b3/images/broker-pod.png
--rw-r--r--   0        0        0    73799 2023-04-03 14:50:53.661878 fabric_cf-1.5.0b3/images/broker.png
--rw-r--r--   0        0        0    90831 2023-04-03 14:50:53.662835 fabric_cf-1.5.0b3/images/cf.png
--rw-r--r--   0        0        0    19611 2023-04-03 14:50:53.663247 fabric_cf-1.5.0b3/images/orchestrator-pod.png
--rw-r--r--   0        0        0    78622 2023-04-03 14:50:53.664084 fabric_cf-1.5.0b3/images/orchestrator.png
--rw-r--r--   0        0        0   145542 2023-04-03 14:50:53.664854 fabric_cf-1.5.0b3/neo4j/AL2S.graphml
--rw-r--r--   0        0        0    96363 2023-04-03 14:50:53.665732 fabric_cf-1.5.0b3/neo4j/LBNL-ad.graphml
--rw-r--r--   0        0        0    68182 2023-04-03 14:50:53.666334 fabric_cf-1.5.0b3/neo4j/Network-ad.graphml
--rw-r--r--   0        0        0    96375 2023-04-03 14:50:53.666804 fabric_cf-1.5.0b3/neo4j/RENCI-ad.graphml
--rw-r--r--   0        0        0    96286 2023-04-03 14:50:53.667143 fabric_cf-1.5.0b3/neo4j/UKY-ad.graphml
--rw-r--r--   0        0        0  1297955 2023-04-03 14:50:53.672629 fabric_cf-1.5.0b3/neo4j/UKY2.graphml
--rw-r--r--   0        0        0    14808 2023-04-03 14:50:53.673167 fabric_cf-1.5.0b3/neo4j/abqm.graphml
--rw-r--r--   0        0        0     1757 2023-04-03 14:50:53.673435 fabric_cf-1.5.0b3/neo4j/certs/fullchain.pem
--rw-r--r--   0        0        0     3272 2023-04-03 14:50:53.673617 fabric_cf-1.5.0b3/neo4j/certs/privkey.pem
--rwxr-xr-x   0        0        0       91 2023-04-03 14:50:53.673785 fabric_cf-1.5.0b3/orchestrator.sh
--rw-r--r--   0        0        0      698 2023-04-03 14:50:53.673962 fabric_cf-1.5.0b3/psql.upgrade
--rw-r--r--   0        0        0     1252 2023-05-11 15:29:39.647926 fabric_cf-1.5.0b3/pyproject.toml
--rwxr-xr-x   0        0        0     2421 2023-04-03 18:36:31.758196 fabric_cf-1.5.0b3/secrets/create-certs.sh
--rw-r--r--   0        0        0    12796 2023-05-11 16:31:49.237238 fabric_cf-1.5.0b3/tools/audit.py
--rw-r--r--   0        0        0     8005 2023-04-03 14:50:53.675250 fabric_cf-1.5.0b3/tools/db_cli.py
--rw-r--r--   0        0        0      354 2023-05-11 16:31:49.238481 fabric_cf-1.5.0b3/tools/install.sh
--rw-r--r--   0        0        0      143 2023-04-03 14:50:53.675627 fabric_cf-1.5.0b3/tox.ini
--rw-r--r--   0        0        0     3317 1970-01-01 00:00:00.000000 fabric_cf-1.5.0b3/PKG-INFO
+-rw-r--r--   0        0        0     2035 2023-05-24 00:04:26.799239 fabric_cf-1.5.0b4/.gitignore
+-rw-r--r--   0        0        0      851 2023-06-08 15:00:06.716071 fabric_cf-1.5.0b4/Dockerfile-auth
+-rw-r--r--   0        0        0      769 2023-05-24 00:05:54.479631 fabric_cf-1.5.0b4/Dockerfile-broker
+-rw-r--r--   0        0        0     1037 2023-05-24 00:05:30.194703 fabric_cf-1.5.0b4/Dockerfile-cf
+-rw-r--r--   0        0        0      787 2023-05-24 00:05:40.587772 fabric_cf-1.5.0b4/Dockerfile-orchestrator
+-rw-r--r--   0        0        0     1071 2023-04-03 14:50:53.535054 fabric_cf-1.5.0b4/LICENSE
+-rw-r--r--   0        0        0     2046 2023-04-03 14:50:53.535620 fabric_cf-1.5.0b4/README.md
+-rwxr-xr-x   0        0        0       74 2023-04-03 14:50:53.535840 fabric_cf-1.5.0b4/authority.sh
+-rwxr-xr-x   0        0        0       79 2023-04-03 14:50:53.535996 fabric_cf-1.5.0b4/broker.sh
+-rw-r--r--   0        0        0      947 2023-04-03 14:50:53.536169 fabric_cf-1.5.0b4/cleanup_old_schema_from_schema_registry.sh
+-rw-r--r--   0        0        0     2861 2023-04-03 19:02:18.268979 fabric_cf-1.5.0b4/docker-compose-kafka.yaml
+-rw-r--r--   0        0        0     1560 2023-04-03 14:50:53.536634 fabric_cf-1.5.0b4/docker-compose-no-ssl-kafka.yaml
+-rw-r--r--   0        0        0    10307 2023-05-24 00:04:37.572022 fabric_cf-1.5.0b4/docker-compose-test.yaml
+-rwxr-xr-x   0        0        0       45 2023-04-03 14:50:53.536998 fabric_cf-1.5.0b4/docker-entrypoint.sh
+-rw-r--r--   0        0        0      350 2023-04-03 14:50:53.537353 fabric_cf-1.5.0b4/env.template
+-rw-r--r--   0        0        0     1135 2023-04-03 17:25:25.716942 fabric_cf-1.5.0b4/env.template.test
+-rw-r--r--   0        0        0    16609 2023-04-03 14:50:53.537818 fabric_cf-1.5.0b4/fabricNo.AnyActorNoPolicy.xml
+-rw-r--r--   0        0        0     6343 2023-04-03 14:50:53.538166 fabric_cf-1.5.0b4/fabric_cf/Design.md
+-rw-r--r--   0        0        0       50 2023-06-08 15:00:39.735944 fabric_cf-1.5.0b4/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.538462 fabric_cf-1.5.0b4/fabric_cf/actor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.538776 fabric_cf-1.5.0b4/fabric_cf/actor/boot/__init__.py
+-rw-r--r--   0        0        0    15281 2023-04-03 14:50:53.539116 fabric_cf-1.5.0b4/fabric_cf/actor/boot/configuration.py
+-rw-r--r--   0        0        0     1268 2023-04-03 14:50:53.539529 fabric_cf-1.5.0b4/fabric_cf/actor/boot/configuration_exception.py
+-rw-r--r--   0        0        0     2509 2023-04-03 14:50:53.539906 fabric_cf-1.5.0b4/fabric_cf/actor/boot/configuration_loader.py
+-rw-r--r--   0        0        0    23003 2023-05-22 19:03:15.215562 fabric_cf-1.5.0b4/fabric_cf/actor/boot/configuration_processor.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.540419 fabric_cf-1.5.0b4/fabric_cf/actor/boot/inventory/__init__.py
+-rw-r--r--   0        0        0     4969 2023-04-03 14:50:53.540687 fabric_cf-1.5.0b4/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.540852 fabric_cf-1.5.0b4/fabric_cf/actor/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.541039 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/__init__.py
+-rw-r--r--   0        0        0     4907 2023-04-03 14:50:53.541250 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_container.py
+-rw-r--r--   0        0        0     1530 2023-04-03 14:50:53.541590 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_event.py
+-rw-r--r--   0        0        0     2176 2023-04-03 14:50:53.541925 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_identity.py
+-rw-r--r--   0        0        0    10558 2023-06-05 15:22:22.261326 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_management_object.py
+-rw-r--r--   0        0        0    21823 2023-06-07 01:58:31.085841 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_mixin.py
+-rw-r--r--   0        0        0     1918 2023-04-03 14:50:53.543106 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_proxy.py
+-rw-r--r--   0        0        0     1323 2023-04-03 14:50:53.543429 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_runnable.py
+-rw-r--r--   0        0        0     4745 2023-06-05 21:47:12.221980 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_authority.py
+-rw-r--r--   0        0        0     8736 2023-04-03 14:50:53.543930 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_authority_policy.py
+-rw-r--r--   0        0        0     3657 2023-06-05 19:29:44.111472 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_authority_proxy.py
+-rw-r--r--   0        0        0     3367 2023-04-03 14:50:53.545583 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_authority_reservation.py
+-rw-r--r--   0        0        0     6071 2023-04-03 14:50:53.545879 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_base_plugin.py
+-rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.546104 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_broker_mixin.py
+-rw-r--r--   0        0        0     1492 2023-04-03 14:50:53.546359 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py
+-rw-r--r--   0        0        0     3690 2023-04-03 14:50:53.546566 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_broker_proxy.py
+-rw-r--r--   0        0        0     4012 2023-04-03 14:50:53.546780 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_broker_reservation.py
+-rw-r--r--   0        0        0     2442 2023-04-03 14:50:53.547038 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_callback_proxy.py
+-rw-r--r--   0        0        0     9846 2023-06-07 18:02:40.743977 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_client_actor.py
+-rw-r--r--   0        0        0     6811 2023-06-03 00:45:11.686084 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_client_actor_management_object.py
+-rw-r--r--   0        0        0     2640 2023-04-03 14:50:53.547942 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_client_callback_proxy.py
+-rw-r--r--   0        0        0     5802 2023-04-03 14:50:53.548385 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_client_policy.py
+-rw-r--r--   0        0        0     7724 2023-04-03 14:50:53.548730 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_client_reservation.py
+-rw-r--r--   0        0        0     1936 2023-04-03 14:50:53.548982 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_component.py
+-rw-r--r--   0        0        0    10115 2023-06-07 13:40:25.955302 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_concrete_set.py
+-rw-r--r--   0        0        0     2729 2023-04-03 14:50:53.549801 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_container_clock.py
+-rw-r--r--   0        0        0     3976 2023-04-03 14:50:53.550228 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_container_database.py
+-rw-r--r--   0        0        0     3367 2023-04-03 14:50:53.550497 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_controller.py
+-rw-r--r--   0        0        0     2855 2023-06-07 03:05:18.086990 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py
+-rw-r--r--   0        0        0     2787 2023-04-03 14:50:53.550900 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_controller_policy.py
+-rw-r--r--   0        0        0     5713 2023-06-05 19:31:03.613781 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_controller_reservation.py
+-rw-r--r--   0        0        0    11685 2023-06-05 16:15:36.866668 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_database.py
+-rw-r--r--   0        0        0    11127 2023-06-04 19:23:51.043944 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_delegation.py
+-rw-r--r--   0        0        0     1867 2023-04-03 14:50:53.551767 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_event.py
+-rw-r--r--   0        0        0     1943 2023-04-03 14:50:53.552014 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_management_object.py
+-rw-r--r--   0        0        0     9713 2023-06-05 15:21:49.991965 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_actor.py
+-rw-r--r--   0        0        0     2534 2023-04-03 14:50:53.552486 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_authority.py
+-rw-r--r--   0        0        0     1452 2023-04-03 14:50:53.552674 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py
+-rw-r--r--   0        0        0     6191 2023-04-03 14:50:53.552834 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py
+-rw-r--r--   0        0        0     5041 2023-04-03 14:50:53.553039 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_container.py
+-rw-r--r--   0        0        0     2486 2023-06-04 10:41:04.551953 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py
+-rw-r--r--   0        0        0     5014 2023-04-03 14:50:53.553457 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py
+-rw-r--r--   0        0        0    11147 2023-04-03 14:50:53.553629 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_policy.py
+-rw-r--r--   0        0        0     2304 2023-04-03 14:50:53.553847 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_proxy.py
+-rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.554059 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_proxy_factory.py
+-rw-r--r--   0        0        0     1658 2023-04-03 14:50:53.554593 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_query_response_handler.py
+-rw-r--r--   0        0        0    14613 2023-06-07 18:18:48.933077 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_reservation_mixin.py
+-rw-r--r--   0        0        0     9388 2023-04-03 14:50:53.555129 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_reservation_resources.py
+-rw-r--r--   0        0        0     5581 2023-04-03 14:50:53.555376 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_reservation_status.py
+-rw-r--r--   0        0        0     8963 2023-04-03 14:50:53.555582 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_resource_control.py
+-rw-r--r--   0        0        0     1336 2023-04-03 14:50:53.555785 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_response_handler.py
+-rw-r--r--   0        0        0     2246 2023-04-03 14:50:53.556014 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_rpc_request_state.py
+-rw-r--r--   0        0        0     5634 2023-04-03 14:50:53.556345 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_server_actor.py
+-rw-r--r--   0        0        0     6415 2023-04-03 14:50:53.556589 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_server_policy.py
+-rw-r--r--   0        0        0     4846 2023-04-03 14:50:53.556782 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_server_reservation.py
+-rw-r--r--   0        0        0    13280 2023-04-03 14:50:53.557016 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_slice.py
+-rw-r--r--   0        0        0     3548 2023-06-06 14:29:28.086810 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_substrate.py
+-rw-r--r--   0        0        0     2225 2023-04-03 14:50:53.557477 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_substrate_database.py
+-rw-r--r--   0        0        0     2943 2023-04-03 14:50:53.557727 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_tick.py
+-rw-r--r--   0        0        0     6121 2023-04-03 14:50:53.557931 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_ticker.py
+-rw-r--r--   0        0        0     1590 2023-04-03 14:50:53.558112 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_timer_queue.py
+-rw-r--r--   0        0        0     1387 2023-04-03 14:50:53.558344 fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_timer_task.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.558543 fabric_cf-1.5.0b4/fabric_cf/actor/core/common/__init__.py
+-rw-r--r--   0        0        0    12944 2023-06-07 21:37:19.770105 fabric_cf-1.5.0b4/fabric_cf/actor/core/common/constants.py
+-rw-r--r--   0        0        0     3254 2023-04-03 14:50:53.559144 fabric_cf-1.5.0b4/fabric_cf/actor/core/common/event_logger.py
+-rw-r--r--   0        0        0     5517 2023-04-03 14:50:53.559364 fabric_cf-1.5.0b4/fabric_cf/actor/core/common/exceptions.py
+-rw-r--r--   0        0        0     6108 2023-04-03 14:50:53.559599 fabric_cf-1.5.0b4/fabric_cf/actor/core/common/resource_config.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.559841 fabric_cf-1.5.0b4/fabric_cf/actor/core/container/__init__.py
+-rw-r--r--   0        0        0    24564 2023-04-03 14:50:53.560251 fabric_cf-1.5.0b4/fabric_cf/actor/core/container/container.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.560471 fabric_cf-1.5.0b4/fabric_cf/actor/core/container/db/__init__.py
+-rw-r--r--   0        0        0     8667 2023-05-22 19:03:15.216759 fabric_cf-1.5.0b4/fabric_cf/actor/core/container/db/container_database.py
+-rw-r--r--   0        0        0    19263 2023-04-03 14:50:53.561010 fabric_cf-1.5.0b4/fabric_cf/actor/core/container/globals.py
+-rw-r--r--   0        0        0     9216 2023-05-22 19:03:15.217738 fabric_cf-1.5.0b4/fabric_cf/actor/core/container/maintenance.py
+-rw-r--r--   0        0        0     5472 2023-04-03 14:50:53.561525 fabric_cf-1.5.0b4/fabric_cf/actor/core/container/message_service.py
+-rw-r--r--   0        0        0     1508 2023-04-03 14:50:53.561724 fabric_cf-1.5.0b4/fabric_cf/actor/core/container/protocol_descriptor.py
+-rw-r--r--   0        0        0    13005 2023-04-03 14:50:53.562081 fabric_cf-1.5.0b4/fabric_cf/actor/core/container/remote_actor_cache.py
+-rw-r--r--   0        0        0     8040 2023-04-03 14:50:53.562299 fabric_cf-1.5.0b4/fabric_cf/actor/core/container/rpc_producer.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.562481 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/__init__.py
+-rw-r--r--   0        0        0    35815 2023-06-07 01:58:41.008165 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/actor.py
+-rw-r--r--   0        0        0     1975 2023-04-03 14:50:53.563319 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/actor_identity.py
+-rw-r--r--   0        0        0    15513 2023-06-06 00:51:23.659209 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/authority.py
+-rw-r--r--   0        0        0     4845 2023-04-03 14:50:53.563854 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/authority_policy.py
+-rw-r--r--   0        0        0    20447 2023-06-07 18:02:40.735686 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/broker.py
+-rw-r--r--   0        0        0     5914 2023-04-03 14:50:53.565067 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/broker_policy.py
+-rw-r--r--   0        0        0    20420 2023-06-07 18:02:40.726399 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/controller.py
+-rw-r--r--   0        0        0     8604 2023-05-22 19:03:15.220393 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/event_processor.py
+-rw-r--r--   0        0        0     5467 2023-04-03 14:50:53.565861 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/inventory_slice_manager.py
+-rw-r--r--   0        0        0     6171 2023-04-03 14:50:53.566145 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/policy.py
+-rw-r--r--   0        0        0     2042 2023-04-03 14:50:53.566366 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/rpc_request_state.py
+-rw-r--r--   0        0        0     8688 2023-04-03 14:50:53.566587 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/ticket.py
+-rw-r--r--   0        0        0    16474 2023-06-07 12:30:10.407659 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/unit.py
+-rw-r--r--   0        0        0    13814 2023-06-07 13:44:16.632376 fabric_cf-1.5.0b4/fabric_cf/actor/core/core/unit_set.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.567201 fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/__init__.py
+-rw-r--r--   0        0        0    11038 2023-06-04 21:22:05.931803 fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/broker_delegation.py
+-rw-r--r--   0        0        0     1933 2023-06-04 19:26:54.315067 fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/broker_delegation_factory.py
+-rw-r--r--   0        0        0    17061 2023-06-04 21:11:48.413964 fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/delegation.py
+-rw-r--r--   0        0        0     1916 2023-06-04 19:26:54.320155 fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/delegation_factory.py
+-rw-r--r--   0        0        0     5364 2023-04-03 14:50:53.568399 fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/resource_ticket.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.568570 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/__init__.py
+-rw-r--r--   0        0        0    31962 2023-06-08 03:23:28.143902 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/authority_reservation.py
+-rw-r--r--   0        0        0     3384 2023-04-03 14:50:53.569249 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/broker_query_model_publisher.py
+-rw-r--r--   0        0        0    26805 2023-04-03 14:50:53.569537 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/broker_reservation.py
+-rw-r--r--   0        0        0     2992 2023-04-03 14:50:53.569880 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/claim_timeout.py
+-rw-r--r--   0        0        0     4396 2023-04-03 14:50:53.570217 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/failed_rpc.py
+-rw-r--r--   0        0        0     3639 2023-04-03 14:50:53.570449 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/failed_rpc_event.py
+-rw-r--r--   0        0        0     2668 2023-04-03 14:50:53.570827 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py
+-rw-r--r--   0        0        0     2708 2023-04-03 14:50:53.571106 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_failed_rpc.py
+-rw-r--r--   0        0        0     2274 2023-06-05 19:22:20.651878 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_poa_rpc.py
+-rw-r--r--   0        0        0     2105 2023-04-03 14:50:53.571543 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_query_rpc.py
+-rw-r--r--   0        0        0     2703 2023-04-03 14:50:53.571750 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py
+-rw-r--r--   0        0        0     4158 2023-04-03 14:50:53.571968 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_rpc.py
+-rw-r--r--   0        0        0    11227 2023-06-07 18:01:05.602995 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_rpc_event.py
+-rw-r--r--   0        0        0    65468 2023-06-07 19:06:48.466059 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/kernel.py
+-rw-r--r--   0        0        0     3314 2023-04-03 14:50:53.572703 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/kernel_tick.py
+-rw-r--r--   0        0        0    57774 2023-06-07 19:15:09.691801 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/kernel_wrapper.py
+-rw-r--r--   0        0        0    12127 2023-06-07 21:13:07.618249 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/poa.py
+-rw-r--r--   0        0        0     2363 2023-04-03 14:50:53.573675 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/predecessor_state.py
+-rw-r--r--   0        0        0     2860 2023-04-03 14:50:53.573873 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/query_timeout.py
+-rw-r--r--   0        0        0     1404 2023-04-03 14:50:53.574038 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/request_types.py
+-rw-r--r--   0        0        0    24726 2023-06-07 18:18:48.950395 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/reservation.py
+-rw-r--r--   0        0        0    92717 2023-06-08 03:05:02.413534 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/reservation_client.py
+-rw-r--r--   0        0        0     9994 2023-04-03 14:50:53.575366 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/reservation_server.py
+-rw-r--r--   0        0        0     3311 2023-06-06 19:30:17.506570 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/reservation_states.py
+-rw-r--r--   0        0        0    21131 2023-06-07 13:40:25.959703 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/resource_set.py
+-rw-r--r--   0        0        0     1614 2023-04-03 14:50:53.576176 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/retry_rpc.py
+-rw-r--r--   0        0        0     1899 2023-04-03 14:50:53.576398 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/retry_rpc_event.py
+-rw-r--r--   0        0        0     4128 2023-06-07 16:02:47.944144 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/rpc_executor.py
+-rw-r--r--   0        0        0    32934 2023-06-07 18:21:09.698878 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/rpc_manager.py
+-rw-r--r--   0        0        0     1772 2023-04-03 14:50:53.577467 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/rpc_manager_singleton.py
+-rw-r--r--   0        0        0     3793 2023-06-05 19:23:36.478485 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/rpc_request.py
+-rw-r--r--   0        0        0     1650 2023-05-25 14:10:16.486302 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/rpc_request_type.py
+-rw-r--r--   0        0        0     1340 2023-04-03 14:50:53.578168 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/sequence_comparison_codes.py
+-rw-r--r--   0        0        0    12284 2023-04-03 14:50:53.578451 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/slice.py
+-rw-r--r--   0        0        0    12613 2023-05-22 19:03:15.225078 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/slice_state_machine.py
+-rw-r--r--   0        0        0     8319 2023-04-03 14:50:53.578901 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/slice_table.py
+-rw-r--r--   0        0        0     6527 2023-04-03 14:50:53.579044 fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/tick.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.579204 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/__init__.py
+-rw-r--r--   0        0        0    39488 2023-06-05 19:19:17.248142 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/actor_management_object.py
+-rw-r--r--   0        0        0     8431 2023-04-03 14:50:53.579975 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/authority_management_object.py
+-rw-r--r--   0        0        0     7315 2023-06-03 00:46:19.033938 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/broker_management_object.py
+-rw-r--r--   0        0        0    29438 2023-06-07 20:50:24.500801 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/client_actor_management_object_helper.py
+-rw-r--r--   0        0        0     9605 2023-04-03 14:50:53.580935 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/container_management_object.py
+-rw-r--r--   0        0        0     9165 2023-06-03 00:46:19.030418 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/controller_management_object.py
+-rw-r--r--   0        0        0    13007 2023-04-03 14:50:53.581333 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/converter.py
+-rw-r--r--   0        0        0     1624 2023-04-03 14:50:53.581543 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/error.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.581729 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/__init__.py
+-rw-r--r--   0        0        0    10483 2023-06-05 15:21:22.058890 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_actor.py
+-rw-r--r--   0        0        0     3509 2023-04-03 14:50:53.582317 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_authority.py
+-rw-r--r--   0        0        0     8200 2023-05-22 19:03:15.226498 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_broker.py
+-rw-r--r--   0        0        0     4483 2023-04-03 14:50:53.583057 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_container.py
+-rw-r--r--   0        0        0     5462 2023-06-04 10:41:04.545539 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_controller.py
+-rw-r--r--   0        0        0     5462 2023-04-03 14:50:53.583439 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py
+-rw-r--r--   0        0        0     6960 2023-05-22 19:03:15.226922 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_proxy.py
+-rw-r--r--   0        0        0     5730 2023-04-03 14:50:53.583847 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.584078 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/__init__.py
+-rw-r--r--   0        0        0    24550 2023-04-03 14:50:53.584410 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py
+-rw-r--r--   0        0        0     5715 2023-04-03 14:50:53.584691 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py
+-rw-r--r--   0        0        0     5797 2023-04-03 14:50:53.585104 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py
+-rw-r--r--   0        0        0    15846 2023-04-03 14:50:53.585409 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py
+-rw-r--r--   0        0        0     4008 2023-04-03 14:50:53.585584 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py
+-rw-r--r--   0        0        0     8228 2023-04-03 14:50:53.585867 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py
+-rw-r--r--   0        0        0     2148 2023-04-03 14:50:53.586169 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_service.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.586361 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/__init__.py
+-rw-r--r--   0        0        0    11659 2023-06-05 15:21:49.995325 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_actor.py
+-rw-r--r--   0        0        0     3902 2023-04-03 14:50:53.586852 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_authority.py
+-rw-r--r--   0        0        0     8391 2023-04-03 14:50:53.587036 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_broker.py
+-rw-r--r--   0        0        0    10119 2023-04-03 14:50:53.587201 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_container.py
+-rw-r--r--   0        0        0     9646 2023-06-05 13:51:33.170079 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_controller.py
+-rw-r--r--   0        0        0     2954 2023-06-04 10:58:11.003716 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_proxy.py
+-rw-r--r--   0        0        0     8655 2023-04-03 14:50:53.587724 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_server_actor.py
+-rw-r--r--   0        0        0     7217 2023-04-03 14:50:53.588020 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/management_object.py
+-rw-r--r--   0        0        0     7841 2023-04-03 14:50:53.588258 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/management_object_manager.py
+-rw-r--r--   0        0        0     4972 2023-04-03 14:50:53.588521 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/management_utils.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.588706 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/__init__.py
+-rw-r--r--   0        0        0     1604 2023-04-03 14:50:53.588914 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/client_mng.py
+-rw-r--r--   0        0        0     1570 2023-04-03 14:50:53.589110 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/event_mng.py
+-rw-r--r--   0        0        0     1802 2023-04-03 14:50:53.589285 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py
+-rw-r--r--   0        0        0     1741 2023-04-03 14:50:53.589460 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/result_client_mng.py
+-rw-r--r--   0        0        0     1554 2023-04-03 14:50:53.589750 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/result_event_mng.py
+-rw-r--r--   0        0        0     1904 2023-04-03 14:50:53.590017 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py
+-rw-r--r--   0        0        0    15777 2023-04-03 14:50:53.590202 fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/server_actor_management_object.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.590369 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/__init__.py
+-rw-r--r--   0        0        0     7965 2023-05-24 00:04:26.812780 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/base_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.590945 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/db/__init__.py
+-rw-r--r--   0        0        0    34972 2023-06-07 19:26:06.331761 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/db/actor_database.py
+-rw-r--r--   0        0        0     2624 2023-05-22 19:03:15.227552 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/db/client_database.py
+-rw-r--r--   0        0        0     3792 2023-05-22 19:03:15.227772 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/db/server_actor_database.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.591940 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/handlers/__init__.py
+-rw-r--r--   0        0        0    13211 2023-06-06 15:52:10.224219 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py
+-rw-r--r--   0        0        0     2955 2023-06-07 12:30:10.412924 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/handlers/config_token.py
+-rw-r--r--   0        0        0     2286 2023-04-03 14:50:53.592660 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py
+-rw-r--r--   0        0        0     7556 2023-06-06 15:06:13.741788 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/handlers/handler_processor.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.593035 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/substrate/__init__.py
+-rw-r--r--   0        0        0     3612 2023-04-03 14:50:53.593263 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/substrate/authority_substrate.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.593460 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/substrate/db/__init__.py
+-rw-r--r--   0        0        0     4365 2023-05-22 19:03:15.228408 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py
+-rw-r--r--   0        0        0    16978 2023-06-08 03:02:06.490817 fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.594246 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/__init__.py
+-rw-r--r--   0        0        0    28295 2023-04-03 14:50:53.594548 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/authority_calendar_policy.py
+-rw-r--r--   0        0        0     8891 2023-04-03 14:50:53.595030 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/broker_calendar_policy.py
+-rw-r--r--   0        0        0    64810 2023-05-22 19:03:15.229809 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/broker_simpler_units_policy.py
+-rw-r--r--   0        0        0    19840 2023-05-22 19:03:15.230194 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/controller_calendar_policy.py
+-rw-r--r--   0        0        0     9815 2023-05-22 19:03:15.230558 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/controller_simple_policy.py
+-rw-r--r--   0        0        0     9546 2023-05-22 19:03:15.231097 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/controller_ticket_review_policy.py
+-rw-r--r--   0        0        0     1814 2023-04-03 14:50:53.596494 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/fifo_queue.py
+-rw-r--r--   0        0        0     2981 2023-04-03 14:50:53.596828 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/inventory.py
+-rw-r--r--   0        0        0     2785 2023-04-03 14:50:53.597031 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/inventory_for_type.py
+-rw-r--r--   0        0        0    14503 2023-05-23 18:34:16.940038 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/network_node_control.py
+-rw-r--r--   0        0        0    28363 2023-04-03 14:50:53.597532 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/network_node_inventory.py
+-rw-r--r--   0        0        0     5435 2023-04-03 14:50:53.597856 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/network_service_control.py
+-rw-r--r--   0        0        0    22745 2023-04-03 14:50:53.598106 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/network_service_inventory.py
+-rw-r--r--   0        0        0     2032 2023-04-03 14:50:53.598641 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/queue_wrapper.py
+-rw-r--r--   0        0        0     5157 2023-04-03 14:50:53.598857 fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/resource_control.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.599020 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/__init__.py
+-rw-r--r--   0        0        0     1821 2023-04-03 14:50:53.599277 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/actor_location.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.599432 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/__init__.py
+-rw-r--r--   0        0        0     8301 2023-06-07 21:13:21.627970 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py
+-rw-r--r--   0        0        0     8924 2023-06-07 15:26:30.917385 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py
+-rw-r--r--   0        0        0     6744 2023-06-07 15:24:37.984624 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py
+-rw-r--r--   0        0        0     4809 2023-04-03 14:50:53.600099 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py
+-rw-r--r--   0        0        0     9066 2023-06-07 20:55:24.703849 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/kafka_retun.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.600601 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/services/__init__.py
+-rw-r--r--   0        0        0    12672 2023-06-07 20:50:24.507512 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/services/actor_service.py
+-rw-r--r--   0        0        0     7627 2023-06-07 20:50:24.518854 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/services/authority_service.py
+-rw-r--r--   0        0        0     8288 2023-06-04 19:39:58.806875 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/services/broker_service.py
+-rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.601562 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/services/controller_service.py
+-rw-r--r--   0        0        0    19087 2023-06-08 03:38:28.010487 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/translate.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.601999 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/__init__.py
+-rw-r--r--   0        0        0     4948 2023-06-05 19:28:12.432180 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/local_authority.py
+-rw-r--r--   0        0        0     5754 2023-06-04 19:32:53.734156 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/local_broker.py
+-rw-r--r--   0        0        0     6924 2023-06-02 20:44:37.570787 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/local_proxy.py
+-rw-r--r--   0        0        0     2868 2023-04-03 14:50:53.604580 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/local_proxy_factory.py
+-rw-r--r--   0        0        0     6762 2023-06-07 03:07:24.561220 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/local_return.py
+-rw-r--r--   0        0        0     8222 2023-06-06 19:40:39.807904 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/proxy.py
+-rw-r--r--   0        0        0     3013 2023-04-03 14:50:53.605545 fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/proxy_factory.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.605762 fabric_cf-1.5.0b4/fabric_cf/actor/core/registry/__init__.py
+-rw-r--r--   0        0        0     7672 2023-04-03 14:50:53.605950 fabric_cf-1.5.0b4/fabric_cf/actor/core/registry/actor_registry.py
+-rw-r--r--   0        0        0     2177 2023-04-03 14:50:53.606181 fabric_cf-1.5.0b4/fabric_cf/actor/core/registry/callback_registry.py
+-rw-r--r--   0        0        0     4926 2023-04-03 14:50:53.606408 fabric_cf-1.5.0b4/fabric_cf/actor/core/registry/peer_registry.py
+-rw-r--r--   0        0        0     3912 2023-04-03 14:50:53.606565 fabric_cf-1.5.0b4/fabric_cf/actor/core/registry/proxy_registry.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.606740 fabric_cf-1.5.0b4/fabric_cf/actor/core/time/__init__.py
+-rw-r--r--   0        0        0     7165 2023-04-03 14:50:53.606931 fabric_cf-1.5.0b4/fabric_cf/actor/core/time/actor_clock.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.607146 fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/__init__.py
+-rw-r--r--   0        0        0     8224 2023-04-03 14:50:53.607463 fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/authority_calendar.py
+-rw-r--r--   0        0        0     1667 2023-04-03 14:50:53.607755 fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/base_calendar.py
+-rw-r--r--   0        0        0    11573 2023-04-03 14:50:53.607991 fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/broker_calendar.py
+-rw-r--r--   0        0        0     9733 2023-04-03 14:50:53.608213 fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/client_calendar.py
+-rw-r--r--   0        0        0     5239 2023-04-03 14:50:53.608505 fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/controller_calendar.py
+-rw-r--r--   0        0        0     2550 2023-04-03 14:50:53.608738 fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/source_calendar.py
+-rw-r--r--   0        0        0    15769 2023-04-03 14:50:53.609015 fabric_cf-1.5.0b4/fabric_cf/actor/core/time/term.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.609215 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/__init__.py
+-rw-r--r--   0        0        0     2213 2023-04-03 14:50:53.609476 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/bids.py
+-rw-r--r--   0        0        0     2905 2023-04-03 14:50:53.609992 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/client.py
+-rw-r--r--   0        0        0     2063 2023-04-03 14:50:53.610294 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/graceful_interrupt_handler.py
+-rw-r--r--   0        0        0     2163 2023-04-03 14:50:53.610582 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/id.py
+-rw-r--r--   0        0        0     1488 2023-04-03 14:50:53.610758 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/iterable_queue.py
+-rw-r--r--   0        0        0     2263 2023-04-03 14:50:53.611043 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/kernel_timer.py
+-rw-r--r--   0        0        0     2905 2023-04-03 14:50:53.611261 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/log_helper.py
+-rw-r--r--   0        0        0     2238 2023-04-03 14:50:53.611511 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/notice.py
+-rw-r--r--   0        0        0     1999 2023-04-03 14:50:53.611700 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/reflection_utils.py
+-rw-r--r--   0        0        0     8380 2023-04-03 14:50:53.612072 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/reservation_holdings.py
+-rw-r--r--   0        0        0     8864 2023-04-03 14:50:53.612305 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/reservation_list.py
+-rw-r--r--   0        0        0     6700 2023-06-06 00:51:32.745023 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/reservation_set.py
+-rw-r--r--   0        0        0     3144 2023-04-03 14:50:53.612687 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/reservation_state.py
+-rw-r--r--   0        0        0     2250 2023-04-03 14:50:53.612855 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/resource_type.py
+-rw-r--r--   0        0        0     1690 2023-04-03 14:50:53.613024 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/rpc_exception.py
+-rw-r--r--   0        0        0     4440 2023-04-03 14:50:53.613195 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/update_data.py
+-rw-r--r--   0        0        0     4188 2023-04-03 14:50:53.613384 fabric_cf-1.5.0b4/fabric_cf/actor/core/util/utils.py
+-rw-r--r--   0        0        0     8424 2023-06-05 16:02:16.602759 fabric_cf-1.5.0b4/fabric_cf/actor/db/__init__.py
+-rw-r--r--   0        0        0    63500 2023-06-05 20:42:05.208304 fabric_cf-1.5.0b4/fabric_cf/actor/db/psql_database.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.614689 fabric_cf-1.5.0b4/fabric_cf/actor/fim/__init__.py
+-rw-r--r--   0        0        0     6326 2023-05-22 19:03:15.233111 fabric_cf-1.5.0b4/fabric_cf/actor/fim/asm_update_thread.py
+-rw-r--r--   0        0        0    28243 2023-05-22 19:03:15.233510 fabric_cf-1.5.0b4/fabric_cf/actor/fim/fim_helper.py
+-rw-r--r--   0        0        0        1 2023-04-03 14:50:53.616623 fabric_cf-1.5.0b4/fabric_cf/actor/fim/plugins/__init__.py
+-rw-r--r--   0        0        0        1 2023-04-03 14:50:53.616848 fabric_cf-1.5.0b4/fabric_cf/actor/fim/plugins/broker/__init__.py
+-rw-r--r--   0        0        0    23911 2023-05-24 00:04:37.573265 fabric_cf-1.5.0b4/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.617325 fabric_cf-1.5.0b4/fabric_cf/actor/handlers/__init__.py
+-rw-r--r--   0        0        0     3015 2023-06-06 15:30:36.172408 fabric_cf-1.5.0b4/fabric_cf/actor/handlers/handler_base.py
+-rw-r--r--   0        0        0    10968 2023-06-07 20:00:42.105998 fabric_cf-1.5.0b4/fabric_cf/actor/handlers/no_op_handler.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.617898 fabric_cf-1.5.0b4/fabric_cf/actor/security/__init__.py
+-rw-r--r--   0        0        0     4348 2023-04-03 14:50:53.618115 fabric_cf-1.5.0b4/fabric_cf/actor/security/access_checker.py
+-rw-r--r--   0        0        0     2955 2023-04-03 14:50:53.618313 fabric_cf-1.5.0b4/fabric_cf/actor/security/auth_token.py
+-rw-r--r--   0        0        0     3983 2023-05-22 19:03:15.233844 fabric_cf-1.5.0b4/fabric_cf/actor/security/fabric_token.py
+-rw-r--r--   0        0        0     8648 2023-06-04 01:13:37.501221 fabric_cf-1.5.0b4/fabric_cf/actor/security/pdp_auth.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.618864 fabric_cf-1.5.0b4/fabric_cf/actor/test/__init__.py
+-rw-r--r--   0        0        0    10932 2023-04-04 13:01:29.470229 fabric_cf-1.5.0b4/fabric_cf/actor/test/base_test_case.py
+-rw-r--r--   0        0        0     4679 2023-04-03 14:50:53.619270 fabric_cf-1.5.0b4/fabric_cf/actor/test/client_callback_helper.py
+-rw-r--r--   0        0        0     4639 2023-05-24 00:04:26.820084 fabric_cf-1.5.0b4/fabric_cf/actor/test/config/config.jenkins.yaml
+-rw-r--r--   0        0        0     4305 2023-04-04 15:28:06.631503 fabric_cf-1.5.0b4/fabric_cf/actor/test/config/config.orchestrator.yaml
+-rw-r--r--   0        0        0     4696 2023-05-24 00:04:26.821563 fabric_cf-1.5.0b4/fabric_cf/actor/test/config/config.test.yaml
+-rw-r--r--   0        0        0     5376 2023-04-03 14:50:53.620212 fabric_cf-1.5.0b4/fabric_cf/actor/test/controller_callback_helper.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.620415 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.620599 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/container/__init__.py
+-rw-r--r--   0        0        0     2815 2023-04-04 13:02:25.891866 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/container/container_database_test.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.621040 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/core/__init__.py
+-rw-r--r--   0        0        0     4091 2023-04-04 13:02:48.136107 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/core/unit_test.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.621493 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/kernel/__init__.py
+-rw-r--r--   0        0        0    21480 2023-04-04 15:12:06.450576 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/kernel/kernel_test.py
+-rw-r--r--   0        0        0     3378 2023-04-04 15:11:51.860496 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/kernel/tick_test.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.624033 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/__init__.py
+-rw-r--r--   0        0        0     3176 2023-04-04 15:15:43.466105 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/actor_database_test.py
+-rw-r--r--   0        0        0     4729 2023-04-04 17:23:55.100076 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py
+-rw-r--r--   0        0        0     1963 2023-04-03 14:50:53.624564 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/authority_substrate_test.py
+-rw-r--r--   0        0        0     3263 2023-04-03 14:50:53.624725 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/substrate_database_test.py
+-rw-r--r--   0        0        0     2280 2023-04-04 15:15:47.470348 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/substrate_test_base.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.625348 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/__init__.py
+-rw-r--r--   0        0        0    21995 2023-05-24 00:04:26.823837 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py
+-rw-r--r--   0        0        0    23678 2023-05-24 00:04:26.824675 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py
+-rw-r--r--   0        0        0     4515 2023-05-24 00:04:26.825465 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py
+-rw-r--r--   0        0        0     1561 2023-04-03 14:50:53.626668 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py
+-rw-r--r--   0        0        0     8437 2023-04-03 14:50:53.626899 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/controller_test_wrapper.py
+-rw-r--r--   0        0        0     7719 2023-05-24 00:04:26.826204 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py
+-rw-r--r--   0        0        0     1586 2023-04-03 14:50:53.627291 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.627471 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/time/__init__.py
+-rw-r--r--   0        0        0     3786 2023-04-03 14:50:53.627666 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/time/actor_clock_test.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.627830 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/time/calendar/__init__.py
+-rw-r--r--   0        0        0     4290 2023-04-03 14:50:53.628007 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py
+-rw-r--r--   0        0        0     2225 2023-04-03 14:50:53.628189 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py
+-rw-r--r--   0        0        0    14887 2023-04-03 14:50:53.628405 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/time/term_test.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.628584 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/util/__init__.py
+-rw-r--r--   0        0        0     8041 2023-04-03 14:50:53.628792 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/util/reservation_holdings_test.py
+-rw-r--r--   0        0        0     5072 2023-04-03 14:50:53.628930 fabric_cf-1.5.0b4/fabric_cf/actor/test/core/util/reservation_list_test.py
+-rw-r--r--   0        0        0     3738 2023-04-03 14:50:53.629079 fabric_cf-1.5.0b4/fabric_cf/actor/test/dummy_authority_proxy.py
+-rw-r--r--   0        0        0     1953 2023-04-03 14:50:53.629248 fabric_cf-1.5.0b4/fabric_cf/actor/test/dummy_proxy.py
+-rw-r--r--   0        0        0     2498 2023-04-04 16:00:31.265177 fabric_cf-1.5.0b4/fabric_cf/actor/test/fim_test_helper.py
+-rw-r--r--   0        0        0       92 2023-04-03 15:02:26.648185 fabric_cf-1.5.0b4/fabric_cf/actor/test/schema/key.avsc
+-rw-r--r--   0        0        0    27389 2023-04-03 15:02:26.648701 fabric_cf-1.5.0b4/fabric_cf/actor/test/schema/message.avsc
+-rw-r--r--   0        0        0     4532 2023-04-03 15:21:18.938300 fabric_cf-1.5.0b4/fabric_cf/actor/test/test_abqm.py
+-rw-r--r--   0        0        0     1892 2023-04-03 14:50:53.630509 fabric_cf-1.5.0b4/fabric_cf/actor/test/test_actor.py
+-rw-r--r--   0        0        0     1249 2023-04-03 14:50:53.630745 fabric_cf-1.5.0b4/fabric_cf/actor/test/test_exception.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.630912 fabric_cf-1.5.0b4/fabric_cf/aits/__init__.py
+-rw-r--r--   0        0        0     4826 2023-05-24 00:04:26.827397 fabric_cf-1.5.0b4/fabric_cf/aits/config/config.broker.yaml
+-rw-r--r--   0        0        0     4808 2023-05-24 00:04:26.828508 fabric_cf-1.5.0b4/fabric_cf/aits/config/config.netam.yaml
+-rw-r--r--   0        0        0     4414 2023-05-24 00:04:26.829350 fabric_cf-1.5.0b4/fabric_cf/aits/config/config.orchestrator.yaml
+-rw-r--r--   0        0        0     4788 2023-05-24 00:04:26.829999 fabric_cf-1.5.0b4/fabric_cf/aits/config/config.siteam.yaml
+-rw-r--r--   0        0        0    49220 2023-05-24 00:04:26.831078 fabric_cf-1.5.0b4/fabric_cf/aits/integration_test.py
+-rw-r--r--   0        0        0     7393 2023-05-24 00:04:26.832468 fabric_cf-1.5.0b4/fabric_cf/aits/kafka_processor.py
+-rw-r--r--   0        0        0     8633 2023-05-24 00:04:26.833310 fabric_cf-1.5.0b4/fabric_cf/aits/manage_helper.py
+-rw-r--r--   0        0        0     8339 2023-05-24 00:04:26.834033 fabric_cf-1.5.0b4/fabric_cf/aits/orchestrator_helper.py
+-rw-r--r--   0        0        0    16256 2023-04-03 14:50:53.634161 fabric_cf-1.5.0b4/fabric_cf/authority/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.634241 fabric_cf-1.5.0b4/fabric_cf/authority/__init__.py
+-rw-r--r--   0        0        0     2164 2023-04-03 14:50:53.634418 fabric_cf-1.5.0b4/fabric_cf/authority/__main__.py
+-rw-r--r--   0        0        0    32973 2023-04-03 14:50:53.634699 fabric_cf-1.5.0b4/fabric_cf/authority/am-yes.xml
+-rw-r--r--   0        0        0     4936 2023-04-03 14:50:53.634941 fabric_cf-1.5.0b4/fabric_cf/authority/config.al2s.am.yaml
+-rw-r--r--   0        0        0     5030 2023-04-03 14:50:53.635111 fabric_cf-1.5.0b4/fabric_cf/authority/config.net.am.yaml
+-rw-r--r--   0        0        0     5401 2023-05-24 00:04:26.834770 fabric_cf-1.5.0b4/fabric_cf/authority/config.site.am.geni.yaml
+-rw-r--r--   0        0        0     4895 2023-05-24 00:04:26.835456 fabric_cf-1.5.0b4/fabric_cf/authority/config.site.am.yaml
+-rw-r--r--   0        0        0     3427 2023-05-24 00:04:26.837834 fabric_cf-1.5.0b4/fabric_cf/authority/docker-compose.geni.yml
+-rw-r--r--   0        0        0     3336 2023-05-24 00:04:26.838762 fabric_cf-1.5.0b4/fabric_cf/authority/docker-compose.yml
+-rw-r--r--   0        0        0     1188 2023-05-24 00:04:26.839829 fabric_cf-1.5.0b4/fabric_cf/authority/env.template
+-rw-r--r--   0        0        0    16080 2023-04-03 14:50:53.636162 fabric_cf-1.5.0b4/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml
+-rw-r--r--   0        0        0     1588 2023-04-03 14:50:53.636606 fabric_cf-1.5.0b4/fabric_cf/authority/net_handler_config.yml
+-rw-r--r--   0        0        0     1523 2023-04-03 14:50:53.636812 fabric_cf-1.5.0b4/fabric_cf/authority/oess_handler_config.yml
+-rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.636998 fabric_cf-1.5.0b4/fabric_cf/authority/pdp.xml
+-rwxr-xr-x   0        0        0     2446 2023-04-03 14:50:53.637179 fabric_cf-1.5.0b4/fabric_cf/authority/setup.sh
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.637346 fabric_cf-1.5.0b4/fabric_cf/authority/test/__init__.py
+-rw-r--r--   0        0        0     2463 2023-04-03 14:50:53.637572 fabric_cf-1.5.0b4/fabric_cf/authority/test/al2s_am.py
+-rw-r--r--   0        0        0     2459 2023-04-03 14:50:53.637740 fabric_cf-1.5.0b4/fabric_cf/authority/test/net_am.py
+-rw-r--r--   0        0        0     2456 2023-04-03 14:50:53.637876 fabric_cf-1.5.0b4/fabric_cf/authority/test/site_am.py
+-rw-r--r--   0        0        0     2461 2023-04-03 14:50:53.638045 fabric_cf-1.5.0b4/fabric_cf/authority/test/site_am_geni.py
+-rw-r--r--   0        0        0     4730 2023-05-24 00:04:37.574097 fabric_cf-1.5.0b4/fabric_cf/authority/test/test-al2sam.yaml
+-rw-r--r--   0        0        0     4839 2023-05-23 17:37:14.086091 fabric_cf-1.5.0b4/fabric_cf/authority/test/test-netam.yaml
+-rw-r--r--   0        0        0     5071 2023-04-03 14:50:53.638536 fabric_cf-1.5.0b4/fabric_cf/authority/test/test.geni.yaml
+-rw-r--r--   0        0        0     4685 2023-05-23 17:37:14.088483 fabric_cf-1.5.0b4/fabric_cf/authority/test/test.yaml
+-rw-r--r--   0        0        0     2779 2023-05-22 19:03:15.235304 fabric_cf-1.5.0b4/fabric_cf/authority/vm_handler_config.yml
+-rw-r--r--   0        0        0     1448 2023-04-03 14:50:53.639031 fabric_cf-1.5.0b4/fabric_cf/authority/vnic_net_handler_config.yml
+-rw-r--r--   0        0        0    14262 2023-04-03 14:50:53.639328 fabric_cf-1.5.0b4/fabric_cf/broker/Readme.md
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.639412 fabric_cf-1.5.0b4/fabric_cf/broker/__init__.py
+-rw-r--r--   0        0        0     2290 2023-04-03 14:50:53.639603 fabric_cf-1.5.0b4/fabric_cf/broker/__main__.py
+-rw-r--r--   0        0        0    27944 2023-04-03 14:50:53.639781 fabric_cf-1.5.0b4/fabric_cf/broker/broker-yes.xml
+-rw-r--r--   0        0        0     5034 2023-05-24 00:04:26.841463 fabric_cf-1.5.0b4/fabric_cf/broker/config.broker.yaml
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.640163 fabric_cf-1.5.0b4/fabric_cf/broker/core/__init__.py
+-rw-r--r--   0        0        0     3314 2023-04-03 14:50:53.640348 fabric_cf-1.5.0b4/fabric_cf/broker/core/broker_kernel.py
+-rw-r--r--   0        0        0     3135 2023-05-24 00:04:26.842130 fabric_cf-1.5.0b4/fabric_cf/broker/docker-compose.yml
+-rw-r--r--   0        0        0     1192 2023-05-24 00:04:26.843033 fabric_cf-1.5.0b4/fabric_cf/broker/env.template
+-rw-r--r--   0        0        0    16080 2023-04-03 14:50:53.640954 fabric_cf-1.5.0b4/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml
+-rw-r--r--   0        0        0     1380 2023-04-03 14:50:53.641105 fabric_cf-1.5.0b4/fabric_cf/broker/pdp.xml
+-rwxr-xr-x   0        0        0     2239 2023-04-03 14:50:53.641257 fabric_cf-1.5.0b4/fabric_cf/broker/setup.sh
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.641487 fabric_cf-1.5.0b4/fabric_cf/broker/test/__init__.py
+-rw-r--r--   0        0        0     2507 2023-04-03 14:50:53.641689 fabric_cf-1.5.0b4/fabric_cf/broker/test/broker.py
+-rw-r--r--   0        0        0     5042 2023-05-23 17:33:26.677448 fabric_cf-1.5.0b4/fabric_cf/broker/test/test.yaml
+-rw-r--r--   0        0        0    20305 2023-05-22 19:03:15.236804 fabric_cf-1.5.0b4/fabric_cf/orchestrator/README.md
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.642384 fabric_cf-1.5.0b4/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0     3355 2023-05-22 19:03:15.237157 fabric_cf-1.5.0b4/fabric_cf/orchestrator/__main__.py
+-rw-r--r--   0        0        0     1757 2023-04-03 14:50:53.642803 fabric_cf-1.5.0b4/fabric_cf/orchestrator/certs/fullchain.pem
+-rw-r--r--   0        0        0     3272 2023-04-03 14:50:53.642965 fabric_cf-1.5.0b4/fabric_cf/orchestrator/certs/privkey.pem
+-rw-r--r--   0        0        0     4858 2023-05-24 00:04:26.844226 fabric_cf-1.5.0b4/fabric_cf/orchestrator/config.orchestrator.yaml
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.643278 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/__init__.py
+-rw-r--r--   0        0        0     2917 2023-04-03 14:50:53.643501 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/active_status_checker.py
+-rw-r--r--   0        0        0     3050 2023-04-03 14:50:53.643707 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/bqm_wrapper.py
+-rw-r--r--   0        0        0     1556 2023-04-03 14:50:53.643947 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/exceptions.py
+-rw-r--r--   0        0        0     1884 2023-04-03 14:50:53.644155 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/i_status_update_callback.py
+-rw-r--r--   0        0        0    44213 2023-06-08 14:58:07.020596 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/orchestrator_handler.py
+-rw-r--r--   0        0        0     5389 2023-04-03 14:50:53.644692 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/orchestrator_kernel.py
+-rw-r--r--   0        0        0    34864 2023-05-22 18:59:29.517601 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py
+-rw-r--r--   0        0        0     3581 2023-04-03 14:50:53.645306 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/reservation_converter.py
+-rw-r--r--   0        0        0     4880 2023-04-03 14:50:53.645464 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/reservation_status_update.py
+-rw-r--r--   0        0        0     7876 2023-04-03 14:50:53.645708 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/reservation_status_update_thread.py
+-rw-r--r--   0        0        0     7054 2023-06-08 13:03:31.950909 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/response_builder.py
+-rw-r--r--   0        0        0     8722 2023-05-24 00:04:26.845643 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/slice_defer_thread.py
+-rw-r--r--   0        0        0     1972 2023-04-03 14:50:53.646372 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/status_checker.py
+-rw-r--r--   0        0        0     1581 2023-04-03 14:50:53.646556 fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/watch_entry.py
+-rw-r--r--   0        0        0     3501 2023-05-24 00:04:26.846779 fabric_cf-1.5.0b4/fabric_cf/orchestrator/docker-compose.yml
+-rw-r--r--   0        0        0     1198 2023-05-24 00:04:26.847620 fabric_cf-1.5.0b4/fabric_cf/orchestrator/env.template
+-rw-r--r--   0        0        0    72323 2023-04-03 14:50:53.647218 fabric_cf-1.5.0b4/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml
+-rw-r--r--   0        0        0     1626 2023-04-03 14:50:53.647500 fabric_cf-1.5.0b4/fabric_cf/orchestrator/nginx/default.conf
+-rw-r--r--   0        0        0    58562 2023-06-08 13:40:39.072943 fabric_cf-1.5.0b4/fabric_cf/orchestrator/openapi.json
+-rw-r--r--   0        0        0    30829 2023-04-03 14:50:53.648266 fabric_cf-1.5.0b4/fabric_cf/orchestrator/orchestrator-yes.xml
+-rw-r--r--   0        0        0     1548 2023-04-03 14:50:53.648514 fabric_cf-1.5.0b4/fabric_cf/orchestrator/pdp.xml
+-rwxr-xr-x   0        0        0     2284 2023-04-03 14:50:53.648696 fabric_cf-1.5.0b4/fabric_cf/orchestrator/setup.sh
+-rw-r--r--   0        0        0      430 2023-06-08 14:44:49.898518 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/__init__.py
+-rw-r--r--   0        0        0      392 2023-06-08 14:44:49.904039 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:44:49.878471 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/controllers/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-08 14:47:34.916836 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/controllers/authorization_controller.py
+-rw-r--r--   0        0        0     1249 2023-06-08 14:47:41.564653 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py
+-rw-r--r--   0        0        0     6147 2023-06-08 14:47:54.797076 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py
+-rw-r--r--   0        0        0     2612 2023-06-08 14:50:52.330160 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/controllers/slivers_controller.py
+-rw-r--r--   0        0        0      305 2023-06-08 14:48:00.320639 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/controllers/version_controller.py
+-rw-r--r--   0        0        0      631 2023-06-08 14:44:49.877361 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/encoder.py
+-rw-r--r--   0        0        0     2757 2023-06-08 14:44:49.870070 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/__init__.py
+-rw-r--r--   0        0        0     1889 2023-06-08 14:44:49.871855 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/base_model_.py
+-rw-r--r--   0        0        0     3400 2023-06-08 14:44:49.868723 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/poa.py
+-rw-r--r--   0        0        0     4131 2023-06-08 14:44:49.876223 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/poa_data.py
+-rw-r--r--   0        0        0     2624 2023-06-08 14:44:49.867405 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/poa_post.py
+-rw-r--r--   0        0        0     2712 2023-06-08 14:44:49.870370 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/poa_post_data.py
+-rw-r--r--   0        0        0     2254 2023-06-08 14:44:49.877067 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     1628 2023-06-08 14:44:49.869816 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/resource.py
+-rw-r--r--   0        0        0     3564 2023-06-08 14:44:49.872466 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/resources.py
+-rw-r--r--   0        0        0     7311 2023-06-08 14:44:49.868459 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/slice.py
+-rw-r--r--   0        0        0     3616 2023-06-08 14:44:49.866799 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/slice_details.py
+-rw-r--r--   0        0        0     5251 2023-06-08 14:44:49.873862 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/slices.py
+-rw-r--r--   0        0        0     2634 2023-06-08 14:44:49.872181 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/slices_post.py
+-rw-r--r--   0        0        0     8995 2023-06-08 14:44:49.876584 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/sliver.py
+-rw-r--r--   0        0        0     5301 2023-06-08 14:44:49.873519 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/slivers.py
+-rw-r--r--   0        0        0     3896 2023-06-08 14:44:49.874408 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     2464 2023-06-08 14:44:49.869004 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     4929 2023-06-08 14:44:49.871494 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     2870 2023-06-08 14:44:49.870652 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py
+-rw-r--r--   0        0        0     1983 2023-06-08 14:44:49.871163 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py
+-rw-r--r--   0        0        0     4503 2023-06-08 14:44:49.875103 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     3984 2023-06-08 14:44:49.873193 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     2512 2023-06-08 14:44:49.867118 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     3879 2023-06-08 14:44:49.872837 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py
+-rw-r--r--   0        0        0     2461 2023-06-08 14:44:49.869556 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     3846 2023-06-08 14:44:49.870907 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py
+-rw-r--r--   0        0        0     2446 2023-06-08 14:44:49.875848 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     4233 2023-06-08 14:44:49.869279 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     2635 2023-06-08 14:44:49.867678 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3540 2023-06-08 14:44:49.868184 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/version.py
+-rw-r--r--   0        0        0     2536 2023-06-08 14:44:49.867936 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/version_data.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:44:49.887095 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/__init__.py
+-rw-r--r--   0        0        0     1355 2023-06-08 14:44:49.891764 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py
+-rw-r--r--   0        0        0     2062 2023-06-08 14:56:16.236641 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/constants.py
+-rw-r--r--   0        0        0     5537 2023-06-08 14:44:49.886605 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/cors_response.py
+-rw-r--r--   0        0        0     4321 2023-06-08 14:44:49.892505 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/resources_controller.py
+-rw-r--r--   0        0        0    15437 2023-06-08 14:44:49.891045 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/slices_controller.py
+-rw-r--r--   0        0        0     9160 2023-06-08 14:58:07.024943 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/slivers_controller.py
+-rw-r--r--   0        0        0     2530 2023-06-08 14:44:49.890741 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/utils.py
+-rw-r--r--   0        0        0     2632 2023-06-08 14:44:49.892154 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/version_controller.py
+-rw-r--r--   0        0        0    42358 2023-06-08 14:44:49.865553 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml
+-rw-r--r--   0        0        0      438 2023-06-08 14:44:49.864888 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/test/__init__.py
+-rw-r--r--   0        0        0     2094 2023-06-08 14:44:49.864547 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py
+-rw-r--r--   0        0        0     5271 2023-06-08 14:44:49.863985 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py
+-rw-r--r--   0        0        0     3518 2023-06-08 14:44:49.863608 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/test/test_slivers_controller.py
+-rw-r--r--   0        0        0      855 2023-06-08 14:44:49.864291 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py
+-rw-r--r--   0        0        0      809 2023-06-08 14:44:49.877812 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/type_util.py
+-rw-r--r--   0        0        0     3452 2023-06-08 14:44:49.865880 fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/util.py
+-rw-r--r--   0        0        0        0 2023-04-03 14:50:53.659106 fabric_cf-1.5.0b4/fabric_cf/orchestrator/test/__init__.py
+-rw-r--r--   0        0        0     3542 2023-04-03 14:50:53.659281 fabric_cf-1.5.0b4/fabric_cf/orchestrator/test/orchestrator.py
+-rwxr-xr-x   0        0        0       78 2023-04-03 14:50:53.659409 fabric_cf-1.5.0b4/fabric_cf/orchestrator/test/test.sh
+-rw-r--r--   0        0        0     4453 2023-06-07 16:39:01.078654 fabric_cf-1.5.0b4/fabric_cf/orchestrator/test/test.yaml
+-rwxr-xr-x   0        0        0     2900 2023-04-03 14:50:53.659782 fabric_cf-1.5.0b4/fabric_cf/orchestrator/update_swagger_stub.sh
+-rw-r--r--   0        0        0    18177 2023-04-03 14:50:53.660187 fabric_cf-1.5.0b4/images/am-pod.png
+-rw-r--r--   0        0        0    74927 2023-04-03 14:50:53.660890 fabric_cf-1.5.0b4/images/am.png
+-rw-r--r--   0        0        0    18471 2023-04-03 14:50:53.661225 fabric_cf-1.5.0b4/images/broker-pod.png
+-rw-r--r--   0        0        0    73799 2023-04-03 14:50:53.661878 fabric_cf-1.5.0b4/images/broker.png
+-rw-r--r--   0        0        0    90831 2023-04-03 14:50:53.662835 fabric_cf-1.5.0b4/images/cf.png
+-rw-r--r--   0        0        0    19611 2023-04-03 14:50:53.663247 fabric_cf-1.5.0b4/images/orchestrator-pod.png
+-rw-r--r--   0        0        0    78622 2023-04-03 14:50:53.664084 fabric_cf-1.5.0b4/images/orchestrator.png
+-rw-r--r--   0        0        0   145542 2023-04-03 14:50:53.664854 fabric_cf-1.5.0b4/neo4j/AL2S.graphml
+-rw-r--r--   0        0        0    96363 2023-04-03 14:50:53.665732 fabric_cf-1.5.0b4/neo4j/LBNL-ad.graphml
+-rw-r--r--   0        0        0    68182 2023-04-03 14:50:53.666334 fabric_cf-1.5.0b4/neo4j/Network-ad.graphml
+-rw-r--r--   0        0        0    96375 2023-04-03 14:50:53.666804 fabric_cf-1.5.0b4/neo4j/RENCI-ad.graphml
+-rw-r--r--   0        0        0    96286 2023-04-03 14:50:53.667143 fabric_cf-1.5.0b4/neo4j/UKY-ad.graphml
+-rw-r--r--   0        0        0  1297955 2023-04-03 14:50:53.672629 fabric_cf-1.5.0b4/neo4j/UKY2.graphml
+-rw-r--r--   0        0        0    14808 2023-04-03 14:50:53.673167 fabric_cf-1.5.0b4/neo4j/abqm.graphml
+-rw-r--r--   0        0        0     1757 2023-04-03 14:50:53.673435 fabric_cf-1.5.0b4/neo4j/certs/fullchain.pem
+-rw-r--r--   0        0        0     3272 2023-04-03 14:50:53.673617 fabric_cf-1.5.0b4/neo4j/certs/privkey.pem
+-rwxr-xr-x   0        0        0       91 2023-04-03 14:50:53.673785 fabric_cf-1.5.0b4/orchestrator.sh
+-rw-r--r--   0        0        0      698 2023-04-03 14:50:53.673962 fabric_cf-1.5.0b4/psql.upgrade
+-rw-r--r--   0        0        0     1250 2023-06-08 14:59:43.875860 fabric_cf-1.5.0b4/pyproject.toml
+-rwxr-xr-x   0        0        0     2594 2023-05-24 00:04:26.854514 fabric_cf-1.5.0b4/secrets/create-certs.sh
+-rw-r--r--   0        0        0    12796 2023-05-22 19:03:15.242478 fabric_cf-1.5.0b4/tools/audit.py
+-rw-r--r--   0        0        0     8005 2023-04-03 14:50:53.675250 fabric_cf-1.5.0b4/tools/db_cli.py
+-rw-r--r--   0        0        0      354 2023-05-22 19:03:15.243289 fabric_cf-1.5.0b4/tools/install.sh
+-rw-r--r--   0        0        0      143 2023-04-03 14:50:53.675627 fabric_cf-1.5.0b4/tox.ini
+-rw-r--r--   0        0        0     3315 1970-01-01 00:00:00.000000 fabric_cf-1.5.0b4/PKG-INFO
```

### Comparing `fabric_cf-1.5.0b3/.gitignore` & `fabric_cf-1.5.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/Dockerfile-auth` & `fabric_cf-1.5.0b4/Dockerfile-auth`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 FROM python:3.9.0
 MAINTAINER Komal Thareja<komal.thareja@gmail.com>
 
-ARG HANDLERS_VER=1.5.0b2
+ARG HANDLERS_VER=1.5.0b4
 
 RUN mkdir -p /usr/src/app
 WORKDIR /usr/src/app
 VOLUME ["/usr/src/app"]
 
 EXPOSE 11000
```

### Comparing `fabric_cf-1.5.0b3/Dockerfile-broker` & `fabric_cf-1.5.0b4/Dockerfile-broker`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/Dockerfile-cf` & `fabric_cf-1.5.0b4/Dockerfile-cf`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/Dockerfile-orchestrator` & `fabric_cf-1.5.0b4/Dockerfile-orchestrator`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/LICENSE` & `fabric_cf-1.5.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/README.md` & `fabric_cf-1.5.0b4/README.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/cleanup_old_schema_from_schema_registry.sh` & `fabric_cf-1.5.0b4/cleanup_old_schema_from_schema_registry.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/docker-compose-kafka.yaml` & `fabric_cf-1.5.0b4/docker-compose-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/docker-compose-no-ssl-kafka.yaml` & `fabric_cf-1.5.0b4/docker-compose-no-ssl-kafka.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/docker-compose-test.yaml` & `fabric_cf-1.5.0b4/docker-compose-test.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -66,15 +66,15 @@
        - POSTGRES_HOST=${POSTGRES_HOST:-database}
        - POSTGRES_PORT=5432
        - POSTGRES_MULTIPLE_DATABASES=${POSTGRES_DB:-postgres}
        - POSTGRES_USER=${POSTGRES_USER:-postgres}
        - POSTGRES_PASSWORD=${POSTGRES_PASSWORD:-fabric}
        - PGDATA=${PGDATA:-/var/lib/postgresql/data}
   neo4j1:
-    image: fabrictestbed/neo4j-apoc:4.0.3
+    image: fabrictestbed/neo4j-apoc:5.3.0
     container_name: neo4j1
     user: ${NEO4J_UID:-1000}:${NEO4J_GID:-1000}
     restart: always
     ports:
       - 7474:7474  # for HTTP
       - 7473:7473  # for HTTPS
       - 7687:7687  # for Bolt
@@ -82,22 +82,22 @@
       - ${NEO4DATA_HOST:-.}/neo4j1/data:/data
       - ${NEO4DATA_HOST:-.}/neo4j1/imports:/imports
       - ${NEO4DATA_HOST:-.}/neo4j1/logs:/logs
       - ./neo4j/certs/fullchain.pem:/ssl/neo4j.cert:ro  # SSL development certificate
       - ./neo4j/certs/privkey.pem:/ssl/neo4j.key:ro     # SSL development key
     environment:
       - NEO4J_AUTH=${NEO4J_USER:-neo4j}/${NEO4J_PASS:-password}
-      - NEO4J_dbms_connector_bolt_advertised__address=0.0.0.0:7687
-      - NEO4J_dbms_connector_bolt_listen__address=0.0.0.0:7687
-      - NEO4J_dbms_connector_http_advertised__address=0.0.0.0:7474
-      - NEO4J_dbms_connector_http_listen__address=0.0.0.0:7474
-      - NEO4J_dbms_connector_https_advertised__address=0.0.0.0:7473
-      - NEO4J_dbms_connector_https_listen__address=0.0.0.0:7473
+      - NEO4J_server_bolt_advertised__address=:7687
+      - NEO4J_server_bolt_listen__address=:7687
+      - NEO4J_server_http_advertised__address=:7474
+      - NEO4J_server_http_listen__address=:7474
+      - NEO4J_server_https_advertised__address=:7473
+      - NEO4J_server_https_listen__address=:7473
   neo4j2:
-    image: fabrictestbed/neo4j-apoc:4.0.3
+    image: fabrictestbed/neo4j-apoc:5.3.0
     container_name: neo4j2
     user: ${NEO4J_UID:-1000}:${NEO4J_GID:-1000}
     restart: always
     ports:
       - 8474:8474  # for HTTP
       - 8473:8473  # for HTTPS
       - 8687:8687  # for Bolt
@@ -105,22 +105,22 @@
       - ${NEO4DATA_HOST:-.}/neo4j2/data:/data
       - ${NEO4DATA_HOST:-.}/neo4j2/imports:/imports
       - ${NEO4DATA_HOST:-.}/neo4j2/logs:/logs
       - ./neo4j/certs/fullchain.pem:/ssl/neo4j.cert:ro  # SSL development certificate
       - ./neo4j/certs/privkey.pem:/ssl/neo4j.key:ro     # SSL development key
     environment:
       - NEO4J_AUTH=${NEO4J_USER:-neo4j}/${NEO4J_PASS:-password}
-      - NEO4J_dbms_connector_bolt_advertised__address=0.0.0.0:8687
-      - NEO4J_dbms_connector_bolt_listen__address=0.0.0.0:8687
-      - NEO4J_dbms_connector_http_advertised__address=0.0.0.0:8474
-      - NEO4J_dbms_connector_http_listen__address=0.0.0.0:8474
-      - NEO4J_dbms_connector_https_advertised__address=0.0.0.0:8473
-      - NEO4J_dbms_connector_https_listen__address=0.0.0.0:8473
+      - NEO4J_server_bolt_advertised__address=:8687
+      - NEO4J_server_bolt_listen__address=:8687
+      - NEO4J_server_http_advertised__address=:8474
+      - NEO4J_server_http_listen__address=:8474
+      - NEO4J_server_https_advertised__address=:8473
+      - NEO4J_server_https_listen__address=:8473
   neo4j3:
-    image: fabrictestbed/neo4j-apoc:4.0.3
+    image: fabrictestbed/neo4j-apoc:5.3.0
     container_name: neo4j3
     user: ${NEO4J_UID:-1000}:${NEO4J_GID:-1000}
     restart: always
     ports:
       - 9474:9474  # for HTTP
       - 9473:9473  # for HTTPS
       - 9687:9687  # for Bolt
@@ -128,22 +128,22 @@
       - ${NEO4DATA_HOST:-.}/neo4j3/data:/data
       - ${NEO4DATA_HOST:-.}/neo4j3/imports:/imports
       - ${NEO4DATA_HOST:-.}/neo4j3/logs:/logs
       - ./neo4j/certs/fullchain.pem:/ssl/neo4j.cert:ro  # SSL development certificate
       - ./neo4j/certs/privkey.pem:/ssl/neo4j.key:ro     # SSL development key
     environment:
       - NEO4J_AUTH=${NEO4J_USER:-neo4j}/${NEO4J_PASS:-password}
-      - NEO4J_dbms_connector_bolt_advertised__address=0.0.0.0:9687
-      - NEO4J_dbms_connector_bolt_listen__address=0.0.0.0:9687
-      - NEO4J_dbms_connector_http_advertised__address=0.0.0.0:9474
-      - NEO4J_dbms_connector_http_listen__address=0.0.0.0:9474
-      - NEO4J_dbms_connector_https_advertised__address=0.0.0.0:9473
-      - NEO4J_dbms_connector_https_listen__address=0.0.0.0:9473
+      - NEO4J_server_bolt_advertised__address=:9687
+      - NEO4J_server_bolt_listen__address=:9687
+      - NEO4J_server_http_advertised__address=:9474
+      - NEO4J_server_http_listen__address=:9474
+      - NEO4J_server_https_advertised__address=:9473
+      - NEO4J_server_https_listen__address=:9473
   neo4j4:
-    image: fabrictestbed/neo4j-apoc:4.0.3
+    image: fabrictestbed/neo4j-apoc:5.3.0
     container_name: neo4j4
     user: ${NEO4J_UID:-1000}:${NEO4J_GID:-1000}
     restart: always
     ports:
       - 6474:6474  # for HTTP
       - 6473:6473  # for HTTPS
       - 6687:6687  # for Bolt
@@ -151,22 +151,22 @@
       - ${NEO4DATA_HOST:-.}/neo4j4/data:/data
       - ${NEO4DATA_HOST:-.}/neo4j4/imports:/imports
       - ${NEO4DATA_HOST:-.}/neo4j4/logs:/logs
       - ./neo4j/certs/fullchain.pem:/ssl/neo4j.cert:ro  # SSL development certificate
       - ./neo4j/certs/privkey.pem:/ssl/neo4j.key:ro     # SSL development key
     environment:
       - NEO4J_AUTH=${NEO4J_USER:-neo4j}/${NEO4J_PASS:-password}
-      - NEO4J_dbms_connector_bolt_advertised__address=0.0.0.0:6687
-      - NEO4J_dbms_connector_bolt_listen__address=0.0.0.0:6687
-      - NEO4J_dbms_connector_http_advertised__address=0.0.0.0:6474
-      - NEO4J_dbms_connector_http_listen__address=0.0.0.0:6474
-      - NEO4J_dbms_connector_https_advertised__address=0.0.0.0:6473
-      - NEO4J_dbms_connector_https_listen__address=0.0.0.0:6473
+      - NEO4J_server_bolt_advertised__address=:6687
+      - NEO4J_server_bolt_listen__address=:6687
+      - NEO4J_server_http_advertised__address=:6474
+      - NEO4J_server_http_listen__address=:6474
+      - NEO4J_server_https_advertised__address=:6473
+      - NEO4J_server_https_listen__address=:6473
   neo4j5:
-    image: fabrictestbed/neo4j-apoc:4.0.3
+    image: fabrictestbed/neo4j-apoc:5.3.0
     container_name: neo4j5
     user: ${NEO4J_UID:-1000}:${NEO4J_GID:-1000}
     restart: always
     ports:
       - 10474:10474  # for HTTP
       - 10473:10473  # for HTTPS
       - 10687:10687  # for Bolt
@@ -174,20 +174,20 @@
       - ${NEO4DATA_HOST:-.}/neo4j5/data:/data
       - ${NEO4DATA_HOST:-.}/neo4j5/imports:/imports
       - ${NEO4DATA_HOST:-.}/neo4j5/logs:/logs
       - ./neo45/certs/fullchain.pem:/ssl/neo4j.cert:ro  # SSL development certificate
       - ./neo45/certs/privkey.pem:/ssl/neo4j.key:ro     # SSL development key
     environment:
       - NEO4J_AUTH=${NEO4J_USER:-neo4j}/${NEO4J_PASS:-password}
-      - NEO4J_dbms_connector_bolt_advertised__address=0.0.0.0:10687
-      - NEO4J_dbms_connector_bolt_listen__address=0.0.0.0:10687
-      - NEO4J_dbms_connector_http_advertised__address=0.0.0.0:10474
-      - NEO4J_dbms_connector_http_listen__address=0.0.0.0:10474
-      - NEO4J_dbms_connector_https_advertised__address=0.0.0.0:10473
-      - NEO4J_dbms_connector_https_listen__address=0.0.0.0:10473
+      - NEO4J_server_bolt_advertised__address=:10687
+      - NEO4J_server_bolt_listen__address=:10687
+      - NEO4J_server_http_advertised__address=:10474
+      - NEO4J_server_http_listen__address=:10474
+      - NEO4J_server_https_advertised__address=:10473
+      - NEO4J_server_https_listen__address=:10473
   cf-base:
     build:
       context: .
       dockerfile: Dockerfile-cf
     image: controlframework:latest
   am:
     image: controlframework:latest
```

### Comparing `fabric_cf-1.5.0b3/env.template.test` & `fabric_cf-1.5.0b4/env.template.test`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabricNo.AnyActorNoPolicy.xml` & `fabric_cf-1.5.0b4/fabricNo.AnyActorNoPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/Design.md` & `fabric_cf-1.5.0b4/fabric_cf/Design.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/boot/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_exception.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/boot/configuration_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_loader.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/boot/configuration_loader.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/boot/configuration_processor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/boot/configuration_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/boot/inventory/aggregate_resource_model_creator.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_container.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_event.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_identity.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_identity.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_management_object.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_proxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,31 +24,28 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import TYPE_CHECKING
 
-from fabric_cf.actor.core.apis.abc_management_object import ABCManagementObject
+from fabric_cf.actor.core.apis.abc_proxy import ABCProxy
+
 if TYPE_CHECKING:
-    from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
+    from fabric_cf.actor.core.apis.abc_callback_proxy import ABCCallbackProxy
     from fabric_cf.actor.security.auth_token import AuthToken
 
 
-class ABCActorManagementObject(ABCManagementObject):
+class ABCActorProxy(ABCProxy):
     """
-    Interface for Management Object for an Actor
+    IActorProxy represents the proxy interface to a generic actor
     """
     @abstractmethod
-    def set_actor(self, *, actor: ABCActorMixin):
-        """
-        Set an actor
-        @params actor: actor
+    def prepare_query(self, *, callback: ABCCallbackProxy, query: dict, caller: AuthToken):
         """
+        Prepares the query
 
-    @abstractmethod
-    def update_reservation(self, *, reservation, caller: AuthToken):
-        """
-        Update Reservation
-        @params reservation: reservation
-        @params caller: caller
+        Args:
+            callback: proxy call back which handles the query
+            query: query
+            caller: caller of the query
         """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_mixin.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,21 +25,21 @@
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from abc import abstractmethod
 from enum import Enum
 from typing import TYPE_CHECKING, List, Dict
 
+
 from fabric_cf.actor.boot.configuration import ActorConfig
 from fabric_cf.actor.core.apis.abc_actor_runnable import ABCActorRunnable
 from fabric_cf.actor.core.apis.abc_timer_queue import ABCTimerQueue
 from fabric_cf.actor.core.apis.abc_actor_identity import ABCActorIdentity
 
 from fabric_cf.actor.core.apis.abc_tick import ABCTick
-from fabric_cf.actor.core.container.maintenance import Site
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_actor_event import ABCActorEvent
     from fabric_cf.actor.core.apis.abc_actor_proxy import ABCActorProxy
     from fabric_cf.actor.core.apis.abc_base_plugin import ABCBasePlugin
     from fabric_cf.actor.core.apis.abc_query_response_handler import ABCQueryResponseHandler
     from fabric_cf.actor.core.kernel.failed_rpc import FailedRPC
@@ -49,14 +49,16 @@
     from fabric_cf.actor.core.apis.abc_policy import ABCPolicy
     from fabric_cf.actor.core.apis.abc_slice import ABCSlice
     from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
     from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
     from fabric_cf.actor.core.util.reservation_set import ReservationSet
     from fabric_cf.actor.core.kernel.resource_set import ResourceSet
     from fabric_cf.actor.core.time.term import Term
+    from fabric_cf.actor.core.kernel.poa import Poa
+    from fabric_cf.actor.core.container.maintenance import Site
 
 
 class ActorType(Enum):
     """
     Enum for Actor Type
     """
     All = 0
@@ -725,8 +727,8 @@
     def update_maintenance_mode(self, *, properties: Dict[str, str], sites: List[Site] = None):
         """
         Update Maintenance mode
         @param properties properties
         @param sites sites
 
         @raises Exception in case of failure
-        """
+        """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_proxy_factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,31 +21,39 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
-from abc import abstractmethod
+from abc import abstractmethod, ABC
 from typing import TYPE_CHECKING
 
-from fabric_cf.actor.core.apis.abc_proxy import ABCProxy
-
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_callback_proxy import ABCCallbackProxy
-    from fabric_cf.actor.security.auth_token import AuthToken
+    from fabric_cf.actor.core.apis.abc_proxy import ABCProxy
+    from fabric_cf.actor.core.apis.abc_actor_identity import ABCActorIdentity
+    from fabric_cf.actor.core.proxies.actor_location import ActorLocation
 
 
-class ABCActorProxy(ABCProxy):
+class ABCProxyFactory(ABC):
     """
-    IActorProxy represents the proxy interface to a generic actor
+    Interface for Factory class for creating Proxies
     """
     @abstractmethod
-    def prepare_query(self, *, callback: ABCCallbackProxy, query: dict, caller: AuthToken):
+    def new_callback(self, *, identity: ABCActorIdentity, location: ActorLocation) -> ABCCallbackProxy:
+        """
+        Create a new callback
+        @param identity: identity
+        @param location: location
+        @return ICallbackProxy
         """
-        Prepares the query
 
-        Args:
-            callback: proxy call back which handles the query
-            query: query
-            caller: caller of the query
+    @abstractmethod
+    def new_proxy(self, *, identity: ABCActorIdentity, location: ActorLocation, proxy_type: str = None) -> ABCProxy:
+        """
+        Create a new proxy
+        @param identity: identity
+        @param location: location
+        @param proxy_type: proxy_type
+        @return IProxy
         """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_actor_runnable.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_actor_runnable.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_authority.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from abc import abstractmethod
 from typing import TYPE_CHECKING
 
 from fim.graph.resources.neo4j_arm import Neo4jARMGraph
 
 from fabric_cf.actor.core.apis.abc_server_actor import ABCServerActor
+from fabric_cf.actor.core.kernel.poa import Poa
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_authority_reservation import ABCAuthorityReservation
     from fabric_cf.actor.core.apis.abc_controller_callback_proxy import ABCControllerCallbackProxy
     from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
     from fabric_cf.actor.core.kernel.resource_set import ResourceSet
     from fabric_cf.actor.security.auth_token import AuthToken
@@ -104,14 +105,23 @@
         @param reservation reservation representing a request for a new lease
         @param callback callback
         @param caller caller
         @raises Exception in case of error
         """
 
     @abstractmethod
+    def poa(self, *, poa: Poa):
+        """
+        Processes a redeem request for the reservation.
+
+        @param poa POA
+        @raises Exception in case of error
+        """
+
+    @abstractmethod
     def close_by_caller(self, *, reservation: ABCReservationMixin, caller: AuthToken):
         """
         Closes the reservation.
 
         @params reservation:  the reservation
         @params caller : the slice owner
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_authority_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_authority_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from fabric_cf.actor.core.apis.abc_broker_proxy import ABCBrokerProxy
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_controller_callback_proxy import ABCControllerCallbackProxy
     from fabric_cf.actor.core.apis.abc_controller_reservation import ABCControllerReservation
     from fabric_cf.actor.core.apis.abc_rpc_request_state import ABCRPCRequestState
     from fabric_cf.actor.security.auth_token import AuthToken
+    from fabric_cf.actor.core.kernel.poa import Poa
 
 
 class ABCAuthorityProxy(ABCBrokerProxy):
     """
     IAuthorityProxy represents the proxy interface to an actor acting in the authority role.
     """
     @abstractmethod
@@ -69,14 +70,24 @@
         Prepare a modify lease
         @params reservation: reservation
         @params callback: callback
         @params caller: caller
         """
 
     @abstractmethod
+    def prepare_poa(self, *, callback: ABCControllerCallbackProxy, caller: AuthToken,
+                    poa: Poa) -> ABCRPCRequestState:
+        """
+        Prepare a modify lease
+        @params poa: poa
+        @params callback: callback
+        @params caller: caller
+        """
+
+    @abstractmethod
     def prepare_redeem(self, *, reservation: ABCControllerReservation, callback: ABCControllerCallbackProxy,
                        caller: AuthToken) -> ABCRPCRequestState:
         """
         Prepare a redeem
         @params reservation: reservation
         @params callback: callback
         @params caller: caller
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_authority_reservation.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_authority_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_base_plugin.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_base_plugin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_mixin.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_broker_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_broker_policy_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_broker_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_broker_reservation.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_broker_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_callback_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_client_actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,27 +24,29 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import TYPE_CHECKING
 
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fim.slivers.base_sliver import BaseSliver
 
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_broker_proxy import ABCBrokerProxy
     from fabric_cf.actor.core.apis.abc_client_reservation import ABCClientReservation
     from fabric_cf.actor.core.apis.abc_slice import ABCSlice
     from fabric_cf.actor.core.util.id import ID
     from fabric_cf.actor.core.util.reservation_set import ReservationSet
     from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
     from fabric_cf.actor.security.auth_token import AuthToken
+    from fabric_cf.actor.core.kernel.poa import Poa
 
 
 class ABCClientActor(ABCActorMixin):
     """
     IClientActor defines the common functionality for actors acting
     as clients of other actors (controllers and brokers). Every client actor
     is connected to one or more server actors. Each server actor is represented
@@ -238,8 +240,28 @@
         @param reservation reservation represented by this update. The
                reservation object will contain the lease (if any) as well
                information about the actually leased resources.
         @param update_data status of the remote operation.
         @param caller identity of the caller
 
         @throws Exception in case of error
+        """
+
+    @abstractmethod
+    def poa(self, *, poa: Poa):
+        """
+        Issue POA request for given reservation. Note: the reservation
+        must have already been registered with the actor.
+
+        @param poa Poa
+        @throws Exception in case of error
+        """
+
+    @abstractmethod
+    def poa_info(self, *, poa: Poa, caller: AuthToken):
+        """
+        Process POA response from the Authority
+
+        @param poa Poa
+        @param caller caller
+        @throws Exception in case of error
         """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_actor_management_object.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_client_actor_management_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from abc import abstractmethod, ABC
 from datetime import datetime
 from typing import TYPE_CHECKING, List
 
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fabric_mb.message_bus.messages.reservation_predecessor_avro import ReservationPredecessorAvro
 from fabric_mb.message_bus.messages.result_delegation_avro import ResultDelegationAvro
 from fabric_mb.message_bus.messages.result_strings_avro import ResultStringsAvro
 from fabric_mb.message_bus.messages.result_avro import ResultAvro
 from fim.slivers.base_sliver import BaseSliver
 from fim.user import GraphFormat
 
@@ -153,7 +154,26 @@
         """
         ReClaim delegations
         @param broker : broker ID
         @param did : delegations ID
         @param caller: caller
         @return ResultDelegationAvro
         """
+
+    @abstractmethod
+    def modify_reservation(self, *, rid: ID, modified_sliver: BaseSliver, caller: AuthToken) -> ResultAvro:
+        """
+        Modify Reservation
+        @param rid reservation id
+        @param modified_sliver modified sliver
+        @param caller caller
+        @return ResultAvro
+        """
+
+    @abstractmethod
+    def poa(self, *, poa: PoaAvro, caller: AuthToken) -> ResultAvro:
+        """
+        Modify Reservation
+        @param poa POA
+        @param caller caller
+        @return ResultAvro
+        """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_callback_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_client_callback_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_client_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_client_reservation.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_client_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_component.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_component.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_concrete_set.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_concrete_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_authority_proxy import ABCAuthorityProxy
     from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
     from fabric_cf.actor.core.time.term import Term
     from fabric_cf.actor.core.util.notice import Notice
     from fabric_cf.actor.core.util.resource_type import ResourceType
     from fabric_cf.actor.core.apis.abc_base_plugin import ABCBasePlugin
+    from fabric_cf.actor.core.kernel.poa import Poa
 
 
 class ABCConcreteSet(ABC):
     """
     IConcreteSet defines the interface for concrete set resources. A
     concrete set is intended to represent a set of resources. For example,
     compute servers, storage servers, network paths, etc.
@@ -245,7 +246,17 @@
     @abstractmethod
     def restore(self, *, plugin: ABCBasePlugin, reservation: ABCReservationMixin):
         """
         Restore the Concrete set
         @param plugin plugin
         @param reservation reservation
         """
+
+    def poa(self, *, poa: Poa):
+        """
+        Initiates POA operations on all resources contained in the set.
+        """
+
+    def get_poa_info(self) -> dict:
+        """
+        Get POA info returned by handler
+        """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_container_clock.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_container_clock.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_container_database.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_container_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_controller_callback_proxy.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_authority_reservation import ABCAuthorityReservation
     from fabric_cf.actor.core.apis.abc_callback_proxy import ABCCallbackProxy
     from fabric_cf.actor.core.apis.abc_rpc_request_state import ABCRPCRequestState
     from fabric_cf.actor.security.auth_token import AuthToken
     from fabric_cf.actor.core.util.update_data import UpdateData
+    from fabric_cf.actor.core.kernel.poa import Poa
 
 
 class ABCControllerCallbackProxy(ABCClientCallbackProxy):
     """
     IControllerCallbackProxy represents the proxy callback interface to an actor acting in the orchestrator role.
     """
 
@@ -50,8 +51,19 @@
         """
         Prepare Update Lease
         @params reservation: reservation
         @params update_data: Update Data
         @params callback: callback
         @params caller: caller
         @returns returns IRPCRequestState
+        """
+
+    @abstractmethod
+    def prepare_poa_result(self, *, poa: Poa, callback: ABCCallbackProxy, caller: AuthToken) -> ABCRPCRequestState:
+        """
+        Prepare Update Lease
+        @params reservation: reservation
+        @params update_data: Update Data
+        @params callback: callback
+        @params caller: caller
+        @returns returns IRPCRequestState
         """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_controller_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_controller_reservation.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_controller_reservation.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,16 +69,16 @@
         Returns the reservation sequence number for incoming ticket/extend ticket messages.
         @returns reservation sequence number for incoming ticket/extend ticket messages
         """
 
     @abstractmethod
     def get_lease_sequence_out(self) -> int:
         """
-        Returns the reservation sequence number for outgoing ticket/extend ticket messages.
-        @returns reservation sequence number for outgoing ticket/extend ticket messages
+        Returns the reservation sequence number for outgoing modify/extend lease messages.
+        @returns reservation sequence number for outgoing modify/extend lease messages
         """
 
     @abstractmethod
     def get_lease_term(self) -> Term:
         """
         Returns the term of the current lease.
         @returns current lease term
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_database.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from abc import abstractmethod, ABC
 from datetime import datetime
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, List, Union
 
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.kernel.slice import SliceTypes
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_broker_proxy import ABCBrokerProxy
     from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
     from fabric_cf.actor.core.apis.abc_slice import ABCSlice
     from fabric_cf.actor.core.util.id import ID
@@ -357,8 +358,55 @@
         Remove maintenance properties
         """
 
     def get_maintenance_properties(self) -> dict:
         """
         Get maintenance Properties
         @return properties
+        """
+
+    @abstractmethod
+    def add_poa(self, *, poa: Poa):
+        """
+        Adds a new record to the database representing this slice
+        object.
+
+        @param poa POA object
+
+        @throws Exception in case of error
+        """
+
+    @abstractmethod
+    def update_poa(self, *, poa: Poa):
+        """
+        Updates the corresponding database poa record.
+
+        @param poa poa info object
+
+        @throws Exception in case of error
+        """
+
+    @abstractmethod
+    def remove_poa(self, *, poa_id: str):
+        """
+        Removes the corresponding database slice record.
+
+        @param poa_id poa id
+
+        @throws Exception in case of error
+        """
+
+    @abstractmethod
+    def get_poas(self, *, poa_id: str = None, email: str = None, sliver_id: ID = None, slice_id: ID = None,
+                 project_id: str = None, limit: int = None, offset: int = None, last_update_time: datetime = None,
+                 states: list[int] = None) -> Union[List[Poa] or None]:
+        """
+        Get POAs
+        @param poa_id poa id
+        @param email email
+        @param sliver_id sliver id
+        @param slice_id slice id
+        @param project_id project id
+        @param limit limit
+        @param offset offset
+        @param last_update_time last update time
         """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_delegation.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_delegation.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,8 +405,14 @@
         Lock delegation
         """
 
     @abstractmethod
     def unlock(self):
         """
         Unlock delegation
+        """
+
+    @abstractmethod
+    def get_site(self) -> str:
+        """
+        Return Site name
         """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_event.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_management_object.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_actor.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import TYPE_CHECKING, List, Tuple, Dict
 
 from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
+from fabric_mb.message_bus.messages.poa_info_avro import PoaInfoAvro
 from fabric_mb.message_bus.messages.site_avro import SiteAvro
 
 from fabric_cf.actor.core.apis.abc_component import ABCComponent
 from fabric_cf.actor.core.container.maintenance import Site
 
 if TYPE_CHECKING:
     from fabric_mb.message_bus.messages.reservation_mng import ReservationMng
@@ -94,14 +96,15 @@
         """
 
     @abstractmethod
     def get_reservations(self, *, states: List[int] = None, slice_id: ID = None,
                          rid: ID = None, oidc_claim_sub: str = None, email: str = None, rid_list: List[str] = None,
                          type: str = None, site: str = None, node_id: str = None) -> List[ReservationMng]:
         """
+        Get Reservations
         @param states states
         @param slice_id slice ID
         @param rid reservation id
         @param oidc_claim_sub: oidc claim sub
         @param email: user email
         @param rid_list: list of Reservation Id
         @param type type of reservations like NodeSliver/NetworkServiceSliver
@@ -247,8 +250,23 @@
         Determine if slice can be provisioned
         Slice provisioning can be prohibited if Testbed is in maintenance mode
         Slice provisioning in maintenance mode may be allowed for specific projects/users
         @param project project
         @param email user's email
         @return True if allowed; False otherwise
         """
-        return True
+        return True
+
+    @abstractmethod
+    def get_poas(self, *, states: List[int] = None, slice_id: ID = None, rid: ID = None,
+                 email: str = None, poa_id: str = None, project_id: str = None) -> List[PoaInfoAvro]:
+        """
+        Get POA
+        @param states states
+        @param slice_id slice ID
+        @param rid reservation id
+        @param email: user email
+        @param project_id: project_id
+        @param poa_id: poa_id
+        Obtains all POAs
+        @return returns list of the poas
+        """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_authority.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_broker_mixin.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_client_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_container.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_controller_mixin.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import TYPE_CHECKING, List
 
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fim.slivers.base_sliver import BaseSliver
 
 from fabric_cf.actor.core.apis.abc_mgmt_client_actor import ABCMgmtClientActor
 from fabric_cf.actor.core.apis.abc_mgmt_actor import ABCMgmtActor
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.util.id import ID
@@ -55,7 +56,13 @@
     def modify_reservation(self, *, rid: ID, modified_sliver: BaseSliver) -> bool:
         """
         Modify a reservation
         @params rid: reservation id
         @params modified_sliver: modified_sliver
         @returns true for success and false for failure
         """
+
+    @abstractmethod
+    def poa(self, *, poa: PoaAvro) -> bool:
+        """
+        Issue a POA
+        """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_mgmt_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_proxy_factory.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/actor_identity.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,40 +20,39 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
-
-from abc import abstractmethod, ABC
 from typing import TYPE_CHECKING
 
+from fabric_cf.actor.core.apis.abc_actor_identity import ABCActorIdentity
+from fabric_cf.actor.security.auth_token import AuthToken
+
 if TYPE_CHECKING:
-    from fabric_cf.actor.core.apis.abc_callback_proxy import ABCCallbackProxy
-    from fabric_cf.actor.core.apis.abc_proxy import ABCProxy
-    from fabric_cf.actor.core.apis.abc_actor_identity import ABCActorIdentity
-    from fabric_cf.actor.core.proxies.actor_location import ActorLocation
+    from fabric_cf.actor.core.util.id import ID
 
 
-class ABCProxyFactory(ABC):
+class ActorIdentity(ABCActorIdentity):
     """
-    Interface for Factory class for creating Proxies
+    Represent Actor Identity
     """
-    @abstractmethod
-    def new_callback(self, *, identity: ABCActorIdentity, location: ActorLocation) -> ABCCallbackProxy:
+    def __init__(self, *, name: str, guid: ID):
+        self.auth = AuthToken(name=name, guid=guid)
+
+    def get_guid(self) -> ID:
         """
-        Create a new callback
-        @param identity: identity
-        @param location: location
-        @return ICallbackProxy
+        Return guid
+        @return guid
         """
+        return self.auth.get_guid()
 
-    @abstractmethod
-    def new_proxy(self, *, identity: ABCActorIdentity, location: ActorLocation, proxy_type: str = None) -> ABCProxy:
+    def get_identity(self) -> AuthToken:
         """
-        Create a new proxy
-        @param identity: identity
-        @param location: location
-        @param proxy_type: proxy_type
-        @return IProxy
+        Return identity
+        @return identity
         """
+        return self.auth
+
+    def get_name(self) -> str:
+        return self.auth.get_name()
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_query_response_handler.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_query_response_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_mixin.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_reservation_mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,27 +28,27 @@
 from abc import abstractmethod
 from enum import Enum
 from typing import TYPE_CHECKING
 
 from fabric_cf.actor.core.apis.abc_reservation_resources import ABCReservationResources
 from fabric_cf.actor.core.apis.abc_reservation_status import ABCReservationStatus
 
-
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
     from fabric_cf.actor.core.apis.abc_slice import ABCSlice
     from fabric_cf.actor.core.util.id import ID
     from fabric_cf.actor.core.util.reservation_state import ReservationState
     from fabric_cf.actor.core.util.resource_type import ResourceType
     from fabric_cf.actor.core.apis.abc_callback_proxy import ABCCallbackProxy
     from fabric_cf.actor.core.apis.abc_policy import ABCPolicy
     from fabric_cf.actor.core.kernel.failed_rpc import FailedRPC
     from fabric_cf.actor.core.kernel.request_types import RequestTypes
     from fabric_cf.actor.core.kernel.reservation_states import ReservationStates, ReservationPendingStates
     from fabric_cf.actor.core.util.update_data import UpdateData
+    from fabric_cf.actor.core.kernel.poa import Poa
 
 
 class ReservationCategory(Enum):
     """
     Enumeration for Reservation Category
     """
     # Unspecified reservation category.
@@ -515,8 +515,31 @@
         Lock the reservation
         """
 
     @abstractmethod
     def unlock(self):
         """
         Unlock the reservation
+        """
+
+    @abstractmethod
+    def service_poa(self):
+        """
+        Finishes processing POA.
+        @throws Exception in case of error
+        """
+
+    @abstractmethod
+    def poa(self, *, poa: Poa):
+        """
+        Trigger POA the reservation.
+
+        @throws Exception in case of error
+        """
+
+    @abstractmethod
+    def poa_info(self, *, incoming: Poa):
+        """
+        Process POA response
+
+        @throws Exception in case of error
         """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_resources.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_reservation_resources.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_reservation_status.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_reservation_status.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_resource_control.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_resource_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_response_handler.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_response_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_rpc_request_state.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_rpc_request_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_server_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_server_reservation.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_server_reservation.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_slice.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_substrate.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_substrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
 from fabric_cf.actor.core.apis.abc_base_plugin import ABCBasePlugin
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
     from fabric_cf.actor.core.core.unit import Unit
     from fabric_cf.actor.core.apis.abc_substrate_database import ABCSubstrateDatabase
+    from fabric_cf.actor.core.kernel.poa import Poa
 
 
 class ABCSubstrate(ABCBasePlugin):
     """
     Base class for Substrate Plugin
     """
     @abstractmethod
@@ -76,7 +77,15 @@
     @abstractmethod
     def update_props(self, *, reservation: ABCReservationMixin, unit: Unit):
         """
         Updates only the properties of an existing unit that is already part of the substrate.
         @param reservation reservation that contains the unit
         @param unit unit to be modified.
         """
+
+    @abstractmethod
+    def poa(self, *, unit: Unit, poa: Poa):
+        """
+        POA on an existing unit that is already part of the substrate.
+        @param poa POA that contains the unit
+        @param unit unit on which to perform operational action
+        """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_substrate_database.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_substrate_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_tick.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_ticker.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_ticker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_timer_queue.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_timer_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/apis/abc_timer_task.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/apis/abc_timer_task.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/common/constants.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/common/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     ErrorInvalidSlice = 10
     ErrorNoSuchActor = 11
     ErrorTransportFailure = 12
     ErrorTransportTimeout = 13
     ErrorNoSuchDelegation = 14
     ErrorInvalidToken = 15
     ErrorSliceExists = 16
+    ErrorNoSuchPoa = 17
 
     def interpret(self, exception=None):
         interpretations = {
             1: "Invalid Arguments",
             2: "Invalid Actor",
             3: "Invalid Reservation",
             4: "Database Error occurred",
@@ -63,15 +64,16 @@
             9: "No such broker",
             10: "Invalid Slice",
             11: "No such actor",
             12: "Transport failure",
             13: "Transport timeout",
             14: "No such delegation found",
             15: "Invalid Token",
-            16: "Slice exists"
+            16: "Slice exists",
+            17: "No such poa found"
           }
         if exception is None:
             return interpretations[self.value]
         else:
             return str(exception) + ". " + interpretations[self.value]
 
 
@@ -261,20 +263,25 @@
     DEADLINE = "deadline"
 
     PROPERTY_EXCEPTION_MESSAGE = "exception.message"
     PROPERTY_TARGET_NAME = "target.name"
     PROPERTY_TARGET_RESULT_CODE = "target.code"
     PROPERTY_TARGET_RESULT_CODE_MESSAGE = "target.code.message"
     PROPERTY_ACTION_SEQUENCE_NUMBER = "action.sequence"
+    PROPERTY_POA_INFO = "poa_info"
+    PROPERTY_INFO = "info"
+    PROPERTY_CODE = "code"
+    POA_ID = "poa_id"
 
     RESULT_CODE_EXCEPTION = -1
     RESULT_CODE_OK = 0
     TARGET_CREATE = "create"
     TARGET_DELETE = "delete"
     TARGET_MODIFY = "modify"
+    TARGET_POA = "poa"
     TARGET_CLEAN_RESTART = "clean_restart"
 
     RSV_SLC_ID = 'rsv_slc_id'
     DLG_SLC_ID = 'dlg_slc_id'
 
     USER_SSH_KEY = "user.ssh.key"
     ALGORITHM = 'algorithm'
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/common/event_logger.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/common/event_logger.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/common/exceptions.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/common/resource_config.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/common/resource_config.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/container.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/container/container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/db/container_database.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/container/db/container_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/globals.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/container/globals.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/maintenance.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/container/maintenance.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from datetime import datetime, timezone
-from typing import List, Dict, Tuple
+from typing import List, Dict, Tuple, Union
 
 from fim.slivers.maintenance_mode import MaintenanceInfo, MaintenanceState
 
 from fabric_cf.actor.core.apis.abc_database import ABCDatabase
 from fabric_cf.actor.core.common.constants import Constants
 
 
@@ -88,24 +88,64 @@
             return True
 
         return False
 
     def __str__(self):
         return f"Name: {self.name} MaintInfo: {self.maintenance_info} Properties: {self.properties}"
 
+    def clone_maintenance_info(self) -> Union[MaintenanceInfo or None]:
+        if self.maintenance_info is not None:
+            return self.maintenance_info.copy()
+        return None
+
+    def update_maintenance_info(self, maint_info: MaintenanceInfo):
+        self.maintenance_info = maint_info
+
 
 class Maintenance:
     @staticmethod
     def update_maintenance_mode(*, database: ABCDatabase, properties: Dict[str, str], sites: List[Site] = None):
+        """
+        Update Maintenance Mode at Testbed/Site/Worker Level
+        - Tesbed level Maintenance - single Site object is passed with Name = ALL
+        - Site level Maintenance - single Site object per site is passed with Name = SiteName
+        - Worker level Maintenance - single Site object per site with one entry per worker
+        @param database database
+        @param properties properties container project ids/ user emails
+        @param sites Maintenance information for the sites
+        """
         for s in sites:
+            # Set the list of allowed projects/users at the site level
             if properties is not None:
                 s.set_properties(properties=properties)
 
-            if database.get_site(site_name=s.get_name()) is not None:
-                database.update_site(site=s)
+            # Get Current Maintenance mode for the Site
+            existing_site = database.get_site(site_name=s.get_name())
+            # Site entry exists
+            if existing_site is not None:
+                # Site level Maintenance Update
+                if s.get_maintenance_info().get(s.get_name()) is not None:
+                    database.update_site(site=s)
+                # Worker level Maintenance Update
+                else:
+                    new_maint_info = existing_site.clone_maintenance_info()
+                    if new_maint_info.get(s.get_name()):
+                        new_maint_info.rem(s.get_name())
+                    for worker_name, entry in s.get_maintenance_info().list_details():
+                        # Remove existing entry
+                        if new_maint_info.get(worker_name):
+                            new_maint_info.rem(worker_name)
+
+                        # Add worker entry using the new information only if worker is in Maintenance
+                        if entry.state != MaintenanceState.Active:
+                            new_maint_info.add(worker_name, entry)
+                    new_maint_info.finalize()
+                    existing_site.update_maintenance_info(maint_info=new_maint_info)
+                    database.update_site(site=existing_site)
+            # Adding Maintenance State First Time
             else:
                 database.add_site(site=s)
 
     @staticmethod
     def is_testbed_in_maintenance(*, database: ABCDatabase) -> Tuple[bool, Dict[str, str] or None]:
         test_bed = database.get_site(site_name=Constants.ALL)
         if test_bed is not None:
@@ -133,15 +173,15 @@
         @param email user's email
         @param site site name
         @param worker worker name
         @return True if allowed; False otherwise
         """
         status, site = Maintenance.is_site_in_maintenance(database=database, site_name=site)
 
-        if not status:
+        if not status and site is None:
             return True, None
 
         projects = site.get_properties().get(Constants.PROJECT_ID)
         users = site.get_properties().get(Constants.USERS)
 
         if project is not None and projects is not None and project in projects:
             return True, None
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/message_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/container/message_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/protocol_descriptor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/container/protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/remote_actor_cache.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/container/remote_actor_cache.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/container/rpc_producer.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/container/rpc_producer.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import time
 import traceback
 from typing import List, Dict
 
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
+from fabric_mb.message_bus.messages.poa_info_avro import PoaInfoAvro
+
 from fabric_cf.actor.boot.configuration import ActorConfig
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.apis.abc_policy import ABCPolicy
 from fabric_cf.actor.core.apis.abc_timer_task import ABCTimerTask
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin, ActorType
 from fabric_cf.actor.core.apis.abc_actor_event import ABCActorEvent
 from fabric_cf.actor.core.apis.abc_actor_proxy import ABCActorProxy
@@ -39,14 +42,15 @@
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.apis.abc_slice import ABCSlice
 from fabric_cf.actor.core.common.exceptions import ActorException
 from fabric_cf.actor.core.container.message_service import MessageService
 from fabric_cf.actor.core.core.event_processor import TickEvent, EventType, EventProcessor
 from fabric_cf.actor.core.kernel.failed_rpc import FailedRPC
 from fabric_cf.actor.core.kernel.kernel_wrapper import KernelWrapper
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.kernel.rpc_manager_singleton import RPCManagerSingleton
 from fabric_cf.actor.core.kernel.resource_set import ResourceSet
 from fabric_cf.actor.core.kernel.slice import SliceTypes
 from fabric_cf.actor.core.kernel.slice_state_machine import SliceState
 from fabric_cf.actor.core.proxies.proxy import Proxy
 from fabric_cf.actor.core.container.maintenance import Site
 from fabric_cf.actor.core.time.actor_clock import ActorClock
@@ -814,15 +818,15 @@
 
         if rid is not None:
             self.wrapper.unregister_reservation(rid=rid)
 
     def unregister_slice(self, *, slice_object: ABCSlice):
         """
         Unregister slice
-        @param slice_obj slice object
+        @param slice_object slice object
         """
         self.wrapper.unregister_slice(slice_id=slice_object.get_slice_id())
 
     def unregister_slice_by_slice_id(self, *, slice_id: ID):
         """
         Unregister slice by slice id
         @param slice_id slice id
@@ -913,8 +917,8 @@
         if self.plugin is not None:
             self.plugin.set_logger(logger=logger)
 
     def load_model(self, *, graph_id: str):
         return
 
     def update_maintenance_mode(self, *, properties: Dict[str, str], sites: List[Site] = None):
-        self.wrapper.update_maintenance_mode(properties=properties, sites=sites)
+        self.wrapper.update_maintenance_mode(properties=properties, sites=sites)
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/actor_identity.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/proxy_factory.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,37 +22,56 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
-from fabric_cf.actor.core.apis.abc_actor_identity import ABCActorIdentity
-from fabric_cf.actor.security.auth_token import AuthToken
+from fabric_cf.actor.core.common.exceptions import ProxyException
+from fabric_cf.actor.core.proxies.kafka.kafka_proxy_factory import KafkaProxyFactory
+from fabric_cf.actor.core.common.constants import Constants
+from fabric_cf.actor.core.proxies.local.local_proxy_factory import LocalProxyFactory
 
 if TYPE_CHECKING:
-    from fabric_cf.actor.core.util.id import ID
+    from fabric_cf.actor.core.apis.abc_actor_identity import ABCActorIdentity
+    from fabric_cf.actor.core.proxies.actor_location import ActorLocation
 
 
-class ActorIdentity(ABCActorIdentity):
-    """
-    Represent Actor Identity
-    """
-    def __init__(self, *, name: str, guid: ID):
-        self.auth = AuthToken(name=name, guid=guid)
+class ProxyFactory:
+    def __init__(self):
+        self.factories = {}
+        self.load_factories()
 
-    def get_guid(self) -> ID:
-        """
-        Return guid
-        @return guid
-        """
-        return self.auth.get_guid()
+    def load_factories(self):
+        self.factories[Constants.PROTOCOL_LOCAL] = LocalProxyFactory()
+        self.factories[Constants.PROTOCOL_KAFKA] = KafkaProxyFactory()
+
+    def new_callback(self, *, protocol: str, identity: ABCActorIdentity, location: ActorLocation):
+        if protocol in self.factories:
+            factory = self.factories[protocol]
+            return factory.new_callback(identity=identity, location=location)
+        return None
+
+    def new_proxy(self, *, protocol: str, identity: ABCActorIdentity, location: ActorLocation, proxy_type: str = None):
+        if protocol in self.factories:
+            factory = self.factories[protocol]
+            return factory.new_proxy(identity=identity, location=location, proxy_type=proxy_type)
+        return None
 
-    def get_identity(self) -> AuthToken:
+
+class ProxyFactorySingleton:
+    __instance = None
+
+    def __init__(self):
+        if self.__instance is not None:
+            raise ProxyException("Singleton can't be created twice !")
+
+    def get(self):
         """
-        Return identity
-        @return identity
+        Actually create an instance
         """
-        return self.auth
+        if self.__instance is None:
+            self.__instance = ProxyFactory()
+        return self.__instance
+
+    get = classmethod(get)
 
-    def get_name(self) -> str:
-        return self.auth.get_name()
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/authority.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/authority.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,28 +22,30 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import queue
 import threading
 
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fim.graph.abc_property_graph import ABCPropertyGraph
 from fim.graph.resources.neo4j_arm import Neo4jARMGraph
 
 from fabric_cf.actor.core.apis.abc_actor_mixin import ActorType
 from fabric_cf.actor.core.apis.abc_authority import ABCAuthority
 from fabric_cf.actor.core.apis.abc_authority_reservation import ABCAuthorityReservation
 from fabric_cf.actor.core.apis.abc_client_callback_proxy import ABCClientCallbackProxy
 from fabric_cf.actor.core.apis.abc_controller_callback_proxy import ABCControllerCallbackProxy
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.apis.abc_slice import ABCSlice
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import AuthorityException
 from fabric_cf.actor.core.core.actor import ActorMixin
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.kernel.resource_set import ResourceSet
 from fabric_cf.actor.core.kernel.slice import SliceFactory
 from fabric_cf.actor.core.manage.authority_management_object import AuthorityManagementObject
 from fabric_cf.actor.core.manage.kafka.services.kafka_authority_service import KafkaAuthorityService
 from fabric_cf.actor.core.proxies.kafka.services.authority_service import AuthorityService
 from fabric_cf.actor.core.delegation.delegation_factory import DelegationFactory
 from fabric_cf.actor.core.time.actor_clock import ActorClock
@@ -330,7 +332,26 @@
         :return:
         """
         self.policy.set_aggregate_resource_model(aggregate_resource_model=aggregate_resource_model)
 
     def load_model(self, *, graph_id: str):
         self.policy.set_aggregate_resource_model_graph_id(graph_id=graph_id)
         self.policy.load_aggregate_resource_model()
+
+    def poa(self, *, poa: Poa):
+        if not self.recovered:
+            raise AuthorityException(Constants.INVALID_ACTOR_STATE)
+
+        if poa.sliver_id is None or poa.operation is None:
+            self.logger.error(f"rid {poa.sliver_id} operation {poa.operation}")
+            raise AuthorityException(f"Unknown reservation: {poa.sliver_id}")
+
+        reservation = None
+        try:
+            reservation = self.get_reservation(rid=poa.get_sliver_id())
+        except Exception as e:
+            self.logger.error(f"Could not find reservation #{poa.sliver_id} e: {e}")
+
+        if reservation is None:
+            raise AuthorityException(f"Unknown reservation: {poa.sliver_id}")
+
+        self.wrapper.poa(reservation=reservation, poa=poa)
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/authority_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/authority_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/broker.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,27 +21,26 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
-import queue
-import threading
 from typing import TYPE_CHECKING
 
 from fim.graph.abc_property_graph import ABCPropertyGraph
 from fim.slivers.base_sliver import BaseSliver
 
 from fabric_cf.actor.boot.configuration import ActorConfig
 from fabric_cf.actor.core.apis.abc_actor_mixin import ActorType
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.common.exceptions import BrokerException, ExceptionErrorCode
 from fabric_cf.actor.core.delegation.broker_delegation_factory import BrokerDelegationFactory
 from fabric_cf.actor.core.delegation.delegation_factory import DelegationFactory
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.kernel.slice import SliceFactory
 from fabric_cf.actor.core.manage.broker_management_object import BrokerManagementObject
 from fabric_cf.actor.core.manage.kafka.services.kafka_broker_service import KafkaBrokerService
 from fabric_cf.actor.core.proxies.kafka.services.broker_service import BrokerService
 from fabric_cf.actor.core.registry.actor_registry import ActorRegistrySingleton
 from fabric_cf.actor.core.util.id import ID
 from fabric_cf.actor.core.apis.abc_broker_reservation import ABCBrokerReservation
@@ -426,14 +425,20 @@
             raise BrokerException(error_code=ExceptionErrorCode.NOT_FOUND, msg=f"client: {guid} e: {e}")
 
         return ret_val
 
     def modify(self, *, reservation_id: ID, modified_sliver: BaseSliver):
         return
 
+    def poa(self, *, poa: Poa):
+        pass
+
+    def poa_info(self, *, poa: Poa, caller: AuthToken):
+        pass
+
     @staticmethod
     def get_management_object_class() -> str:
         return BrokerManagementObject.__name__
 
     @staticmethod
     def get_management_object_module() -> str:
         return BrokerManagementObject.__module__
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/broker_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/broker_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/controller.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,31 +33,32 @@
 from fim.slivers.base_sliver import BaseSliver
 
 from fabric_cf.actor.boot.configuration import ActorConfig
 from fabric_cf.actor.core.apis.abc_actor_mixin import ActorType
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.common.exceptions import ControllerException
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.manage.controller_management_object import ControllerManagementObject
 from fabric_cf.actor.core.manage.kafka.services.kafka_controller_service import KafkaControllerService
 from fabric_cf.actor.core.proxies.kafka.services.controller_service import ControllerService
 from fabric_cf.actor.core.apis.abc_controller import ABCController
 from fabric_cf.actor.core.core.actor import ActorMixin
 from fabric_cf.actor.core.registry.peer_registry import PeerRegistry
 from fabric_cf.actor.core.util.reservation_set import ReservationSet
 from fabric_cf.actor.core.apis.abc_controller_reservation import ABCControllerReservation
 from fabric_cf.actor.fim.asm_update_thread import AsmUpdateThread
+from fabric_cf.actor.core.util.id import ID
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.time.actor_clock import ActorClock
     from fabric_cf.actor.security.auth_token import AuthToken
     from fabric_cf.actor.core.apis.abc_broker_proxy import ABCBrokerProxy
     from fabric_cf.actor.core.apis.abc_client_reservation import ABCClientReservation
     from fabric_cf.actor.core.apis.abc_slice import ABCSlice
-    from fabric_cf.actor.core.util.id import ID
 
 
 class Controller(ActorMixin, ABCController):
     """
     Implements Controller
     """
     saved_extended_renewable = ReservationSet()
@@ -419,14 +420,40 @@
 
         self.redeem_reservations(rset=self.redeeming)
         self.redeeming.clear()
 
         self.extend_lease(rset=self.extending_lease)
         self.extending_lease.clear()
 
+    def poa(self, *, poa: Poa):
+        if poa.sliver_id is None or poa.operation is None:
+            self.logger.error(f"rid {poa.sliver_id} operation {poa.operation}")
+            raise ControllerException(f"Unknown reservation: {poa.sliver_id}")
+
+        reservation = None
+        try:
+            reservation = self.get_reservation(rid=poa.sliver_id)
+        except Exception as e:
+            self.logger.error(f"Could not find reservation #{poa.sliver_id} e: {e}")
+
+        if reservation is None:
+            raise ControllerException(f"Unknown reservation: {poa.sliver_id}")
+
+        if reservation.get_leased_resources() is None:
+            self.logger.warning(f"There are no approved resources for {poa.sliver_id}, do nothing!")
+            return
+
+        self.wrapper.poa(reservation=reservation, poa=poa, raise_exception=True)
+
+    def poa_info(self, *, poa: Poa, caller: AuthToken):
+        if not self.is_recovered() or self.is_stopped():
+            raise ControllerException("This actor cannot receive calls")
+
+        self.wrapper.poa_info(poa=poa, caller=caller)
+
     @staticmethod
     def get_management_object_class() -> str:
         return ControllerManagementObject.__name__
 
     @staticmethod
     def get_management_object_module() -> str:
         return ControllerManagementObject.__module__
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/event_processor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/event_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/inventory_slice_manager.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/inventory_slice_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/rpc_request_state.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/rpc_request_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/ticket.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/ticket.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/unit.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/unit.py`

 * *Files 13% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     DEFAULT = 0
     PRIMING = 1
     ACTIVE = 2
     MODIFYING = 3
     CLOSING = 4
     CLOSED = 5
     FAILED = 6
+    POA_IN_PROGRESS = 7
 
 
 class Unit(ConfigToken):
     def __init__(self, *, rid: ID, sliver: BaseSliver = None, slice_id: ID = None, actor_id: ID = None,
                  properties: dict = None, state: UnitState = None, rtype: ResourceType = None):
         # Reservation this unit belongs to (id).
         self.reservation_id = rid
@@ -75,28 +76,31 @@
         # Reservation this unit belongs to.
         self.reservation = None
         # The modified version of the sliver.
         self.modified = None
         self.transfer_out_started = False
         self.sliver = sliver
         self.lock = threading.Lock()
+        self.poa_info = {}
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state['transfer_out_started']
         del state['reservation']
         del state['lock']
+        del state['poa_info']
 
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self.transfer_out_started = False
         self.reservation = None
         self.lock = threading.Lock()
+        self.poa_info = {}
 
     def transition(self, *, to_state: UnitState):
         """
         Transition the state
         @param to_state ti state
         """
         self.state = to_state
@@ -125,14 +129,27 @@
             self.notices.add(msg=message, ex=exception)
             self.transition(to_state=UnitState.ACTIVE)
             self.sliver = self.modified
             self.modified = None
         finally:
             self.lock.release()
 
+    def fail_on_poa(self, *, message: str, exception: Exception = None):
+        """
+        Fail on modify
+        @param message message
+        @param exception exception
+        """
+        try:
+            self.lock.acquire()
+            self.notices.add(msg=message, ex=exception)
+            self.transition(to_state=UnitState.ACTIVE)
+        finally:
+            self.lock.release()
+
     def set_state(self, *, state: UnitState):
         """
         Set state
         @param state state
         """
         try:
             self.lock.acquire()
@@ -147,14 +164,24 @@
         try:
             self.lock.acquire()
             self.transition(to_state=UnitState.CLOSING)
             self.transfer_out_started = True
         finally:
             self.lock.release()
 
+    def start_poa(self):
+        """
+        Start close on a unit
+        """
+        try:
+            self.lock.acquire()
+            self.transition(to_state=UnitState.POA_IN_PROGRESS)
+        finally:
+            self.lock.release()
+
     def start_prime(self) -> bool:
         """
         Start priming the unit
         """
         try:
             self.lock.acquire()
             if self.state == UnitState.DEFAULT or self.state == UnitState.PRIMING:
@@ -421,14 +448,25 @@
             self.lock.acquire()
             self.transition(to_state=UnitState.ACTIVE)
             self.sliver = self.modified
             self.modified = None
         finally:
             self.lock.release()
 
+    def complete_poa(self, poa_info: dict):
+        """
+        Complete POA operation
+        """
+        try:
+            self.lock.acquire()
+            self.poa_info = poa_info.copy()
+            self.transition(to_state=UnitState.ACTIVE)
+        finally:
+            self.lock.release()
+
     def get_actor_id(self) -> ID:
         """
         Get Actor id
         @return actor id
         """
         return self.actor_id
 
@@ -522,8 +560,8 @@
                             ns = device.network_service_info.network_services[ns_name]
                             existing_ifs = existing_device.network_service_info.network_services[ns_name].interface_info.interfaces
                             for ifs in ns.interface_info.interfaces.values():
                                 existing_ifs[ifs.get_name()].label_allocations = ifs.label_allocations
 
                         #self.sliver.attached_components_info.devices[device.get_name()].label_allocations = device.label_allocations
         finally:
-            self.lock.release()
+            self.lock.release()
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/core/unit_set.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/core/unit_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from datetime import datetime
 from typing import TYPE_CHECKING
 
 from fim.slivers.base_sliver import BaseSliver
 
 from fabric_cf.actor.core.common.exceptions import UnitException
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.util.id import ID
 from fabric_cf.actor.core.util.notice import Notice
 
 from fabric_cf.actor.core.apis.abc_concrete_set import ABCConcreteSet
 from fabric_cf.actor.core.core.unit import UnitState, Unit
 
 if TYPE_CHECKING:
@@ -411,7 +412,25 @@
             self.transfer_out(u=u)
 
     def get_set(self) -> dict:
         """
         Get a copy of the units
         """
         return self.units.copy()
+
+    def poa(self, *, poa: Poa):
+        units = self.units.copy()
+        for u in units.values():
+            if u.transfer_out_started:
+                continue
+
+            try:
+                u.start_modify()
+                self.plugin.poa(unit=u, poa=poa)
+            except Exception as e:
+                self.fail(u=u, message="POA error", e=e)
+
+    def get_poa_info(self) -> dict:
+        result = {}
+        for u in self.units.values():
+            return u.poa_info
+        return result
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/broker_delegation.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/broker_delegation.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 from fabric_cf.actor.core.delegation.delegation import Delegation
 from fabric_cf.actor.core.kernel.rpc_manager_singleton import RPCManagerSingleton
 from fabric_cf.actor.core.util.id import ID
 from fabric_cf.actor.core.util.update_data import UpdateData
 
 
 class BrokerDelegation(Delegation):
-    def __init__(self, dlg_graph_id: str, slice_id: ID, broker: ABCBrokerProxy = None):
-        super().__init__(dlg_graph_id=dlg_graph_id, slice_id=slice_id)
+    def __init__(self, dlg_graph_id: str, slice_id: ID, broker: ABCBrokerProxy = None, site: str = None):
+        super().__init__(dlg_graph_id=dlg_graph_id, slice_id=slice_id, site=site)
         self.exported = False
         self.broker = broker
         self.authority = None
         # The status of the last ticket update.
         self.last_delegation_update = UpdateData()
 
     def __getstate__(self):
@@ -188,14 +188,15 @@
         @throws Exception
         """
         self.logger.debug("absorb_update: {}".format(incoming))
         if self.authority is None and incoming.get_site_proxy() is not None:
             self.authority = incoming.get_site_proxy()
 
         self.graph = incoming.get_graph()
+        self.site = incoming.get_site()
         self.policy.update_delegation_complete(delegation=self)
         if self.graph is not None:
             self.graph.delete_graph()
             self.graph = None
 
     def accept_delegation_update(self, *, incoming: ABCDelegation, update_data: UpdateData):
         """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/broker_delegation_factory.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/broker_delegation_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 
 
 class BrokerDelegationFactory:
     """
     Factory class to create broker delegation instances
     """
     @staticmethod
-    def create(did: str, slice_id: ID, broker: ABCBrokerProxy) -> ABCDelegation:
+    def create(did: str, slice_id: ID, broker: ABCBrokerProxy, site: str = None) -> ABCDelegation:
         """
         Create a broker delegation
         @param did delegation id
         @param slice_id slice id
         @param broker broker
+        @param site site name
         @return delegation
         """
-        delegation = BrokerDelegation(dlg_graph_id=did, slice_id=slice_id, broker=broker)
+        delegation = BrokerDelegation(dlg_graph_id=did, slice_id=slice_id, broker=broker, site=site)
         return delegation
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/delegation.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/delegation.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 from fabric_cf.actor.security.auth_token import AuthToken
 
 
 class Delegation(ABCDelegation):
     error_string_prefix = 'error for delegation: {} : {}'
     invalid_state_prefix = "Invalid state for {}. Did you already {} this Delegation?"
 
-    def __init__(self, dlg_graph_id: str, slice_id: ID, delegation_name: str = None):
+    def __init__(self, dlg_graph_id: str, slice_id: ID, delegation_name: str = None, site: str = None):
         self.dlg_graph_id = dlg_graph_id
         self.slice_id = slice_id
         self.state = DelegationState.Nascent
         self.dirty = False
         self.state_transition = False
         self.sequence_in = 0
         self.update_count = 0
@@ -61,14 +61,15 @@
         self.slice_object = None
         self.logger = None
         self.policy = None
         self.callback = None
         self.error_message = None
         self.owner = None
         self.delegation_name = delegation_name
+        self.site = site
         self.thread_lock = threading.Lock()
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state['graph']
         del state['actor']
         del state['slice_object']
@@ -95,14 +96,17 @@
                 self.callback.set_logger(logger=actor.get_logger())
         if actor.get_type() == ActorType.Authority:
             self.graph = FimHelper.get_arm_graph(graph_id=str(self.dlg_graph_id))
 
         if actor.get_policy() is not None:
             self.policy = actor.get_policy()
 
+    def get_site(self) -> str:
+        return self.site
+
     def set_graph(self, graph: ABCPropertyGraph):
         self.graph = graph
 
     def get_graph(self) -> ABCPropertyGraph:
         return self.graph
 
     def get_actor(self) -> ABCActorMixin:
@@ -112,15 +116,14 @@
         return self.dlg_graph_id
 
     def get_slice_id(self) -> ID:
         if self.slice_id is not None:
             return self.slice_id
         elif self.slice_object is not None:
             return self.slice_object.get_slice_id()
-        return None
 
     def get_slice_object(self) -> ABCSlice:
         return self.slice_object
 
     def get_state(self) -> DelegationState:
         return self.state
 
@@ -363,14 +366,17 @@
             self.generate_update()
 
     def __str__(self):
         msg = "del: "
         if self.dlg_graph_id is not None:
             msg += "#{} ".format(self.dlg_graph_id)
 
+        if self.site is not None:
+            msg += "site: {} ".format(self.site)
+
         if self.slice_object is not None:
             msg += "slice: [{}] ".format(self.slice_object)
         elif self.slice_id is not None:
             msg += "slice_id: [{}] ".format(self.get_slice_id())
 
         msg += "state:[{}] ".format(self.get_state_name())
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/delegation_factory.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/delegation_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,19 @@
 
 
 class DelegationFactory:
     """
     Factory class to create delegation instances
     """
     @staticmethod
-    def create(did: str, slice_id: ID, delegation_name: str = None) -> ABCDelegation:
+    def create(did: str, slice_id: ID, delegation_name: str = None, site: str = None) -> ABCDelegation:
         """
         Create a delegation
         @param did delegation id
         @param slice_id slice id
         @param delegation_name delegation_name
+        @param site site name
         @return delegation
         """
-        delegation = Delegation(dlg_graph_id=did, slice_id=slice_id, delegation_name=delegation_name)
+        delegation = Delegation(dlg_graph_id=did, slice_id=slice_id, delegation_name=delegation_name,
+                                site=site)
         return delegation
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/delegation/resource_ticket.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/delegation/resource_ticket.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/authority_reservation.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/broker_reservation.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,60 +19,79 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
+
 from __future__ import annotations
 
 import threading
 import traceback
+from datetime import datetime
 from typing import TYPE_CHECKING
-from fabric_cf.actor.core.apis.abc_reservation_mixin import ReservationCategory
-from fabric_cf.actor.core.apis.abc_authority_reservation import ABCAuthorityReservation
-from fabric_cf.actor.core.common.exceptions import AuthorityException
+
+from fabric_cf.actor.core.common.exceptions import BrokerException, ExceptionErrorCode
+from fabric_cf.actor.core.util.id import ID
+from fabric_cf.actor.core.apis.abc_authority_policy import ABCAuthorityPolicy
+from fabric_cf.actor.core.apis.abc_broker_policy_mixin import ABCBrokerPolicyMixin
+from fabric_cf.actor.core.apis.abc_reservation_mixin import ReservationCategory, ABCReservationMixin
+from fabric_cf.actor.core.apis.abc_broker_reservation import ABCBrokerReservation
+from fabric_cf.actor.core.kernel.rpc_manager_singleton import RPCManagerSingleton
 from fabric_cf.actor.core.kernel.rpc_request_type import RPCRequestType
 from fabric_cf.actor.core.kernel.request_types import RequestTypes
 from fabric_cf.actor.core.kernel.reservation_server import ReservationServer
 from fabric_cf.actor.core.kernel.reservation_states import ReservationStates, ReservationPendingStates
-from fabric_cf.actor.core.util.rpc_exception import RPCError
-from fabric_cf.actor.core.util.utils import sliver_to_str
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
+    from fabric_cf.actor.core.apis.abc_authority_proxy import ABCAuthorityProxy
     from fabric_cf.actor.core.apis.abc_callback_proxy import ABCCallbackProxy
+    from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
     from fabric_cf.actor.core.apis.abc_policy import ABCPolicy
     from fabric_cf.actor.core.apis.abc_slice import ABCSlice
     from fabric_cf.actor.core.kernel.failed_rpc import FailedRPC
-    from fabric_cf.actor.core.apis.abc_slice import ABCSlice
     from fabric_cf.actor.core.kernel.resource_set import ResourceSet
     from fabric_cf.actor.core.time.term import Term
-    from fabric_cf.actor.core.util.id import ID
 
 
-class AuthorityReservation(ReservationServer, ABCAuthorityReservation):
+class BrokerReservation(ReservationServer, ABCBrokerReservation):
     """
-    AuthorityReservation controls the state machine for a reservation on the
-    authority side. It coordinates resource allocation, lease generation,
-    priming, and shutdown of reservations.
+    A note on exported "will call" reservations. An export() operation may be
+    locally initiated on an agent. It binds and forms a ticket in the same way as
+    if the request came from a client, but there is no client rid (remoteRid) and
+    no callback object. The prepare method in AgentReservation and
+    register/unregister in ReservationServer handle these cases: the export
+    proceeds as a normal reserve request, but it leaves the callback and
+    remoteRid null, does not register the reservation with its slice (since there
+    is no remoteRid), and does not issue an updateTicket (since there is no
+    callback).
     """
-    UnexpectedExceptionString = "Unexpected reservation state: state={} pending={}"
+    updated_absorbed = "update absorbed"
 
-    def __init__(self, *, rid: ID, resources: ResourceSet, term: Term, slice_object: ABCSlice):
-        super().__init__(rid=rid, resources=resources, term=term, slice_object=slice_object)
-        # The ticket.
-        self.ticket = None
-        # Policies use this flag to instruct the core to send reservations to the client even if they have deficit.
-        self.send_with_deficit = True
+    def __init__(self, *, rid: ID, resources: ResourceSet, term: Term, slice_obj: ABCSlice):
+        super().__init__(rid=rid, resources=resources, term=term, slice_object=slice_obj)
+        # Delegation backing the ticket granted to this reservation. For now only
+        # one source delegation can be used to issue a ticket to satisfy a client
+        # request.
+        self.source = None
+        # If this flag is true, then the reservation represents a request to export
+        # resources to a client.
+        self.exporting = False
+        # The authority in control of the resources.
+        self.authority = None
+        # True if an updateTicket() must be sent on the next service probe.
+        self.must_send_update = None
         # True if we notified the client about the fact that the reservation had failed
-        self.notified_about_failure = False
-        # Creates a new "blank" reservation instance. Used during recovery.
-        self.category = ReservationCategory.Authority
-        self.broker_callback = None
+        self.notified_failed = False
+        # True if the reservation was closed in the priming state.
+        self.closed_in_priming = False
+        self.category = ReservationCategory.Broker
+        self.extend_failure = False
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state['actor']
         del state['logger']
         del state['slice']
         del state['approved']
@@ -82,17 +101,19 @@
         del state['expired']
         del state['pending_recover']
         del state['state_transition']
         del state['service_pending']
 
         del state['policy']
 
-        del state['notified_about_failure']
+        del state['source']
+        del state['notified_failed']
+        del state['closed_in_priming']
+        del state['extend_failure']
         del state['thread_lock']
-
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self.actor = None
         self.logger = None
         self.slice = None
@@ -103,497 +124,443 @@
         self.expired = False
         self.pending_recover = False
         self.state_transition = False
         self.service_pending = ReservationPendingStates.None_
 
         self.policy = None
 
-        self.notified_about_failure = False
+        self.source = None
+        self.notified_failed = False
+        self.closed_in_priming = False
+        self.extend_failure = False
         self.thread_lock = threading.Lock()
 
     def restore(self, *, actor: ABCActorMixin, slice_obj: ABCSlice):
         """
         Must be invoked after creating reservation from unpickling
         """
         super().restore(actor=actor, slice_obj=slice_obj)
-        self.notified_about_failure = False
+        self.source = None
+        if actor is not None and self.resources is not None and self.resources.get_resources() is not None:
+            delegation_id = self.resources.get_resources().get_delegation_id()
+            delegation = self.actor.get_delegation(did=delegation_id)
+            self.source = delegation
+        self.notified_failed = False
+        self.closed_in_priming = False
+
+    def print_state(self):
+        """
+        Converts the reservation to a state string.
+        @return state string representing the reservation
+        """
+        return "[{},{}] ({})({})".format(self.get_state_name(), self.get_pending_state_name(), self.get_sequence_in(),
+                                         self.get_sequence_out())
+
+    def recover(self):
+        """
+        Recover the reservation post stateful restart
+        """
+        if isinstance(self.policy, ABCAuthorityPolicy):
+            self.logger.debug("No recovery necessary for reservation #{}".format(self.get_reservation_id()))
+            return
+
+        if not isinstance(self.policy, ABCBrokerPolicyMixin):
+            raise BrokerException(msg=f"Do not know how to recover: policy={self.policy}")
+
+        if self.state == ReservationStates.Nascent:
+            if self.pending_state == ReservationPendingStates.None_:
+                self.actor.ticket(self)
+                self.logger.info("Added reservation #{} to the ticketing list. State={}".format(
+                    self.get_reservation_id(), self.print_state()))
+
+            elif self.pending_state == ReservationPendingStates.Ticketing:
+                self.set_pending_recover(pending_recover=True)
+                self.transition(prefix="[recovery]", state=self.state, pending=ReservationPendingStates.None_)
+                self.actor.ticket(self)
+                self.logger.info(
+                    "Added reservation #{} to the ticketing list. State={}".format(self.get_reservation_id(),
+                                                                                   self.print_state()))
 
-    def set_broker_callback(self, *, broker_callback: ABCCallbackProxy):
-        self.broker_callback = broker_callback
+            else:
+                raise BrokerException(error_code=ExceptionErrorCode.UNEXPECTED_STATE,
+                                      msg=f"pending_state={self.pending_state}")
 
-    def get_broker_callback(self) -> ABCCallbackProxy:
-        return self.broker_callback
+        elif self.state == ReservationStates.Ticketed:
+            if self.pending_state == ReservationPendingStates.None_ or \
+                    self.pending_state == ReservationPendingStates.Priming:
+                self.set_service_pending(code=ReservationPendingStates.None_)
+                self.logger.debug("No recovery necessary for reservation #{}".format(self.get_reservation_id()))
+
+            elif self.pending_state == ReservationPendingStates.ExtendingTicket:
+                self.set_pending_recover(pending_recover=True)
+                self.transition(prefix="[recovery]", state=self.state,
+                                pending=ReservationPendingStates.None_)
+                self.actor.extend_ticket(reservation=self)
+                self.logger.info(
+                    "Added reservation #{} to the extending list. State={}".format(self.get_reservation_id(),
+                                                                                   self.print_state()))
+            else:
+                raise BrokerException(error_code=ExceptionErrorCode.UNEXPECTED_STATE,
+                                      msg=f"pending_state={self.pending_state}")
+
+        elif self.state == ReservationStates.Failed:
+            self.logger.warning("Reservation #{} has failed".format(self.get_reservation_id()))
+        else:
+            raise BrokerException(error_code=ExceptionErrorCode.UNEXPECTED_STATE,
+                                  msg=f"state={self.state}")
 
     def prepare(self, *, callback: ABCCallbackProxy, logger):
         self.set_logger(logger=logger)
         self.callback = callback
-        self.requested_resources.validate_incoming_ticket(term=self.requested_term)
 
-        if self.rid is None:
+        # Null callback indicates a locally initiated request to create an
+        # exported reservation. Else the request is from a client and must have
+        # a client-specified RID.
+
+        if self.callback is not None and self.rid is None:
             self.error(err="no reservation ID specified for request")
 
-        self.state = ReservationStates.Ticketed
+        self.set_dirty()
 
     def reserve(self, *, policy: ABCPolicy):
-        self.nothing_pending()
+        # These handlers may need to be slightly more sophisticated, since a
+        # client may bid multiple times on a ticket as part of an auction
+        # protocol: so we may receive a reserve or extend when there is already
+        # a request pending.
         self.incoming_request()
-        if self.is_active():
-            self.error(err="reservation already holds a lease")
+
+        if self.pending_state != ReservationPendingStates.None_ and \
+                self.pending_state != ReservationPendingStates.Ticketing:
+            # We do not want to fail the reservation simply log a warning and exit from reserve
+            self.logger.warning("Duplicate ticket request")
+            return
 
         self.policy = policy
         self.approved = False
         self.bid_pending = True
-        self.pending_recover = False
-        self.map_and_update(extend=False)
+        self.map_and_update(ticketed=False)
 
     def service_reserve(self):
-        try:
-            if self.resources is not None:
-                self.resources.service_reserve_site()
-        except Exception as e:
-            self.logger.error("authority failed servicing reserve", exception=e)
-            self.fail_notify(message=str(e))
+        # resources is null initially. It becomes non-null once the
+        # policy completes its allocation.
+        if self.resources is not None:
+            self.resources.service_update(reservation=self)
+            if not self.is_failed():
+                self.transition(prefix=self.updated_absorbed, state=ReservationStates.Ticketed,
+                                pending=ReservationPendingStates.None_)
+                self.generate_update()
 
-    def extend_lease(self):
-        self.nothing_pending()
+    def extend_ticket(self, *, actor: ABCActorMixin):
         self.incoming_request()
 
-        if not self.is_active():
-            self.error(err="reservation does not yet hold a lease")
+        # State must be ticketed. The reservation may be active, but the agent wouldn't know that
+        if self.state != ReservationStates.Ticketed:
+            self.error(err="extending unticketed reservation")
+
+        if self.pending_state != ReservationPendingStates.None_ and self.pending_state != \
+                ReservationPendingStates.ExtendingTicket:
+            self.error(err="extending reservation with another pending request")
 
         if not self.requested_term.extends_term(old_term=self.term):
-            self.error(err="requested term does not extend current term for extendLease")
+            self.error(err=f"new term {self.requested_term} does not extend current term {self.term}")
 
         self.approved = False
         self.bid_pending = True
         self.pending_recover = False
-        self.map_and_update(extend=True)
+        self.map_and_update(ticketed=True)
 
-    def modify_lease(self):
-        self.nothing_pending()
-        self.incoming_request()
+    def service_extend_ticket(self):
+        if self.pending_state == ReservationPendingStates.None_:
+            self.resources.service_update(self)
+            if not self.is_failed():
+                self.transition(prefix=self.updated_absorbed, state=ReservationStates.Ticketed,
+                                pending=ReservationPendingStates.None_)
+                self.generate_update()
 
-        if not self.is_active():
-            self.error(err="reservation does not yet hold a lease")
+    def close(self):
+        send_notification = False
+        if self.state == ReservationStates.Nascent or self.pending_state != ReservationPendingStates.None_:
+            self.logger.warning("Closing a reservation in progress")
+            send_notification = True
+
+        if self.state != ReservationStates.Closed:
+            if self.pending_state == ReservationPendingStates.Priming or \
+                    (self.pending_state == ReservationPendingStates.Ticketing and not self.bid_pending):
+                # Close in Priming is a special case: when processing the close
+                # event inside the policy we cannot rely on resources to
+                # represent the resources allocated to the reservation. They
+                # may either represent the previous resources or a mixture of
+                # both. So here we will mark the reservation that it was closed
+                # while it was in the Priming state. When processing the close
+                # event the policy must free previousResources (if any) and
+                # approvedResources. The policy should not free resources.
+                self.logger.debug("closing reservation #{} while in Priming".format(self.rid))
+                self.closed_in_priming = True
 
-        self.approved = True
-        self.bid_pending = True
-        self.pending_recover = False
-        self.map_and_update_modify_lease()
+            self.transition(prefix="closed", state=ReservationStates.Closed, pending=ReservationPendingStates.None_)
+            self.policy.closed(reservation=self)
 
-    def service_extend_lease(self):
-        assert (self.state == ReservationStates.Failed and self.pending_state == ReservationPendingStates.None_) or \
-                self.pending_state == ReservationPendingStates.ExtendingLease or \
-                self.pending_state == ReservationPendingStates.Priming
+        if send_notification:
+            self.update_data.error(message="Closed while allocating ticket")
+            self.generate_update()
 
-        try:
-            if self.pending_state == ReservationPendingStates.Priming:
-                self.resources.service_extend()
-        except Exception as e:
-            self.logger.error("authority failed servicing extendLease e: {}".format(e))
-            self.fail_notify(message=str(e))
+    def probe_pending(self):
+        if self.service_pending != ReservationPendingStates.None_:
+            self.internal_error(err="service overrun in probePending")
 
-    def service_modify_lease(self):
-        assert (self.state == ReservationStates.Failed and self.pending_state == ReservationPendingStates.None_) or \
-               self.pending_state == ReservationPendingStates.ModifyingLease or \
-               self.pending_state == ReservationPendingStates.Priming
+        if self.is_failed() and not self.notified_failed:
+            self.generate_update()
+            self.notified_failed = True
+            if self.extend_failure:
+                self.transition(prefix="Recover from Extend Failure", state=ReservationStates.Ticketed,
+                                pending=ReservationPendingStates.None_)
+                self.extend_failure = False
+        else:
+            if self.pending_state == ReservationPendingStates.Ticketing:
+                # Check for a pending ticket operation that may have completed
+                if not self.bid_pending and self.map_and_update(ticketed=False):
+                    self.service_pending = ReservationPendingStates.AbsorbUpdate
+
+            elif self.pending_state == ReservationPendingStates.ExtendingTicket:
+                # Check for a pending extendTicket operation
+                if not self.bid_pending and self.map_and_update(ticketed=True):
+                    self.service_pending = ReservationPendingStates.AbsorbUpdate
 
+            elif self.pending_state == ReservationPendingStates.Redeeming:
+                self.logger.error("AgentReservation in unexpected state")
+
+            elif self.pending_state == ReservationPendingStates.Priming:
+                self.service_pending = ReservationPendingStates.AbsorbUpdate
+
+            elif self.pending_state == ReservationPendingStates.None_ and self.must_send_update:
+                # for exported reservations that have been claimed, we need to
+                # schedule a ticketUpdate
+                self.service_pending = ReservationPendingStates.SendUpdate
+                self.must_send_update = False
+
+    def service_probe(self):
         try:
-            if self.pending_state == ReservationPendingStates.Priming:
-                self.resources.service_modify()
+            if self.service_pending == ReservationPendingStates.AbsorbUpdate:
+                self.resources.service_update(reservation=self)
+                if not self.is_failed():
+                    self.transition(prefix=self.updated_absorbed, state=ReservationStates.Ticketed,
+                                    pending=ReservationPendingStates.None_)
+                    self.generate_update()
+
+            elif self.service_pending == ReservationPendingStates.SendUpdate:
+                self.generate_update()
+
         except Exception as e:
-            self.logger.error("authority failed servicing modifylease e: {}".format(e))
+            self.logger.error(traceback.format_exc())
+            self.logger.error("failed while servicing probe e:{}".format(e))
             self.fail_notify(message=str(e))
 
-    def close(self):
-        self.logger.debug("Processing  close for #{}".format(self.rid))
-        self.transition(prefix="external close", state=self.state, pending=ReservationPendingStates.Closing)
-
-    def service_close(self):
-        if self.resources is not None:
-            self.resources.close()
+        self.service_pending = ReservationPendingStates.None_
 
     def handle_duplicate_request(self, *, operation: RequestTypes):
         # The general idea is to do nothing if we are in the process of
         # performing a pending operation or about to reissue a
         # ticket/extendTicket after recovery. If there is nothing pending for
         # this reservation, we resend the last update.
-
-        if operation == RequestTypes.RequestRedeem or operation == RequestTypes.RequestExtendLease or \
-                operation == RequestTypes.RequestModifyLease:
-            if self.pending_state == ReservationPendingStates.None_ and not self.bid_pending and \
+        if operation == RequestTypes.RequestTicket:
+            if self.pending_state == ReservationPendingStates.None_ and self.state != ReservationStates.Nascent and \
                     not self.pending_recover:
                 self.generate_update()
-        else:
-            raise AuthorityException("Unsupported operation: {}".format(operation))
 
-    def map_and_update(self, *, extend: bool) -> bool:
-        """
-        Calls the policy to fill a request, with associated state transitions.
+        elif operation == RequestTypes.RequestExtendTicket:
+            if self.pending_state == ReservationPendingStates.None_ and not self.pending_recover:
+                self.generate_update()
 
-        @param extend
-                   true if this request is an extend
-        @return boolean success
-        """
-        success = False
-        granted = False
-        if self.state == ReservationStates.Failed:
-            # Must be a previous failure, or policy marked it as failed. Send update to reset client.
-            self.generate_update()
-        elif self.state == ReservationStates.Ticketed:
-            assert not extend
-            try:
-                self.transition(prefix="redeeming", state=ReservationStates.Ticketed,
-                                pending=ReservationPendingStates.Redeeming)
-                # If the policy has processed this reservation, set granted to
-                # true so that we can start priming the resources. If the
-                # policy has not yet processed this reservation (binPending is
-                # true) then call the policy. The policy may choose to process
-                # the request immediately (true) or to defer it (false). In
-                # case of a deferred request, we will eventually come back to
-                # this method after the policy has done its job.
-                if self.is_bid_pending():
-                    granted = self.policy.bind(reservation=self)
-                else:
-                    granted = True
-            except Exception as e:
-                self.logger.error("authority policy bind e: {}".format(e))
-                self.fail_notify(message=str(e))
+        elif operation == RequestTypes.RequestRelinquish:
+            self.logger.debug("no op")
 
-            if granted:
-                try:
-                    success = True
-                    self.ticket = self.requested_resources
-                    self.term = self.approved_term
-                    self.resources = self.requested_resources.abstract_clone()
-                    self.resources.units = 0
-                    self.resources.update(reservation=self, resource_set=self.approved_resources)
-                    self.transition(prefix="redeem", state=ReservationStates.Ticketed,
-                                    pending=ReservationPendingStates.Priming)
-                except Exception as e:
-                    self.logger.error("authority redeem e: {}".format(e))
-                    self.logger.error(traceback.format_exc())
-                    self.fail_notify(message=str(e))
-        elif self.state == ReservationStates.Active:
-            assert extend
-            try:
-                self.transition(prefix="extending lease", state=ReservationStates.Active,
-                                pending=ReservationPendingStates.ExtendingLease)
-                # If the policy has processed this reservation, set granted to
-                # true so that we can start priming the resources. If the
-                # policy has not yet processed this reservation (binPending is
-                # true) then call the policy. The policy may choose to process
-                # the request immediately (true) or to defer it (false). In
-                # case of a deferred request, we will eventually come back to
-                # this method after the policy has done its job.
-                if self.is_bid_pending():
-                    granted = self.policy.extend_authority(reservation=self)
-                else:
-                    granted = True
-
-                if granted:
-                    success = True
-                    self.extended = True
-                    self.previous_term = self.term
-                    self.ticket = self.requested_resources
-                    self.term = self.approved_term
-
-                    self.resources.update(reservation=self, resource_set=self.approved_resources)
-                    self.transition(prefix="extend lease", state=ReservationStates.Active,
-                                    pending=ReservationPendingStates.Priming)
-            except Exception as e:
-                self.logger.error("authority mapper extend e: {}".format(e))
-                self.logger.error(traceback.format_exc())
-                self.fail_notify(message=str(e))
         else:
-            self.fail(message="mapAndUpdate: unexpected state", exception=None)
-        return success
-
-    def map_and_update_modify_lease(self) -> bool:
-        """
-        Calls the policy to fill a request, with associated state transitions.
-
-        @return boolean success
-        """
-        success = False
-        granted = False
-        if self.state == ReservationStates.Failed:
-            # Must be a previous failure, or policy marked it as failed. Send update to reset client.
-            self.generate_update()
-        elif self.state == ReservationStates.Active:
-            try:
-                self.transition(prefix="modifying lease", state=ReservationStates.Active,
-                                pending=ReservationPendingStates.ModifyingLease)
-                granted = True
-                if granted:
-                    success = True
-                    self.ticket = self.requested_resources
-                    if self.requested_resources.get_sliver() is not None:
-                        self.approved_resources.set_sliver(sliver=self.requested_resources.get_sliver())
-
-                    self.resources.update_properties(reservation=self, resource_set=self.approved_resources)
-                    self.logger.debug(f"Updated Sliver post modify: {sliver_to_str(sliver=self.resources.get_sliver())}")
-                    self.transition(prefix="modify lease", state=ReservationStates.Active,
-                                    pending=ReservationPendingStates.Priming)
-            except Exception as e:
-                self.logger.error("authority mapper modify e: {}".format(e))
-                self.fail_notify(message=str(e))
-        else:
-            self.fail(message="mapAndUpdateModifyLease: unexpected state")
-
-        return success
+            raise BrokerException(error_code=ExceptionErrorCode.NOT_SUPPORTED,
+                                  msg=f"operation {RequestTypes(operation).name}")
 
     def generate_update(self):
+        self.logger.debug("Generating update")
         if self.callback is None:
-            self.logger.warning("cannot generate update: no callback")
+            self.logger.warning("Cannot generate update: no callback.")
             return
 
+        self.logger.debug("Generating update: update count={}".format(self.update_count))
         try:
             self.update_count += 1
             self.sequence_out += 1
-            from fabric_cf.actor.core.kernel.rpc_manager_singleton import RPCManagerSingleton
-            RPCManagerSingleton.get().update_lease(reservation=self)
+            RPCManagerSingleton.get().update_ticket(reservation=self)
         except Exception as e:
+            self.logger.error(traceback.format_exc())
+            # Note that this may result in a "stuck" reservation... not much we
+            # can do if the receiver has failed or rejects our update. We will
+            # regenerate on any user-initiated probe.
             self.logger.error("callback failed e:{}".format(e))
 
-    def prepare_extend_lease(self):
-        self.requested_resources.validate_incoming_ticket(term=self.requested_term)
-
-    def prepare_modify_lease(self):
-        self.requested_resources.validate_incoming_ticket(term=self.requested_term)
-
-    def prepare_probe(self):
-        try:
-            if self.resources is not None:
-                self.resources.prepare_probe()
-        except Exception as e:
-            self.logger.error("exception in authority prepareProbe e:{}".format(e))
-
-    def probe_pending(self):
-        if self.service_pending != ReservationPendingStates.None_:
-            self.logger.error("service overrun in probePending")
-            return
-
-        self.reap()
-
-        if self.pending_state == ReservationPendingStates.None_:
-            if self.is_failed() and not self.notified_about_failure:
-                self.generate_update()
-                self.notified_about_failure = True
-
-        elif self.pending_state == ReservationPendingStates.Redeeming:
-            # We are an authority trying to satisfy a ticket redeem on behalf of a client. Retry policy bind.
-            assert self.state == ReservationStates.Ticketed
-            if not self.bid_pending and self.map_and_update(extend=False):
-                self.logger.debug("Resource assignment (redeem) for #{} completed".format(self.rid))
-                self.service_pending = ReservationPendingStates.Redeeming
-
-        elif self.pending_state == ReservationPendingStates.ExtendingLease:
-            assert self.state == ReservationStates.Active
-            if not self.bid_pending and self.map_and_update(extend=True):
-                self.logger.debug("Resource assignment (extend) for #{} completed".format(self.rid))
-                self.service_pending = ReservationPendingStates.ExtendingLease
-
-        elif self.pending_state == ReservationPendingStates.ModifyingLease:
-            assert self.state == ReservationStates.Active
-            if not self.bid_pending and self.map_and_update_modify_lease():
-                self.logger.debug("Resource assignment (modify) for #{} completed".format(self.rid))
-                self.service_pending = ReservationPendingStates.ModifyingLease
-
-        elif self.pending_state == ReservationPendingStates.Closing:
-            if self.resources is None or self.resources.is_closed():
-                self.transition(prefix="close complete", state=ReservationStates.Closed,
-                                pending=ReservationPendingStates.None_)
-                self.pending_recover = False
-                self.generate_update()
-
-        elif self.pending_state == ReservationPendingStates.Priming and self.resources.is_active():
-            # We are an authority filling a ticket claim. Got resources? Note
-            # that active() just means no primes/closes/modifies are still in
-            # progress. The primes/closes/modifies could have failed. If
-            # something succeeded, then we report what we got as active, else
-            # it's a complete bust.
-            # If something failed or we are recovering, we need to correct
-            # the deficit. For a recovering reservation we need to call
-            # correctDeficit regardless of whether there is a real deficit,
-            # since the individual nodes may be inconsistent with what the
-            # client/broker wanted. For example, they may have the wrong
-            # logical ids and resource shares.
-            if self.pending_recover or self.get_deficit() != 0:
-                # The abstract and the concrete units may be different. We
-                # need to adjust the abstract to equal concrete so that
-                # future additions of resources will not result in
-                # inconsistent abstract unit count.
-                self.resources.fix_abstract_units()
-                # Policies can instruct us to let go a reservation with a
-                # deficit. For example, a policy failed adding resources to
-                # the reservation multiple times and it wants to prevent
-                # exhausting its inventory from servicing this particular
-                # request: probably something is wrong with the request.
-                if not self.send_with_deficit:
-                    # Call the policy to correct the deficit
-                    self.policy.correct_deficit(reservation=self)
-                    # XXX: be careful here. we are reusing extending for
-                    # the purpose of triggering configuration actions on
-                    # the newly assigned nodes. If this is not appropriate,
-                    # we may need a new servicePending value
-                    self.service_pending = ReservationPendingStates.ExtendingLease
-                else:
-                    self.pending_recover = False
-                    if self.resources.get_units() == 0:
-                        message = "no information available"
-                        if self.update_data.get_events() is not None:
-                            message = self.update_data.get_events()
-                        self.fail(message="all units failed priming: {}".format(message))
-                    else:
-                        self.transition(prefix="prime complete1", state=ReservationStates.Active,
-                                        pending=ReservationPendingStates.None_)
-                    self.generate_update()
-            else:
-                self.pending_recover = False
-                self.transition(prefix="prime complete2", state=ReservationStates.Active,
-                                pending=ReservationPendingStates.None_)
-                self.generate_update()
-
-    def service_probe(self):
-        # An exception in one of these service routines should mean some
-        # unrecoverable, reservation-wide failure. It should not occur, e.g.,
-        # if some subset of the resources fail.
-        try:
-            if self.service_pending == ReservationPendingStates.Redeeming:
-                self.service_reserve()
-
-            elif self.service_pending == ReservationPendingStates.ExtendingLease:
-                self.service_extend_lease()
-
-            elif self.service_pending == ReservationPendingStates.ModifyingLease:
-                self.service_modify_lease()
-
-        except Exception as e:
-            self.logger.error("authority failed servicing probe e:{}".format(e))
-            self.fail_notify(message="post-op exception: {}".format(e))
-        self.service_pending = ReservationPendingStates.None_
-
-    def reap(self):
+    def map_and_update(self, *, ticketed: bool):
         """
-        Reaps any failed or closed resources. Need more here: if reservation has
-        a deficit due to failures then we need to find some replacements.
-        @throws Exception
+        Call the policy to fill a request, with associated state transitions.
+        Catch exceptions and report all errors using callback mechanism.
+
+        @param ticketed
+                   true iff this is ticketed (i.e., request is extend)
+        @return boolean success
         """
-        try:
-            if self.resources is not None:
-                released = self.resources.collect_released()
-                if released is not None:
-                    if not released.get_notices().is_empty():
-                        self.update_data.post(event=released.get_notices().get_notice())
-                    self.policy.release(resources=released)
-        except Exception as e:
-            self.logger.error("exception in authority reap e: {}".format(e))
-            self.logger.error(traceback.format_exc())
+        success = False
+        granted = False
 
-    def recover(self):
-        if self.state == ReservationStates.Ticketed:
-            if self.pending_state == ReservationPendingStates.None_:
-                self.actor.redeem(reservation=self, callback=None, caller=None)
+        if self.state == ReservationStates.Failed:
+            # Must be a previous failure, or policy marked as failed. Send
+            # update to reset client. Note: this might be the wrong thing if a
+            # bidding protocol allows the caller to retry a denied request,
+            # e.g., to bid higher after losing in an auction.
+            self.generate_update()
+        elif self.state == ReservationStates.Nascent:
+            if ticketed:
+                self.fail_notify(message="reservation is not yet ticketed")
+            else:
+                self.logger.debug("Using policy {} to bind reservation".format(self.policy.__class__.__name__))
+                try:
+                    granted = False
+                    # If the policy has processed this reservation, granted should
+                    # be set true so that we can send the result back to the
+                    # client. If the policy has not yet processed this reservation
+                    # (binPending is true) then call the policy. The policy may
+                    # choose to process the request immediately (true) or to defer
+                    # it (false). In case of a deferred request, we will eventually
+                    # come back to this method after the policy has done its job.
+                    if self.is_bid_pending():
+                        if not self.is_exporting():
+                            granted = self.policy.bind(reservation=self)
+                        else:
+                            self.internal_error(err="Exporting reservations not implemented")
+                    else:
+                        granted = True
+                    self.transition(prefix="ticket request", state=ReservationStates.Nascent,
+                                    pending=ReservationPendingStates.Ticketing)
+                except Exception as e:
+                    self.logger.error(f"mapAndUpdate bindTicket failed for ticketRequest: {e}")
+                    self.fail_notify(message=str(e))
+                    return success
 
-            elif self.pending_state == ReservationPendingStates.Redeeming:
-                self.transition(prefix="[recover]", state=self.state, pending=ReservationPendingStates.None_)
-                self.actor.redeem(reservation=self, callback=None, caller=None)
+                if granted:
+                    self.logger.debug("Reservation {} has been granted".format(self.get_reservation_id()))
+                    try:
+                        success = True
+                        self.term = self.approved_term
+                        self.resources = self.approved_resources.abstract_clone()
+                        self.resources.update(reservation=self, resource_set=self.approved_resources)
+                        self.transition(prefix="ticketed", state=ReservationStates.Ticketed,
+                                        pending=ReservationPendingStates.Priming)
+                    except Exception as e:
+                        self.logger.error("mapAndUpdate ticket failed for ticketRequest")
+                        self.logger.error(e)
+                        self.logger.error(traceback.format_exc())
+                        self.fail_notify(message=str(e))
+        elif self.state == ReservationStates.Ticketed:
+            if not ticketed:
+                self.fail_notify(message="reservation is already ticketed")
+            else:
+                try:
+                    self.transition(prefix="extending ticket", state=ReservationStates.Ticketed,
+                                    pending=ReservationPendingStates.ExtendingTicket)
 
-            elif self.pending_state == ReservationPendingStates.Priming:
-                self.pending_recover = True
-                self.actor.close(reservation=self)
+                    # If the policy has processed this reservation, set granted to
+                    # true so that we can send the ticket back to the client. If
+                    # the policy has not yet processed this reservation (bid_pending
+                    # is true) then call the policy. The plugin may choose to
+                    # process the request immediately (true) or to defer it
+                    # (false). In case of a deferred request, we will eventually
+                    # come back to this method after the policy has done its job.
 
-            elif self.pending_state == ReservationPendingStates.Closing:
-                self.actor.close(reservation=self)
+                    granted = False
 
-            else:
-                raise AuthorityException(self.UnexpectedExceptionString.format(self.state, self.pending_state))
+                    if self.is_bid_pending():
+                        granted = self.policy.extend_broker(reservation=self)
+                    else:
+                        granted = True
+                except Exception as e:
+                    self.logger.error(f"mapAndUpdate extendTicket failed for ExtendTicket: {e}")
+                    self.fail_notify(message=str(e))
+                    return success
 
-        elif self.state == ReservationStates.Active:
-            if self.pending_state == ReservationPendingStates.None_:
-                self.logger.debug("No op")
+                if granted:
+                    try:
+                        success = True
+                        self.extended = True
+                        self.transition(prefix="extended ticket", state=ReservationStates.Ticketed,
+                                        pending=ReservationPendingStates.Priming)
+                        self.previous_term = self.term
+                        self.previous_resources = self.resources.clone()
+                        self.term = self.approved_term
+                        self.resources.update(reservation=self, resource_set=self.approved_resources)
+                    except Exception as e:
+                        self.logger.error(f"mapAndUpdate extend ticket failed for ExtendTicket: {e}")
+                        self.fail_notify(message=str(e))
+        else:
+            self.logger.error("broker mapAndUpdate: unexpected state")
+            self.fail_notify(message="invalid operation for the current reservation state")
 
-            elif self.pending_state == ReservationPendingStates.ExtendingLease:
-                self.transition(prefix="[recover]", state=self.state,
-                                pending=ReservationPendingStates.None_)
-                self.actor.extend_lease(self, None)
+        return success
 
-            elif self.pending_state == ReservationPendingStates.Priming:
-                self.pending_recover = True
-                self.actor.close(reservation=self)
+    def get_authority(self) -> ABCAuthorityProxy:
+        return self.authority
 
-            elif self.pending_state == ReservationPendingStates.Closing:
-                self.actor.close(reservation=self)
+    def get_source(self) -> ABCDelegation:
+        return self.source
 
-            else:
-                raise AuthorityException(self.UnexpectedExceptionString.format(self.state, self.pending_state))
-        elif self.state == ReservationStates.Failed:
-            self.logger.debug("No op")
-        else:
-            raise AuthorityException(self.UnexpectedExceptionString.format(self.state, self.pending_state))
+    def get_units(self, *, when: datetime = None) -> int:
+        hold = 0
+        if not self.is_terminal():
+            hold = self.resources.get_concrete_units(when=when)
 
-    def set_send_with_deficit(self, *, value: bool):
-        self.send_with_deficit = value
+        return hold
 
-    def get_deficit(self):
-        result = 0
-        if self.requested_resources is not None:
-            result = self.requested_resources.get_units()
+    def is_closed_in_priming(self) -> bool:
+        return self.closed_in_priming
 
-        if self.resources is not None:
-            cs = self.resources.get_resources()
-            if cs is not None:
-                result -= cs.get_units()
+    def is_exporting(self) -> bool:
+        return self.exporting
 
-        return result
+    def set_exporting(self):
+        self.exporting = True
 
-    def get_leased_units(self) -> int:
-        if self.resources is not None:
-            cs = self.resources.get_resources()
-            if cs is not None:
-                return cs.get_units()
-        return 0
-
-    def get_notices(self) -> str:
-        s = super().get_notices()
-        if self.resources is not None and self.resources.get_resources() is not None:
-            resource_notices = self.resources.get_resources().get_notices()
-            if resource_notices is not None:
-                s += f" {resource_notices}"
+    def set_source(self, *, source: ABCDelegation):
+        """
+        Set source
+        @param source source
+        """
+        self.source = source
 
-        return s
+    def set_authority(self, *, authority: ABCAuthorityProxy):
+        self.authority = authority
 
-    def get_ticket(self) -> ResourceSet:
-        return self.ticket
+    def update_lease(self, *, incoming: ABCReservationMixin, update_data):
+        self.logger.info(f"Received Update Lease: {incoming} at Broker")
+        # TODO add any processing if needed
+        self.logger.info(f"Do Nothing!")
 
     def handle_failed_rpc(self, *, failed: FailedRPC):
-        if failed.get_error_type() == RPCError.NetworkError:
-            if self.is_failed() or self.is_closed():
-                return
-
-        # Resources were allocated successfully but Orchestrator could not be informed
-        if failed.get_request_type() == RPCRequestType.UpdateLease and self.resources is not None and \
-                self.last_pending_state != ReservationPendingStates.ExtendingLease:
-            self.logger.error(f"Closing reservation due to non-recoverable RPC error {failed.get_error_type()}")
-            self.update_data.error(message=str(failed.get_error()))
-            self.actor.close(reservation=self)
+        if failed.get_request_type() == RPCRequestType.UpdateTicket and \
+                self.last_pending_state == ReservationPendingStates.ExtendingTicket:
+            return
+        super().handle_failed_rpc(failed=failed)
 
+    def fail_extend(self, *, message: str, exception: Exception = None):
+        self.extend_failure = True
+        super().fail(message=message, exception=exception)
 
-class AuthorityReservationFactory:
-    """
-    Factory class for creating authority reservations
-    """
+
+class BrokerReservationFactory:
     @staticmethod
-    def create(*, resources: ResourceSet, term: Term, slice_obj: ABCSlice, rid: ID, actor: ABCActorMixin = None):
+    def create(*, rid: ID, resources: ResourceSet, term: Term, slice_obj: ABCSlice, actor: ABCActorMixin = None):
         """
-        Create an Authotrity Reservation
+        Create Broker Reservation
+        :param rid:
         :param resources:
         :param term:
         :param slice_obj:
-        :param rid:
         :param actor:
         :return:
         """
-        res = AuthorityReservation(rid=rid, resources=resources, term=term, slice_object=slice_obj)
-        res.restore(actor=actor, slice_obj=slice_obj)
-        return res
+        reservation = BrokerReservation(rid=rid, resources=resources, term=term, slice_obj=slice_obj)
+        reservation.restore(actor=actor, slice_obj=slice_obj)
+        return reservation
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/broker_query_model_publisher.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/broker_query_model_publisher.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/broker_reservation.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/reservation.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,100 +19,151 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-
 from __future__ import annotations
 
 import threading
-import traceback
-from datetime import datetime
 from typing import TYPE_CHECKING
 
-from fabric_cf.actor.core.common.exceptions import BrokerException, ExceptionErrorCode
-from fabric_cf.actor.core.util.id import ID
-from fabric_cf.actor.core.apis.abc_authority_policy import ABCAuthorityPolicy
-from fabric_cf.actor.core.apis.abc_broker_policy_mixin import ABCBrokerPolicyMixin
-from fabric_cf.actor.core.apis.abc_reservation_mixin import ReservationCategory, ABCReservationMixin
-from fabric_cf.actor.core.apis.abc_broker_reservation import ABCBrokerReservation
-from fabric_cf.actor.core.kernel.rpc_manager_singleton import RPCManagerSingleton
-from fabric_cf.actor.core.kernel.rpc_request_type import RPCRequestType
-from fabric_cf.actor.core.kernel.request_types import RequestTypes
-from fabric_cf.actor.core.kernel.reservation_server import ReservationServer
-from fabric_cf.actor.core.kernel.reservation_states import ReservationStates, ReservationPendingStates
+from datetime import datetime, timezone
+
+from fim.slivers.capacities_labels import ReservationInfo
+
+from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin, ReservationCategory
+from fabric_cf.actor.core.common.constants import Constants
+from fabric_cf.actor.core.common.event_logger import EventLogger
+from fabric_cf.actor.core.common.exceptions import ReservationException
+from fabric_cf.actor.core.kernel.reservation_states import ReservationStates, ReservationPendingStates, JoinState
+from fabric_cf.actor.core.proxies.kafka.translate import Translate
+from fabric_cf.actor.core.util.reservation_state import ReservationState
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
-    from fabric_cf.actor.core.apis.abc_authority_proxy import ABCAuthorityProxy
-    from fabric_cf.actor.core.apis.abc_callback_proxy import ABCCallbackProxy
-    from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
     from fabric_cf.actor.core.apis.abc_policy import ABCPolicy
     from fabric_cf.actor.core.apis.abc_slice import ABCSlice
-    from fabric_cf.actor.core.kernel.failed_rpc import FailedRPC
+    from fabric_cf.actor.core.apis.abc_slice import ABCSlice
+    from fabric_cf.actor.core.kernel.request_types import RequestTypes
     from fabric_cf.actor.core.kernel.resource_set import ResourceSet
     from fabric_cf.actor.core.time.term import Term
+    from fabric_cf.actor.core.util.id import ID
+    from fabric_cf.actor.core.util.resource_type import ResourceType
+    from fabric_cf.actor.core.kernel.poa import Poa
 
 
-class BrokerReservation(ReservationServer, ABCBrokerReservation):
+class Reservation(ABCReservationMixin):
     """
-    A note on exported "will call" reservations. An export() operation may be
-    locally initiated on an agent. It binds and forms a ticket in the same way as
-    if the request came from a client, but there is no client rid (remoteRid) and
-    no callback object. The prepare method in AgentReservation and
-    register/unregister in ReservationServer handle these cases: the export
-    proceeds as a normal reserve request, but it leaves the callback and
-    remoteRid null, does not register the reservation with its slice (since there
-    is no remoteRid), and does not issue an updateTicket (since there is no
-    callback).
+    These are the only methods synchronized on the Reservation object itself. The
+    purpose is to allow an external thread to await a state transition in a
+    Reservation without holding the orchestrator lock. State changes are made only
+    while holding the orchestrator lock, so a orchestrator may examine the state without
+    acquiring the reservation lock.
+
+    Reservation objects passed into a slices actor to initiate or request new
+    reservations are taken over by the kernel. Validate the passed-in state, mark
+    some context specific to the operation, and clean out the rest of it in
+    preparation to link it into orchestrator structures. No locks are held, and these
+    routines have no side effects other than to the (new) reservation.
+
+    Reservation is the base for all reservation objects. It
+    implements a part of the IReservation interface and defines the
+    core functions expected by the kernel from all reservation classes. This is
+    an abstract class and is intended as a building block of higher-level
+    reservation classes.
     """
-    updated_absorbed = "update absorbed"
 
-    def __init__(self, *, rid: ID, resources: ResourceSet, term: Term, slice_obj: ABCSlice):
-        super().__init__(rid=rid, resources=resources, term=term, slice_object=slice_obj)
-        # Delegation backing the ticket granted to this reservation. For now only
-        # one source delegation can be used to issue a ticket to satisfy a client
-        # request.
-        self.source = None
-        # If this flag is true, then the reservation represents a request to export
-        # resources to a client.
-        self.exporting = False
-        # The authority in control of the resources.
-        self.authority = None
-        # True if an updateTicket() must be sent on the next service probe.
-        self.must_send_update = None
-        # True if we notified the client about the fact that the reservation had failed
-        self.notified_failed = False
-        # True if the reservation was closed in the priming state.
-        self.closed_in_priming = False
-        self.category = ReservationCategory.Broker
-        self.extend_failure = False
+    def __init__(self, *, rid: ID = None, resources: ResourceSet = None, term: Term = None,
+                 slice_object: ABCSlice = None):
+        # The unique reservation identifier.
+        self.rid = rid
+        # Reservation category. Subclasses should supply the correct value.
+        self.category = ReservationCategory.All
+        # Reservation state.
+        self.state = ReservationStates.Nascent
+        # Reservation pending state.
+        self.pending_state = ReservationPendingStates.None_
+        # Has this reservation ever been extended?
+        self.extended = False
+        # The current resources associated with this reservation.
+        self.resources = resources
+        # Resources representing the last request issued/received for this reservation
+        self.requested_resources = None
+        # Resources approved by the policy for this reservation. This resource set
+        # can be different from what was initially requested (requested_resources)
+        # Eventually, resources will be merged with approved_resources.
+        self.approved_resources = None
+        # The current term of the reservation.
+        self.term = term
+        # The previous term of the reservation.
+        self.previous_term = None
+        # The term of the last request issued/received for this reservation.
+        self.requested_term = None
+        # The term the policy approved for this reservation. This term can be
+        # different from what was initially requested (requested_term). Eventually,
+        # term will be set to equal approved_term.
+        self.approved_term = None
+        # True if this is a renewable reservation. By default, reservations are not renewable
+        self.renewable = None
+        # Last error message.
+        self.error_message = None
+        # Cached pointer to the actor that operates on this reservation.
+        self.actor = None
+        # Logger
+        self.logger = None
+        # Slice this reservation belongs to.
+        self.slice = slice_object
+        if slice_object is not None:
+            # Cached slice name. Necessary so that we can obtain the slice for
+            # reservations that have not been fully recovered.
+            self.slice_name = slice_object.get_name()
+            # Cached slice id. Necessary so that we can obtain the slice for
+            # reservations that have not been fully recovered.
+            self.slice_id = slice_object.get_slice_id()
+        else:
+            self.slice_name = None
+            self.slice_id = None
+        # Indicates if the policy plugin has made a decision about this reservation
+        self.approved = False
+        # The resources assigned to the reservation before the last update.
+        self.previous_resources = None
+        # Is an allocation process in progress?
+        self.bid_pending = False
+        # Dirty flag. Indicates that the state of the reservation object has
+        # changed since the last time it was persisted. Currently only transition
+        # updates the dirty flag
+        self.dirty = False
+        # True if this reservation is expired. Used during recovery.
+        self.expired = False
+        # Recovery flag.
+        self.pending_recover = False
+        # True if the last state transition is not committed to external storage.
+        # false otherwise.
+        self.state_transition = False
+        # Scratch element to trigger post-actions on a probe.
+        self.service_pending = ReservationPendingStates.None_
+        self.last_transition_time = None
+        self.last_pending_state = ReservationPendingStates.None_
+        self.thread_lock = threading.Lock()
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state['actor']
         del state['logger']
         del state['slice']
         del state['approved']
         del state['previous_resources']
         del state['bid_pending']
         del state['dirty']
         del state['expired']
         del state['pending_recover']
         del state['state_transition']
         del state['service_pending']
-
-        del state['policy']
-
-        del state['source']
-        del state['notified_failed']
-        del state['closed_in_priming']
-        del state['extend_failure']
         del state['thread_lock']
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self.actor = None
         self.logger = None
@@ -121,446 +172,551 @@
         self.previous_resources = None
         self.bid_pending = False
         self.dirty = False
         self.expired = False
         self.pending_recover = False
         self.state_transition = False
         self.service_pending = ReservationPendingStates.None_
-
-        self.policy = None
-
-        self.source = None
-        self.notified_failed = False
-        self.closed_in_priming = False
-        self.extend_failure = False
         self.thread_lock = threading.Lock()
 
     def restore(self, *, actor: ABCActorMixin, slice_obj: ABCSlice):
         """
         Must be invoked after creating reservation from unpickling
         """
-        super().restore(actor=actor, slice_obj=slice_obj)
-        self.source = None
-        if actor is not None and self.resources is not None and self.resources.get_resources() is not None:
-            delegation_id = self.resources.get_resources().get_delegation_id()
-            delegation = self.actor.get_delegation(did=delegation_id)
-            self.source = delegation
-        self.notified_failed = False
-        self.closed_in_priming = False
-
-    def print_state(self):
-        """
-        Converts the reservation to a state string.
-        @return state string representing the reservation
-        """
-        return "[{},{}] ({})({})".format(self.get_state_name(), self.get_pending_state_name(), self.get_sequence_in(),
-                                         self.get_sequence_out())
-
-    def recover(self):
-        """
-        Recover the reservation post stateful restart
-        """
-        if isinstance(self.policy, ABCAuthorityPolicy):
-            self.logger.debug("No recovery necessary for reservation #{}".format(self.get_reservation_id()))
-            return
-
-        if not isinstance(self.policy, ABCBrokerPolicyMixin):
-            raise BrokerException(msg=f"Do not know how to recover: policy={self.policy}")
-
-        if self.state == ReservationStates.Nascent:
-            if self.pending_state == ReservationPendingStates.None_:
-                self.actor.ticket(self)
-                self.logger.info("Added reservation #{} to the ticketing list. State={}".format(
-                    self.get_reservation_id(), self.print_state()))
-
-            elif self.pending_state == ReservationPendingStates.Ticketing:
-                self.set_pending_recover(pending_recover=True)
-                self.transition(prefix="[recovery]", state=self.state, pending=ReservationPendingStates.None_)
-                self.actor.ticket(self)
-                self.logger.info(
-                    "Added reservation #{} to the ticketing list. State={}".format(self.get_reservation_id(),
-                                                                                   self.print_state()))
-
-            else:
-                raise BrokerException(error_code=ExceptionErrorCode.UNEXPECTED_STATE,
-                                      msg=f"pending_state={self.pending_state}")
-
-        elif self.state == ReservationStates.Ticketed:
-            if self.pending_state == ReservationPendingStates.None_ or \
-                    self.pending_state == ReservationPendingStates.Priming:
-                self.set_service_pending(code=ReservationPendingStates.None_)
-                self.logger.debug("No recovery necessary for reservation #{}".format(self.get_reservation_id()))
-
-            elif self.pending_state == ReservationPendingStates.ExtendingTicket:
-                self.set_pending_recover(pending_recover=True)
-                self.transition(prefix="[recovery]", state=self.state,
-                                pending=ReservationPendingStates.None_)
-                self.actor.extend_ticket(reservation=self)
-                self.logger.info(
-                    "Added reservation #{} to the extending list. State={}".format(self.get_reservation_id(),
-                                                                                   self.print_state()))
-            else:
-                raise BrokerException(error_code=ExceptionErrorCode.UNEXPECTED_STATE,
-                                      msg=f"pending_state={self.pending_state}")
+        self.actor = actor
+        self.slice = slice_obj
+        if actor is not None:
+            self.logger = self.actor.get_logger()
+        self.approved = False
+        self.previous_resources = None
+        self.bid_pending = False
+        self.dirty = False
+        self.expired = False
+        self.pending_recover = False
+        self.state_transition = False
+        self.service_pending = ReservationPendingStates.None_
+        if actor is not None:
+            if self.resources is not None:
+                self.resources.restore(plugin=actor.get_plugin(), reservation=self)
+            if self.requested_resources is not None:
+                self.requested_resources.restore(plugin=actor.get_plugin(), reservation=self)
+            if self.approved_resources is not None:
+                self.approved_resources.restore(plugin=actor.get_plugin(), reservation=self)
 
-        elif self.state == ReservationStates.Failed:
-            self.logger.warning("Reservation #{} has failed".format(self.get_reservation_id()))
-        else:
-            raise BrokerException(error_code=ExceptionErrorCode.UNEXPECTED_STATE,
-                                  msg=f"state={self.state}")
+    def can_redeem(self) ->bool:
+        return True
 
-    def prepare(self, *, callback: ABCCallbackProxy, logger):
-        self.set_logger(logger=logger)
-        self.callback = callback
-
-        # Null callback indicates a locally initiated request to create an
-        # exported reservation. Else the request is from a client and must have
-        # a client-specified RID.
+    def can_renew(self) -> bool:
+        return True
 
-        if self.callback is not None and self.rid is None:
-            self.error(err="no reservation ID specified for request")
+    def internal_error(self, *, err: str):
+        """
+        Internal error log and raise exception
+        """
+        self.logger.error(f"internal error for reservation: {self} : {err}")
+        raise ReservationException(f"internal error: {err}")
 
-        self.set_dirty()
+    def error(self, *, err: str):
+        """
+        Error log and raise exception
+        """
+        if self.logger is not None:
+            self.logger.error(f"error for reservation: {self} : {err}")
+        else:
+            print(f"error for reservation: {self} : {err}")
+        raise ReservationException(f"error: {err}")
 
-    def reserve(self, *, policy: ABCPolicy):
-        # These handlers may need to be slightly more sophisticated, since a
-        # client may bid multiple times on a ticket as part of an auction
-        # protocol: so we may receive a reserve or extend when there is already
-        # a request pending.
-        self.incoming_request()
-
-        if self.pending_state != ReservationPendingStates.None_ and \
-                self.pending_state != ReservationPendingStates.Ticketing:
-            # We do not want to fail the reservation simply log a warning and exit from reserve
-            self.logger.warning("Duplicate ticket request")
-            return
+    def clear_dirty(self):
+        """
+        Clear dirty flag
+        """
+        self.dirty = False
+        self.state_transition = False
 
-        self.policy = policy
-        self.approved = False
-        self.bid_pending = True
-        self.map_and_update(ticketed=False)
+    def clear_notice(self, clear_fail: bool=False):
+        """
+        Clears all event notices associated with the reservation.
+        """
 
-    def service_reserve(self):
-        # resources is null initially. It becomes non-null once the
-        # policy completes its allocation.
-        if self.resources is not None:
-            self.resources.service_update(reservation=self)
-            if not self.is_failed():
-                self.transition(prefix=self.updated_absorbed, state=ReservationStates.Ticketed,
-                                pending=ReservationPendingStates.None_)
-                self.generate_update()
+    def close(self):
+        """
+        Close a reservation
+        """
+
+    def extend_lease(self):
+        """
+        Extend lease on reservation
+        """
+
+    def modify_lease(self):
+        """
+        Modify lease on reservation
+        """
 
     def extend_ticket(self, *, actor: ABCActorMixin):
-        self.incoming_request()
+        """
+        Extend a ticket
+        """
+        self.internal_error(err="abstract extend_ticket trap")
 
-        # State must be ticketed. The reservation may be active, but the agent wouldn't know that
-        if self.state != ReservationStates.Ticketed:
-            self.error(err="extending unticketed reservation")
-
-        if self.pending_state != ReservationPendingStates.None_ and self.pending_state != \
-                ReservationPendingStates.ExtendingTicket:
-            self.error(err="extending reservation with another pending request")
+    def fail(self, *, message: str, exception: Exception = None):
+        """
+        Fail a reservation
+        """
+        self.error_message = message
+        self.bid_pending = False
+        self.transition(prefix=message, state=ReservationStates.Failed, pending=ReservationPendingStates.None_)
+        self.logger.error(f"{message}  e: {exception}")
 
-        if not self.requested_term.extends_term(old_term=self.term):
-            self.error(err=f"new term {self.requested_term} does not extend current term {self.term}")
+    def fail_warn(self, *, message: str):
+        """
+        Fail with a warning
+        """
+        self.error_message = message
+        self.transition(prefix=message, state=ReservationStates.Failed, pending=ReservationPendingStates.None_)
+        message = f"reservation has failed: {message} : [{self}]"
+        self.logger.warning(message)
 
-        self.approved = False
-        self.bid_pending = True
-        self.pending_recover = False
-        self.map_and_update(ticketed=True)
+    def get_actor(self):
+        return self.actor
 
-    def service_extend_ticket(self):
-        if self.pending_state == ReservationPendingStates.None_:
-            self.resources.service_update(self)
-            if not self.is_failed():
-                self.transition(prefix=self.updated_absorbed, state=ReservationStates.Ticketed,
-                                pending=ReservationPendingStates.None_)
-                self.generate_update()
+    def get_approved_resources(self) -> ResourceSet:
+        return self.approved_resources
 
-    def close(self):
-        send_notification = False
-        if self.state == ReservationStates.Nascent or self.pending_state != ReservationPendingStates.None_:
-            self.logger.warning("Closing a reservation in progress")
-            send_notification = True
-
-        if self.state != ReservationStates.Closed:
-            if self.pending_state == ReservationPendingStates.Priming or \
-                    (self.pending_state == ReservationPendingStates.Ticketing and not self.bid_pending):
-                # Close in Priming is a special case: when processing the close
-                # event inside the policy we cannot rely on resources to
-                # represent the resources allocated to the reservation. They
-                # may either represent the previous resources or a mixture of
-                # both. So here we will mark the reservation that it was closed
-                # while it was in the Priming state. When processing the close
-                # event the policy must free previousResources (if any) and
-                # approvedResources. The policy should not free resources.
-                self.logger.debug("closing reservation #{} while in Priming".format(self.rid))
-                self.closed_in_priming = True
-
-            self.transition(prefix="closed", state=ReservationStates.Closed, pending=ReservationPendingStates.None_)
-            self.policy.closed(reservation=self)
-
-        if send_notification:
-            self.update_data.error(message="Closed while allocating ticket")
-            self.generate_update()
+    def get_approved_term(self) -> Term:
+        return self.approved_term
 
-    def probe_pending(self):
-        if self.service_pending != ReservationPendingStates.None_:
-            self.internal_error(err="service overrun in probePending")
+    def get_approved_type(self) -> ResourceType:
+        if self.approved_resources is not None:
+            return self.approved_resources.get_type()
+        return None
 
-        if self.is_failed() and not self.notified_failed:
-            self.generate_update()
-            self.notified_failed = True
-            if self.extend_failure:
-                self.transition(prefix="Recover from Extend Failure", state=ReservationStates.Ticketed,
-                                pending=ReservationPendingStates.None_)
-                self.extend_failure = False
-        else:
-            if self.pending_state == ReservationPendingStates.Ticketing:
-                # Check for a pending ticket operation that may have completed
-                if not self.bid_pending and self.map_and_update(ticketed=False):
-                    self.service_pending = ReservationPendingStates.AbsorbUpdate
-
-            elif self.pending_state == ReservationPendingStates.ExtendingTicket:
-                # Check for a pending extendTicket operation
-                if not self.bid_pending and self.map_and_update(ticketed=True):
-                    self.service_pending = ReservationPendingStates.AbsorbUpdate
-
-            elif self.pending_state == ReservationPendingStates.Redeeming:
-                self.logger.error("AgentReservation in unexpected state")
-
-            elif self.pending_state == ReservationPendingStates.Priming:
-                self.service_pending = ReservationPendingStates.AbsorbUpdate
-
-            elif self.pending_state == ReservationPendingStates.None_ and self.must_send_update:
-                # for exported reservations that have been claimed, we need to
-                # schedule a ticketUpdate
-                self.service_pending = ReservationPendingStates.SendUpdate
-                self.must_send_update = False
+    def get_approved_units(self) -> int:
+        if self.approved_resources is not None:
+            return self.approved_resources.get_units()
+        return 0
 
-    def service_probe(self):
-        try:
-            if self.service_pending == ReservationPendingStates.AbsorbUpdate:
-                self.resources.service_update(reservation=self)
-                if not self.is_failed():
-                    self.transition(prefix=self.updated_absorbed, state=ReservationStates.Ticketed,
-                                    pending=ReservationPendingStates.None_)
-                    self.generate_update()
-
-            elif self.service_pending == ReservationPendingStates.SendUpdate:
-                self.generate_update()
-
-        except Exception as e:
-            self.logger.error(traceback.format_exc())
-            self.logger.error("failed while servicing probe e:{}".format(e))
-            self.fail_notify(message=str(e))
+    def get_category(self) -> ReservationCategory:
+        return self.category
 
-        self.service_pending = ReservationPendingStates.None_
+    def get_kernel_slice(self) -> ABCSlice:
+        return self.slice
 
-    def handle_duplicate_request(self, *, operation: RequestTypes):
-        # The general idea is to do nothing if we are in the process of
-        # performing a pending operation or about to reissue a
-        # ticket/extendTicket after recovery. If there is nothing pending for
-        # this reservation, we resend the last update.
-        if operation == RequestTypes.RequestTicket:
-            if self.pending_state == ReservationPendingStates.None_ and self.state != ReservationStates.Nascent and \
-                    not self.pending_recover:
-                self.generate_update()
-
-        elif operation == RequestTypes.RequestExtendTicket:
-            if self.pending_state == ReservationPendingStates.None_ and not self.pending_recover:
-                self.generate_update()
+    def get_leased_abstract_units(self) -> int:
+        return 0
 
-        elif operation == RequestTypes.RequestRelinquish:
-            self.logger.debug("no op")
+    def get_leased_units(self) -> int:
+        return 0
 
-        else:
-            raise BrokerException(error_code=ExceptionErrorCode.NOT_SUPPORTED,
-                                  msg=f"operation {RequestTypes(operation).name}")
+    def get_notices(self) -> str:
+        """
+        Returns a descriptive string if this reservation requires attention, else None
 
-    def generate_update(self):
-        self.logger.debug("Generating update")
-        if self.callback is None:
-            self.logger.warning("Cannot generate update: no callback.")
-            return
-
-        self.logger.debug("Generating update: update count={}".format(self.update_count))
-        try:
-            self.update_count += 1
-            self.sequence_out += 1
-            RPCManagerSingleton.get().update_ticket(reservation=self)
-        except Exception as e:
-            self.logger.error(traceback.format_exc())
-            # Note that this may result in a "stuck" reservation... not much we
-            # can do if the receiver has failed or rejects our update. We will
-            # regenerate on any user-initiated probe.
-            self.logger.error("callback failed e:{}".format(e))
-
-    def map_and_update(self, *, ticketed: bool):
-        """
-        Call the policy to fill a request, with associated state transitions.
-        Catch exceptions and report all errors using callback mechanism.
-
-        @param ticketed
-                   true iff this is ticketed (i.e., request is extend)
-        @return boolean success
-        """
-        success = False
-        granted = False
-
-        if self.state == ReservationStates.Failed:
-            # Must be a previous failure, or policy marked as failed. Send
-            # update to reset client. Note: this might be the wrong thing if a
-            # bidding protocol allows the caller to retry a denied request,
-            # e.g., to bid higher after losing in an auction.
-            self.generate_update()
-        elif self.state == ReservationStates.Nascent:
-            if ticketed:
-                self.fail_notify(message="reservation is not yet ticketed")
-            else:
-                self.logger.debug("Using policy {} to bind reservation".format(self.policy.__class__.__name__))
-                try:
-                    granted = False
-                    # If the policy has processed this reservation, granted should
-                    # be set true so that we can send the result back to the
-                    # client. If the policy has not yet processed this reservation
-                    # (binPending is true) then call the policy. The policy may
-                    # choose to process the request immediately (true) or to defer
-                    # it (false). In case of a deferred request, we will eventually
-                    # come back to this method after the policy has done its job.
-                    if self.is_bid_pending():
-                        if not self.is_exporting():
-                            granted = self.policy.bind(reservation=self)
-                        else:
-                            self.internal_error(err="Exporting reservations not implemented")
-                    else:
-                        granted = True
-                    self.transition(prefix="ticket request", state=ReservationStates.Nascent,
-                                    pending=ReservationPendingStates.Ticketing)
-                except Exception as e:
-                    self.logger.error(f"mapAndUpdate bindTicket failed for ticketRequest: {e}")
-                    self.fail_notify(message=str(e))
-                    return success
-
-                if granted:
-                    self.logger.debug("Reservation {} has been granted".format(self.get_reservation_id()))
-                    try:
-                        success = True
-                        self.term = self.approved_term
-                        self.resources = self.approved_resources.abstract_clone()
-                        self.resources.update(reservation=self, resource_set=self.approved_resources)
-                        self.transition(prefix="ticketed", state=ReservationStates.Ticketed,
-                                        pending=ReservationPendingStates.Priming)
-                    except Exception as e:
-                        self.logger.error("mapAndUpdate ticket failed for ticketRequest")
-                        self.logger.error(e)
-                        self.logger.error(traceback.format_exc())
-                        self.fail_notify(message=str(e))
-        elif self.state == ReservationStates.Ticketed:
-            if not ticketed:
-                self.fail_notify(message="reservation is already ticketed")
-            else:
-                try:
-                    self.transition(prefix="extending ticket", state=ReservationStates.Ticketed,
-                                    pending=ReservationPendingStates.ExtendingTicket)
-
-                    # If the policy has processed this reservation, set granted to
-                    # true so that we can send the ticket back to the client. If
-                    # the policy has not yet processed this reservation (bid_pending
-                    # is true) then call the policy. The plugin may choose to
-                    # process the request immediately (true) or to defer it
-                    # (false). In case of a deferred request, we will eventually
-                    # come back to this method after the policy has done its job.
-
-                    granted = False
-
-                    if self.is_bid_pending():
-                        granted = self.policy.extend_broker(reservation=self)
-                    else:
-                        granted = True
-                except Exception as e:
-                    self.logger.error(f"mapAndUpdate extendTicket failed for ExtendTicket: {e}")
-                    self.fail_notify(message=str(e))
-                    return success
-
-                if granted:
-                    try:
-                        success = True
-                        self.extended = True
-                        self.transition(prefix="extended ticket", state=ReservationStates.Ticketed,
-                                        pending=ReservationPendingStates.Priming)
-                        self.previous_term = self.term
-                        self.previous_resources = self.resources.clone()
-                        self.term = self.approved_term
-                        self.resources.update(reservation=self, resource_set=self.approved_resources)
-                    except Exception as e:
-                        self.logger.error(f"mapAndUpdate extend ticket failed for ExtendTicket: {e}")
-                        self.fail_notify(message=str(e))
-        else:
-            self.logger.error("broker mapAndUpdate: unexpected state")
-            self.fail_notify(message="invalid operation for the current reservation state")
+        @return notices string
+        """
+        msg = f"Reservation {self.rid} (Slice {self.slice}) is in state ({self.get_state_name()}," \
+              f"{self.get_pending_state_name()})"
+
+        if self.error_message is not None and self.error_message != "":
+            msg += f", err={self.error_message}"
+        return msg
 
-        return success
+    def get_pending_state(self) -> ReservationPendingStates:
+        return self.pending_state
 
-    def get_authority(self) -> ABCAuthorityProxy:
-        return self.authority
+    def get_pending_state_name(self) -> str:
+        return ReservationPendingStates(self.pending_state).name
 
-    def get_source(self) -> ABCDelegation:
-        return self.source
+    def get_previous_resources(self) -> ResourceSet:
+        return self.previous_resources
+
+    def get_previous_term(self) -> Term:
+        return self.previous_term
+
+    def get_requested_resources(self) -> ResourceSet:
+        return self.requested_resources
+
+    def get_requested_term(self) -> Term:
+        return self.requested_term
+
+    def get_requested_type(self) -> ResourceType:
+        if self.requested_resources is not None:
+            return self.requested_resources.get_type()
+        return None
+
+    def get_requested_units(self) -> int:
+        if self.requested_resources is not None:
+            return self.requested_resources.get_units()
+        return 0
+
+    def get_reservation_id(self) -> ID:
+        return self.rid
+
+    def get_reservation_state(self) -> ReservationState:
+        return ReservationState(state=self.state, pending=self.pending_state)
+
+    def get_resources(self) -> ResourceSet:
+        return self.resources
+
+    def get_slice(self) -> ABCSlice:
+        return self.slice
+
+    def get_slice_id(self):
+        if self.slice is None:
+            return None
+        return self.slice.get_slice_id()
+
+    def get_slice_name(self):
+        if self.slice is None:
+            return None
+        return self.slice.get_name()
+
+    def get_state(self) -> ReservationStates:
+        return self.state
+
+    def get_state_name(self) -> str:
+        return self.state.name
+
+    def get_term(self) -> Term:
+        return self.term
+
+    def get_type(self) -> ResourceType:
+        if self.resources is None:
+            return None
+        return self.resources.get_type()
 
     def get_units(self, *, when: datetime = None) -> int:
-        hold = 0
-        if not self.is_terminal():
-            hold = self.resources.get_concrete_units(when=when)
+        if when is None:
+            if self.resources is None:
+                return 0
+            return self.resources.get_units()
+        if not self.is_terminal() and self.term is not None and self.term.contains(date=when):
+            return self.resources.get_concrete_units(when=when)
+        return 0
 
-        return hold
+    def handle_duplicate_request(self, *, operation: RequestTypes):
+        return
+
+    def has_uncommitted_transition(self) -> bool:
+        return self.state_transition
 
-    def is_closed_in_priming(self) -> bool:
-        return self.closed_in_priming
+    def is_active(self) -> bool:
+        return self.state == ReservationStates.Active or self.state == ReservationStates.ActiveTicketed
 
-    def is_exporting(self) -> bool:
-        return self.exporting
+    def is_active_ticketed(self) -> bool:
+        return self.state == ReservationStates.ActiveTicketed
 
-    def set_exporting(self):
-        self.exporting = True
+    def is_approved(self) -> bool:
+        return self.approved
 
-    def set_source(self, *, source: ABCDelegation):
+    def is_bid_pending(self) -> bool:
         """
-        Set source
-        @param source source
+        Is bid pending
+        @return bid pending
         """
-        self.source = source
+        return self.bid_pending
+
+    def is_closed(self) -> bool:
+        return self.state == ReservationStates.Closed
+
+    def is_closing(self) -> bool:
+        return self.state == ReservationStates.CloseWait or self.pending_state == ReservationPendingStates.Closing
+
+    def is_dirty(self) -> bool:
+        return self.dirty
+
+    def is_expired(self, *, t: datetime = None) -> bool:
+        if t is None:
+            return self.expired
+        return self.term.expired(date=t)
+
+    def is_extended(self) -> bool:
+        return self.extended
+
+    def is_extending_lease(self) -> bool:
+        return self.pending_state == ReservationPendingStates.ExtendingLease
+
+    def is_extending_ticket(self) -> bool:
+        return self.pending_state == ReservationPendingStates.ExtendingTicket
 
-    def set_authority(self, *, authority: ABCAuthorityProxy):
-        self.authority = authority
+    def is_failed(self) -> bool:
+        return self.state == ReservationStates.Failed
+
+    def is_nascent(self) -> bool:
+        return self.state == ReservationStates.Nascent
+
+    def is_no_pending(self) -> bool:
+        return self.pending_state == ReservationPendingStates.None_
+
+    def is_pending_recover(self):
+        return self.pending_recover
+
+    def is_priming(self) -> bool:
+        return self.pending_state == ReservationPendingStates.Priming
+
+    def is_redeeming(self) -> bool:
+        return self.pending_state == ReservationPendingStates.Redeeming
+
+    def is_renewable(self) -> bool:
+        """
+        Is reservation renewable
+        @return true if renewable; false otherwise
+        """
+        return self.renewable
+
+    def is_terminal(self) -> bool:
+        return self.is_closed() or self.is_closing() or self.is_failed()
+
+    def is_ticketed(self) -> bool:
+        return self.state == ReservationStates.Ticketed
+
+    def is_ticketing(self) -> bool:
+        return self.pending_state == ReservationPendingStates.Ticketing
+
+    def nothing_pending(self):
+        """
+        Ensures the reservation does not have a pending operation.
+
+        @throws Exception if the reservation has a pending operation.
+        """
+        if self.pending_state != ReservationPendingStates.None_:
+            self.error(err=Constants.PENDING_OPERATION_ERROR)
+
+    def prepare_probe(self):
+        return
+
+    def probe_pending(self):
+        return
+
+    def ready(self):
+        """
+        An incoming client request named this validated Reservation object for an
+        existing reservation. Check to be sure that it has not been destroyed in
+        a race since the validate.
+
+        @throws Exception thrown if the state is closed or failed
+        """
+        if self.state == ReservationStates.Closed or self.state == ReservationStates.Failed:
+            self.error(err="invalid Reservation")
+
+    def reserve(self, *, policy: ABCPolicy):
+        return
+
+    def setup(self):
+        """
+        Setup a reservation
+        """
+        if self.resources is not None:
+            self.resources.setup(reservation=self)
+
+        if self.approved_resources is not None:
+            self.approved_resources.setup(reservation=self)
+
+        if self.requested_resources is not None:
+            self.requested_resources.setup(reservation=self)
+
+    def service_claim(self):
+        return
+
+    def service_reclaim(self):
+        return
+
+    def service_close(self):
+        return
+
+    def service_extend_lease(self):
+        return
+
+    def service_modify_lease(self):
+        return
+
+    def service_extend_ticket(self):
+        return
+
+    def service_probe(self):
+        return
+
+    def service_reserve(self):
+        return
+
+    def service_update_lease(self):
+        return
+
+    def service_update_ticket(self):
+        return
+
+    def set_actor(self, *, actor: ABCActorMixin):
+        self.actor = actor
+
+    def set_approved(self, *, term: Term = None, approved_resources: ResourceSet = None):
+        self.approved_term = term
+        self.approved_resources = approved_resources
+        self.approved = True
+
+    def set_approved_resources(self, *, approved_resources: ResourceSet):
+        self.approved_resources = approved_resources
+
+    def set_approved_term(self, *, term: Term):
+        self.approved_term = term
+
+    def set_bid_pending(self, *, value: bool):
+        """
+        Set Bid Pending
+        @param value value
+        """
+        self.bid_pending = value
+
+    def set_dirty(self):
+        """
+        Set dirty
+        """
+        self.dirty = True
+
+    def set_expired(self, *, value: bool):
+        self.expired = value
+
+    def set_logger(self, *, logger):
+        self.logger = logger
+
+    def set_pending_recover(self, *, pending_recover: bool):
+        self.pending_recover = pending_recover
+
+    def set_service_pending(self, *, code: ReservationPendingStates):
+        self.service_pending = code
+
+    def set_slice(self, *, slice_object: ABCSlice):
+        self.slice = slice_object
+
+    def __str__(self):
+        msg = "res: "
+        if self.rid is not None:
+            msg += f"#{self.rid} "
+
+        if self.slice is not None:
+            msg += f"slice: [{self.slice}] "
+
+        msg += f"state:[{self.get_state_name()},{self.get_pending_state_name()}] "
+
+        if self.resources is not None:
+            msg += f"resources: [{self.resources}] "
+
+        if self.term is not None:
+            msg += f"term: [{self.term}]"
+
+        return msg
+
+    def transition(self, *, prefix: str, state: ReservationStates, pending: ReservationPendingStates):
+        if self.state == ReservationStates.Failed and self.logger is not None:
+            self.logger.debug("failed")
+
+        if self.logger is not None:
+            self.logger.debug(f"Reservation #{self.rid} {prefix} transition: {self.get_state_name()} -> {state.name}, "
+                              f"{self.get_pending_state_name()} -> {pending.name}")
+
+        change = self.state != state
+        self.state = state
+        self.last_pending_state = pending
+        self.pending_state = pending
+
+        self.set_dirty()
+        self.state_transition = True
+        self.last_transition_time = datetime.now(timezone.utc)
+
+        if change:
+            sliver = None
+            if self.get_resources() is not None:
+                sliver = self.get_resources().get_sliver()
+            elif self.get_requested_resources() is not None:
+                sliver = self.get_requested_resources().get_sliver()
+            if sliver is not None:
+                if sliver.reservation_info is None:
+                    sliver.reservation_info = ReservationInfo()
+                sliver.reservation_info.reservation_id = str(self.get_reservation_id())
+                sliver.reservation_info.reservation_state = str(self.state)
+                EventLogger.log_sliver_event(logger=self.logger,
+                                             slice_object=Translate.translate_slice_to_avro(slice_obj=self.slice),
+                                             sliver=sliver)
 
     def update_lease(self, *, incoming: ABCReservationMixin, update_data):
-        self.logger.info(f"Received Update Lease: {incoming} at Broker")
-        # TODO add any processing if needed
-        self.logger.info(f"Do Nothing!")
-
-    def handle_failed_rpc(self, *, failed: FailedRPC):
-        if failed.get_request_type() == RPCRequestType.UpdateTicket and \
-                self.last_pending_state == ReservationPendingStates.ExtendingTicket:
-            return
-        super().handle_failed_rpc(failed=failed)
-
-    def fail_extend(self, *, message: str, exception: Exception = None):
-        self.extend_failure = True
-        super().fail(message=message, exception=exception)
-
-
-class BrokerReservationFactory:
-    @staticmethod
-    def create(*, rid: ID, resources: ResourceSet, term: Term, slice_obj: ABCSlice, actor: ABCActorMixin = None):
-        """
-        Create Broker Reservation
-        :param rid:
-        :param resources:
-        :param term:
-        :param slice_obj:
-        :param actor:
-        :return:
-        """
-        reservation = BrokerReservation(rid=rid, resources=resources, term=term, slice_obj=slice_obj)
-        reservation.restore(actor=actor, slice_obj=slice_obj)
-        return reservation
+        self.internal_error(err="abstract update_lease trap")
+
+    def update_ticket(self, *, incoming: ABCReservationMixin, update_data):
+        self.internal_error(err="abstract update_ticket trap")
+
+    def validate_outgoing(self):
+        return
+
+    def validate_incoming(self):
+        return
+
+    def validate(self):
+        """
+        Validates the reservation. For use by prepare() methods defined by
+        subclasses.
+
+        @throws Exception
+        """
+        assert self.state == ReservationStates.Nascent
+        self.nothing_pending()
+
+        if self.slice is None:
+            self.error(err="no slice specified")
+
+        if self.resources is None:
+            self.error(err="no resource set specified")
+
+        if self.term is None:
+            self.error(err="no term specified")
+
+        self.term.validate()
+
+    def get_join_state(self) -> JoinState:
+        """
+        Get Join State
+        @return join state
+        """
+        return JoinState.None_
+
+    def get_graph_node_id(self) -> str:
+        if self.requested_resources is not None:
+            request = self.requested_resources.get_sliver()
+            if request is not None:
+                node_map = request.get_node_map()
+                if node_map is not None:
+                    return node_map[1]
+        return None
+
+    def exceeds_timeout(self, timeout: int) -> bool:
+        """
+        Check if Reservation has been in the state for more than the timeout interval
+        @param timeout: timeout
+        @return True if reservation has been in the state for more than timeout; False otherwise
+        """
+        if self.last_transition_time is None:
+            return False
+
+        current_time = datetime.now(timezone.utc)
+        if (current_time - self.last_transition_time).seconds > timeout:
+            return True
+
+        return False
+
+    def get_error_message(self) -> str:
+        return self.error_message
+
+    def lock(self):
+        self.thread_lock.acquire()
+
+    def unlock(self):
+        if self.thread_lock.locked():
+            self.thread_lock.release()
+
+    def service_poa(self):
+        pass
+
+    def poa_info(self, *, incoming: Poa):
+        pass
+
+    def poa(self, *, poa: Poa):
+        """
+        POA on reservation
+        """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/claim_timeout.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/claim_timeout.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/failed_rpc.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/failed_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/failed_rpc_event.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/failed_rpc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_delegation_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_failed_rpc.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_failed_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_query_rpc.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_query_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_reservation_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_rpc.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/incoming_rpc_event.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/incoming_rpc_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,17 @@
                                  caller=self.rpc.get_caller())
             client.get_logger().debug("update ticket processed from <{}>".format(self.rpc.get_caller().get_name()))
         elif self.rpc.get_request_type() == RPCRequestType.UpdateDelegation:
             client.get_logger().debug("processing update delegation from <{}>".format(self.rpc.get_caller().get_name()))
             client.update_delegation(delegation=self.rpc.get(), update_data=self.rpc.get_update_data(),
                                      caller=self.rpc.get_caller())
             client.get_logger().debug("update delegation processed from <{}>".format(self.rpc.get_caller().get_name()))
+        elif self.rpc.get_request_type() == RPCRequestType.PoaInfo:
+            client.get_logger().debug("processing poa info from <{}>".format(self.rpc.get_caller().get_name()))
+            client.poa_info(poa=self.rpc.get(), caller=self.rpc.get_caller())
         else:
             processed = self.do_process_actor(actor=client)
         return processed
 
     def do_process_server(self, *, server: ABCServerActor):
         """
         Process Incoming RPC events common for server actors
@@ -169,14 +172,18 @@
             authority.modify_lease(reservation=self.rpc.get(), caller=self.rpc.get_caller(),
                                    callback=self.rpc.get_callback())
 
         elif self.rpc.get_request_type() == RPCRequestType.Close:
             authority.get_logger().debug("processing close from <{}>".format(self.rpc.get_caller().get_name()))
             authority.close(reservation=self.rpc.get())
 
+        elif self.rpc.get_request_type() == RPCRequestType.Poa:
+            authority.get_logger().debug("processing poa from <{}>".format(self.rpc.get_caller().get_name()))
+            authority.poa(poa=self.rpc.get())
+
         else:
             processed = self.do_process_server(server=authority)
         return processed
 
     def do_process_controller(self, *, controller: ABCController):
         """
         Process Incoming RPC events common for all controller/orchestrator
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/kernel.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from fabric_cf.actor.core.common.exceptions import ReservationNotFoundException, DelegationNotFoundException, \
     KernelException
 from fabric_cf.actor.core.kernel.authority_reservation import AuthorityReservation
 from fabric_cf.actor.core.kernel.failed_rpc import FailedRPC
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.apis.abc_server_reservation import ABCServerReservation
 from fabric_cf.actor.core.apis.abc_slice import ABCSlice
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.kernel.request_types import RequestTypes
 from fabric_cf.actor.core.kernel.reservation import Reservation
 from fabric_cf.actor.core.kernel.reservation_client import ReservationClient
 from fabric_cf.actor.core.kernel.reservation_states import ReservationPendingStates, ReservationStates
 from fabric_cf.actor.core.kernel.resource_set import ResourceSet
 from fabric_cf.actor.core.kernel.sequence_comparison_codes import SequenceComparisonCodes
 from fabric_cf.actor.core.kernel.slice_state_machine import SliceStateMachine, SliceState
@@ -1505,7 +1506,59 @@
             return local
 
         return None
 
     def update_maintenance_mode(self, *, properties: Dict[str, str], sites: List[Site] = None):
         Maintenance.update_maintenance_mode(database=self.plugin.get_database(),
                                             properties=properties, sites=sites)
+
+    def poa(self, *, reservation: ABCReservationMixin, poa: Poa):
+        """
+        Handles a POA for the sliver
+        Client: Issues a POA
+
+        Authority: process a POA
+        @param reservation reservation for which to perform POA
+        @param poa POA
+        @throws Exception
+        """
+        try:
+            # Add POA to the database
+            self.plugin.get_database().add_poa(poa=poa)
+            reservation.lock()
+
+            # Process POA
+            reservation.poa(poa=poa)
+
+            # Update POA
+            self.plugin.get_database().update_poa(poa=poa)
+        except Exception as e:
+            self.logger.error(traceback.format_exc())
+            self.error(err=f"An error occurred during poa for reservation #{reservation.get_reservation_id()}",
+                       e=e)
+        finally:
+            reservation.unlock()
+
+    def poa_info(self, *, reservation: ABCReservationMixin, poa: Poa):
+        """
+        Handles a POA Response for the sliver
+        Client: Issues a POA
+
+        Authority: process a POA
+        @param reservation reservation for which to perform POA
+        @param poa POA
+        @throws Exception
+        """
+        try:
+            reservation.lock()
+
+            # Process POA Info from Authority
+            reservation.poa_info(incoming=poa)
+
+            # Update Reservation
+            self.plugin.get_database().update_reservation(reservation=reservation)
+        except Exception as e:
+            self.logger.error(traceback.format_exc())
+            self.error(err=f"An error occurred during poa for reservation #{reservation.get_reservation_id()}",
+                       e=e)
+        finally:
+            reservation.unlock()
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel_tick.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/kernel_tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/kernel_wrapper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/kernel_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import time
 import traceback
 from datetime import datetime
 from typing import List, Dict
 
+from fabric_mb.message_bus.messages.poa_info_avro import PoaInfoAvro
 from fim.slivers.base_sliver import BaseSliver
 
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
 from fabric_cf.actor.core.apis.abc_actor_identity import ABCActorIdentity
 from fabric_cf.actor.core.apis.abc_base_plugin import ABCBasePlugin
 from fabric_cf.actor.core.apis.abc_authority_reservation import ABCAuthorityReservation
 from fabric_cf.actor.core.apis.abc_broker_reservation import ABCBrokerReservation
@@ -44,16 +45,16 @@
 from fabric_cf.actor.core.apis.abc_slice import ABCSlice
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import SliceNotFoundException
 from fabric_cf.actor.core.kernel.failed_rpc import FailedRPC
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.kernel.kernel import Kernel
 from fabric_cf.actor.core.common.exceptions import KernelException
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.kernel.request_types import RequestTypes
-from fabric_cf.actor.core.kernel.reservation_states import ReservationStates
 from fabric_cf.actor.core.kernel.resource_set import ResourceSet
 from fabric_cf.actor.core.kernel.sequence_comparison_codes import SequenceComparisonCodes
 from fabric_cf.actor.core.registry.actor_registry import ActorRegistrySingleton
 from fabric_cf.actor.core.container.maintenance import Site
 from fabric_cf.actor.core.time.term import Term
 from fabric_cf.actor.core.util.id import ID
 from fabric_cf.actor.core.util.update_data import UpdateData
@@ -228,18 +229,17 @@
                 self.kernel.handle_duplicate_request(current=target, operation=RequestTypes.RequestClose)
         else:
             target = self.kernel.validate(reservation=reservation)
             self.kernel.close(reservation=target)
 
     def advertise(self, *, delegation: ABCDelegation, client: AuthToken):
         """
-        Initiates a ticket export.
+        Advertise a delegation
         Role: Broker or Authority
-        Prepare/hold a ticket for "will call" claim by a client.
-        @param delegation reservation to be exported
+        @param delegation delegation to be exported
         @param client client identity
         @throws Exception in case of error
         """
         if delegation is None or delegation.get_slice_object() is None:
             raise KernelException(Constants.INVALID_ARGUMENT)
 
         delegation.prepare(callback=None, logger=self.logger)
@@ -550,14 +550,19 @@
 
         @throws Exception in case of error
         """
         if delegation.get_slice_object() is None or delegation.get_slice_object().get_name() is None or \
                 delegation.get_slice_object().get_slice_id() is None or delegation.get_delegation_id() is None:
             raise KernelException(Constants.INVALID_ARGUMENT)
 
+        if delegation.get_site() is None:
+            site_name = self.actor.get_name()
+            site_name = site_name.replace("-am", "")
+            delegation.site = site_name
+
         # Obtain the previously created slice or create a new slice. When this
         # function returns we will have a slice object that is registered with the kernel
         s = self.kernel.get_slice(slice_id=delegation.get_slice_id())
         if s is None:
             self.kernel.register_slice(slice_object=delegation.get_slice_object())
 
         # Determine if this is a new or an already existing reservation. We
@@ -670,15 +675,14 @@
         if diff > 0:
             self.logger.info(f"REDEEM VAL TIME: {diff}")
         begin = time.time()
         self.kernel.redeem(reservation=target)
         diff = int(time.time() - begin)
         if diff > 0:
             self.logger.info(f"REDEEM TIME: {diff}")
-        begin = time.time()
 
     def redeem_request(self, *, reservation: ABCAuthorityReservation, caller: AuthToken,
                        callback: ABCControllerCallbackProxy, compare_sequence_numbers: bool):
         """
         Processes an incoming request for a new lease.
         Role: Authority
         @param reservation reservation representing the lease request. Must
@@ -913,18 +917,17 @@
             self.kernel.tick()
         except Exception as e:
             self.logger.error("Tick error: {}".format(e))
             self.logger.error(traceback.format_exc())
 
     def delegate(self, *, delegation: ABCDelegation, destination: ABCActorIdentity):
         """
-        Initiates a delegate request. If the exported flag is set, this is a claim
-        on a pre-reserved "will call" ticket.
-        Role: Broker or Controller.
-        @param delegation delegation parameters for ticket request
+        Trigger a Claim Delegation
+        Role: Broker
+        @param delegation delegation
         @param destination identity of the actor the request must be sent to
         @throws Exception in case of error
         """
         if delegation is None or destination is None:
             raise KernelException(Constants.INVALID_ARGUMENT)
 
         callback = ActorRegistrySingleton.get().get_callback(protocol=Constants.PROTOCOL_KAFKA,
@@ -1138,7 +1141,60 @@
         if project is not None and tags is not None and email is not None:
             tag_list = tags.split(",")
             AccessChecker.check_pdp_access(action_id=action_id, email=email, project=project, tags=tag_list,
                                            resource=sliver, lease_end_time=lease_end_time, logger=self.logger)
 
     def update_maintenance_mode(self, *, properties: Dict[str, str], sites: List[Site] = None):
         self.kernel.update_maintenance_mode(properties=properties, sites=sites)
+
+    def poa(self, *, reservation: ABCReservationMixin, poa: Poa, raise_exception: bool = False):
+        """
+        Initiates a request to trigger POA for a sliver
+        Role: Controller
+        @param reservation reservation
+        @param poa
+        @param raise_exception
+        @throws Exception in case of error
+        """
+
+        if reservation is None:
+            raise KernelException(Constants.INVALID_ARGUMENT)
+
+        target = self.kernel.validate(rid=reservation.get_reservation_id())
+
+        if target is None:
+            self.logger.error("POA for a reservation not registered with the kernel")
+            raise KernelException("POA for a reservation not registered with the kernel")
+
+        try:
+            self.__authorize_request(action_id=ActionId.poa, reservation=reservation,
+                                     sliver=reservation.get_requested_resources().get_sliver(),
+                                     lease_end_time=None)
+
+            poa.restore(actor=self.actor, reservation=target)
+
+            # NOTE: this call does not require access control check, since
+            # it is executed in the context of the actor represented by KernelWrapper.
+            self.kernel.poa(reservation=target, poa=poa)
+
+        except Exception as e:
+            self.logger.error(traceback.format_exc())
+            self.logger.error("Exception occurred in processing POA request {}".format(e))
+            if raise_exception:
+                raise e
+
+    def poa_info(self, *, poa: Poa, caller: AuthToken):
+        if poa.get_sliver_id() is None:
+            raise KernelException(Constants.INVALID_ARGUMENT)
+
+        target = self.kernel.validate(rid=poa.get_sliver_id())
+
+        if target is None:
+            self.logger.error("POA response for a reservation not registered with the kernel")
+            raise KernelException("POA response for a reservation not registered with the kernel")
+
+        try:
+            poa.restore(actor=self.actor, reservation=target)
+            self.kernel.poa_info(reservation=target, poa=poa)
+        except Exception as e:
+            self.logger.error(traceback.format_exc())
+            self.logger.error("Exception occurred in processing POA response {}".format(e))
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/predecessor_state.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/predecessor_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/query_timeout.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/query_timeout.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/request_types.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/request_types.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_client.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/reservation_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from fim.slivers.network_service import NetworkServiceSliver
 
 from fabric_cf.actor.core.apis.abc_authority_policy import ABCAuthorityPolicy
 from fabric_cf.actor.core.apis.abc_controller_reservation import ABCControllerReservation
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import ReservationException
 from fabric_cf.actor.core.kernel.failed_rpc import FailedRPC
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.util.rpc_exception import RPCError
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin, ReservationCategory
 from fabric_cf.actor.core.kernel.predecessor_state import PredecessorState
 from fabric_cf.actor.core.kernel.rpc_manager_singleton import RPCManagerSingleton
 from fabric_cf.actor.core.kernel.reservation import Reservation
 from fabric_cf.actor.core.kernel.reservation_states import ReservationPendingStates, ReservationStates, JoinState
 from fabric_cf.actor.core.util.id import ID
@@ -183,14 +184,15 @@
         self.suggested = True
 
         self.renewable = False
         self.approved_resources = resources
         self.approved_term = term
         self.approved = True
         self.category = ReservationCategory.Client
+        self.poas = {}
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state['actor']
         del state['logger']
         del state['slice']
         del state['approved']
@@ -200,14 +202,15 @@
         del state['expired']
         del state['pending_recover']
         del state['state_transition']
         del state['service_pending']
         del state['suggested']
         del state['thread_lock']
         del state['policy']
+        del state['poas']
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
         self.actor = None
         self.logger = None
         self.slice = None
@@ -218,14 +221,15 @@
         self.expired = False
         self.pending_recover = False
         self.state_transition = False
         self.service_pending = ReservationPendingStates.None_
         self.policy = None
 
         self.suggested = True
+        self.poas = {}
         self.thread_lock = threading.Lock()
 
     def restore(self, *, actor: ABCActorMixin, slice_obj: ABCSlice):
         """
         Must be invoked after creating reservation from unpickling
         """
         super().restore(actor=actor, slice_obj=slice_obj)
@@ -1095,14 +1099,24 @@
         return ret_val
 
     def probe_pending(self):
         # Process join state to complete or restart join-related operations for Controller
         if self.joinstate != JoinState.NoJoin:
             self.probe_join_state()
         else:
+            if self.is_active() and self.pending_state == ReservationPendingStates.PrimingPoa:
+                from fabric_cf.actor.core.container.globals import GlobalsSingleton
+                if self.exceeds_timeout(timeout=GlobalsSingleton.get().RPC_TIMEOUT):
+                    self.logger.info(f"Res# {self.get_reservation_id()} POA timeout! "
+                                     f"No response received in {GlobalsSingleton.get().RPC_TIMEOUT} seconds!")
+
+                    self.transition(prefix="POA timeout", state=self.state,
+                                    pending=ReservationPendingStates.None_)
+                    self.probe_pending_poa()
+
             # Handle pending response for a Redeem or Ticket from AM or broker respectively
             # This happens usually in case of Kafka Message Timeout
             # To avoid the slice from being stuck in Configuring state
             # Close the reservation - send Close to AM and relinquish to Broker
             # Timeout is configurable
             if self.pending_state == ReservationPendingStates.Redeeming or \
                     self.pending_state == ReservationPendingStates.Ticketing:
@@ -1769,15 +1783,16 @@
             sliver = self.requested_resources.sliver
 
         if sliver is not None:
             self.update_slice_graph(sliver=self.requested_resources.sliver)
 
     @staticmethod
     def __remove_special_characters(message: str) -> str:
-        message = re.sub('(\\\\r\\\\n|[%!{}\'\"])', '', message)
+        message = re.sub('(\\\\t\\\\r\\\\n|[%!{}\'\"])', '', message)
+        message = message.replace("\\", "")
         return message
 
     def update_slice_graph(self, *, sliver: BaseSliver):
         """
         Update ASM with Sliver information
         :param sliver: sliver
         :return:
@@ -1812,14 +1827,83 @@
             self.logger.error(traceback.format_exc())
         #self.logger.info(f"ASM TIME: {time.time() - begin:.0f}")
 
     def mark_close_by_ticket_review(self, *, update_data: UpdateData):
         if self.last_ticket_update is not None:
             self.last_ticket_update.absorb(other=update_data)
 
+    def poa(self, *, poa: Poa):
+        """
+        POA triggered by Orchestrator; Send to Authority
+        @param poa
+        """
+        # Not permitted if there is a pending operation.
+        self.nothing_pending()
+
+        # POA already processed
+        if poa.get_poa_id() in self.poas:
+            self.logger.error(f"POA {poa.get_poa_id()} has already been processed!")
+            return
+
+        # Move the reservation to PrimingPoa state
+        if self.state == ReservationStates.Active:
+            self.transition(prefix="performing poa", state=ReservationStates.Active,
+                            pending=ReservationPendingStates.PrimingPoa)
+            # Trigger POA to the Authority
+            poa.send_poa_to_authority()
+        else:
+            msg = f"Wrong state to initiate POA: {self.state}"
+            poa.fail(message=msg)
+            self.error(err=msg)
+
+        # Add POA
+        self.poas[poa.get_poa_id()] = poa
+
+    def probe_pending_poa(self):
+        """
+        Probe Pending POAs and mark them failed due to timeout
+        """
+        try:
+            failed_poas = []
+            for poa_id, poa in self.poas.items():
+                if poa.is_issued():
+                    poa.fail(message="POA timeout")
+                    failed_poas.append(poa_id)
+                self.actor.get_plugin().get_database().update_poa(poa=poa)
+            for poa_id in failed_poas:
+                if poa_id in self.poas:
+                    self.poas.pop(poa_id)
+        except Exception as e:
+            self.logger.error(f"Error occurred during probe POA - {e}", stack_info=True)
+
+    def poa_info(self, *, incoming: Poa):
+        """
+        Accept POA Result response back from the Authority
+        """
+        try:
+            if incoming is None:
+                return
+
+            # Find the target POA
+            target = self.poas.get(incoming.poa_id)
+
+            # Return if target is not found
+            if target is None:
+                self.logger.error(f"POA Request# {incoming.poa_id} not found, Ignoring POA response {incoming}")
+                return
+
+            self.transition(prefix=f"POA {incoming.poa_id} completed", state=self.state,
+                            pending=ReservationPendingStates.None_)
+
+            # Accept POA response from Authority
+            target.accept_poa_info(incoming=incoming)
+            self.actor.get_plugin().get_database().update_poa(poa=target)
+        except Exception as e:
+            self.logger.error(f"Error occurred during processing POA Info - {e}", stack_info=True)
+
 
 class ClientReservationFactory:
     """
     Factory class for creating client reservations
     """
     @staticmethod
     def create(*, rid: ID, resources: ResourceSet = None, term: Term = None, slice_object: ABCSlice = None,
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_server.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/reservation_server.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/reservation_states.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/reservation_states.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,17 @@
     Blocked = 18
     Closing = 19
     Probing = 20
     ClosingJoining = 21
     ModifyingLease = 22
     AbsorbUpdate = 23
     SendUpdate = 24
-    Unknown = 25
+    PrimingPoa = 25
+    WaitingPoaResponse = 26
+    Unknown = 27
 
     def __repr__(self):
         return self.name
 
     def __str__(self):
         return self.name
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/resource_set.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/resource_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,22 +29,23 @@
 
 from fim.slivers.base_sliver import BaseSliver
 
 from fabric_cf.actor.core.apis.abc_base_plugin import ABCBasePlugin
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import ResourcesException
-from fabric_cf.actor.core.util.utils import sliver_to_str
+
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.time.term import Term
     from fabric_cf.actor.core.util.id import ID
     from fabric_cf.actor.core.util.notice import Notice
     from fabric_cf.actor.core.apis.abc_concrete_set import ABCConcreteSet
     from fabric_cf.actor.core.util.resource_type import ResourceType
+    from fabric_cf.actor.core.kernel.poa import Poa
 
 
 class ResourceSet:
     """
     ResourceSet is an abstract set of resources describing some number of
     resource units of a given type, e.g., to represent a resource request. A
     ResourceSet with an attached ConcreteSet is "concrete." The ConcreteSet binds
@@ -249,14 +250,17 @@
         """
         result = self.units
         if self.resources is not None:
             result -= self.resources.get_units()
 
         return result
 
+    def get_poa_info(self) -> dict:
+        return self.resources.get_poa_info()
+
     def get_notices(self) -> Notice:
         """
         Returns a string of notices or events pertaining to the underlying
         resources. The event notices are consumed: subsequent calls return only
         new information. May return null.
         @returns Notice
         """
@@ -542,7 +546,14 @@
         if self.resources is not None:
             self.resources.validate_outgoing()
 
     def clone(self):
         clone = ResourceSet(units=self.units, rtype=self.type, sliver=self.sliver)
         clone.resources = self.resources.clone()
         return clone
+
+    def service_poa(self, *, poa: Poa):
+        """
+        Complete service for a POA.
+        """
+        self.service_check()
+        self.resources.poa(poa=poa)
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/retry_rpc.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/retry_rpc.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/retry_rpc_event.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/retry_rpc_event.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_executor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/rpc_executor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_manager.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/rpc_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,18 +19,21 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
 import logging
 import threading
 import concurrent.futures
-import time
 import traceback
 
 from fabric_mb.message_bus.producer import AvroProducerApi
 
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
 from fabric_cf.actor.core.apis.abc_actor_proxy import ABCActorProxy
 from fabric_cf.actor.core.apis.abc_authority_proxy import ABCAuthorityProxy
@@ -61,14 +64,17 @@
 from fabric_cf.actor.core.util.id import ID
 from fabric_cf.actor.core.util.kernel_timer import KernelTimer
 from fabric_cf.actor.core.util.rpc_exception import RPCException, RPCError
 from fabric_cf.actor.core.util.update_data import UpdateData
 from fabric_cf.actor.core.util.utils import sliver_to_str
 from fabric_cf.actor.security.auth_token import AuthToken
 
+if TYPE_CHECKING:
+    from fabric_cf.actor.core.kernel.poa import Poa
+
 
 class RPCManager:
     """
     Class responsible for message exchange across Kafka
     """
     CLAIM_TIMEOUT_SECONDS = 240
     QUERY_TIMEOUT_SECONDS = 240
@@ -168,23 +174,33 @@
         self.validate(reservation=reservation, check_requested=True)
         self.do_redeem(actor=reservation.get_actor(), proxy=reservation.get_authority(),
                        reservation=reservation, callback=reservation.get_client_callback_proxy(),
                        caller=reservation.get_slice().get_owner())
 
     def extend_lease(self, *, proxy: ABCAuthorityProxy, reservation: ABCControllerReservation, caller: AuthToken):
         self.validate(reservation=reservation, check_requested=True)
-        self.do_extend_lease(actor=reservation.get_actor(), proxy=reservation.get_authority(),
-                             reservation=reservation, callback=reservation.get_client_callback_proxy(),
-                             caller=reservation.get_slice().get_owner())
+        self.do_extend_lease(actor=reservation.get_actor(), proxy=proxy, caller=caller,
+                             reservation=reservation, callback=reservation.get_client_callback_proxy())
 
     def modify_lease(self, *, proxy: ABCAuthorityProxy, reservation: ABCControllerReservation, caller: AuthToken):
         self.validate(reservation=reservation, check_requested=True)
-        self.do_modify_lease(actor=reservation.get_actor(), proxy=reservation.get_authority(),
-                             reservation=reservation, callback=reservation.get_client_callback_proxy(),
-                             caller=reservation.get_slice().get_owner())
+        self.do_modify_lease(actor=reservation.get_actor(), proxy=proxy, caller=caller,
+                             reservation=reservation, callback=reservation.get_client_callback_proxy())
+
+    def poa(self, *, proxy: ABCAuthorityProxy, callback: ABCControllerCallbackProxy, caller: AuthToken, poa: Poa):
+        self.do_poa(actor=poa.get_actor(), proxy=proxy,callback=callback, caller=caller, poa=poa)
+
+    def poa_info(self, *, reservation: ABCAuthorityReservation, poa: Poa):
+        callback = Proxy.get_callback(actor=reservation.get_actor(), protocol=reservation.get_callback().get_type())
+        if callback is None:
+            raise RPCException(message=Constants.NOT_SPECIFIED_PREFIX.format("callback"))
+
+        # Send POA Result back to Orchestrator
+        self.do_poa_info(actor=reservation.get_actor(), proxy=reservation.get_callback(),
+                         poa=poa, callback=callback, caller=reservation.get_actor().get_identity())
 
     def close(self, *, reservation: ABCControllerReservation):
         self.validate(reservation=reservation)
         self.do_close(actor=reservation.get_actor(), proxy=reservation.get_authority(),
                       reservation=reservation, callback=reservation.get_client_callback_proxy(),
                       caller=reservation.get_slice().get_owner())
 
@@ -377,14 +393,31 @@
         state = proxy.prepare_modify_lease(reservation=reservation, callback=callback, caller=caller)
         state.set_caller(caller=caller)
         state.set_type(rtype=RPCRequestType.ModifyLease)
         rpc = RPCRequest(request=state, actor=actor, proxy=proxy, reservation=reservation,
                          sequence=reservation.get_lease_sequence_out())
         self.enqueue(rpc=rpc)
 
+    def do_poa(self, *, actor: ABCActorMixin, proxy: ABCAuthorityProxy, callback: ABCControllerCallbackProxy,
+               caller: AuthToken, poa: Poa):
+        state = proxy.prepare_poa(callback=callback, caller=caller, poa=poa)
+        state.set_caller(caller=caller)
+        state.set_type(rtype=RPCRequestType.Poa)
+        rpc = RPCRequest(request=state, actor=actor, proxy=proxy, poa=poa,
+                         sequence=poa.get_poa_sequence_out())
+        self.enqueue(rpc=rpc)
+
+    def do_poa_info(self, *, actor: ABCActorMixin, proxy: ABCControllerCallbackProxy, poa: Poa,
+                    callback: ABCCallbackProxy, caller: AuthToken):
+        state = proxy.prepare_poa_result(poa=poa,callback=callback, caller=caller)
+        state.set_caller(caller=caller)
+        state.set_type(rtype=RPCRequestType.PoaInfo)
+        rpc = RPCRequest(request=state, actor=actor, proxy=proxy, poa=poa, sequence=poa.get_poa_sequence_out())
+        self.enqueue(rpc=rpc)
+
     def do_close(self, *, actor: ABCActorMixin, proxy: ABCAuthorityProxy, reservation: ABCControllerReservation,
                  callback: ABCControllerCallbackProxy, caller: AuthToken):
         state = proxy.prepare_close(reservation=reservation, callback=callback, caller=caller)
         state.set_caller(caller=caller)
         state.set_type(rtype=RPCRequestType.Close)
         rpc = RPCRequest(request=state, actor=actor, proxy=proxy, reservation=reservation,
                          sequence=reservation.get_lease_sequence_out())
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_manager_singleton.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/rpc_manager_singleton.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_request.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/rpc_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,39 +19,42 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
+
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.apis.abc_proxy import ABCProxy
 from fabric_cf.actor.core.apis.abc_rpc_request_state import ABCRPCRequestState
 from fabric_cf.actor.core.apis.abc_response_handler import ABCResponseHandler
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.kernel.rpc_request_type import RPCRequestType
 
 
 class RPCRequest:
     """
     Represents a RPC request being sent across Kafka
     """
-    def __init__(self, *, request: ABCRPCRequestState, actor: ABCActorMixin, proxy: ABCProxy,
+    def __init__(self, *, request: ABCRPCRequestState, actor: ABCActorMixin, proxy: ABCProxy, poa: Poa = None,
                  sequence: int = None, handler: ABCResponseHandler = None, reservation: ABCReservationMixin = None,
                  delegation: ABCDelegation = None):
         self.request = request
         self.actor = actor
         self.proxy = proxy
         self.reservation = reservation
         self.delegation = delegation
         self.sequence = sequence
         self.handler = handler
         self.retry_count = 0
         self.timer = None
+        self.poa = poa
 
     def get_actor(self) -> ABCActorMixin:
         """
         Get actor
         @return actor
         """
         return self.actor
@@ -66,14 +69,17 @@
     def get_reservation(self) -> ABCReservationMixin:
         """
         Get Reservation
         @return reservation
         """
         return self.reservation
 
+    def get_poa(self) -> Poa:
+        return self.poa
+
     def get_handler(self) -> ABCResponseHandler:
         """
         Get Response Handler
         @return response handler
         """
         return self.handler
 
@@ -88,13 +94,17 @@
         """
         Cancel a timer if started
         """
         if self.timer is not None:
             from fabric_cf.actor.core.container.globals import GlobalsSingleton
             GlobalsSingleton.get().timer_scheduler.cancel(self.timer)
 
-    def get(self) -> ABCReservationMixin or ABCDelegation:
+    def get(self) -> ABCReservationMixin or ABCDelegation or Poa:
         if self.reservation is not None:
             return self.reservation
 
         if self.delegation is not None:
             return self.delegation
+
+        if self.poa is not None:
+            return self.poa
+
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/rpc_request_type.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/rpc_request_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,10 +40,12 @@
     Query = 13
     QueryResult = 14
     FailedRPC = 15
     UpdateDelegation = 16
     ClaimDelegation = 17
     ReclaimDelegation = 18
     DeliveryAck = 19
+    Poa = 20
+    PoaInfo = 21
 
     def __str__(self):
         return self.name
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/sequence_comparison_codes.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/sequence_comparison_codes.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice_state_machine.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/slice_state_machine.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/slice_table.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/slice_table.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/kernel/tick.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/kernel/tick.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/actor_management_object.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/actor_management_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,19 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from datetime import datetime, timezone
 from typing import TYPE_CHECKING, List, Dict, Tuple
 
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
+from fabric_mb.message_bus.messages.poa_info_avro import PoaInfoAvro
 from fabric_mb.message_bus.messages.reservation_mng import ReservationMng
 from fabric_mb.message_bus.messages.result_delegation_avro import ResultDelegationAvro
+from fabric_mb.message_bus.messages.result_poa_avro import ResultPoaAvro
 from fabric_mb.message_bus.messages.result_reservation_avro import ResultReservationAvro
 from fabric_mb.message_bus.messages.result_reservation_state_avro import ResultReservationStateAvro
 from fabric_mb.message_bus.messages.result_sites_avro import ResultSitesAvro
 from fabric_mb.message_bus.messages.result_string_avro import ResultStringAvro
 from fabric_mb.message_bus.messages.result_avro import ResultAvro
 from fabric_mb.message_bus.messages.result_slice_avro import ResultSliceAvro
 from fabric_mb.message_bus.messages.slice_avro import SliceAvro
@@ -513,16 +516,14 @@
     def get_actor(self) -> ABCActorMixin:
         return self.actor
 
     def get_actor_name(self) -> str or None:
         if self.actor is not None:
             return self.actor.get_name()
 
-        return None
-
     def update_reservation(self, *, reservation: ReservationMng, caller: AuthToken) -> ResultAvro:
         result = ResultAvro()
         if reservation is None or caller is None:
             result.set_code(ErrorCodes.ErrorInvalidArguments.value)
             result.set_message(ErrorCodes.ErrorInvalidArguments.interpret())
             return result
 
@@ -778,7 +779,47 @@
         except Exception as e:
             self.logger.error("remove_delegation: {}".format(e))
             result.set_code(ErrorCodes.ErrorInternalError.value)
             result.set_message(ErrorCodes.ErrorInternalError.interpret(exception=e))
             result = ManagementObject.set_exception_details(result=result, e=e)
 
         return result
+
+    def get_poas(self, *, caller: AuthToken, states: List[int] = None,
+                 slice_id: ID = None, rid: ID = None, email: str = None,
+                 poa_id: str = None, project_id: str = None) -> ResultPoaAvro:
+
+        result = ResultPoaAvro()
+        result.status = ResultAvro()
+
+        if caller is None:
+            result.status.set_code(ErrorCodes.ErrorInvalidArguments.value)
+            result.status.set_message(ErrorCodes.ErrorInvalidArguments.interpret())
+            return result
+
+        try:
+            poa_list = None
+            try:
+                poa_list = self.db.get_poas(poa_id=poa_id, sliver_id=rid, email=email, project_id=project_id)
+            except Exception as e:
+                self.logger.error("get_poas:db access {}".format(e))
+                result.status.set_code(ErrorCodes.ErrorDatabaseError.value)
+                result.status.set_message(ErrorCodes.ErrorDatabaseError.interpret(exception=e))
+                result.status = ManagementObject.set_exception_details(result=result.status, e=e)
+
+            if poa_list is not None:
+                result.poas = []
+                for p in poa_list:
+                    poa_info_avro = Translate.translate_poa_to_poa_info_avro(poa=p)
+                    result.poas.append(poa_info_avro)
+
+        except ReservationNotFoundException as e:
+            self.logger.error("get_poas: {}".format(e))
+            result.status.set_code(ErrorCodes.ErrorNoSuchReservation.value)
+            result.status.set_message(e.text)
+        except Exception as e:
+            self.logger.error("get_poas: {}".format(e))
+            result.status.set_code(ErrorCodes.ErrorInternalError.value)
+            result.status.set_message(ErrorCodes.ErrorInternalError.interpret(exception=e))
+            result.status = ManagementObject.set_exception_details(result=result.status, e=e)
+
+        return result
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/authority_management_object.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/authority_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/broker_management_object.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/broker_management_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from datetime import datetime
 from typing import TYPE_CHECKING, List
 
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fabric_mb.message_bus.messages.proxy_avro import ProxyAvro
 from fabric_mb.message_bus.messages.reservation_predecessor_avro import ReservationPredecessorAvro
 from fabric_mb.message_bus.messages.result_delegation_avro import ResultDelegationAvro
 from fim.slivers.base_sliver import BaseSliver
 from fim.user import GraphFormat
 
 from fabric_cf.actor.core.common.constants import Constants
@@ -118,8 +119,14 @@
         return self.client_helper.extend_reservation(reservation=reservation, new_end_time=new_end_time,
                                                      sliver=sliver, caller=caller, dependencies=dependencies)
 
     def claim_delegations(self, *, broker: ID, did: str, caller: AuthToken) -> ResultDelegationAvro:
         return self.client_helper.claim_delegations(broker=broker, did=did, caller=caller)
 
     def reclaim_delegations(self, *, broker: ID, did: str, caller: AuthToken) -> ResultDelegationAvro:
-        return self.client_helper.reclaim_delegations(broker=broker, did=did, caller=caller)
+        return self.client_helper.reclaim_delegations(broker=broker, did=did, caller=caller)
+
+    def modify_reservation(self, *, rid: ID, modified_sliver: BaseSliver, caller: AuthToken) -> ResultAvro:
+        return self.client_helper.modify_reservation(rid=rid, modified_sliver=modified_sliver, caller=caller)
+
+    def poa(self, *, poa: PoaAvro, caller: AuthToken) -> ResultAvro:
+        return self.client_helper.poa(poa=poa, caller=caller)
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/client_actor_management_object_helper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/client_actor_management_object_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from __future__ import annotations
 
 import traceback
 from datetime import datetime
 from typing import TYPE_CHECKING, List
 
 from fabric_mb.message_bus.messages.lease_reservation_avro import LeaseReservationAvro
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fabric_mb.message_bus.messages.reservation_predecessor_avro import ReservationPredecessorAvro
 from fabric_mb.message_bus.messages.result_delegation_avro import ResultDelegationAvro
 from fabric_mb.message_bus.messages.result_broker_query_model_avro import ResultBrokerQueryModelAvro
 from fabric_mb.message_bus.messages.result_proxy_avro import ResultProxyAvro
 from fabric_mb.message_bus.messages.result_string_avro import ResultStringAvro
 from fabric_mb.message_bus.messages.result_strings_avro import ResultStringsAvro
 from fabric_mb.message_bus.messages.result_avro import ResultAvro
@@ -586,7 +587,45 @@
             self.logger.error(traceback.format_exc())
             self.logger.error("reclaim_delegations {}".format(e))
             result.status.set_code(ErrorCodes.ErrorInternalError.value)
             result.status.set_message(ErrorCodes.ErrorInternalError.interpret(exception=e))
             result.status = ManagementObject.set_exception_details(result=result.status, e=e)
 
         return result
+
+    def poa(self, *, poa: PoaAvro, caller: AuthToken) -> ResultAvro:
+        result = ResultAvro()
+
+        if poa.rid is None or poa.operation is None:
+            result.set_code(ErrorCodes.ErrorInvalidArguments.value)
+            result.set_message(ErrorCodes.ErrorInvalidArguments.interpret())
+            return result
+
+        self.logger.debug(f"reservation: {poa.rid} | operation = {poa.operation} | "
+                          f"vcpu_cpu_map = {poa.vcpu_cpu_map} | node_set = {poa.node_set}")
+        try:
+
+            class Runner(ABCActorRunnable):
+                def __init__(self, *, actor: ABCClientActor):
+                    self.actor = actor
+
+                def run(self):
+                    result = ResultAvro()
+                    r = self.actor.get_reservation(rid=ID(uid=poa.rid))
+                    if r is None:
+                        result.set_code(ErrorCodes.ErrorNoSuchReservation.value)
+                        result.set_message(ErrorCodes.ErrorNoSuchReservation.interpret())
+                        return result
+
+                    poa_obj = Translate.translate_poa_avro_to_poa(poa_avro=poa)
+
+                    self.actor.poa(poa=poa_obj)
+
+                    return result
+            result = self.client.execute_on_actor_thread_and_wait(runnable=Runner(actor=self.client))
+        except Exception as e:
+            self.logger.error("poa {}".format(e))
+            result.set_code(ErrorCodes.ErrorInternalError.value)
+            result.set_message(ErrorCodes.ErrorInternalError.interpret(exception=e))
+            result = ManagementObject.set_exception_details(result=result, e=e)
+
+        return result
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/container_management_object.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/container_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/controller_management_object.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/controller_management_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from datetime import datetime
 from typing import TYPE_CHECKING, List
 
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fabric_mb.message_bus.messages.reservation_predecessor_avro import ReservationPredecessorAvro
 from fabric_mb.message_bus.messages.result_delegation_avro import ResultDelegationAvro
 from fabric_mb.message_bus.messages.result_units_avro import ResultUnitsAvro
 from fabric_mb.message_bus.messages.result_avro import ResultAvro
 from fim.slivers.base_sliver import BaseSliver
 from fim.user import GraphFormat
 
@@ -121,14 +122,17 @@
                            caller: AuthToken, dependencies: List[ReservationPredecessorAvro] = None) -> ResultAvro:
         return self.client_helper.extend_reservation(reservation=reservation, new_end_time=new_end_time, 
                                                      sliver=sliver, caller=caller, dependencies=dependencies)
 
     def modify_reservation(self, *, rid: ID, modified_sliver: BaseSliver, caller: AuthToken) -> ResultAvro:
         return self.client_helper.modify_reservation(rid=rid, modified_sliver=modified_sliver, caller=caller)
 
+    def poa(self, *, poa: PoaAvro, caller: AuthToken) -> ResultAvro:
+        return self.client_helper.poa(poa=poa, caller=caller)
+
     def get_reservation_units(self, *, caller: AuthToken, rid: ID) -> ResultUnitsAvro:
         result = ResultUnitsAvro()
         result.status = ResultAvro()
 
         if caller is None:
             result.status.set_code(ErrorCodes.ErrorInvalidArguments.value)
             result.status.set_message(ErrorCodes.ErrorInvalidArguments.interpret())
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/converter.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/converter.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/error.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/error.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 from fabric_mb.message_bus.messages.close_delegations_avro import CloseDelegationsAvro
 from fabric_mb.message_bus.messages.close_reservations_avro import CloseReservationsAvro
 from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
 from fabric_mb.message_bus.messages.get_delegations_avro import GetDelegationsAvro
 from fabric_mb.message_bus.messages.get_sites_request_avro import GetSitesRequestAvro
 from fabric_mb.message_bus.messages.maintenance_request_avro import MaintenanceRequestAvro
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
+from fabric_mb.message_bus.messages.poa_info_avro import PoaInfoAvro
 from fabric_mb.message_bus.messages.remove_delegation_avro import RemoveDelegationAvro
 from fabric_mb.message_bus.messages.reservation_state_avro import ReservationStateAvro
 from fabric_mb.message_bus.messages.get_reservations_state_request_avro import GetReservationsStateRequestAvro
 from fabric_mb.message_bus.messages.add_slice_avro import AddSliceAvro
 from fabric_mb.message_bus.messages.get_reservations_request_avro import GetReservationsRequestAvro
 from fabric_mb.message_bus.messages.get_slices_request_avro import GetSlicesRequestAvro
 from fabric_mb.message_bus.messages.remove_reservation_avro import RemoveReservationAvro
@@ -131,15 +133,14 @@
         request = self.fill_request_by_id_message(request=request, slice_id=slice_id,
                                                   states=states, email=email, rid=rid,
                                                   type=type, site=site)
         status, response = self.send_request(request)
 
         if status.code == 0:
             return response.reservations
-        return None
 
     def get_sites(self, *, site: str) -> List[SiteAvro] or None:
         request = GetSitesRequestAvro()
         request = self.fill_request_by_id_message(request=request, site=site)
         status, response = self.send_request(request)
 
         if status.code == 0:
@@ -151,15 +152,14 @@
         request = GetDelegationsAvro()
         request = self.fill_request_by_id_message(request=request, slice_id=slice_id,
                                                   states=states, delegation_id=delegation_id)
         status, response = self.send_request(request)
 
         if status.code == 0:
             return response.delegations
-        return None
 
     def remove_reservation(self, *, rid: ID) -> bool:
         request = RemoveReservationAvro()
         request = self.fill_request_by_id_message(request=request, rid=rid)
         status, response = self.send_request(request)
 
         return status.code == 0
@@ -201,16 +201,14 @@
             request.reservation_ids.append(str(r))
 
         status, response = self.send_request(request)
 
         if status.code == 0:
             return response.reservation_states
 
-        return None
-
     def clone(self):
         return KafkaActor(guid=self.management_id,
                           kafka_topic=self.kafka_topic,
                           auth=self.auth, logger=self.logger,
                           message_processor=self.message_processor,
                           producer=self.producer)
 
@@ -226,7 +224,11 @@
 
     def close_delegation(self, *, did: str) -> bool:
         request = CloseDelegationsAvro()
         request = self.fill_request_by_id_message(request=request, delegation_id=did)
         status, response = self.send_request(request)
 
         return status.code == 0
+
+    def get_poas(self, *, states: List[int] = None, slice_id: ID = None, rid: ID = None,
+                 email: str = None, poa_id: str = None, project_id: str = None) -> List[PoaInfoAvro]:
+        raise NotImplemented
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_authority.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_broker.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_container.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 from datetime import datetime
 from typing import List
 
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fabric_mb.message_bus.messages.reservation_mng import ReservationMng
 from fabric_mb.message_bus.messages.reservation_predecessor_avro import ReservationPredecessorAvro
 from fabric_mb.message_bus.messages.ticket_reservation_avro import TicketReservationAvro
 from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
 from fabric_mb.message_bus.messages.broker_query_model_avro import BrokerQueryModelAvro
 from fabric_mb.message_bus.messages.get_actors_request_avro import GetActorsRequestAvro
 from fabric_mb.message_bus.messages.proxy_avro import ProxyAvro
@@ -105,7 +106,10 @@
 
     def extend_reservation(self, *, reservation: ID, new_end_time: datetime, sliver: BaseSliver,
                            dependencies: List[ReservationPredecessorAvro] = None) -> bool:
         raise ManageException(Constants.NOT_IMPLEMENTED)
 
     def modify_reservation(self, *, rid: ID, modify_properties: dict) -> bool:
         raise ManageException(Constants.NOT_IMPLEMENTED)
+
+    def poa(self, *, poa: PoaAvro) -> bool:
+        raise ManageException(Constants.NOT_IMPLEMENTED)
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_mgmt_message_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/kafka_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_authority_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_broker_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_client_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_controller_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_server_actor_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/kafka/services/kafka_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/kafka/services/kafka_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_actor.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
 import traceback
 from typing import TYPE_CHECKING, List, Tuple, Dict
 
 from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
+from fabric_mb.message_bus.messages.poa_info_avro import PoaInfoAvro
 from fabric_mb.message_bus.messages.site_avro import SiteAvro
 
 from fabric_cf.actor.core.common.exceptions import ManageException
 from fabric_cf.actor.core.container.maintenance import Site
 from fabric_cf.actor.core.manage.actor_management_object import ActorManagementObject
 from fabric_cf.actor.core.apis.abc_mgmt_actor import ABCMgmtActor
 from fabric_cf.actor.core.manage.local.local_proxy import LocalProxy
@@ -93,20 +95,18 @@
 
             if result.status.get_code() == 0:
                 return result.reservations
 
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def get_sites(self, *, site: str) -> List[SiteAvro] or None:
         self.clear_last()
         try:
-            result = self.manager.get_sites(site=site)
+            result = self.manager.get_sites(site=site, caller=self.auth)
             self.last_status = result.status
 
             if result.status.get_code() == 0:
                 return result.sites
 
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
@@ -153,16 +153,14 @@
 
             if self.last_status.get_code() == 0 and result.get_result() is not None:
                 return ID(uid=result.get_result())
 
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def update_slice(self, *, slice_obj: SliceAvro, modify_state: bool = False) -> bool:
         self.clear_last()
         try:
             result = self.manager.update_slice(slice_mng=slice_obj, caller=self.auth, modify_state=modify_state)
             self.last_status = result
 
             if self.last_status.get_code() == 0:
@@ -224,31 +222,27 @@
 
             if result.status.get_code() == 0:
                 return result.reservation_states
 
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def get_delegations(self, *, slice_id: ID = None, states: List[int] = None,
                         delegation_id: str = None) -> List[DelegationAvro]:
         self.clear_last()
         try:
             result = self.manager.get_delegations(caller=self.auth, slice_id=slice_id, did=delegation_id)
             self.last_status = result.status
 
             if result.status.get_code() == 0:
                 return result.reservations
 
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def close_delegation(self, *, did: str) -> bool:
         self.clear_last()
         try:
             result = self.manager.close_delegation(caller=self.auth, did=did)
             self.last_status = result
 
             return result.get_code() == 0
@@ -278,8 +272,22 @@
         return self.manager.is_site_in_maintenance(site_name=site_name)
 
     def is_slice_provisioning_allowed(self, *, project: str, email: str) -> bool:
         return self.manager.is_slice_provisioning_allowed(project=project, email=email)
 
     def is_sliver_provisioning_allowed(self, *, project: str, email: str, site: str,
                                        worker: str) -> Tuple[bool, str or None]:
-        return self.manager.is_sliver_provisioning_allowed(project=project, email=email, site=site, worker=worker)
+        return self.manager.is_sliver_provisioning_allowed(project=project, email=email, site=site, worker=worker)
+
+    def get_poas(self, *, states: List[int] = None, slice_id: ID = None, rid: ID = None,
+                 email: str = None, poa_id: str = None, project_id: str = None) -> List[PoaInfoAvro]:
+        self.clear_last()
+        try:
+            result = self.manager.get_poas(caller=self.auth, states=states, slice_id=slice_id, rid=rid,
+                                           email=email, poa_id=poa_id, project_id=project_id)
+            self.last_status = result.status
+
+            if result.status.get_code() == 0:
+                return result.poas
+
+        except Exception as e:
+            self.on_exception(e=e, traceback_str=traceback.format_exc())
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_authority.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_authority.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_broker.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_container.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_container.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,37 +27,37 @@
 
 import traceback
 from datetime import datetime
 from typing import TYPE_CHECKING, List
 
 from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
 from fabric_mb.message_bus.messages.broker_query_model_avro import BrokerQueryModelAvro
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fabric_mb.message_bus.messages.reservation_predecessor_avro import ReservationPredecessorAvro
 from fabric_mb.message_bus.messages.ticket_reservation_avro import TicketReservationAvro
 from fabric_mb.message_bus.messages.unit_avro import UnitAvro
 from fim.slivers.base_sliver import BaseSliver
 from fim.user import GraphFormat
 
-from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import ManageException
 from fabric_cf.actor.core.manage.controller_management_object import ControllerManagementObject
 from fabric_cf.actor.core.apis.abc_mgmt_controller_mixin import ABCMgmtControllerMixin
 from fabric_cf.actor.core.manage.local.local_actor import LocalActor
 from fabric_cf.actor.core.util.id import ID
 
 if TYPE_CHECKING:
     from fabric_mb.message_bus.messages.proxy_avro import ProxyAvro
     from fabric_mb.message_bus.messages.reservation_mng import ReservationMng
 
-    from fabric_cf.actor.core.manage.management_object import ManagementObject
+    from fabric_cf.actor.core.apis.abc_client_actor_management_object import ABCClientActorManagementObject
     from fabric_cf.actor.security.auth_token import AuthToken
 
 
 class LocalController(LocalActor, ABCMgmtControllerMixin):
-    def __init__(self, *, manager: ManagementObject, auth: AuthToken):
+    def __init__(self, *, manager: ABCClientActorManagementObject, auth: AuthToken):
         super().__init__(manager=manager, auth=auth)
 
         if not isinstance(manager, ControllerManagementObject):
             raise ManageException("Invalid manager object. Required: {}".format(type(ControllerManagementObject)))
 
     def add_broker(self, *, broker: ProxyAvro) -> bool:
         self.clear_last()
@@ -89,82 +89,70 @@
             result = self.manager.get_brokers(caller=self.auth, broker_id=broker)
             self.last_status = result.status
             if result.status.get_code() == 0:
                 return result.proxies
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def get_broker_query_model(self, *, broker: ID, id_token: str, level: int,
                                graph_format: GraphFormat) -> BrokerQueryModelAvro:
         self.clear_last()
         try:
             result = self.manager.get_broker_query_model(broker=broker, caller=self.auth, id_token=id_token,
                                                          level=level, graph_format=graph_format)
             self.last_status = result.status
 
             if result.status.get_code() == 0:
                 return result.model
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def claim_delegations(self, *, broker: ID, did: ID, id_token: str = None) -> DelegationAvro:
         self.clear_last()
         try:
             result = self.manager.claim_delegations(broker=broker, did=did, caller=self.auth)
             self.last_status = result.status
 
             if result.status.get_code() == 0:
                 return self.get_first(result_list=result.delegations)
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def reclaim_delegations(self, *, broker: ID, did: ID, id_token: str = None) -> DelegationAvro:
         self.clear_last()
         try:
             result = self.manager.reclaim_delegations(broker=broker, did=did, caller=self.auth)
             self.last_status = result.status
 
             if result.status.get_code() == 0:
                 return self.get_first(result_list=result.delegations)
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def get_reservation_units(self, *, rid: ID, id_token: str = None) -> List[UnitAvro]:
         self.clear_last()
         try:
             result = self.manager.get_reservation_units(caller=self.auth, rid=rid)
             self.last_status = result.status
             if result.status.get_code() == 0:
                 return result.units
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def add_reservation(self, *, reservation: TicketReservationAvro) -> ID:
         self.clear_last()
         try:
             result = self.manager.add_reservation(reservation=reservation, caller=self.auth)
             self.last_status = result.status
 
             if result.status.get_code() == 0:
                 return ID(uid=result.get_result())
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def add_reservations(self, *, reservations: List[TicketReservationAvro]) -> List[ID]:
         self.clear_last()
         try:
             result = self.manager.add_reservations(reservations=reservations, caller=self.auth)
             self.last_status = result.status
 
             if result.status.get_code() == 0:
@@ -172,16 +160,14 @@
                 for r in result.result:
                     rids.append(ID(uid=r))
 
                 return rids
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
-        return None
-
     def demand_reservation_rid(self, *, rid: ID) -> bool:
         self.clear_last()
         try:
             result = self.manager.demand_reservation_rid(rid=rid, caller=self.auth)
             self.last_status = result
 
             return result.get_code() == 0
@@ -227,7 +213,19 @@
             self.last_status = result
 
             return result.get_code() == 0
         except Exception as e:
             self.on_exception(e=e, traceback_str=traceback.format_exc())
 
         return False
+
+    def poa(self, *, poa: PoaAvro) -> bool:
+        self.clear_last()
+        try:
+            result = self.manager.poa(poa=poa, caller=self.auth)
+            self.last_status = result
+
+            return result.get_code() == 0
+        except Exception as e:
+            self.on_exception(e=e, traceback_str=traceback.format_exc())
+
+        return False
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,25 +24,26 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 from fabric_mb.message_bus.messages.result_avro import ResultAvro
 
+from fabric_cf.actor.core.apis.abc_actor_management_object import ABCActorManagementObject
 from fabric_cf.actor.core.common.constants import ErrorCodes
 from fabric_cf.actor.core.manage.error import Error
 from fabric_cf.actor.core.apis.abc_component import ABCComponent
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.manage.management_object import ManagementObject
     from fabric_cf.actor.security.auth_token import AuthToken
 
 
 class LocalProxy(ABCComponent):
-    def __init__(self, *, manager: ManagementObject, auth: AuthToken):
+    def __init__(self, *, manager: ABCActorManagementObject, auth: AuthToken):
         self.manager = manager
         self.auth = auth
         self.last_status = None
         self.last_exception = None
 
     def clear_last(self):
         self.last_exception = None
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/local/local_server_actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/local/local_server_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_object.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_object_manager.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/management_object_manager.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/management_utils.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/management_utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/client_mng.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/client_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/event_mng.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/event_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/protocol_proxy_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/result_client_mng.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/result_client_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/messages/result_event_mng.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/messages/result_event_mng.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/proxy_protocol_descriptor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/manage/server_actor_management_object.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/manage/server_actor_management_object.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/base_plugin.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/base_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,16 @@
 
         if target == Constants.TARGET_CREATE:
             self.process_create_complete(unit=unit, properties=properties)
         elif target == Constants.TARGET_DELETE:
             self.process_delete_complete(unit=unit, properties=properties)
         elif target == Constants.TARGET_MODIFY:
             self.process_modify_complete(unit=unit, properties=properties)
+        elif target == Constants.TARGET_POA:
+            self.process_poa_complete(unit=unit, properties=properties)
         else:
             unsupported = True
             self.logger.warning("Unsupported target in configurationComplete(): {}".format(target))
 
         if not unsupported:
             self.actor.get_policy().configuration_complete(action=target, token=unit,
                                                            out_properties=properties)
@@ -176,14 +178,17 @@
 
     def process_delete_complete(self, *, unit: ConfigToken, properties: dict):
         return
 
     def process_modify_complete(self, *, unit: ConfigToken, properties: dict):
         return
 
+    def process_poa_complete(self, *, unit: ConfigToken, properties: dict):
+        return
+
     def set_actor(self, *, actor: ABCActorMixin):
         self.actor = actor
 
     def set_database(self, *, db: ABCDatabase):
         self.db = db
 
     def set_logger(self, *, logger):
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/actor_database.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/db/actor_database.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,26 +24,26 @@
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import pickle
 import threading
 import time
 import traceback
 from datetime import datetime
-from typing import List
-
+from typing import List, Union
 
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin, ActorType
 from fabric_cf.actor.core.apis.abc_broker_proxy import ABCBrokerProxy
 from fabric_cf.actor.core.apis.abc_controller_reservation import ABCControllerReservation
 from fabric_cf.actor.core.apis.abc_database import ABCDatabase
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin, ReservationCategory
 from fabric_cf.actor.core.apis.abc_slice import ABCSlice
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import DatabaseException
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.kernel.slice import SliceTypes
 from fabric_cf.actor.core.plugins.handlers.configuration_mapping import ConfigurationMapping
 from fabric_cf.actor.core.container.maintenance import Site
 from fabric_cf.actor.core.util.id import ID
 from fabric_cf.actor.db.psql_database import PsqlDatabase
 
 
@@ -508,15 +508,16 @@
                                                                     delegation.get_slice_id()))
         try:
             #self.lock.acquire()
             properties = pickle.dumps(delegation)
             self.db.add_delegation(slice_id=str(delegation.get_slice_id()),
                                    dlg_graph_id=str(delegation.get_delegation_id()),
                                    dlg_state=delegation.get_state().value,
-                                   properties=properties)
+                                   properties=properties,
+                                   site=delegation.get_site())
             self.logger.debug(
                 "Delegation {} added to slice {}".format(delegation.get_delegation_id(),
                                                          delegation.get_slice_id()))
         finally:
             if self.lock.locked():
                 self.lock.release()
 
@@ -528,15 +529,16 @@
         try:
             #self.lock.acquire()
             self.logger.debug("Updating delegation {} in slice {}".format(delegation.get_delegation_id(),
                                                                           delegation.get_slice_id()))
             properties = pickle.dumps(delegation)
             self.db.update_delegation(dlg_graph_id=str(delegation.get_delegation_id()),
                                       dlg_state=delegation.get_state().value,
-                                      properties=properties)
+                                      properties=properties,
+                                      site=delegation.get_site())
         finally:
             if self.lock.locked():
                 self.lock.release()
 
     def remove_delegation(self, *, dlg_graph_id: str):
         try:
             #self.lock.acquire()
@@ -726,8 +728,86 @@
             if self.lock.locked():
                 self.lock.release()
         if cfg_map_list is not None:
             for c in cfg_map_list:
                 pickled_cfg_map = c.get(Constants.PROPERTY_PICKLE_PROPERTIES)
                 cfg_obj = pickle.loads(pickled_cfg_map)
                 result.append(cfg_obj)
-        return result
+        return result
+
+    def _load_poa_from_db(self, *, poa_dict_list: List[dict]) -> List[Poa]:
+        result = []
+        if poa_dict_list is None:
+            return result
+
+        for p in poa_dict_list:
+            pickled_poa = p.get(Constants.PROPERTY_PICKLE_PROPERTIES)
+            poa_obj = pickle.loads(pickled_poa)
+            sliver_id = poa_obj.get_sliver_id()
+            reservations = self.get_reservations(rid=sliver_id)
+            if reservations is not None:
+                poa_obj.restore(actor=self.actor, reservation=reservations[0])
+            result.append(poa_obj)
+        return result
+
+    def get_poas(self, *, poa_id: str = None, email: str = None, sliver_id: ID = None, slice_id: ID = None,
+                 project_id: str = None, limit: int = None, offset: int = None, last_update_time: datetime = None,
+                 states: list[int] = None) -> Union[List[Poa] or None]:
+        result = []
+        try:
+            try:
+                sliver_id_str = str(sliver_id) if sliver_id is not None else None
+                slice_id_str = str(slice_id) if slice_id is not None else None
+
+                poa_dict_list = self.db.get_poas(poa_guid=poa_id, email=email, sliver_id=sliver_id_str, limit=limit,
+                                                 offset=offset, last_update_time=last_update_time,
+                                                 project_id=project_id, slice_id=slice_id_str, states=states)
+            finally:
+                if self.lock.locked():
+                    self.lock.release()
+            if poa_dict_list is not None:
+                result = self._load_poa_from_db(poa_dict_list=poa_dict_list)
+        except Exception as e:
+            self.logger.error(e)
+            self.logger.error(traceback.format_exc())
+        finally:
+            if self.lock.locked():
+                self.lock.release()
+        return result
+
+    def add_poa(self, *, poa: Poa):
+        try:
+            poa_list = self.get_poas(poa_id=poa.poa_id)
+            if len(poa_list) > 0:
+                raise DatabaseException("Slice # {} already exists".format(poa.poa_id))
+
+            properties = pickle.dumps(poa)
+            email = None
+            project_id = None
+            slice_id = None
+            if poa.get_slice().get_owner() is not None:
+                email = poa.get_slice().get_owner().get_email()
+                project_id = poa.get_slice().get_project_id()
+                slice_id = str(poa.get_slice().get_slice_id())
+
+            self.db.add_poa(poa_guid=poa.poa_id, sliver_id=str(poa.get_sliver_id()), email=email, project_id=project_id,
+                            slice_id=slice_id, properties=properties, state=poa.get_state().value)
+        finally:
+            if self.lock.locked():
+                self.lock.release()
+
+    def update_poa(self, *, poa: Poa):
+        try:
+            #self.lock.acquire()
+            properties = pickle.dumps(poa)
+            self.db.update_poa(poa_guid=poa.poa_id, state=poa.get_state().value, properties=properties)
+        finally:
+            if self.lock.locked():
+                self.lock.release()
+
+    def remove_poa(self, *, poa_id: str):
+        try:
+            #self.lock.acquire()
+            self.db.remove_poa(poa_guid=poa_id)
+        finally:
+            if self.lock.locked():
+                self.lock.release()
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/client_database.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/db/client_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/db/server_actor_database.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/db/server_actor_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/handlers/ansible_handler_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,28 +153,28 @@
         @param unit Unit being processed; This is needed
         """
         with self.future_lock:
             self.futures.append((future, unit))
             self.logger.debug("Added future to Future queue")
             self.future_lock.notify_all()
 
-    def invoke_handler(self, unit: ConfigToken, operation: str):
+    def invoke_handler(self, unit: ConfigToken, operation: str, data: dict = None):
         try:
             # clean restart
             if unit is None:
                 if len(self.config_mappings) == 0:
                     return
                 handler = list(self.config_mappings.values())[0]
             else:
                 handler = self.config_mappings.get(str(unit.get_resource_type()), None)
             if handler is None:
                 raise AuthorityException(f"No handler found for resource type {unit.get_resource_type()}")
 
             future = self.executor.submit(self.process_pool_main, operation, handler.get_class_name(),
-                                          handler.get_module_name(), handler.get_properties(), unit,
+                                          handler.get_module_name(), handler.get_properties(), unit, data,
                                           self.process_pool_lock)
 
             self.queue_future(future=future, unit=unit)
             if unit:
                 self.logger.debug(f"Handler operation {operation} scheduled for Resource Type: {unit.get_resource_type()} "
                                   f"Unit: {unit.get_id()} Reservation: {unit.get_reservation_id()}")
 
@@ -191,26 +191,31 @@
 
     def create(self, unit: ConfigToken):
         self.invoke_handler(unit=unit, operation=Constants.TARGET_CREATE)
 
     def modify(self, unit: ConfigToken):
         self.invoke_handler(unit=unit, operation=Constants.TARGET_MODIFY)
 
+    def poa(self, unit: ConfigToken, data: dict):
+        self.invoke_handler(unit=unit, operation=Constants.TARGET_POA, data=data)
+
     def delete(self, unit: ConfigToken):
         self.invoke_handler(unit=unit, operation=Constants.TARGET_DELETE)
 
     def clean_restart(self):
         self.invoke_handler(unit=None, operation=Constants.TARGET_CLEAN_RESTART)
 
     def handler_complete(self, properties: dict, unit: ConfigToken, old_unit: ConfigToken):
         try:
             self.lock.acquire()
             self.logger.debug(f"Properties: {properties} Unit: {unit}")
-            # Copy the sliver from the Unit to
-            old_unit.update_sliver(sliver=unit.get_sliver())
+            target = properties.get(Constants.PROPERTY_TARGET_NAME)
+            if target != Constants.TARGET_POA:
+                # Copy the sliver from the Unit to
+                old_unit.update_sliver(sliver=unit.get_sliver())
             self.plugin.configuration_complete(token=old_unit, properties=properties)
         except Exception as e:
             self.logger.error(f"Exception occurred {e}")
             self.logger.error(traceback.format_exc())
         finally:
             self.lock.release()
 
@@ -269,26 +274,28 @@
 
                 done.clear()
 
             time.sleep(5)
 
     @staticmethod
     def process_pool_main(operation: str, handler_class: str, handler_module: str, properties: dict,
-                          unit: ConfigToken, process_lock: multiprocessing.Lock):
+                          unit: ConfigToken, data: dict, process_lock: multiprocessing.Lock):
         global process_pool_logger
         handler_class = ReflectionUtils.create_instance_with_params(module_name=handler_module,
                                                                     class_name=handler_class)
         handler_obj = handler_class(process_pool_logger, properties, process_lock)
 
         if operation == Constants.TARGET_CREATE:
             return handler_obj.create(unit)
         elif operation == Constants.TARGET_DELETE:
             return handler_obj.delete(unit)
         elif operation == Constants.TARGET_MODIFY:
             return handler_obj.modify(unit)
+        elif operation == Constants.TARGET_POA:
+            return handler_obj.poa(unit, data)
         elif operation == Constants.TARGET_CLEAN_RESTART:
             return handler_obj.clean_restart()
         else:
             process_pool_logger.error("Invalid operation")
             result = {Constants.PROPERTY_TARGET_NAME: operation,
                       Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_EXCEPTION,
                       Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/config_token.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/handlers/config_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,20 @@
     @abstractmethod
     def complete_modify(self):
         """
         Complete the modify operation
         """
 
     @abstractmethod
+    def complete_poa(self, poa_info: dict):
+        """
+        Complete the poa operation
+        """
+
+    @abstractmethod
     def get_sequence(self) -> int:
         """
         Get Sequence number
         @return sequence number
         """
 
     @abstractmethod
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/handlers/configuration_mapping.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/handlers/handler_processor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/handlers/handler_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,14 +128,24 @@
         result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_MODIFY,
                   Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
                   Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
 
         self.plugin.configuration_complete(token=unit, properties=result)
         self.logger.debug("Executing Modify completed")
 
+    def poa(self, unit: ConfigToken, data: dict):
+        self.logger.debug("Executing POA")
+
+        result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_POA,
+                  Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
+                  Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
+
+        self.plugin.configuration_complete(token=unit, properties=result)
+        self.logger.debug("Executing POA completed")
+
     def set_logger(self, *, logger):
         self.logger = logger
 
     def set_plugin(self, *, plugin: BasePlugin):
         self.plugin = plugin
 
     @staticmethod
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/authority_substrate.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/substrate/authority_substrate.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/substrate/db/substrate_actor_database.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/plugins/substrate/substrate_mixin.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from fabric_cf.actor.core.apis.abc_substrate import ABCSubstrate
 
 if TYPE_CHECKING:
     from fabric_cf.actor.core.apis.abc_database import ABCDatabase
     from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
     from fabric_cf.actor.core.core.unit import Unit
     from fabric_cf.actor.core.plugins.handlers.config_token import ConfigToken
+    from fabric_cf.actor.core.kernel.poa import Poa
 
 
 class SubstrateMixin(BasePlugin, ABCSubstrate):
     def __init__(self, *, actor: ActorMixin, db: ABCSubstrateDatabase, handler_processor: HandlerProcessor):
         super().__init__(actor=actor, db=db, handler_processor=handler_processor)
 
     def __getstate__(self):
@@ -103,14 +104,24 @@
             self.db.update_unit(u=unit)
             # perform the node configuration
             self.do_modify(reservation=reservation, unit=unit)
         except Exception as e:
             self.logger.error(traceback.format_exc())
             self.fail_and_update(unit=unit, message="modify error", e=e)
 
+    def poa(self, *, unit: Unit, poa: Poa):
+        try:
+            # prepare the POA
+            self.prepare_poa(unit=unit)
+            # perform the node configuration
+            self.do_poa(poa=poa, unit=unit)
+        except Exception as e:
+            self.logger.error(traceback.format_exc())
+            self.fail_and_update(unit=unit, message="modify error", e=e)
+
     def prepare_transfer_in(self, *, reservation: ABCReservationMixin, unit: Unit):
         """
         Performs additional setup operations before configuring the unit. This is
         an optional step of the transfer in process and can be used to set custom
         properties on the reservation/unit objects before invoking the
         configuration subsystem. For example, if the policy did not allocate an
         IP address for the unit, but an IP address is required to configure the
@@ -134,23 +145,34 @@
     def prepare_modify(self, *, reservation: ABCReservationMixin, unit: Unit):
         """
         Prepares the unit for modification.
         @param reservation reservation containing the unit
         @param unit unit to prepare
         @throws Exception in case of error
         """
+
+    def prepare_poa(self, *, unit: Unit):
+        """
+        Prepares the unit for POA.
+        @param unit unit to prepare
+        @throws Exception in case of error
+        """
+
     def do_transfer_in(self, *, reservation: ABCReservationMixin, unit: Unit):
         self.handler_processor.create(unit=unit)
 
     def do_transfer_out(self, *, reservation: ABCReservationMixin, unit: Unit):
         self.handler_processor.delete(unit=unit)
 
     def do_modify(self, *, reservation: ABCReservationMixin, unit: Unit):
         self.handler_processor.modify(unit=unit)
 
+    def do_poa(self, *, poa: Poa, unit: Unit):
+        self.handler_processor.poa(unit=unit, data=poa.to_dict())
+
     def fail_and_update(self, *, unit: Unit, message: str, e: Exception):
         self.logger.error(message)
         self.logger.error(str(e))
 
         try:
             unit.fail(message=message, exception=e)
             self.db.update_unit(u=unit)
@@ -169,14 +191,20 @@
         if e:
             self.logger.error(e)
         if unit.is_network_service():
             unit.fail(message=message, exception=e)
         else:
             unit.fail_on_modify(message=message, exception=e)
 
+    def fail_poa_no_update(self, *, unit: Unit, message: str, e: Exception = None):
+        self.logger.error(message)
+        if e:
+            self.logger.error(e)
+        unit.fail_on_poa(message=message, exception=e)
+
     def merge_unit_properties(self, *, unit: Unit, properties: dict):
         # TODO
         return
 
     def process_create_complete(self, *, unit: ConfigToken, properties: dict):
         self.logger.debug("Create")
         self.logger.debug(properties)
@@ -304,14 +332,53 @@
         try:
             self.get_substrate_database().update_unit(u=unit)
         except Exception as e:
             self.logger.error(e)
         finally:
             self.logger.debug("process modify complete")
 
+    def process_poa_complete(self, *, unit: ConfigToken, properties: dict):
+        self.logger.debug("POA")
+        self.logger.debug(properties)
+
+        if self.actor.is_stopped():
+            raise PluginException(Constants.INVALID_ACTOR_STATE)
+
+        sequence = HandlerProcessor.get_action_sequence_number(properties=properties)
+        notice = None
+        if sequence != unit.get_sequence():
+            self.logger.warning("(poa complete) sequences mismatch: incoming ({}) local: ({}). "
+                                "Ignoring event.".format(sequence, unit.get_sequence()))
+            return
+        else:
+            self.logger.debug("(poa complete) incoming ({}) local: ({})".format(sequence, unit.get_sequence()))
+
+        result = HandlerProcessor.get_result_code(properties=properties)
+        msg = HandlerProcessor.get_exception_message(properties=properties)
+        if msg is None:
+            msg = HandlerProcessor.get_result_code_message(properties=properties)
+
+        poa_info = properties.get(Constants.PROPERTY_POA_INFO)
+
+        if result == 0:
+            self.logger.debug("poa code 0 (success)")
+            unit.complete_poa(poa_info=poa_info)
+
+        elif result == -1:
+            self.logger.debug("poa code -1 with message: {}".format(msg))
+            notice = "Exception during poa for unit: {} {}".format(unit.get_id(), msg)
+            self.fail_poa_no_update(unit=unit, message=notice)
+
+        else:
+            self.logger.debug("modify code {} with message: {}".format(result, msg))
+            notice = "Error code= {} during modify for unit: {} with message: {}".format(result, unit.get_id(), msg)
+            self.fail_poa_no_update(unit=unit, message=notice)
+
+        self.logger.debug("process poa complete")
+
     def get_substrate_database(self) -> ABCSubstrateDatabase:
         return self.db
 
     def set_database(self, *, db: ABCDatabase):
         if db is not None and not isinstance(db, ABCSubstrateDatabase):
             raise PluginException("db must implement ISubstrateDatabase")
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/authority_calendar_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/authority_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/broker_calendar_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/broker_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/broker_simpler_units_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/broker_simpler_units_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from fim.slivers.network_service import NetworkServiceSliver, ServiceType
 
 from fabric_cf.actor.boot.configuration import ActorConfig
 from fabric_cf.actor.core.apis.abc_broker_reservation import ABCBrokerReservation
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.common.constants import Constants
+from fabric_cf.actor.core.container.maintenance import Maintenance
 from fabric_cf.actor.core.delegation.resource_ticket import ResourceTicketFactory
 from fabric_cf.actor.core.common.exceptions import BrokerException, ExceptionErrorCode
 from fabric_cf.actor.core.kernel.reservation_states import ReservationStates
 from fabric_cf.actor.core.policy.broker_calendar_policy import BrokerCalendarPolicy
 from fabric_cf.actor.core.policy.fifo_queue import FIFOQueue
 from fabric_cf.actor.core.policy.network_node_inventory import NetworkNodeInventory
 from fabric_cf.actor.core.policy.network_service_inventory import NetworkServiceInventory
@@ -504,14 +505,40 @@
         # re-add storage components
         if len(storage_components) > 0:
             for c in storage_components:
                 sliver.attached_components_info.add_device(device_info=c)
 
         return result
 
+    def __prune_nodes_in_maintenance(self, node_id_list: List[str], site: str, reservation: ABCBrokerReservation):
+        """
+        Prune the candidate node list to exclude the workers in Maintenance
+        @param node_id_list: Candidate Node List identified to allocate the reservation
+        @param site: Site Name
+        @param reservation: Reservation to be allocated
+        """
+        project_id = reservation.get_slice().get_project_id()
+        email = reservation.get_slice().get_owner().get_email()
+
+        nodes_to_remove = []
+        for node_id in node_id_list:
+            graph_node = self.get_network_node_from_graph(node_id=node_id)
+            status, error_message = Maintenance.is_sliver_provisioning_allowed(database=self.actor.get_plugin().get_database(),
+                                                                               project=project_id, site=site,
+                                                                               worker=graph_node.get_name(),
+                                                                               email=email)
+            if not status:
+                self.logger.info(f"Excluding {graph_node.get_name()} as allocation candidate due to {error_message}")
+                nodes_to_remove.append(node_id)
+
+        for x in nodes_to_remove:
+            node_id_list.remove(x)
+
+        return node_id_list
+
     def __find_first_fit(self, node_id_list: List[str], node_id_to_reservations: dict, inv: InventoryForType,
                          reservation: ABCBrokerReservation) -> Tuple[str, BaseSliver, Any]:
         """
         Find First Available Node which can serve the reservation
         @param node_id_list: Candidate Nodes
         @param node_id_to_reservations:
         @param inv: Inventory
@@ -567,14 +594,18 @@
         @param sliver Requested sliver
         @param node_id_to_reservations
         @return tuple containing delegation id, sliver, error message if any
         """
         delegation_id = None
         node_id_list = self.__candidate_nodes(sliver=sliver)
 
+        node_id_list = self.__prune_nodes_in_maintenance(node_id_list=node_id_list,
+                                                         site=sliver.site,
+                                                         reservation=reservation)
+
         # no candidate nodes found
         if len(node_id_list) == 0:
             error_msg = f'Insufficient resources: No candidates nodes found to serve {reservation}'
             self.logger.error(error_msg)
             return delegation_id, sliver, error_msg
 
         if self.get_algorithm_type().lower() == BrokerAllocationAlgorithm.FirstFit.name.lower():
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_calendar_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/controller_calendar_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_simple_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/controller_simple_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/controller_ticket_review_policy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/controller_ticket_review_policy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/fifo_queue.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/fifo_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/inventory.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/inventory_for_type.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/inventory_for_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_node_control.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/network_node_control.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,15 @@
 
                     for ac in allocated_components:
                         ac_node_map = ac.get_node_map()
                         if ac_node_map[1] == node_map[1]:
                             # For Shared NIC, make sure PCI devices are not same
                             # For other components, having same node map is an error
                             if (ac.get_type() == ComponentType.SharedNIC and
-                                ac.get_labels().bdf == c.get_labels()) or \
+                                ac.get_labels().bdf == c.get_labels().bdf) or \
                                     ac.get_type() != ComponentType.SharedNIC:
                                 raise AuthorityException(
                                     f"Component of type: {resource_type} BQM Node Id: {node_map[1]} "
                                     f"in graph {graph_node.node_id}"
                                     f"is already assigned to reservation# {reservation}")
 
     def assign(self, *, reservation: ABCAuthorityReservation, delegation_name: str,
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_node_inventory.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/network_node_inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_service_control.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/network_service_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/network_service_inventory.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/network_service_inventory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/queue_wrapper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/queue_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/policy/resource_control.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/policy/resource_control.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/actor_location.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/actor_location.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,124 +22,145 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
-from fabric_mb.message_bus.messages.close_avro import CloseAvro
-from fabric_mb.message_bus.messages.extend_lease_avro import ExtendLeaseAvro
-from fabric_mb.message_bus.messages.modify_lease_avro import ModifyLeaseAvro
-from fabric_mb.message_bus.messages.redeem_avro import RedeemAvro
+from fabric_mb.message_bus.messages.claim_delegation_avro import ClaimDelegationAvro
+from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
+from fabric_mb.message_bus.messages.extend_ticket_avro import ExtendTicketAvro
+from fabric_mb.message_bus.messages.reclaim_delegation_avro import ReclaimDelegationAvro
+from fabric_mb.message_bus.messages.relinquish_avro import RelinquishAvro
 from fabric_mb.message_bus.messages.reservation_avro import ReservationAvro
+from fabric_mb.message_bus.messages.ticket_avro import TicketAvro
 from fabric_mb.message_bus.producer import AvroProducerApi
 
-from fabric_cf.actor.core.apis.abc_authority_proxy import ABCAuthorityProxy
-from fabric_cf.actor.core.common.constants import Constants
-from fabric_cf.actor.core.common.exceptions import ProxyException
+from fabric_cf.actor.core.apis.abc_broker_proxy import ABCBrokerProxy
+from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.core.ticket import Ticket
 from fabric_cf.actor.core.core.unit_set import UnitSet
 from fabric_cf.actor.core.kernel.rpc_request_type import RPCRequestType
-from fabric_cf.actor.core.proxies.kafka.kafka_broker_proxy import KafkaBrokerProxy
-from fabric_cf.actor.core.proxies.kafka.kafka_proxy import KafkaProxyRequestState
+from fabric_cf.actor.core.proxies.kafka.kafka_proxy import KafkaProxy, KafkaProxyRequestState
 from fabric_cf.actor.core.proxies.kafka.translate import Translate
 
 if TYPE_CHECKING:
     from fabric_cf.actor.security.auth_token import AuthToken
     from fabric_cf.actor.core.apis.abc_rpc_request_state import ABCRPCRequestState
-    from fabric_cf.actor.core.apis.abc_controller_callback_proxy import ABCControllerCallbackProxy
-    from fabric_cf.actor.core.apis.abc_controller_reservation import ABCControllerReservation
+    from fabric_cf.actor.core.proxies.kafka.kafka_retun import KafkaReturn
     from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 
 
-class KafkaAuthorityProxy(KafkaBrokerProxy, ABCAuthorityProxy):
+class KafkaBrokerProxy(KafkaProxy, ABCBrokerProxy):
     def __init__(self, *, kafka_topic: str, identity: AuthToken, logger):
         super().__init__(kafka_topic=kafka_topic, identity=identity, logger=logger)
-        self.type = self.TypeSite
+        self.type = KafkaProxy.TypeBroker
 
-    def execute(self, *, request: ABCRPCRequestState, producer: AvroProducerApi):
+    def execute(self, *, request: KafkaProxyRequestState, producer: AvroProducerApi):
         avro_message = None
-        if request.get_type() == RPCRequestType.Redeem:
-            avro_message = RedeemAvro()
+        if request.get_type() == RPCRequestType.Ticket:
+            avro_message = TicketAvro()
             avro_message.message_id = str(request.get_message_id())
-            avro_message.callback_topic = request.callback_topic
             avro_message.reservation = request.reservation
+            avro_message.callback_topic = request.callback_topic
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
-        elif request.get_type() == RPCRequestType.ExtendLease:
-            avro_message = ExtendLeaseAvro()
+        elif request.get_type() == RPCRequestType.ClaimDelegation:
+            avro_message = ClaimDelegationAvro()
             avro_message.message_id = str(request.get_message_id())
+            avro_message.delegation = request.delegation
             avro_message.callback_topic = request.callback_topic
-            avro_message.reservation = request.reservation
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
-        elif request.get_type() == RPCRequestType.ModifyLease:
-            avro_message = ModifyLeaseAvro()
+        elif request.get_type() == RPCRequestType.ReclaimDelegation:
+            avro_message = ReclaimDelegationAvro()
             avro_message.message_id = str(request.get_message_id())
+            avro_message.delegation = request.delegation
             avro_message.callback_topic = request.callback_topic
-            avro_message.reservation = request.reservation
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
-        elif request.get_type() == RPCRequestType.Close:
-            avro_message = CloseAvro()
+        elif request.get_type() == RPCRequestType.ExtendTicket:
+            avro_message = ExtendTicketAvro()
             avro_message.message_id = str(request.get_message_id())
-            avro_message.callback_topic = request.callback_topic
             avro_message.reservation = request.reservation
+            avro_message.callback_topic = request.callback_topic
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
+        elif request.get_type() == RPCRequestType.Relinquish:
+            avro_message = RelinquishAvro()
+            avro_message.message_id = str(request.get_message_id())
+            avro_message.reservation = request.reservation
+            avro_message.callback_topic = request.callback_topic
+            avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
         else:
             super().execute(request=request, producer=producer)
             return
 
         if producer is not None and producer.produce(topic=self.kafka_topic, record=avro_message):
             self.logger.debug("Message {} written to {}".format(avro_message.name, self.kafka_topic))
         else:
             self.logger.error("Failed to send message {} to {} via producer {}".format(avro_message.name,
                                                                                        self.kafka_topic, producer))
 
-    def _prepare(self, *, reservation: ABCControllerReservation, callback: ABCControllerCallbackProxy,
+    def _prepare_delegation(self, *, delegation: ABCDelegation, callback: KafkaReturn,
+                            caller: AuthToken) -> ABCRPCRequestState:
+        request = KafkaProxyRequestState()
+        request.delegation = self.pass_broker_delegation(delegation=delegation, auth=caller)
+        request.callback_topic = callback.get_kafka_topic()
+        request.caller = caller
+        return request
+
+    def prepare_claim_delegation(self, *, delegation: ABCDelegation, callback: KafkaReturn,
+                                 caller: AuthToken) -> ABCRPCRequestState:
+        return self._prepare_delegation(delegation=delegation, callback=callback, caller=caller)
+
+    def prepare_reclaim_delegation(self, *, delegation: ABCDelegation, callback: KafkaReturn,
+                                   caller: AuthToken) -> ABCRPCRequestState:
+        return self._prepare_delegation(delegation=delegation, callback=callback, caller=caller)
+
+    def _prepare(self, *, reservation: ABCReservationMixin, callback: KafkaReturn,
                  caller: AuthToken) -> ABCRPCRequestState:
         request = KafkaProxyRequestState()
+        request.reservation = self.pass_broker_reservation(reservation=reservation, auth=caller)
         request.callback_topic = callback.get_kafka_topic()
-        request.reservation = self.pass_authority_reservation(reservation=reservation, caller=caller)
         request.caller = caller
         return request
 
-    def prepare_redeem(self, *, reservation: ABCControllerReservation, callback: ABCControllerCallbackProxy,
+    def prepare_ticket(self, *, reservation: ABCReservationMixin, callback: KafkaReturn,
                        caller: AuthToken) -> ABCRPCRequestState:
         return self._prepare(reservation=reservation, callback=callback, caller=caller)
 
-    def prepare_extend_lease(self, *, reservation: ABCControllerReservation, callback: ABCControllerCallbackProxy,
-                             caller: AuthToken) -> ABCRPCRequestState:
+    def prepare_extend_ticket(self, *, reservation: ABCReservationMixin, callback: KafkaReturn,
+                              caller: AuthToken) -> ABCRPCRequestState:
         return self._prepare(reservation=reservation, callback=callback, caller=caller)
 
-    def prepare_modify_lease(self, *, reservation: ABCControllerReservation, callback: ABCControllerCallbackProxy,
-                             caller: AuthToken) -> ABCRPCRequestState:
-        return self._prepare(reservation=reservation, callback=callback, caller=caller)
-
-    def prepare_close(self, *, reservation: ABCControllerReservation, callback: ABCControllerCallbackProxy,
-                      caller: AuthToken) -> ABCRPCRequestState:
+    def prepare_relinquish(self, *, reservation: ABCReservationMixin, callback: KafkaReturn,
+                           caller: AuthToken) -> ABCRPCRequestState:
         return self._prepare(reservation=reservation, callback=callback, caller=caller)
 
     @staticmethod
-    def pass_authority_reservation(reservation: ABCReservationMixin, caller: AuthToken) -> ReservationAvro:
-        concrete = reservation.get_resources().get_resources()
-        if concrete is None:
-            raise ProxyException(Constants.NOT_SPECIFIED_PREFIX.format("ticket"))
-
+    def pass_broker_reservation(reservation: ABCReservationMixin, auth: AuthToken) -> ReservationAvro:
         avro_reservation = ReservationAvro()
         avro_reservation.slice = Translate.translate_slice_to_avro(slice_obj=reservation.get_slice())
         avro_reservation.term = Translate.translate_term(term=reservation.get_requested_term())
         avro_reservation.reservation_id = str(reservation.get_reservation_id())
-        avro_reservation.sequence = reservation.get_lease_sequence_out()
+        avro_reservation.sequence = reservation.get_ticket_sequence_out()
+
+        rset = Translate.translate_resource_set(resource_set=reservation.get_requested_resources())
 
-        rset = Translate.translate_resource_set(resource_set=reservation.get_resources())
+        if reservation.get_requested_resources() is not None:
+            cset = reservation.get_requested_resources().get_resources()
 
-        if concrete is not None and isinstance(concrete, Ticket):
-            rset.ticket = Translate.translate_ticket(ticket=concrete)
+            if cset is not None and isinstance(cset, Ticket):
+                rset.ticket = Translate.translate_ticket(ticket=cset)
 
-        if concrete is not None and isinstance(concrete, UnitSet):
-            rset.unit_set = Translate.translate_unit_set(unit_set=concrete)
+            if cset is not None and isinstance(cset, UnitSet):
+                rset.units = Translate.translate_unit_set(unit_set=cset)
 
         avro_reservation.resource_set = rset
 
         return avro_reservation
+
+    @staticmethod
+    def pass_broker_delegation(delegation: ABCDelegation, auth: AuthToken) -> DelegationAvro:
+        avro_delegation = Translate.translate_delegation_to_avro(delegation=delegation)
+        return avro_delegation
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_broker_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/kafka_retun.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,145 +22,148 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
-from fabric_mb.message_bus.messages.claim_delegation_avro import ClaimDelegationAvro
 from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
-from fabric_mb.message_bus.messages.extend_ticket_avro import ExtendTicketAvro
-from fabric_mb.message_bus.messages.reclaim_delegation_avro import ReclaimDelegationAvro
-from fabric_mb.message_bus.messages.relinquish_avro import RelinquishAvro
 from fabric_mb.message_bus.messages.reservation_avro import ReservationAvro
-from fabric_mb.message_bus.messages.ticket_avro import TicketAvro
+from fabric_mb.message_bus.messages.result_avro import ResultAvro
+from fabric_mb.message_bus.messages.result_poa_avro import ResultPoaAvro
+from fabric_mb.message_bus.messages.update_delegation_avro import UpdateDelegationAvro
+from fabric_mb.message_bus.messages.update_lease_avro import UpdateLeaseAvro
+from fabric_mb.message_bus.messages.update_ticket_avro import UpdateTicketAvro
 from fabric_mb.message_bus.producer import AvroProducerApi
 
-from fabric_cf.actor.core.apis.abc_broker_proxy import ABCBrokerProxy
+from fabric_cf.actor.core.apis.abc_controller_callback_proxy import ABCControllerCallbackProxy
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.core.ticket import Ticket
 from fabric_cf.actor.core.core.unit_set import UnitSet
 from fabric_cf.actor.core.kernel.rpc_request_type import RPCRequestType
 from fabric_cf.actor.core.proxies.kafka.kafka_proxy import KafkaProxy, KafkaProxyRequestState
 from fabric_cf.actor.core.proxies.kafka.translate import Translate
 
 if TYPE_CHECKING:
     from fabric_cf.actor.security.auth_token import AuthToken
     from fabric_cf.actor.core.apis.abc_rpc_request_state import ABCRPCRequestState
-    from fabric_cf.actor.core.apis.abc_client_callback_proxy import ABCClientCallbackProxy
-    from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
+    from fabric_cf.actor.core.apis.abc_broker_reservation import ABCBrokerReservation
+    from fabric_cf.actor.core.apis.abc_authority_reservation import ABCAuthorityReservation
+    from fabric_cf.actor.core.apis.abc_server_reservation import ABCServerReservation
+    from fabric_cf.actor.core.util.update_data import UpdateData
+    from fabric_cf.actor.core.kernel.poa import Poa
 
 
-class KafkaBrokerProxy(KafkaProxy, ABCBrokerProxy):
+class KafkaReturn(KafkaProxy, ABCControllerCallbackProxy):
     def __init__(self, *, kafka_topic: str, identity: AuthToken, logger):
         super().__init__(kafka_topic=kafka_topic, identity=identity, logger=logger)
-        self.type = KafkaProxy.TypeBroker
+        self.type = KafkaProxy.TypeReturn
+        self.callback = True
 
-    def execute(self, *, request: ABCRPCRequestState, producer: AvroProducerApi):
-        avro_message = None
-        if request.get_type() == RPCRequestType.Ticket:
-            avro_message = TicketAvro()
+    def execute(self, *, request: KafkaProxyRequestState, producer: AvroProducerApi):
+        if request.get_type() == RPCRequestType.UpdateTicket:
+            avro_message = UpdateTicketAvro()
             avro_message.message_id = str(request.get_message_id())
             avro_message.reservation = request.reservation
             avro_message.callback_topic = request.callback_topic
+            avro_message.update_data = request.udd
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
-        elif request.get_type() == RPCRequestType.ClaimDelegation:
-            avro_message = ClaimDelegationAvro()
+        elif request.get_type() == RPCRequestType.UpdateLease:
+            avro_message = UpdateLeaseAvro()
             avro_message.message_id = str(request.get_message_id())
-            avro_message.delegation = request.delegation
+            avro_message.reservation = request.reservation
             avro_message.callback_topic = request.callback_topic
+            avro_message.update_data = request.udd
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
-        elif request.get_type() == RPCRequestType.ReclaimDelegation:
-            avro_message = ReclaimDelegationAvro()
+        elif request.get_type() == RPCRequestType.UpdateDelegation:
+            avro_message = UpdateDelegationAvro()
             avro_message.message_id = str(request.get_message_id())
             avro_message.delegation = request.delegation
             avro_message.callback_topic = request.callback_topic
+            avro_message.update_data = request.udd
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
-        elif request.get_type() == RPCRequestType.ExtendTicket:
-            avro_message = ExtendTicketAvro()
+        elif request.get_type() == RPCRequestType.PoaInfo:
+            avro_message = request.poa
             avro_message.message_id = str(request.get_message_id())
-            avro_message.reservation = request.reservation
             avro_message.callback_topic = request.callback_topic
-            avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
-        elif request.get_type() == RPCRequestType.Relinquish:
-            avro_message = RelinquishAvro()
-            avro_message.message_id = str(request.get_message_id())
-            avro_message.reservation = request.reservation
-            avro_message.callback_topic = request.callback_topic
-            avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
         else:
             super().execute(request=request, producer=producer)
             return
 
         if producer is not None and producer.produce(topic=self.kafka_topic, record=avro_message):
             self.logger.debug("Message {} written to {}".format(avro_message.name, self.kafka_topic))
         else:
             self.logger.error("Failed to send message {} to {} via producer {}".format(avro_message.name,
                                                                                        self.kafka_topic, producer))
 
-    def _prepare_delegation(self, *, delegation: ABCDelegation, callback: ABCClientCallbackProxy,
-                            caller: AuthToken) -> ABCRPCRequestState:
+    def prepare_update_delegation(self, *, delegation: ABCDelegation, update_data: UpdateData,
+                                  callback: KafkaProxy, caller: AuthToken) -> ABCRPCRequestState:
         request = KafkaProxyRequestState()
-        request.delegation = self.pass_broker_delegation(delegation=delegation, auth=caller)
+        request.delegation = self.pass_delegation(delegation=delegation, auth=caller)
+        request.udd = Translate.translate_udd(udd=update_data)
         request.callback_topic = callback.get_kafka_topic()
         request.caller = caller
         return request
 
-    def prepare_claim_delegation(self, *, delegation: ABCDelegation, callback: ABCClientCallbackProxy,
-                                 caller: AuthToken) -> ABCRPCRequestState:
-        return self._prepare_delegation(delegation=delegation, callback=callback, caller=caller)
-
-    def prepare_reclaim_delegation(self, *, delegation: ABCDelegation, callback: ABCClientCallbackProxy,
-                                   caller: AuthToken) -> ABCRPCRequestState:
-        return self._prepare_delegation(delegation=delegation, callback=callback, caller=caller)
-
-    def _prepare(self, *, reservation: ABCReservationMixin, callback: ABCClientCallbackProxy,
-                 caller: AuthToken) -> ABCRPCRequestState:
+    def _prepare(self, *, reservation: ABCServerReservation, update_data: UpdateData,
+                 callback: KafkaProxy, caller: AuthToken) -> ABCRPCRequestState:
         request = KafkaProxyRequestState()
-        request.reservation = self.pass_broker_reservation(reservation=reservation, auth=caller)
+        request.reservation = self.pass_reservation(reservation=reservation, auth=caller)
+        request.udd = Translate.translate_udd(udd=update_data)
         request.callback_topic = callback.get_kafka_topic()
         request.caller = caller
         return request
 
-    def prepare_ticket(self, *, reservation: ABCReservationMixin, callback: ABCClientCallbackProxy,
-                       caller: AuthToken) -> ABCRPCRequestState:
-        return self._prepare(reservation=reservation, callback=callback, caller=caller)
-
-    def prepare_extend_ticket(self, *, reservation: ABCReservationMixin, callback: ABCClientCallbackProxy,
-                              caller: AuthToken) -> ABCRPCRequestState:
-        return self._prepare(reservation=reservation, callback=callback, caller=caller)
-
-    def prepare_relinquish(self, *, reservation: ABCReservationMixin, callback: ABCClientCallbackProxy,
-                           caller: AuthToken) -> ABCRPCRequestState:
-        return self._prepare(reservation=reservation, callback=callback, caller=caller)
+    def prepare_update_ticket(self, *, reservation: ABCBrokerReservation, update_data: UpdateData,
+                              callback: KafkaProxy, caller: AuthToken) -> ABCRPCRequestState:
+        return self._prepare(reservation=reservation, update_data=update_data, callback=callback, caller=caller)
+
+    def prepare_update_lease(self, *, reservation: ABCAuthorityReservation, update_data: UpdateData,
+                             callback: KafkaProxy, caller: AuthToken) -> ABCRPCRequestState:
+        return self._prepare(reservation=reservation, update_data=update_data, callback=callback, caller=caller)
+
+    def prepare_poa_result(self, *, poa: Poa, callback: KafkaProxy, caller: AuthToken) -> ABCRPCRequestState:
+        request = KafkaProxyRequestState()
+        request.poa = Translate.translate_poa_to_result_poa_avro(poa=poa)
+        request.callback_topic = callback.get_kafka_topic()
+        request.caller = caller
+        return request
 
     @staticmethod
-    def pass_broker_reservation(reservation: ABCReservationMixin, auth: AuthToken) -> ReservationAvro:
+    def pass_reservation(reservation: ABCServerReservation, auth: AuthToken) -> ReservationAvro:
         avro_reservation = ReservationAvro()
         avro_reservation.slice = Translate.translate_slice_to_avro(slice_obj=reservation.get_slice())
-        avro_reservation.term = Translate.translate_term(term=reservation.get_requested_term())
-        avro_reservation.reservation_id = str(reservation.get_reservation_id())
-        avro_reservation.sequence = reservation.get_ticket_sequence_out()
+        if reservation.get_term() is None:
+            term = reservation.get_requested_term().clone()
+        else:
+            term = reservation.get_term().clone()
 
-        rset = Translate.translate_resource_set(resource_set=reservation.get_requested_resources())
+        avro_reservation.term = Translate.translate_term(term=term)
+        avro_reservation.reservation_id = str(reservation.get_reservation_id())
 
-        if reservation.get_requested_resources() is not None:
-            cset = reservation.get_requested_resources().get_resources()
+        if reservation.get_resources() is None:
+            from fabric_cf.actor.core.kernel.resource_set import ResourceSet
+            rset = Translate.translate_resource_set(resource_set=ResourceSet(units=0,
+                                                                             rtype=reservation.get_requested_type()))
+        else:
+            rset = Translate.translate_resource_set(resource_set=reservation.get_resources())
+        if reservation.get_resources() is not None:
+            cset = reservation.get_resources().get_resources()
 
             if cset is not None and isinstance(cset, Ticket):
                 rset.ticket = Translate.translate_ticket(ticket=cset)
 
             if cset is not None and isinstance(cset, UnitSet):
-                rset.units = Translate.translate_unit_set(unit_set=cset)
+                rset.unit_set = Translate.translate_unit_set(unit_set=cset)
 
         avro_reservation.resource_set = rset
-
         return avro_reservation
 
     @staticmethod
-    def pass_broker_delegation(delegation: ABCDelegation, auth: AuthToken) -> DelegationAvro:
+    def pass_delegation(delegation: ABCDelegation, auth: AuthToken) -> DelegationAvro:
         avro_delegation = Translate.translate_delegation_to_avro(delegation=delegation)
+        avro_delegation.sequence = delegation.get_sequence_out()
         return avro_delegation
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/kafka_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,18 @@
 
 
 class KafkaProxyRequestState(RPCRequestState):
     def __init__(self):
         super().__init__()
         self.callback_topic = None
         self.reservation = None
+        self.delegation = None
         self.udd = None
         self.query = None
+        self.poa = None
         self.request_id = None
         self.failed_reservation_id = None
         self.failed_request_type = None
         self.error_detail = None
 
 
 class KafkaProxy(Proxy, ABCCallbackProxy):
@@ -84,15 +86,15 @@
         peer_dict = GlobalsSingleton.get().get_config().get_peers_dict()
         self.logger = GlobalsSingleton.get().get_logger()
         peer = peer_dict.get(self.get_name())
         if peer is not None:
             self.kafka_topic = peer.get_kafka_topic()
         self.logger = None
 
-    def execute(self, *, request: ABCRPCRequestState, producer: AvroProducerApi):
+    def execute(self, *, request: KafkaProxyRequestState, producer: AvroProducerApi):
         avro_message = None
         if request.get_type() == RPCRequestType.Query:
             avro_message = QueryAvro()
             avro_message.message_id = str(request.get_message_id())
             avro_message.properties = request.query
             avro_message.callback_topic = request.callback_topic
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
@@ -111,15 +113,15 @@
             avro_message.request_type = request.failed_request_type.value
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
             if request.failed_reservation_id is not None:
                 avro_message.reservation_id = request.failed_reservation_id
             else:
                 avro_message.reservation_id = ""
-            avro_message.error_details = request.error_details
+            avro_message.error_details = request.error_detail
 
         else:
             raise ProxyException("Unsupported RPC: type={}".format(request.get_type()))
 
         if producer is not None and producer.produce(topic=self.kafka_topic, record=avro_message):
             self.logger.debug("Message {} written to {}".format(avro_message.name, self.kafka_topic))
         else:
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/kafka_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/kafka_retun.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/kafka_authority_proxy.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,137 +22,137 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
-from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
+from fabric_mb.message_bus.messages.close_avro import CloseAvro
+from fabric_mb.message_bus.messages.extend_lease_avro import ExtendLeaseAvro
+from fabric_mb.message_bus.messages.modify_lease_avro import ModifyLeaseAvro
+from fabric_mb.message_bus.messages.redeem_avro import RedeemAvro
 from fabric_mb.message_bus.messages.reservation_avro import ReservationAvro
-from fabric_mb.message_bus.messages.update_delegation_avro import UpdateDelegationAvro
-from fabric_mb.message_bus.messages.update_lease_avro import UpdateLeaseAvro
-from fabric_mb.message_bus.messages.update_ticket_avro import UpdateTicketAvro
 from fabric_mb.message_bus.producer import AvroProducerApi
 
-from fabric_cf.actor.core.apis.abc_controller_callback_proxy import ABCControllerCallbackProxy
-from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
+from fabric_cf.actor.core.apis.abc_authority_proxy import ABCAuthorityProxy
+from fabric_cf.actor.core.common.constants import Constants
+from fabric_cf.actor.core.common.exceptions import ProxyException
 from fabric_cf.actor.core.core.ticket import Ticket
 from fabric_cf.actor.core.core.unit_set import UnitSet
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.kernel.rpc_request_type import RPCRequestType
-from fabric_cf.actor.core.proxies.kafka.kafka_proxy import KafkaProxy, KafkaProxyRequestState
+from fabric_cf.actor.core.proxies.kafka.kafka_broker_proxy import KafkaBrokerProxy
+from fabric_cf.actor.core.proxies.kafka.kafka_proxy import KafkaProxyRequestState
 from fabric_cf.actor.core.proxies.kafka.translate import Translate
 
 if TYPE_CHECKING:
     from fabric_cf.actor.security.auth_token import AuthToken
     from fabric_cf.actor.core.apis.abc_rpc_request_state import ABCRPCRequestState
-    from fabric_cf.actor.core.apis.abc_broker_reservation import ABCBrokerReservation
-    from fabric_cf.actor.core.apis.abc_callback_proxy import ABCCallbackProxy
-    from fabric_cf.actor.core.apis.abc_authority_reservation import ABCAuthorityReservation
-    from fabric_cf.actor.core.apis.abc_server_reservation import ABCServerReservation
-    from fabric_cf.actor.core.util.update_data import UpdateData
+    from fabric_cf.actor.core.apis.abc_controller_reservation import ABCControllerReservation
+    from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
+    from fabric_cf.actor.core.proxies.kafka.kafka_retun import KafkaReturn
 
 
-class KafkaReturn(KafkaProxy, ABCControllerCallbackProxy):
+class KafkaAuthorityProxy(KafkaBrokerProxy, ABCAuthorityProxy):
     def __init__(self, *, kafka_topic: str, identity: AuthToken, logger):
         super().__init__(kafka_topic=kafka_topic, identity=identity, logger=logger)
-        self.type = KafkaProxy.TypeReturn
-        self.callback = True
+        self.type = self.TypeSite
 
-    def execute(self, *, request: ABCRPCRequestState, producer: AvroProducerApi):
-        avro_message = None
-        if request.get_type() == RPCRequestType.UpdateTicket:
-            avro_message = UpdateTicketAvro()
+    def execute(self, *, request: KafkaProxyRequestState, producer: AvroProducerApi):
+        if request.get_type() == RPCRequestType.Redeem:
+            avro_message = RedeemAvro()
             avro_message.message_id = str(request.get_message_id())
-            avro_message.reservation = request.reservation
             avro_message.callback_topic = request.callback_topic
-            avro_message.update_data = request.udd
+            avro_message.reservation = request.reservation
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
-        elif request.get_type() == RPCRequestType.UpdateLease:
-            avro_message = UpdateLeaseAvro()
+        elif request.get_type() == RPCRequestType.ExtendLease:
+            avro_message = ExtendLeaseAvro()
             avro_message.message_id = str(request.get_message_id())
+            avro_message.callback_topic = request.callback_topic
             avro_message.reservation = request.reservation
+            avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
+
+        elif request.get_type() == RPCRequestType.ModifyLease:
+            avro_message = ModifyLeaseAvro()
+            avro_message.message_id = str(request.get_message_id())
             avro_message.callback_topic = request.callback_topic
-            avro_message.update_data = request.udd
+            avro_message.reservation = request.reservation
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
-        elif request.get_type() == RPCRequestType.UpdateDelegation:
-            avro_message = UpdateDelegationAvro()
+        elif request.get_type() == RPCRequestType.Close:
+            avro_message = CloseAvro()
             avro_message.message_id = str(request.get_message_id())
-            avro_message.delegation = request.delegation
             avro_message.callback_topic = request.callback_topic
-            avro_message.update_data = request.udd
+            avro_message.reservation = request.reservation
             avro_message.auth = Translate.translate_auth_to_avro(auth=request.caller)
 
+        elif request.get_type() == RPCRequestType.Poa:
+            avro_message = request.poa
+            avro_message.message_id = str(request.get_message_id())
+            avro_message.callback_topic = request.callback_topic
+
         else:
             super().execute(request=request, producer=producer)
             return
 
         if producer is not None and producer.produce(topic=self.kafka_topic, record=avro_message):
             self.logger.debug("Message {} written to {}".format(avro_message.name, self.kafka_topic))
         else:
             self.logger.error("Failed to send message {} to {} via producer {}".format(avro_message.name,
                                                                                        self.kafka_topic, producer))
 
-    def prepare_update_delegation(self, *, delegation: ABCDelegation, update_data: UpdateData,
-                                  callback: ABCCallbackProxy, caller: AuthToken) -> ABCRPCRequestState:
+    def _prepare(self, *, reservation: ABCControllerReservation, callback: KafkaReturn,
+                 caller: AuthToken) -> ABCRPCRequestState:
         request = KafkaProxyRequestState()
-        request.delegation = self.pass_delegation(delegation=delegation, auth=caller)
-        request.udd = Translate.translate_udd(udd=update_data)
         request.callback_topic = callback.get_kafka_topic()
+        request.reservation = self.pass_authority_reservation(reservation=reservation, caller=caller)
         request.caller = caller
         return request
 
-    def _prepare(self, *, reservation: ABCServerReservation, update_data: UpdateData,
-                 callback: ABCCallbackProxy, caller: AuthToken) -> ABCRPCRequestState:
+    def prepare_redeem(self, *, reservation: ABCControllerReservation, callback: KafkaReturn,
+                       caller: AuthToken) -> ABCRPCRequestState:
+        return self._prepare(reservation=reservation, callback=callback, caller=caller)
+
+    def prepare_extend_lease(self, *, reservation: ABCControllerReservation, callback: KafkaReturn,
+                             caller: AuthToken) -> ABCRPCRequestState:
+        return self._prepare(reservation=reservation, callback=callback, caller=caller)
+
+    def prepare_modify_lease(self, *, reservation: ABCControllerReservation, callback: KafkaReturn,
+                             caller: AuthToken) -> ABCRPCRequestState:
+        return self._prepare(reservation=reservation, callback=callback, caller=caller)
+
+    def prepare_poa(self, *, callback: KafkaReturn, caller: AuthToken,
+                    poa: Poa) -> ABCRPCRequestState:
         request = KafkaProxyRequestState()
-        request.reservation = self.pass_reservation(reservation=reservation, auth=caller)
-        request.udd = Translate.translate_udd(udd=update_data)
         request.callback_topic = callback.get_kafka_topic()
+        request.poa = Translate.translate_poa_to_poa_avro(poa=poa)
         request.caller = caller
         return request
 
-    def prepare_update_ticket(self, *, reservation: ABCBrokerReservation, update_data: UpdateData,
-                              callback: ABCCallbackProxy, caller: AuthToken) -> ABCRPCRequestState:
-        return self._prepare(reservation=reservation, update_data=update_data, callback=callback, caller=caller)
-
-    def prepare_update_lease(self, *, reservation: ABCAuthorityReservation, update_data: UpdateData,
-                             callback: ABCCallbackProxy, caller: AuthToken) -> ABCRPCRequestState:
-        return self._prepare(reservation=reservation, update_data=update_data, callback=callback, caller=caller)
+    def prepare_close(self, *, reservation: ABCControllerReservation, callback: KafkaReturn,
+                      caller: AuthToken) -> ABCRPCRequestState:
+        return self._prepare(reservation=reservation, callback=callback, caller=caller)
 
     @staticmethod
-    def pass_reservation(reservation: ABCServerReservation, auth: AuthToken) -> ReservationAvro:
+    def pass_authority_reservation(reservation: ABCReservationMixin, caller: AuthToken) -> ReservationAvro:
+        concrete = reservation.get_resources().get_resources()
+        if concrete is None:
+            raise ProxyException(Constants.NOT_SPECIFIED_PREFIX.format("ticket"))
+
         avro_reservation = ReservationAvro()
         avro_reservation.slice = Translate.translate_slice_to_avro(slice_obj=reservation.get_slice())
-        term = None
-        if reservation.get_term() is None:
-            term = reservation.get_requested_term().clone()
-        else:
-            term = reservation.get_term().clone()
-
-        avro_reservation.term = Translate.translate_term(term=term)
+        avro_reservation.term = Translate.translate_term(term=reservation.get_requested_term())
         avro_reservation.reservation_id = str(reservation.get_reservation_id())
+        avro_reservation.sequence = reservation.get_lease_sequence_out()
 
-        rset = None
-        if reservation.get_resources() is None:
-            from fabric_cf.actor.core.kernel.resource_set import ResourceSet
-            rset = Translate.translate_resource_set(resource_set=ResourceSet(units=0,
-                                                                             rtype=reservation.get_requested_type()))
-        else:
-            rset = Translate.translate_resource_set(resource_set=reservation.get_resources())
-        if reservation.get_resources() is not None:
-            cset = reservation.get_resources().get_resources()
+        rset = Translate.translate_resource_set(resource_set=reservation.get_resources())
 
-            if cset is not None and isinstance(cset, Ticket):
-                rset.ticket = Translate.translate_ticket(ticket=cset)
+        if concrete is not None and isinstance(concrete, Ticket):
+            rset.ticket = Translate.translate_ticket(ticket=concrete)
 
-            if cset is not None and isinstance(cset, UnitSet):
-                rset.unit_set = Translate.translate_unit_set(unit_set=cset)
+        if concrete is not None and isinstance(concrete, UnitSet):
+            rset.unit_set = Translate.translate_unit_set(unit_set=concrete)
 
         avro_reservation.resource_set = rset
-        return avro_reservation
 
-    @staticmethod
-    def pass_delegation(delegation: ABCDelegation, auth: AuthToken) -> DelegationAvro:
-        avro_delegation = Translate.translate_delegation_to_avro(delegation=delegation)
-        avro_delegation.sequence = delegation.get_sequence_out()
-        return avro_delegation
+        return avro_reservation
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/actor_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/services/actor_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,23 +26,25 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
 from fabric_mb.message_bus.messages.reservation_avro import ReservationAvro
 from fabric_mb.message_bus.messages.abc_message_avro import AbcMessageAvro
+from fabric_mb.message_bus.messages.result_poa_avro import ResultPoaAvro
 from fabric_mb.message_bus.messages.update_delegation_avro import UpdateDelegationAvro
 
 from fabric_cf.actor.core.apis.abc_concrete_set import ABCConcreteSet
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import ProxyException
 from fabric_cf.actor.core.delegation.broker_delegation_factory import BrokerDelegationFactory
 from fabric_cf.actor.core.kernel.incoming_delegation_rpc import IncomingDelegationRPC
 from fabric_cf.actor.core.kernel.incoming_failed_rpc import IncomingFailedRPC
+from fabric_cf.actor.core.kernel.incoming_poa_rpc import IncomingPoaRPC
 from fabric_cf.actor.core.kernel.incoming_query_rpc import IncomingQueryRPC
 from fabric_cf.actor.core.kernel.incoming_rpc import IncomingRPC
 from fabric_cf.actor.core.kernel.incoming_reservation_rpc import IncomingReservationRPC
 from fabric_cf.actor.core.kernel.reservation_client import ClientReservationFactory
 from fabric_cf.actor.core.kernel.rpc_manager_singleton import RPCManagerSingleton
 from fabric_cf.actor.core.kernel.rpc_request_type import RPCRequestType
 from fabric_cf.actor.core.proxies.kafka.kafka_retun import KafkaReturn
@@ -81,16 +83,14 @@
         if reservation.resource_set.ticket is not None:
             return Translate.translate_ticket_from_avro(avro_ticket=ticket)
 
         unit_set = reservation.resource_set.unit_set
         if unit_set is not None:
             return Translate.translate_unit_set_from_avro(unit_list=unit_set)
 
-        return None
-
     def pass_client(self, *, reservation: ReservationAvro) -> ABCClientReservation:
         slice_obj = Translate.translate_slice(slice_avro=reservation.slice)
         term = Translate.translate_term_from_avro(term=reservation.term)
 
         resource_set = Translate.translate_resource_set_from_avro(rset=reservation.resource_set)
         resource_set.set_resources(cset=self.get_concrete(reservation=reservation))
 
@@ -98,15 +98,16 @@
                                                term=term, slice_object=slice_obj, actor=self.actor)
 
     def pass_client_delegation(self, *, delegation: DelegationAvro, caller: AuthToken) -> ABCDelegation:
         slice_obj = Translate.translate_slice(slice_avro=delegation.slice)
 
         dlg = BrokerDelegationFactory.create(did=delegation.get_delegation_id(),
                                              slice_id=slice_obj.get_slice_id(),
-                                             broker=None)
+                                             broker=None,
+                                             site=delegation.get_site())
         dlg.restore(actor=self.actor, slice_obj=slice_obj)
 
         site_proxy = ActorRegistrySingleton.get().get_proxy(protocol=Constants.PROTOCOL_KAFKA,
                                                             actor_name=caller.get_name())
         dlg.set_site_proxy(site_proxy=site_proxy)
 
         if delegation.graph is not None:
@@ -142,57 +143,68 @@
             rpc = IncomingQueryRPC(request_type=RPCRequestType.QueryResult, message_id=ID(uid=request.get_message_id()),
                                    query=query, caller=auth_token, request_id=ID(uid=request.request_id))
         except Exception as e:
             self.logger.error("Invalid query_result request: {}".format(e))
             raise e
         self.do_dispatch(rpc=rpc)
 
+    def poa_info(self, *, request: ResultPoaAvro):
+        try:
+            poa = Translate.translate_result_poa_avro_to_poa(poa_result=request)
+            if request.poas is not None and len(request.poas) > 0:
+                poa_info = request.poas[0]
+                auth_token = Translate.translate_auth_from_avro(auth_avro=poa_info.auth)
+            else:
+                auth_token = None
+            rpc = IncomingPoaRPC(message_id=ID(uid=request.message_id), request_type=RPCRequestType.PoaInfo,
+                                 poa=poa, caller=auth_token)
+        except Exception as e:
+            self.logger.error("Invalid update_lease request: {}".format(e))
+            raise e
+        self.do_dispatch(rpc=rpc)
+
     def update_lease(self, *, request: UpdateLeaseAvro):
-        rpc = None
         auth_token = Translate.translate_auth_from_avro(auth_avro=request.auth)
         try:
             rsvn = self.pass_client(reservation=request.reservation)
             udd = Translate.translate_udd_from_avro(udd=request.update_data)
             rpc = IncomingReservationRPC(message_id=ID(uid=request.message_id), request_type=RPCRequestType.UpdateLease,
                                          reservation=rsvn, update_data=udd, caller=auth_token)
         except Exception as e:
             self.logger.error("Invalid update_lease request: {}".format(e))
             raise e
         self.do_dispatch(rpc=rpc)
 
     def update_ticket(self, *, request: UpdateTicketAvro):
-        rpc = None
         auth_token = Translate.translate_auth_from_avro(auth_avro=request.auth)
         try:
             rsvn = self.pass_client(reservation=request.reservation)
             udd = Translate.translate_udd_from_avro(udd=request.update_data)
             rpc = IncomingReservationRPC(message_id=ID(uid=request.message_id),
                                          request_type=RPCRequestType.UpdateTicket, reservation=rsvn, update_data=udd,
                                          caller=auth_token)
         except Exception as e:
             self.logger.error("Invalid update_ticket request: {}".format(e))
             raise e
         self.do_dispatch(rpc=rpc)
 
     def update_delegation(self, *, request: UpdateDelegationAvro):
-        rpc = None
         auth_token = Translate.translate_auth_from_avro(auth_avro=request.auth)
         try:
             dlg = self.pass_client_delegation(delegation=request.delegation, caller=auth_token)
             udd = Translate.translate_udd_from_avro(udd=request.update_data)
             rpc = IncomingDelegationRPC(message_id=ID(uid=request.message_id),
                                         request_type=RPCRequestType.UpdateDelegation, delegation=dlg, update_data=udd,
                                         caller=auth_token)
         except Exception as e:
             self.logger.error("Invalid update_delegation request: {}".format(e))
             raise e
         self.do_dispatch(rpc=rpc)
 
     def failed_rpc(self, *, request: FailedRpcAvro):
-        rpc = None
         auth_token = Translate.translate_auth_from_avro(auth_avro=request.auth)
         try:
             failed_request_type = RPCRequestType(request.request_type)
             if request.reservation_id is not None and request.reservation_id != "":
                 rpc = IncomingFailedRPC(message_id=ID(uid=request.message_id), failed_request_type=failed_request_type,
                                         request_id=request.request_id,
                                         failed_reservation_id=ID(uid=request.reservation_id),
@@ -213,10 +225,12 @@
             self.query_result(request=message)
         elif message.get_message_name() == AbcMessageAvro.update_lease:
             self.update_lease(request=message)
         elif message.get_message_name() == AbcMessageAvro.update_ticket:
             self.update_ticket(request=message)
         elif message.get_message_name() == AbcMessageAvro.update_delegation:
             self.update_delegation(request=message)
+        elif message.get_message_name() == AbcMessageAvro.result_poa:
+            self.poa_info(request=message)
         else:
             self.logger.error("Unsupported message {}".format(message))
             raise ProxyException("Unsupported message {}".format(message.get_message_name()))
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/authority_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/services/authority_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,22 @@
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 from fabric_mb.message_bus.messages.close_avro import CloseAvro
 from fabric_mb.message_bus.messages.extend_lease_avro import ExtendLeaseAvro
 from fabric_mb.message_bus.messages.modify_lease_avro import ModifyLeaseAvro
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fabric_mb.message_bus.messages.redeem_avro import RedeemAvro
 from fabric_mb.message_bus.messages.reservation_avro import ReservationAvro
 from fabric_mb.message_bus.messages.abc_message_avro import AbcMessageAvro
 
 from fabric_cf.actor.core.common.exceptions import ProxyException
 from fabric_cf.actor.core.kernel.authority_reservation import AuthorityReservationFactory
+from fabric_cf.actor.core.kernel.incoming_poa_rpc import IncomingPoaRPC
 from fabric_cf.actor.core.kernel.incoming_reservation_rpc import IncomingReservationRPC
 from fabric_cf.actor.core.kernel.rpc_request_type import RPCRequestType
 from fabric_cf.actor.core.proxies.kafka.translate import Translate
 from fabric_cf.actor.core.proxies.kafka.services.broker_service import BrokerService
 from fabric_cf.actor.core.util.id import ID
 
 if TYPE_CHECKING:
@@ -115,22 +117,34 @@
                                          request_type=RPCRequestType.ModifyLease, reservation=rsvn,
                                          caller=auth_token, callback=callback)
         except Exception as e:
             self.logger.error("Invalid modify_lease request: {}".format(e))
             raise e
         self.do_dispatch(rpc=rpc)
 
+    def poa(self, *, request: PoaAvro):
+        try:
+            poa_obj = Translate.translate_poa_avro_to_poa(poa_avro=request)
+            rpc = IncomingPoaRPC(message_id=ID(uid=request.message_id), request_type=RPCRequestType.Poa,
+                                 poa=poa_obj, caller=request.auth)
+        except Exception as e:
+            self.logger.error("Invalid update_lease request: {}".format(e))
+            raise e
+        self.do_dispatch(rpc=rpc)
+
     def process(self, *, message: AbcMessageAvro):
         if message.get_message_name() == AbcMessageAvro.close:
             self.close(request=message)
         elif message.get_message_name() == AbcMessageAvro.redeem:
             self.redeem(request=message)
         elif message.get_message_name() == AbcMessageAvro.extend_lease:
             self.extend_lease(request=message)
         elif message.get_message_name() == AbcMessageAvro.modify_lease:
             self.modify_lease(request=message)
+        elif message.get_message_name() == AbcMessageAvro.poa:
+            self.poa(request=message)
         elif message.get_message_name() == AbcMessageAvro.result_reservation:
             self.logger.debug("Claim Resources Response receieved: {}".format(message))
         elif message.get_message_name() == AbcMessageAvro.result_delegation:
             self.logger.debug("Claim Delegation Response receieved: {}".format(message))
         else:
             super().process(message=message)
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/broker_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/services/broker_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,16 @@
         result.set_sequence_in(sequence=reservation.sequence)
 
         return result
 
     def pass_agent_delegation(self, *, delegation: DelegationAvro) -> ABCDelegation:
         slice_obj = Translate.translate_slice(slice_avro=delegation.slice)
 
-        result = DelegationFactory.create(did=delegation.get_delegation_id(), slice_id=slice_obj.get_slice_id())
+        result = DelegationFactory.create(did=delegation.get_delegation_id(), slice_id=slice_obj.get_slice_id(),
+                                          site=delegation.get_site())
         result.set_slice_object(slice_object=slice_obj)
         result.set_owner(owner=self.actor.get_identity())
         result.set_sequence_in(value=delegation.sequence)
 
         return result
 
     def ticket(self, *, request: TicketAvro):
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/services/controller_service.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/services/controller_service.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/kafka/translate.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/kafka/translate.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,35 +21,40 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, List, Union
 
 from fabric_mb.message_bus.messages.auth_avro import AuthAvro
 from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
 from fabric_mb.message_bus.messages.broker_query_model_avro import BrokerQueryModelAvro
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
+from fabric_mb.message_bus.messages.poa_info_avro import PoaInfoAvro
 from fabric_mb.message_bus.messages.resource_ticket_avro import ResourceTicketAvro
 from fabric_mb.message_bus.messages.resource_set_avro import ResourceSetAvro
+from fabric_mb.message_bus.messages.result_avro import ResultAvro
+from fabric_mb.message_bus.messages.result_poa_avro import ResultPoaAvro
 from fabric_mb.message_bus.messages.site_avro import SiteAvro
 from fabric_mb.message_bus.messages.slice_avro import SliceAvro
 from fabric_mb.message_bus.messages.term_avro import TermAvro
 from fabric_mb.message_bus.messages.unit_avro import UnitAvro
 from fabric_mb.message_bus.messages.update_data_avro import UpdateDataAvro
 from fabric_mb.message_bus.messages.ticket import Ticket as AvroTicket
 
 from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import ProxyException
 from fabric_cf.actor.core.core.ticket import Ticket
 from fabric_cf.actor.core.core.unit import Unit, UnitState
 from fabric_cf.actor.core.core.unit_set import UnitSet
 from fabric_cf.actor.core.delegation.resource_ticket import ResourceTicket
+from fabric_cf.actor.core.kernel.poa import Poa, PoaFactory
 from fabric_cf.actor.core.kernel.resource_set import ResourceSet
 from fabric_cf.actor.core.kernel.slice import SliceFactory
 from fabric_cf.actor.core.registry.actor_registry import ActorRegistrySingleton
 from fabric_cf.actor.core.container.maintenance import Site
 from fabric_cf.actor.core.time.actor_clock import ActorClock
 from fabric_cf.actor.core.time.term import Term
 from fabric_cf.actor.core.util.id import ID
@@ -300,14 +305,15 @@
 
     @staticmethod
     def translate_delegation_to_avro(*, delegation: ABCDelegation) -> DelegationAvro:
         avro_delegation = DelegationAvro()
         avro_delegation.delegation_id = delegation.get_delegation_id()
         avro_delegation.state = delegation.get_state().value
         avro_delegation.slice = Translate.translate_slice_to_avro(slice_obj=delegation.get_slice_object())
+        avro_delegation.site = delegation.get_site()
         if delegation.get_graph() is not None and not (delegation.is_reclaimed() or delegation.is_closed()):
             avro_delegation.graph = delegation.get_graph().serialize_graph()
         return avro_delegation
 
     @staticmethod
     def translate_to_broker_query_model(*, query_response: dict, level: int) -> BrokerQueryModelAvro:
         bqm = BrokerQueryModelAvro()
@@ -374,7 +380,81 @@
     def translate_unit_set_from_avro(*, unit_list: List[UnitAvro]) -> UnitSet:
         unit_set = UnitSet(plugin=None)
         unit_set.units = {}
         for u in unit_list:
            obj = Translate.translate_unit_from_avro(unit_avro=u)
            unit_set.units[obj.get_id()] = obj
         return unit_set
+
+    @staticmethod
+    def translate_poa_avro_to_poa(*, poa_avro: PoaAvro) -> Union[Poa, None]:
+        if poa_avro is None:
+            return poa_avro
+        if poa_avro.poa_id is None and poa_avro.rid is None:
+            return None
+
+        poa_obj = PoaFactory.create(poa_id=poa_avro.poa_id, operation=poa_avro.get_operation(),
+                                    sliver_id=ID(uid=poa_avro.rid), vcpu_cpu_map=poa_avro.get_vcpu_cpu_map(),
+                                    node_set=poa_avro.get_node_set())
+        poa_obj.sequence_poa_in = poa_avro.sequence
+        poa_obj.slice_id = poa_avro.slice_id
+        # NOTE: Sliver, Slice and Project Info to be set by the caller
+        return poa_obj
+
+    @staticmethod
+    def translate_poa_to_poa_avro(*, poa: Poa) -> Union[PoaAvro, None]:
+        if poa is None:
+            return poa
+
+        auth_avro = Translate.translate_auth_to_avro(auth=poa.get_slice().get_owner())
+        poa_avro = PoaAvro(operation=poa.operation, rid=str(poa.sliver_id), poa_id=poa.poa_id,
+                           vcpu_cpu_map=poa.vcpu_cpu_map, node_set=poa.node_set, auth=auth_avro,
+                           project_id=poa.get_slice().get_project_id(), slice_id=str(poa.get_slice_id()))
+        poa_avro.sequence = poa.sequence_poa_out
+        return poa_avro
+
+    @staticmethod
+    def translate_poa_to_poa_info_avro(*, poa: Poa) -> Union[PoaInfoAvro, None]:
+        if poa is None:
+            return poa
+
+        auth_avro = Translate.translate_auth_to_avro(auth=poa.get_slice().get_owner())
+        poa_avro = PoaInfoAvro(operation=poa.operation, rid=str(poa.sliver_id), poa_id=str(poa.poa_id),
+                               auth=auth_avro, project_id=poa.get_slice().get_project_id(),
+                               slice_id=str(poa.get_slice().get_slice_id()))
+
+        if poa.get_info() is not None:
+            poa_avro.info = poa.get_info().copy()
+        return poa_avro
+
+    @staticmethod
+    def translate_poa_to_result_poa_avro(*, poa: Poa) -> Union[ResultPoaAvro, None]:
+        if poa is None:
+            return poa
+
+        poa_info_avro = Translate.translate_poa_to_poa_info_avro(poa=poa)
+
+        poa_result_avro = ResultPoaAvro()
+        poa_result_avro.status = ResultAvro()
+        poa_result_avro.status.code = poa.get_error_code()
+        poa_result_avro.status.message = poa.get_message()
+        poa_result_avro.poas = [poa_info_avro]
+
+        return poa_result_avro
+
+    @staticmethod
+    def translate_result_poa_avro_to_poa(*, poa_result: ResultPoaAvro) -> Union[Poa, None]:
+        if poa_result is None:
+            return poa_result
+        if poa_result.poas is None or len(poa_result.poas) <= 0:
+            return None
+
+        poa_info = poa_result.poas[0]
+
+        poa_obj = PoaFactory.create(poa_id=poa_info.poa_id, operation=poa_info.get_operation(),
+                                    sliver_id=ID(uid=poa_info.rid))
+        poa_obj.slice_id = poa_info.get_slice_id()
+        poa_obj.error_code = poa_result.get_status().get_code()
+        poa_obj.message = poa_result.get_status().get_message()
+        poa_obj.info = poa_info.get_info()
+
+        return poa_obj
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_authority.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/local_authority.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,25 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
+
 from fabric_cf.actor.core.apis.abc_authority_proxy import ABCAuthorityProxy
 from fabric_cf.actor.core.apis.abc_controller_callback_proxy import ABCControllerCallbackProxy
 from fabric_cf.actor.core.apis.abc_controller_reservation import ABCControllerReservation
 from fabric_cf.actor.core.apis.abc_rpc_request_state import ABCRPCRequestState
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import ProxyException
 from fabric_cf.actor.core.kernel.authority_reservation import AuthorityReservationFactory
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.proxies.local.local_broker import LocalBroker
 from fabric_cf.actor.core.proxies.local.local_proxy import LocalProxy
 from fabric_cf.actor.security.auth_token import AuthToken
 
 
 class LocalAuthority(LocalBroker, ABCAuthorityProxy):
     def _prepare(self, *, reservation: ABCControllerReservation, callback: ABCControllerCallbackProxy,
@@ -52,19 +55,27 @@
                              caller: AuthToken) -> ABCRPCRequestState:
         return self._prepare(reservation=reservation, callback=callback, caller=caller)
 
     def prepare_modify_lease(self, *, reservation: ABCControllerReservation, callback: ABCControllerCallbackProxy,
                              caller: AuthToken) -> ABCRPCRequestState:
         return self._prepare(reservation=reservation, callback=callback, caller=caller)
 
+    def prepare_poa(self, *, callback: ABCControllerCallbackProxy, caller: AuthToken,
+                    poa: Poa) -> ABCRPCRequestState:
+        state = LocalProxy.LocalProxyRequestState()
+        state.poa = poa.clone()
+        state.callback = callback
+        return state
+
     def prepare_close(self, *, reservation: ABCControllerReservation, callback: ABCControllerCallbackProxy,
                       caller: AuthToken) -> ABCRPCRequestState:
         return self._prepare(reservation=reservation, callback=callback, caller=caller)
 
-    def pass_reservation_authority(self, *, reservation: ABCControllerReservation, auth: AuthToken) -> ABCReservationMixin:
+    def pass_reservation_authority(self, *, reservation: ABCControllerReservation,
+                                   auth: AuthToken) -> ABCReservationMixin:
         if reservation.get_resources().get_resources() is None:
             raise ProxyException(Constants.NOT_SPECIFIED_PREFIX.format("concrete set"))
 
         slice_obj = reservation.get_slice().clone_request()
         term = reservation.get_term().clone()
 
         rset = self.abstract_clone_authority(rset=reservation.get_resources())
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_broker.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/local_broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,12 +93,12 @@
         return broker_reservation
 
     def pass_delegation(self, *, delegation: ABCDelegation, auth: AuthToken) -> ABCDelegation:
         slice_obj = delegation.get_slice_object().clone_request()
 
         broker_delegation = BrokerDelegationFactory.create(did=str(delegation.get_delegation_id()),
                                                            slice_id=slice_obj.get_slice_id(),
-                                                           broker=self)
+                                                           broker=self, site=delegation.get_site())
         broker_delegation.set_sequence_in(sequence=delegation.get_sequence_out())
         broker_delegation.set_owner(owner=self.get_identity())
 
         return broker_delegation
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/local_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     class LocalProxyRequestState(RPCRequestState):
         def __init__(self):
             super().__init__()
             self.reservation = None
             self.update_data = None
             self.callback = None
             self.query = None
+            self.poa = None
             self.request_id = None
             self.failed_reservation_id = None
             self.failed_request_type = None
             self.error_detail = None
             self.delegation = None
 
     def __init__(self, *, actor: ABCActorMixin):
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_proxy_factory.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/local_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/local/local_return.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/local/local_return.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,19 +25,20 @@
 # Author: Komal Thareja (kthare10@renci.org)
 from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
 from fabric_cf.actor.core.apis.abc_authority_reservation import ABCAuthorityReservation
 from fabric_cf.actor.core.apis.abc_base_plugin import ABCBasePlugin
 from fabric_cf.actor.core.apis.abc_broker_reservation import ABCBrokerReservation
 from fabric_cf.actor.core.apis.abc_callback_proxy import ABCCallbackProxy
 from fabric_cf.actor.core.apis.abc_controller_callback_proxy import ABCControllerCallbackProxy
-from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation, DelegationState
+from fabric_cf.actor.core.apis.abc_delegation import ABCDelegation
 from fabric_cf.actor.core.apis.abc_rpc_request_state import ABCRPCRequestState
 from fabric_cf.actor.core.apis.abc_reservation_mixin import ABCReservationMixin
 from fabric_cf.actor.core.apis.abc_server_reservation import ABCServerReservation
 from fabric_cf.actor.core.delegation.delegation_factory import DelegationFactory
+from fabric_cf.actor.core.kernel.poa import Poa
 from fabric_cf.actor.core.kernel.reservation_client import ClientReservationFactory
 from fabric_cf.actor.core.kernel.resource_set import ResourceSet
 from fabric_cf.actor.core.proxies.local.local_proxy import LocalProxy
 from fabric_cf.actor.core.util.update_data import UpdateData
 from fabric_cf.actor.security.auth_token import AuthToken
 
 
@@ -70,14 +71,20 @@
                               callback: ABCCallbackProxy, caller: AuthToken) -> ABCRPCRequestState:
         return self._prepare(reservation=reservation, update_data=update_data, callback=callback, caller=caller)
 
     def prepare_update_lease(self, *, reservation: ABCAuthorityReservation, update_data, callback: ABCCallbackProxy,
                              caller: AuthToken) -> ABCRPCRequestState:
         return self._prepare(reservation=reservation, update_data=update_data, callback=callback, caller=caller)
 
+    def prepare_poa_result(self, *, poa: Poa, callback: ABCCallbackProxy, caller: AuthToken) -> ABCRPCRequestState:
+        state = LocalProxy.LocalProxyRequestState()
+        state.poa = poa.clone()
+        state.callback = callback
+        return state
+
     @staticmethod
     def pass_reservation(*, reservation: ABCServerReservation, plugin: ABCBasePlugin) -> ABCReservationMixin:
         slice_obj = reservation.get_slice().clone_request()
         term = None
 
         if reservation.get_term() is None:
             term = reservation.get_requested_term().clone()
@@ -110,13 +117,14 @@
             return controller_reservation
 
     @staticmethod
     def pass_delegation(*, delegation: ABCDelegation) -> ABCDelegation:
         slice_obj = delegation.get_slice_object().clone_request()
 
         delegation_new = DelegationFactory.create(did=delegation.get_delegation_id(),
-                                                  slice_id=delegation.get_slice_id())
+                                                  slice_id=delegation.get_slice_id(),
+                                                  site=delegation.get_site())
         delegation_new.set_slice_object(slice_object=slice_obj)
         # TODO
         if not delegation.is_reclaimed():
             delegation_new.set_graph(delegation.get_graph())
         return delegation_new
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/proxies/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
                 ActorRegistrySingleton.get().register_proxy(proxy=proxy_reload_from_db)
         return proxy_reload_from_db
 
     @staticmethod
     def decode(*, encoded, plugin: ABCBasePlugin) -> ABCConcreteSet:
         try:
             decoded_resource = pickle.loads(encoded)
-            print("Decoded object is of type={}".format(type(decoded_resource)))
             decoded_resource.restore(plugin=plugin, reservation=None)
             return decoded_resource
         except Exception as e:
             traceback.print_exc()
             print("Exception occurred while decoding {}".format(e))
         return None
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/proxies/proxy_factory.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/authority_substrate_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,59 +19,24 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-from fabric_cf.actor.core.common.exceptions import ProxyException
-from fabric_cf.actor.core.proxies.kafka.kafka_proxy_factory import KafkaProxyFactory
-from fabric_cf.actor.core.common.constants import Constants
-from fabric_cf.actor.core.proxies.local.local_proxy_factory import LocalProxyFactory
-
-if TYPE_CHECKING:
-    from fabric_cf.actor.core.apis.abc_actor_identity import ABCActorIdentity
-    from fabric_cf.actor.core.proxies.actor_location import ActorLocation
-
-
-class ProxyFactory:
-    def __init__(self):
-        self.factories = {}
-        self.load_factories()
-
-    def load_factories(self):
-        self.factories[Constants.PROTOCOL_LOCAL] = LocalProxyFactory()
-        self.factories[Constants.PROTOCOL_KAFKA] = KafkaProxyFactory()
-
-    def new_callback(self, *, protocol: str, identity: ABCActorIdentity, location: ActorLocation):
-        if protocol in self.factories:
-            factory = self.factories[protocol]
-            return factory.new_callback(identity=identity, location=location)
-        return None
-
-    def new_proxy(self, *, protocol: str, identity: ABCActorIdentity, location: ActorLocation, proxy_type: str = None):
-        if protocol in self.factories:
-            factory = self.factories[protocol]
-            return factory.new_proxy(identity=identity, location=location, proxy_type=proxy_type)
-        return None
-
-
-class ProxyFactorySingleton:
-    __instance = None
-
-    def __init__(self):
-        if self.__instance is not None:
-            raise ProxyException("Singleton can't be created twice !")
-
-    def get(self):
-        """
-        Actually create an instance
-        """
-        if self.__instance is None:
-            self.__instance = ProxyFactory()
-        return self.__instance
-
-    get = classmethod(get)
-
+from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
+from fabric_cf.actor.core.core.authority import Authority
+from fabric_cf.actor.core.time.term import Term
+from fabric_cf.actor.core.util.id import ID
+from fabric_cf.actor.test.base_test_case import BaseTestCase
+from fabric_cf.actor.test.core.plugins.substrate_test_base import SubstrateTestBase
+
+
+class AuthoritySubstrateTest(SubstrateTestBase):
+    def get_actor_instance(self) -> ABCActorMixin:
+        return Authority()
+
+    def get_authority(self, name: str = BaseTestCase.authority_name, guid: ID = BaseTestCase.authority_guid):
+        authority = self.get_registered_new_actor()
+        authority.set_recovered(value=True)
+        Term.set_clock(clock=authority.get_actor_clock())
+        return authority
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/actor_registry.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/registry/actor_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/callback_registry.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/registry/callback_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/peer_registry.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/registry/peer_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/registry/proxy_registry.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/registry/proxy_registry.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/actor_clock.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/time/actor_clock.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/authority_calendar.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/authority_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/base_calendar.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/base_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/broker_calendar.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/broker_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/client_calendar.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/client_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/controller_calendar.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/controller_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/calendar/source_calendar.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/time/calendar/source_calendar.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/time/term.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/time/term.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/bids.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/bids.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/client.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/client.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/graceful_interrupt_handler.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/graceful_interrupt_handler.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/id.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/id.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/iterable_queue.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/iterable_queue.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/kernel_timer.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/kernel_timer.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/log_helper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/log_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/notice.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/notice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reflection_utils.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/reflection_utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_holdings.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/reservation_holdings.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_list.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/reservation_list.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_set.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/reservation_set.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/reservation_state.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/reservation_state.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/resource_type.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/resource_type.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/rpc_exception.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/rpc_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/update_data.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/update_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/core/util/utils.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/core/util/utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/db/__init__.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/db/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -187,7 +187,29 @@
     Represents Sites Database Table
     """
     __tablename__ = 'Sites'
     site_id = Column(Integer, Sequence('site_id', start=1, increment=1), autoincrement=True, primary_key=True)
     name = Column(String, index=True)
     state = Column(Integer, nullable=False)
     properties = Column(LargeBinary)
+
+
+class Poas(Base):
+    """
+    Represents Poas Database Table
+    """
+    __tablename__ = 'Poas'
+    poa_id = Column(Integer, Sequence('poa_id', start=1, increment=1), autoincrement=True, primary_key=True)
+    poa_guid = Column(String, nullable=False, index=True)
+    email = Column(String, nullable=True, index=True)
+    project_id = Column(String, nullable=True, index=True)
+    sliver_id = Column(String, nullable=True, index=True)
+    state = Column(Integer, nullable=False, index=True)
+    slice_id = Column(String, nullable=True, index=True)
+    last_update_time = Column(TIMESTAMP, nullable=True)
+    properties = Column(LargeBinary)
+
+    Index('idx_poa_guid_email', poa_guid, email)
+    Index('idx_poa_guid_project_id', poa_guid, project_id)
+    Index('idx_poa_guid_sliver_id', poa_guid, sliver_id)
+    Index('idx_poa_guid_email_sliver_id', poa_guid, email, sliver_id)
+    Index('idx_poa_guid_email_project_id', poa_guid, email, project_id)
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/db/psql_database.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/db/psql_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 from sqlalchemy import create_engine, desc
 from sqlalchemy.orm import scoped_session, sessionmaker
 
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.common.exceptions import DatabaseException
 from fabric_cf.actor.db import Base, Clients, ConfigMappings, Proxies, Units, Reservations, Slices, ManagerObjects, \
-    Miscellaneous, Actors, Delegations, Sites
+    Miscellaneous, Actors, Delegations, Sites, Poas
 
 
 @contextmanager
 def session_scope(psql_db_engine):
     """Provide a transactional scope around a series of operations."""
     session = scoped_session(sessionmaker(psql_db_engine))
     try:
@@ -100,14 +100,16 @@
             session.query(Units).delete()
             session.query(Delegations).delete()
             session.query(Reservations).delete()
             session.query(Slices).delete()
             session.query(ManagerObjects).delete()
             session.query(Miscellaneous).delete()
             session.query(Actors).delete()
+            session.query(Sites).delete()
+            session.query(Poas).delete()
             session.commit()
         except Exception as e:
             session.rollback()
             self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
             raise e
 
     def add_actor(self, *, name: str, guid: str, act_type: int, properties):
@@ -1147,14 +1149,15 @@
 
     def update_delegation(self, *, dlg_graph_id: str, dlg_state: int, properties, site: str = None):
         """
         Update delegation
         @param dlg_graph_id graph id
         @param dlg_state state
         @param properties properties
+        @param site site
         """
         session = self.get_session()
         try:
             dlg_obj = session.query(Delegations).filter_by(dlg_graph_id=dlg_graph_id).one_or_none()
             if dlg_obj is not None:
                 dlg_obj.dlg_state = dlg_state
                 dlg_obj.properties = properties
@@ -1320,14 +1323,143 @@
     def generate_dict_from_row(row):
         d = row.__dict__.copy()
         for k in row.__dict__:
             if d[k] is None:
                 d.pop(k)
         return d
 
+    def add_poa(self, *, poa_guid: str, properties, email: str, project_id: str, sliver_id: str, slice_id: str,
+                state: int):
+        """
+        Add a POA
+        @param poa_guid POA id
+        @param properties pickled instance
+        @param project_id User OIDC Sub
+        @param email User Email
+        @param sliver_id Sliver Id
+        @param slice_id slice id
+        @param state state
+        """
+        session = self.get_session()
+        try:
+            poa_obj = Poas(poa_guid=poa_guid, project_id=project_id, email=email, sliver_id=sliver_id,
+                           slice_id=slice_id, state=state,last_update_time=datetime.now(timezone.utc),
+                           properties=properties)
+            session.add(poa_obj)
+            session.commit()
+        except Exception as e:
+            session.rollback()
+            self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
+            raise e
+
+    def update_poa(self, *, poa_guid: str, properties, state: int, email: str = None, project_id: str = None,
+                   sliver_id: str = None):
+        """
+        Update a POA
+        @param poa_guid POA id
+        @param properties pickled instance
+        @param state state
+        @param project_id User OIDC Sub
+        @param email User Email
+        @param sliver_id Sliver Id
+        """
+        session = self.get_session()
+        try:
+            poa_obj = session.query(Poas).filter_by(poa_guid=poa_guid).one_or_none()
+            if poa_obj is not None:
+                poa_obj.properties = properties
+                if email is not None:
+                    poa_obj.email = email
+                if project_id is not None:
+                    poa_obj.project_id = project_id
+                if sliver_id is not None:
+                    poa_obj.sliver_id = sliver_id
+                poa_obj.last_update_time = datetime.now(timezone.utc)
+                poa_obj.state = state
+            else:
+                raise DatabaseException(self.OBJECT_NOT_FOUND.format("Poa", poa_guid))
+            session.commit()
+        except Exception as e:
+            session.rollback()
+            self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
+            raise e
+
+    def remove_poa(self, *, poa_guid: str):
+        """
+        Remove POA
+        @param poa_guid POA Guid
+        """
+        session = self.get_session()
+        try:
+            session.query(Poas).filter_by(poa_guid=poa_guid).delete()
+            session.commit()
+        except Exception as e:
+            session.rollback()
+            self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
+            raise e
+
+    @staticmethod
+    def create_poa_filter(*, poa_guid: str = None, sliver_id: str = None, project_id: str = None,
+                          email: str = None, slice_id: str = None) -> dict:
+
+        filter_dict = {}
+        if poa_guid is not None:
+            filter_dict['poa_guid'] = poa_guid
+        if sliver_id is not None:
+            filter_dict['sliver_id'] = str(sliver_id)
+        if slice_id is not None:
+            filter_dict['slice_id'] = str(slice_id)
+        if project_id is not None:
+            filter_dict['project_id'] = project_id
+        if email is not None:
+            filter_dict['email'] = email
+        return filter_dict
+
+    def get_poas(self, *, poa_guid: str = None, project_id: str = None, email: str = None, sliver_id: str = None,
+                 slice_id: str, limit: int = None, offset: int = None, last_update_time: datetime = None,
+                 states: list[int] = None) -> List[dict]:
+        """
+        Get slices for an actor
+        @param poa_guid POA Guid
+        @param project_id project id
+        @param email email
+        @param limit limit
+        @param offset offset
+        @param sliver_id Sliver Id
+        @param slice_id Slice Id
+        @param last_update_time Last Update Time
+        @param states
+        @return list of POAs
+        """
+        result = []
+        session = self.get_session()
+        try:
+            filter_dict = self.create_poa_filter(poa_guid=poa_guid, project_id=project_id, email=email,
+                                                 sliver_id=sliver_id, slice_id=slice_id)
+
+            rows = session.query(Poas).filter_by(**filter_dict)
+
+            if last_update_time is not None:
+                rows = rows.filter(Poas.last_update_time < last_update_time)
+
+            if states is not None:
+                rows = rows.filter(Poas.state.in_(states))
+
+            rows = rows.order_by(desc(Poas.last_update_time))
+
+            if offset is not None and limit is not None:
+                rows = rows.offset(offset).limit(limit)
+
+            for row in rows.all():
+                result.append(self.generate_dict_from_row(row=row))
+        except Exception as e:
+            self.logger.error(Constants.EXCEPTION_OCCURRED.format(e))
+            raise e
+        return result
+
 
 def test():
     logger = logging.getLogger('PsqlDatabase')
     db = PsqlDatabase(user='fabric', password='fabric', database='am', db_host='127.0.0.1:5432', logger=logger)
     db.create_db()
     db.reset_db()
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/fim/asm_update_thread.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/fim/asm_update_thread.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/fim/fim_helper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/fim/fim_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/fim/plugins/broker/aggregate_bqm_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import uuid
 
 from fim.graph.abc_property_graph import ABCPropertyGraph, PropertyGraphQueryException
 from fim.graph.resources.abc_cbm import ABCCBMPropertyGraph
 from fim.graph.resources.abc_bqm import ABCBQMPropertyGraph
 from fim.graph.networkx_property_graph import NetworkXGraphImporter
 from fim.graph.resources.networkx_abqm import NetworkXAggregateBQM
-from fim.slivers.capacities_labels import Capacities
+from fim.slivers.capacities_labels import Capacities, Flags
 from fim.slivers.delegations import DelegationFormat
 from fim.slivers.maintenance_mode import MaintenanceInfo, MaintenanceEntry, MaintenanceState
 from fim.slivers.network_node import CompositeNodeSliver, NodeType
 from fim.slivers.attached_components import ComponentSliver, ComponentType
 from fim.slivers.interface_info import InterfaceType
 from fim.slivers.network_service import ServiceType
 
@@ -133,14 +133,15 @@
         :param kwargs:
         :return:
         """
         if kwargs.get('query_level', None) is None or kwargs['query_level'] != 1:
             return cbm.clone_graph(new_graph_id=str(uuid.uuid4()))
 
         # do a one-pass aggregation of servers, their components and interfaces
+        # and some flags (e.g. PTP availability)
         # this includes facilities
         nnodes = cbm.get_all_nodes_by_class(label=ABCPropertyGraph.CLASS_NetworkNode)
         slivers_by_site = defaultdict(list)
         for n in nnodes:
             # build deep slivers for each advertised server, aggregate by site
             node_sliver = cbm.build_deep_node_sliver(node_id=n)
             slivers_by_site[node_sliver.site].append(node_sliver)
@@ -168,14 +169,15 @@
             # available components organized by [type][model]
             site_comps_by_type = defaultdict(dict)
             # occupied component capacities organized by [type][model] into lists (by server)
             site_allocated_comps_caps_by_type = defaultdict(dict)
             site_sliver.maintenance_info = self.__site_maintenance_info(site_name=s)
 
             loc = None
+            ptp = False
             for sliver in ls:
                 if sliver.get_type() != NodeType.Server:
                     # skipping NAS, Facility and dataplane switches
                     if sliver.get_type() == NodeType.Facility:
                         # keep track of facilities for each site
                         facilities_by_site[s].append(sliver)
                     continue
@@ -187,14 +189,19 @@
                     allocated_caps, allocated_comp_caps = self.__occupied_node_capacity(node_id=sliver.node_id)
                     site_sliver.capacity_allocations = site_sliver.capacity_allocations + allocated_caps
 
                 # get the location if available
                 if loc is None:
                     loc = sliver.get_location()
 
+                # look at flags
+                flags = sliver.get_flags()
+                if flags and not ptp and flags.ptp:
+                    ptp = True
+
                 # calculate available node capacities based on delegations
                 if sliver.get_capacity_delegations() is not None:
                     # CBM only has one delegation if it has one
                     _, delegation = sliver.get_capacity_delegations().get_sole_delegation()
                     # FIXME: skip pool definitions and references for now
                     if delegation.get_format() == DelegationFormat.SinglePool:
                         site_sliver.capacities = site_sliver.capacities + \
@@ -217,14 +224,15 @@
                     if site_comps_by_type[rt].get(rm) is None:
                         site_comps_by_type[rt][rm] = list()
                     site_comps_by_type[rt][rm].append(comp)
 
             # set location to whatever is available
             site_sliver.set_location(loc)
             site_sliver.set_site(s)
+            site_sliver.set_flags(Flags(ptp=ptp))
 
             # create a Composite node for every site
             site_to_composite_node_id[s] = site_sliver.node_id
             site_props = abqm.node_sliver_to_graph_properties_dict(site_sliver)
             abqm.add_node(node_id=site_sliver.node_id, label=ABCPropertyGraph.CLASS_CompositeNode,
                           props=site_props)
             # add a network service
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/handlers/handler_base.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/handlers/handler_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,8 +76,14 @@
         Delete
         """
 
     @abstractmethod
     def clean_restart(self):
         """
         Clean Restart - delete all existing VMs before start
-        """
+        """
+
+    @abstractmethod
+    def poa(self, unit: ConfigToken, data: dict) -> Tuple[dict, ConfigToken]:
+        """
+        POA - perform operational action on a VM
+        """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/handlers/no_op_handler.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/handlers/no_op_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -186,7 +186,36 @@
                       Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
         finally:
             self.get_logger().info(f"Modify completed")
         return result, unit
 
     def clean_restart(self):
         pass
+
+    def poa(self, unit: ConfigToken, data: dict) -> Tuple[dict, ConfigToken]:
+        print(f"KOMAL AM handler {data}")
+        result = None
+        try:
+            self.get_logger().info(f"POA invoked for unit: {unit}")
+
+            result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_POA,
+                      Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_OK,
+                      Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0,
+                      Constants.PROPERTY_POA_INFO: {
+                          "operation": data.get("operation"),
+                          "poa_id": data.get("poa_id"),
+                          "code": Constants.RESULT_CODE_OK,
+                          "info": {"cpu_info": {"uky-w1.fabric-tested.net": {"value": {"a": "b"},
+                                                                             "pinned_cpus": ["1", "2"]},
+                                                "instance-1111": {"value": {"a": "b"}}},
+                                   "numa_info": {"uky-w1.fabric-tested.net": {"value": {"a": "b"}},
+                                                 "instance-1111": {"value": {"a": "b"}}}}
+                      }}
+        except Exception as e:
+            self.get_logger().error(e)
+            self.get_logger().error(traceback.format_exc())
+            result = {Constants.PROPERTY_TARGET_NAME: Constants.TARGET_POA,
+                      Constants.PROPERTY_TARGET_RESULT_CODE: Constants.RESULT_CODE_EXCEPTION,
+                      Constants.PROPERTY_ACTION_SEQUENCE_NUMBER: 0}
+        finally:
+            self.get_logger().info(f"Modify completed")
+        return result, unit
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/security/access_checker.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/security/access_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/security/auth_token.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/security/auth_token.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/security/fabric_token.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/security/fabric_token.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/security/pdp_auth.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/security/pdp_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,15 @@
     close = 11
     claim = 12
     reclaim = 13
     ticket = 14
     extend = 15
     relinquish = 16
     accept = 17
+    poa = 18
 
     def __str__(self):
         return self.name
 
 
 class PdpAuth:
     """
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/base_test_case.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/client_callback_helper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/client_callback_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.jenkins.yaml` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/config/config.jenkins.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.orchestrator.yaml` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/config/config.orchestrator.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/config/config.test.yaml` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/config/config.test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/controller_callback_helper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/controller_callback_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/container/container_database_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/container/container_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/core/unit_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/core/unit_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/kernel/kernel_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/kernel/kernel_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/kernel/tick_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/kernel/tick_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/actor_database_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/actor_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/ansible_handler_processor_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/authority_substrate_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/substrate_test_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,24 +19,33 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-from fabric_cf.actor.core.apis.abc_actor_mixin import ABCActorMixin
-from fabric_cf.actor.core.core.authority import Authority
-from fabric_cf.actor.core.time.term import Term
-from fabric_cf.actor.core.util.id import ID
+import unittest
+import time
+from fabric_cf.actor.core.apis.abc_database import ABCDatabase
+from fabric_cf.actor.core.common.constants import Constants
+from fabric_cf.actor.core.plugins.substrate.db.substrate_actor_database import SubstrateActorDatabase
 from fabric_cf.actor.test.base_test_case import BaseTestCase
-from fabric_cf.actor.test.core.plugins.substrate_test_base import SubstrateTestBase
 
 
-class AuthoritySubstrateTest(SubstrateTestBase):
-    def get_actor_instance(self) -> ABCActorMixin:
-        return Authority()
+class SubstrateTestBase(BaseTestCase, unittest.TestCase):
+    from fabric_cf.actor.core.container.globals import Globals
+    Globals.config_file = "./config/config.test.yaml"
+    Constants.SUPERBLOCK_LOCATION = './state_recovery.lock'
 
-    def get_authority(self, name: str = BaseTestCase.authority_name, guid: ID = BaseTestCase.authority_guid):
-        authority = self.get_registered_new_actor()
-        authority.set_recovered(value=True)
-        Term.set_clock(clock=authority.get_actor_clock())
-        return authority
+    from fabric_cf.actor.core.container.globals import GlobalsSingleton
+    GlobalsSingleton.get().start(force_fresh=True)
+    while not GlobalsSingleton.get().start_completed:
+        time.sleep(0.0001)
+
+    def make_actor_database(self) -> ABCDatabase:
+        db = SubstrateActorDatabase(user=self.db_user, password=self.db_pwd, database=self.db_name, db_host=self.db_host,
+                                    logger=self.logger)
+        return db
+
+    def test_actor(self):
+        actor = self.get_actor()
+        self.assertIsNotNone(actor)
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/substrate_database_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/plugins/substrate_database_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/plugins/substrate_test_base.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/watch_entry.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,33 +19,18 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-import unittest
-import time
-from fabric_cf.actor.core.apis.abc_database import ABCDatabase
-from fabric_cf.actor.core.common.constants import Constants
-from fabric_cf.actor.core.plugins.substrate.db.substrate_actor_database import SubstrateActorDatabase
-from fabric_cf.actor.test.base_test_case import BaseTestCase
+from fabric_cf.actor.core.util.id import ID
+from fabric_cf.orchestrator.core.i_status_update_callback import IStatusUpdateCallback
 
 
-class SubstrateTestBase(BaseTestCase, unittest.TestCase):
-    from fabric_cf.actor.core.container.globals import Globals
-    Globals.config_file = "./config/config.test.yaml"
-    Constants.SUPERBLOCK_LOCATION = './state_recovery.lock'
+class WatchEntry:
+    def __init__(self, *, watch: ID, callback: IStatusUpdateCallback):
+        self.reservation_to_watch = watch
+        self.callback = callback
 
-    from fabric_cf.actor.core.container.globals import GlobalsSingleton
-    GlobalsSingleton.get().start(force_fresh=True)
-    while not GlobalsSingleton.get().start_completed:
-        time.sleep(0.0001)
-
-    def make_actor_database(self) -> ABCDatabase:
-        db = SubstrateActorDatabase(user=self.db_user, password=self.db_pwd, database=self.db_name, db_host=self.db_host,
-                                    logger=self.logger)
-        return db
-
-    def test_actor(self):
-        actor = self.get_actor()
-        self.assertIsNotNone(actor)
+    def __str__(self):
+        return f"watch: {self.reservation_to_watch} callback: {self.callback}"
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/authoity_calendar_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/broker_simpler_units_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/controller_simple_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/controller_simple_policy_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_test_wrapper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/controller_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/policy/controller_ticket_review_policy_test_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/actor_clock_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/time/actor_clock_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/time/calendar/client_calendar_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/time/calendar/controller_calendar_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/time/term_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/time/term_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/util/reservation_holdings_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/util/reservation_holdings_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/core/util/reservation_list_test.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/core/util/reservation_list_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/dummy_authority_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/dummy_authority_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/dummy_proxy.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/dummy_proxy.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/fim_test_helper.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/fim_test_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/schema/message.avsc` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/schema/message.avsc`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/test_abqm.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/test_abqm.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/test_actor.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/test_actor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/actor/test/test_exception.py` & `fabric_cf-1.5.0b4/fabric_cf/actor/test/test_exception.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/aits/config/config.broker.yaml` & `fabric_cf-1.5.0b4/fabric_cf/aits/config/config.broker.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/aits/config/config.netam.yaml` & `fabric_cf-1.5.0b4/fabric_cf/aits/config/config.netam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/aits/config/config.orchestrator.yaml` & `fabric_cf-1.5.0b4/fabric_cf/aits/config/config.orchestrator.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/aits/config/config.siteam.yaml` & `fabric_cf-1.5.0b4/fabric_cf/aits/config/config.siteam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/aits/integration_test.py` & `fabric_cf-1.5.0b4/fabric_cf/aits/integration_test.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/aits/kafka_processor.py` & `fabric_cf-1.5.0b4/fabric_cf/aits/kafka_processor.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/aits/manage_helper.py` & `fabric_cf-1.5.0b4/fabric_cf/aits/manage_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/aits/orchestrator_helper.py` & `fabric_cf-1.5.0b4/fabric_cf/aits/orchestrator_helper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/Readme.md` & `fabric_cf-1.5.0b4/fabric_cf/authority/Readme.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/__main__.py` & `fabric_cf-1.5.0b4/fabric_cf/authority/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/am-yes.xml` & `fabric_cf-1.5.0b4/fabric_cf/authority/am-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/config.al2s.am.yaml` & `fabric_cf-1.5.0b4/fabric_cf/authority/config.al2s.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/config.net.am.yaml` & `fabric_cf-1.5.0b4/fabric_cf/authority/config.net.am.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/config.site.am.geni.yaml` & `fabric_cf-1.5.0b4/fabric_cf/authority/config.site.am.geni.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
   ## The filename to be used for actor's log file.
   log-file: actor.log
 
   handler-log-file: handler.log
 
   ## The default log level for actor.
-  log-level: DEBUG
+  log-level: INFO
 
   ## actor rotates log files. You may specify how many archived log files to keep here.
   log-retain: 5
 
   ## actor rotates log files after they exceed a certain size.
   ## You may specify the file size that results in a log file being rotated here.
   log-size: 5000000
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/config.site.am.yaml` & `fabric_cf-1.5.0b4/fabric_cf/authority/config.site.am.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
   ## The filename to be used for actor's log file.
   log-file: actor.log
 
   handler-log-file: handler.log
 
   ## The default log level for actor.
-  log-level: DEBUG
+  log-level: INFO
 
   ## actor rotates log files. You may specify how many archived log files to keep here.
   log-retain: 5
 
   ## actor rotates log files after they exceed a certain size.
   ## You may specify the file size that results in a log file being rotated here.
   log-size: 5000000
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/docker-compose.geni.yml` & `fabric_cf-1.5.0b4/fabric_cf/authority/docker-compose.geni.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/docker-compose.yml` & `fabric_cf-1.5.0b4/fabric_cf/authority/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/env.template` & `fabric_cf-1.5.0b4/fabric_cf/authority/env.template`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml` & `fabric_cf-1.5.0b4/fabric_cf/authority/fabricYes.AnyActorYesPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/net_handler_config.yml` & `fabric_cf-1.5.0b4/fabric_cf/authority/net_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/oess_handler_config.yml` & `fabric_cf-1.5.0b4/fabric_cf/authority/oess_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/pdp.xml` & `fabric_cf-1.5.0b4/fabric_cf/authority/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/setup.sh` & `fabric_cf-1.5.0b4/fabric_cf/authority/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/test/al2s_am.py` & `fabric_cf-1.5.0b4/fabric_cf/authority/test/al2s_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/test/net_am.py` & `fabric_cf-1.5.0b4/fabric_cf/authority/test/net_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/test/site_am.py` & `fabric_cf-1.5.0b4/fabric_cf/authority/test/site_am.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/test/site_am_geni.py` & `fabric_cf-1.5.0b4/fabric_cf/authority/test/site_am_geni.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/test/test-al2sam.yaml` & `fabric_cf-1.5.0b4/fabric_cf/authority/test/test-al2sam.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 # After making modifications to this file, please restart actor to re-read it.
 
 # This file is a sample; to alter a particular value, uncomment it, and set as desired.
 # actor will use sane defaults, in the absence of this configuration file.
 
 runtime:
-  kafka-server: localhost:9092
+  kafka-server: localhost:19092
   kafka-schema-registry-url: http://0.0.0.0:8081
   kafka-key-schema: ../../../schema/key.avsc
   kafka-value-schema: ../../../schema/message.avsc
   kafka-ssl-ca-location:
   kafka-ssl-certificate-location:
   kafka-ssl-key-location:
   kafka-ssl-key-password:
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/test/test-netam.yaml` & `fabric_cf-1.5.0b4/fabric_cf/authority/test/test-netam.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/test/test.geni.yaml` & `fabric_cf-1.5.0b4/fabric_cf/authority/test/test.geni.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/test/test.yaml` & `fabric_cf-1.5.0b4/fabric_cf/authority/test/test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/vm_handler_config.yml` & `fabric_cf-1.5.0b4/fabric_cf/authority/vm_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/authority/vnic_net_handler_config.yml` & `fabric_cf-1.5.0b4/fabric_cf/authority/vnic_net_handler_config.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/Readme.md` & `fabric_cf-1.5.0b4/fabric_cf/broker/Readme.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/__main__.py` & `fabric_cf-1.5.0b4/fabric_cf/broker/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/broker-yes.xml` & `fabric_cf-1.5.0b4/fabric_cf/broker/broker-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/config.broker.yaml` & `fabric_cf-1.5.0b4/fabric_cf/broker/config.broker.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
   ## This directory will be automatically created if it does not exist.
   log-directory: /var/log/actor
 
   ## The filename to be used for actor's log file.
   log-file: actor.log
 
   ## The default log level for actor.
-  log-level: DEBUG
+  log-level: INFO
 
   ## actor rotates log files. You may specify how many archived log files to keep here.
   log-retain: 5
 
   ## actor rotates log files after they exceed a certain size.
   ## You may specify the file size that results in a log file being rotated here.
   log-size: 5000000
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/core/broker_kernel.py` & `fabric_cf-1.5.0b4/fabric_cf/broker/core/broker_kernel.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/docker-compose.yml` & `fabric_cf-1.5.0b4/fabric_cf/broker/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/env.template` & `fabric_cf-1.5.0b4/fabric_cf/broker/env.template`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml` & `fabric_cf-1.5.0b4/fabric_cf/broker/fabricYes.AnyActorYesPolicy.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/pdp.xml` & `fabric_cf-1.5.0b4/fabric_cf/broker/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/setup.sh` & `fabric_cf-1.5.0b4/fabric_cf/broker/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/test/broker.py` & `fabric_cf-1.5.0b4/fabric_cf/broker/test/broker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/broker/test/test.yaml` & `fabric_cf-1.5.0b4/fabric_cf/broker/test/test.yaml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/README.md` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/README.md`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/__main__.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/__main__.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/certs/fullchain.pem` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/certs/fullchain.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/certs/privkey.pem` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/certs/privkey.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/config.orchestrator.yaml` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/config.orchestrator.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
   ## This directory will be automatically created if it does not exist.
   log-directory: /var/log/actor
 
   ## The filename to be used for actor's log file.
   log-file: actor.log
 
   ## The default log level for actor.
-  log-level: DEBUG
+  log-level: INFO
 
   ## actor rotates log files. You may specify how many archived log files to keep here.
   log-retain: 5
 
   ## actor rotates log files after they exceed a certain size.
   ## You may specify the file size that results in a log file being rotated here.
   log-size: 5000000
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/active_status_checker.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/active_status_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/bqm_wrapper.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/bqm_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/exceptions.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/i_status_update_callback.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/i_status_update_callback.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_handler.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/orchestrator_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 import time
 import traceback
 from datetime import datetime, timedelta, timezone
 from http.client import NOT_FOUND, BAD_REQUEST, UNAUTHORIZED
-from typing import List
+from typing import List, Dict
 
 from fabric_mb.message_bus.messages.auth_avro import AuthAvro
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
 from fabric_mb.message_bus.messages.reservation_mng import ReservationMng
 from fabric_mb.message_bus.messages.slice_avro import SliceAvro
 from fim.graph.networkx_property_graph_disjoint import NetworkXGraphImporterDisjoint
 from fim.slivers.base_sliver import BaseSliver
 from fim.slivers.network_service import NetworkServiceSliver
 from fim.user import GraphFormat
 from fim.user.topology import ExperimentTopology
@@ -234,14 +235,16 @@
             fabric_token = self.__authorize_request(id_token=token, action_id=ActionId.create, resource=topology,
                                                     lease_end_time=end_time)
             self.logger.info(f"PDP authorize: TIME= {time.time() - create_ts:.0f}")
 
             # Check if an Active slice exists already with the same name for the user
             create_ts = time.time()
             project, tags, project_name = fabric_token.get_first_project()
+            if tags is not None and isinstance(tags, list):
+                tags = ','.join(tags)
             existing_slices = controller.get_slices(slice_name=slice_name,
                                                     email=fabric_token.get_email(), project=project)
             self.logger.info(f"GET slices: TIME= {time.time() - create_ts:.0f}")
 
             if existing_slices is not None and len(existing_slices) != 0:
                 for es in existing_slices:
                     slice_state = SliceState(es.get_state())
@@ -256,15 +259,15 @@
             slice_obj = SliceAvro()
             slice_obj.set_slice_name(slice_name)
             slice_obj.set_client_slice(True)
             slice_obj.set_description("Description")
             slice_obj.graph_id = asm_graph.get_graph_id()
             slice_obj.set_config_properties(value={Constants.USER_SSH_KEY: ssh_key,
                                                    Constants.PROJECT_ID: project,
-                                                   Constants.TAGS: ','.join(tags),
+                                                   Constants.TAGS: tags,
                                                    Constants.CLAIMS_EMAIL: fabric_token.get_email()})
             slice_obj.set_lease_end(lease_end=end_time)
             auth = AuthAvro()
             auth.name = self.controller_state.get_management_actor().get_name()
             auth.guid = self.controller_state.get_management_actor().get_guid()
             auth.oidc_sub_claim = fabric_token.get_uuid()
             auth.email = fabric_token.get_email()
@@ -320,34 +323,39 @@
         finally:
             if topology is not None and topology.graph_model is not None:
                 topology.graph_model.delete_graph()
             if new_slice_object is not None:
                 new_slice_object.unlock()
             self.logger.info(f"OH : TIME= {time.time() - start:.0f}")
 
-    def get_slivers(self, *, token: str, slice_id: str, sliver_id: str = None) -> List[dict]:
+    def get_slivers(self, *, token: str, slice_id: str, sliver_id: str = None, as_self: bool = True) -> List[dict]:
         """
         Get Slivers for a Slice
         :param token Fabric Identity Token
         :param slice_id Slice Id
         :param sliver_id Sliver Id
+        :param as_self flag; True - return calling user's slivers otherwise, return all slivers in the project
         :raises Raises an exception in case of failure
         :returns List of reservations created for the Slice on success
         """
         try:
             controller = self.controller_state.get_management_actor()
             self.logger.debug(f"get_slivers invoked for Controller: {controller}")
 
             slice_guid = ID(uid=slice_id) if slice_id is not None else None
             rid = ID(uid=sliver_id) if sliver_id is not None else None
 
             fabric_token = self.__authorize_request(id_token=token, action_id=ActionId.query)
 
-            reservations = controller.get_reservations(slice_id=slice_guid, rid=rid, email=fabric_token.get_email(),
-                                                       oidc_claim_sub=fabric_token.get_subject())
+            # Filter slices based on user's email only when querying as_self
+            email = fabric_token.get_email()
+            if not as_self:
+                email = None
+
+            reservations = controller.get_reservations(slice_id=slice_guid, rid=rid, email=email)
             if reservations is None:
                 if controller.get_last_error() is not None:
                     self.logger.error(controller.get_last_error())
                     if controller.get_last_error().status.code == ErrorCodes.ErrorNoSuchSlice:
                         raise OrchestratorException(f"Slice# {slice_id} not found",
                                                     http_error_code=NOT_FOUND)
                     elif controller.get_last_error().status.code == ErrorCodes.ErrorNoSuchReservation:
@@ -359,22 +367,24 @@
 
             return ResponseBuilder.get_reservation_summary(res_list=reservations)
         except Exception as e:
             self.logger.error(traceback.format_exc())
             self.logger.error(f"Exception occurred processing get_slivers e: {e}")
             raise e
 
-    def get_slices(self, *, token: str, states: List[str], name: str, limit: int, offset: int) -> List[dict]:
+    def get_slices(self, *, token: str, states: List[str], name: str, limit: int, offset: int,
+                   as_self: bool = True) -> List[dict]:
         """
         Get User Slices
         :param token Fabric Identity Token
         :param states Slice states
         :param name Slice name
         :param limit Number of slices to return
         :param offset Offset
+        :param as_self flag; True - return calling user's slices otherwise, return all slices in the project
         :raises Raises an exception in case of failure
         :returns List of Slices on success
         """
         try:
             controller = self.controller_state.get_management_actor()
             self.logger.debug(f"get_slices invoked for Controller: {controller}")
 
@@ -382,15 +392,22 @@
 
             fabric_token = self.__authorize_request(id_token=token, action_id=ActionId.query)
 
             projects = fabric_token.get_projects()
             project = None
             if len(projects) == 1:
                 project, tags, project_name = fabric_token.get_first_project()
-            slice_list = controller.get_slices(states=slice_states, email=fabric_token.get_email(), project=project,
+            else:
+                as_self = True
+
+            # Filter slices based on user's email only when querying as_self
+            email = fabric_token.get_email()
+            if not as_self:
+                email = None
+            slice_list = controller.get_slices(states=slice_states, email=email, project=project,
                                                slice_name=name, limit=limit, offset=offset)
             return ResponseBuilder.get_slice_summary(slice_list=slice_list)
         except Exception as e:
             self.logger.error(traceback.format_exc())
             self.logger.error(f"Exception occurred processing get_slices e: {e}")
             raise e
 
@@ -580,32 +597,38 @@
             slice_model_str = slice_topology.serialize()
             return ResponseBuilder.get_slice_summary(slice_list=slice_list, slice_model=slice_model_str)[0]
         except Exception as e:
             self.logger.error(traceback.format_exc())
             self.logger.error(f"Exception occurred processing modify_accept e: {e}")
             raise e
 
-    def get_slice_graph(self, *, token: str, slice_id: str, graph_format_str: str) -> dict:
+    def get_slice_graph(self, *, token: str, slice_id: str, graph_format_str: str, as_self: bool) -> dict:
         """
         Get User Slice
         :param token Fabric Identity Token
         :param slice_id Slice Id
         :param graph_format_str
+        :param as_self flag; True - return calling user's slices otherwise, return all slices in the project
         :raises Raises an exception in case of failure
         :returns Slice Graph on success
         """
         try:
             controller = self.controller_state.get_management_actor()
             self.logger.debug(f"get_slice_graph invoked for Controller: {controller}")
 
             slice_guid = ID(uid=slice_id) if slice_id is not None else None
 
-            self.__authorize_request(id_token=token, action_id=ActionId.query)
+            fabric_token = self.__authorize_request(id_token=token, action_id=ActionId.query)
 
-            slice_list = controller.get_slices(slice_id=slice_guid)
+            # Filter slices based on user's email only when querying as_self
+            email = fabric_token.get_email()
+            if not as_self:
+                email = None
+
+            slice_list = controller.get_slices(slice_id=slice_guid, email=email)
             if slice_list is None or len(slice_list) == 0:
                 if controller.get_last_error() is not None:
                     self.logger.error(controller.get_last_error())
                 raise OrchestratorException(f"User# has no Slices",
                                             http_error_code=NOT_FOUND)
 
             slice_obj = next(iter(slice_list))
@@ -770,7 +793,87 @@
                     status, message = controller.is_sliver_provisioning_allowed(project=project,
                                                                                 site=sliver.get_site(),
                                                                                 email=token.get_email(),
                                                                                 worker=worker)
                     if not status:
                         raise OrchestratorException(message=message,
                                                     http_error_code=Constants.INTERNAL_SERVER_ERROR_MAINT_MODE)
+
+    def poa(self, *, token: str, sliver_id: str, poa: PoaAvro) -> str:
+        try:
+            controller = self.controller_state.get_management_actor()
+            self.logger.debug(f"poa invoked for Controller: {controller}")
+
+            rid = ID(uid=sliver_id) if sliver_id is not None else None
+
+            fabric_token = self.__authorize_request(id_token=token, action_id=ActionId.poa)
+            email = fabric_token.get_email()
+            project, tags, project_name = fabric_token.get_first_project()
+
+            auth = AuthAvro()
+            auth.name = self.controller_state.get_management_actor().get_name()
+            auth.guid = self.controller_state.get_management_actor().get_guid()
+            auth.oidc_sub_claim = fabric_token.get_uuid()
+            auth.email = fabric_token.get_email()
+            poa.auth = auth
+            poa.project_id = project
+            poa.rid = sliver_id
+
+            reservations = controller.get_reservations(rid=rid, email=email)
+            if reservations is None:
+                if controller.get_last_error() is not None:
+                    self.logger.error(controller.get_last_error())
+                    if controller.get_last_error().status.code == ErrorCodes.ErrorNoSuchReservation:
+                        raise OrchestratorException(f"Reservation# {rid} not found",
+                                                    http_error_code=NOT_FOUND)
+
+                raise OrchestratorException(f"{controller.get_last_error()}")
+
+            res_state = ReservationStates(reservations[0].get_state())
+
+            if res_state != ReservationStates.Active:
+                raise OrchestratorException(f"Cannot trigger POA; Reservation# {rid} is not {ReservationStates.Active}")
+
+            if not controller.poa(poa=poa):
+                raise OrchestratorException(f"Failed to trigger POA: "
+                                            f"{controller.get_last_error().get_status().get_message()}")
+            self.logger.debug(f"POA {poa.operation}/{sliver_id} added successfully")
+            return poa.poa_id
+        except Exception as e:
+            self.logger.error(traceback.format_exc())
+            self.logger.error(f"Exception occurred processing poa e: {e}")
+            raise e
+
+    def get_poas(self, *, token: str, sliver_id: str = None, poa_id: str = None):
+        try:
+            if sliver_id is None and poa_id is None:
+                raise OrchestratorException(f"Sliver ID or POA ID must be specified")
+
+            controller = self.controller_state.get_management_actor()
+            self.logger.debug(f"poa invoked for Controller: {controller}")
+
+            rid = ID(uid=sliver_id) if sliver_id is not None else None
+
+            fabric_token = self.__authorize_request(id_token=token, action_id=ActionId.query)
+            email = fabric_token.get_email()
+            project, tags, project_name = fabric_token.get_first_project()
+
+            auth = AuthAvro()
+            auth.name = self.controller_state.get_management_actor().get_name()
+            auth.guid = self.controller_state.get_management_actor().get_guid()
+            auth.oidc_sub_claim = fabric_token.get_uuid()
+            auth.email = fabric_token.get_email()
+
+            poa_list = controller.get_poas(rid=rid, poa_id=poa_id, email=email, project_id=project)
+            if poa_list is None:
+                if controller.get_last_error() is not None:
+                    self.logger.error(controller.get_last_error())
+                    if controller.get_last_error().status.code == ErrorCodes.ErrorNoSuchPoa:
+                        raise OrchestratorException(f"Reservation# {rid} not found",
+                                                    http_error_code=NOT_FOUND)
+
+                raise OrchestratorException(f"{controller.get_last_error()}")
+            return ResponseBuilder.get_poa_summary(poa_list=poa_list)
+        except Exception as e:
+            self.logger.error(traceback.format_exc())
+            self.logger.error(f"Exception occurred processing poa e: {e}")
+            raise e
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_kernel.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/orchestrator_kernel.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/orchestrator_slice_wrapper.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_converter.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/reservation_converter.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_status_update.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/reservation_status_update.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/reservation_status_update_thread.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/reservation_status_update_thread.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/response_builder.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/response_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 from typing import List
 
 from fabric_mb.message_bus.messages.lease_reservation_avro import LeaseReservationAvro
+from fabric_mb.message_bus.messages.poa_info_avro import PoaInfoAvro
 from fabric_mb.message_bus.messages.reservation_mng import ReservationMng
 from fabric_mb.message_bus.messages.slice_avro import SliceAvro
 from fim.graph.abc_property_graph import ABCPropertyGraph
 
 from fabric_cf.actor.core.common.constants import Constants
 from fabric_cf.actor.core.kernel.reservation_states import ReservationStates, ReservationPendingStates, JoinState
 from fabric_cf.actor.core.kernel.slice_state_machine import SliceState
@@ -51,14 +52,17 @@
     PROP_PENDING_STATE = "pending_state"
     PROP_JOIN_STATE = "join_state"
     PROP_GRAPH_NODE_ID = "graph_node_id"
     PROP_SLIVER = "sliver"
     PROP_SLIVER_TYPE = "sliver_type"
     PROP_NOTICE = "notice"
 
+    PROP_OPERATION = "operation"
+    PROP_REQUEST_ID = "request_id"
+
     @staticmethod
     def get_reservation_summary(*, res_list: List[ReservationMng]) -> List[dict]:
         """
         Get Reservation summary
         :param res_list:
         :return:
         """
@@ -140,7 +144,27 @@
     def get_broker_query_model_summary(*, bqm: str):
         """
         Get BQM
         :param bqm:
         :return:
         """
         return {ResponseBuilder.PROP_MODEL: bqm}
+
+    @staticmethod
+    def get_poa_summary(*, poa_list: List[PoaInfoAvro]) -> List[dict]:
+        """
+        Get POA summary
+        :param poa_list:
+        :return:
+        """
+        poas = []
+
+        if poa_list is not None:
+            for poa in poa_list:
+                poa_dict = {ResponseBuilder.PROP_REQUEST_ID: poa.poa_id,
+                            ResponseBuilder.PROP_OPERATION: poa.operation,
+                            ResponseBuilder.PROP_SLIVER_ID: poa.rid,
+                            ResponseBuilder.PROP_SLICE_ID: poa.get_slice_id()}
+                if poa.get_info() is not None:
+                    poa_dict[Constants.PROPERTY_INFO] = poa.get_info()
+                poas.append(poa_dict)
+        return poas
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/slice_defer_thread.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/slice_defer_thread.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/status_checker.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/core/status_checker.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/core/watch_entry.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/authorization_controller.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
-from fabric_cf.actor.core.util.id import ID
-from fabric_cf.orchestrator.core.i_status_update_callback import IStatusUpdateCallback
 
+"""
+controller generated to handled auth operation described at:
+https://connexion.readthedocs.io/en/latest/security.html
+"""
+
+
+def check_bearerAuth(token):
+    return {}
 
-class WatchEntry:
-    def __init__(self, *, watch: ID, callback: IStatusUpdateCallback):
-        self.reservation_to_watch = watch
-        self.callback = callback
 
-    def __str__(self):
-        return f"watch: {self.reservation_to_watch} callback: {self.callback}"
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/docker-compose.yml` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/env.template` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/env.template`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/fabricTags.OrchestratorTags.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/nginx/default.conf` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/nginx/default.conf`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/openapi.json` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/openapi.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9672295257602562%*

 * *Differences: {"'components'": "{'schemas': {'poa_post': OrderedDict([('required', ['operation']), ('type', "*

 * *                 "'object'), ('properties', OrderedDict([('operation', OrderedDict([('type', "*

 * *                 "'string'), ('enum', ['cpuinfo', 'numainfo', 'cpupin', 'numatune', 'reboot'])])), "*

 * *                 "('data', OrderedDict([('$ref', '#/components/schemas/poa_post_data')]))]))]), "*

 * *                 "'slices_post': OrderedDict([('required', ['graph_model', 'ssh_keys']), ('type', "*

 * *                 "'obj […]*

```diff
@@ -1,22 +1,133 @@
 {
     "components": {
         "requestBodies": {
-            "payload_slices": {
+            "payload_poa": {
+                "content": {
+                    "application/json": {
+                        "schema": {
+                            "$ref": "#/components/schemas/poa_post"
+                        }
+                    }
+                },
+                "description": "Perform Operation Action",
+                "required": true
+            },
+            "payload_slices_create": {
+                "content": {
+                    "application/json": {
+                        "schema": {
+                            "$ref": "#/components/schemas/slices_post"
+                        }
+                    }
+                },
+                "description": "Create new Slice",
+                "required": true
+            },
+            "payload_slices_modify": {
                 "content": {
                     "text/plain": {
                         "schema": {
                             "type": "string"
                         }
                     }
                 },
+                "description": "Modify a Slice",
                 "required": true
             }
         },
         "schemas": {
+            "poa": {
+                "allOf": [
+                    {
+                        "$ref": "#/components/schemas/status_200_ok_single"
+                    },
+                    {
+                        "properties": {
+                            "data": {
+                                "items": {
+                                    "$ref": "#/components/schemas/poa_data"
+                                },
+                                "type": "array"
+                            }
+                        },
+                        "type": "object"
+                    }
+                ],
+                "type": "object"
+            },
+            "poa_data": {
+                "properties": {
+                    "info": {
+                        "type": "object"
+                    },
+                    "operation": {
+                        "type": "string"
+                    },
+                    "poa_id": {
+                        "type": "string"
+                    },
+                    "slice_id": {
+                        "type": "string"
+                    },
+                    "sliver_id": {
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
+            "poa_post": {
+                "properties": {
+                    "data": {
+                        "$ref": "#/components/schemas/poa_post_data"
+                    },
+                    "operation": {
+                        "enum": [
+                            "cpuinfo",
+                            "numainfo",
+                            "cpupin",
+                            "numatune",
+                            "reboot"
+                        ],
+                        "type": "string"
+                    }
+                },
+                "required": [
+                    "operation"
+                ],
+                "type": "object"
+            },
+            "poa_post_data": {
+                "properties": {
+                    "node_set": {
+                        "items": {
+                            "type": "string"
+                        },
+                        "type": "array"
+                    },
+                    "vcpu_cpu_map": {
+                        "items": {
+                            "$ref": "#/components/schemas/poa_post_data_vcpu_cpu_map"
+                        },
+                        "type": "array"
+                    }
+                },
+                "type": "object"
+            },
+            "poa_post_data_vcpu_cpu_map": {
+                "properties": {
+                    "cpu": {
+                        "type": "string"
+                    },
+                    "vcpu": {
+                        "type": "string"
+                    }
+                },
+                "type": "object"
+            },
             "resource": {
                 "properties": {
                     "model": {
                         "type": "string"
                     }
                 },
                 "required": [
@@ -114,14 +225,33 @@
                             }
                         },
                         "type": "object"
                     }
                 ],
                 "type": "object"
             },
+            "slices_post": {
+                "properties": {
+                    "graph_model": {
+                        "type": "string"
+                    },
+                    "ssh_keys": {
+                        "items": {
+                            "type": "string"
+                        },
+                        "maxItems": 10,
+                        "type": "array"
+                    }
+                },
+                "required": [
+                    "graph_model",
+                    "ssh_keys"
+                ],
+                "type": "object"
+            },
             "sliver": {
                 "properties": {
                     "graph_node_id": {
                         "type": "string"
                     },
                     "join_state": {
                         "type": "string"
@@ -684,29 +814,41 @@
                 "tags": [
                     "resources"
                 ]
             }
         },
         "/slices": {
             "get": {
-                "description": "Retrieve a listing of user slices",
+                "description": "Retrieve a listing of user slices. It returns list of all slices belonging to all members in a project when 'as_self' is False otherwise returns only the all user's slices in a project.",
                 "parameters": [
                     {
                         "description": "Search for Slices with the name",
                         "explode": true,
                         "in": "query",
                         "name": "name",
                         "required": false,
                         "schema": {
                             "minLength": 3,
                             "type": "string"
                         },
                         "style": "form"
                     },
                     {
+                        "description": "GET object as Self",
+                        "explode": true,
+                        "in": "query",
+                        "name": "as_self",
+                        "required": false,
+                        "schema": {
+                            "default": true,
+                            "type": "boolean"
+                        },
+                        "style": "form"
+                    },
+                    {
                         "description": "Search for Slices in the specified states",
                         "explode": true,
                         "in": "query",
                         "name": "states",
                         "required": false,
                         "schema": {
                             "items": {
@@ -844,38 +986,27 @@
                         "schema": {
                             "minLength": 3,
                             "type": "string"
                         },
                         "style": "form"
                     },
                     {
-                        "description": "User SSH Key",
-                        "explode": true,
-                        "in": "query",
-                        "name": "ssh_key",
-                        "required": true,
-                        "schema": {
-                            "type": "string"
-                        },
-                        "style": "form"
-                    },
-                    {
-                        "description": "New Lease End Time for the Slice",
+                        "description": "Lease End Time for the Slice",
                         "explode": true,
                         "in": "query",
                         "name": "lease_end_time",
                         "required": false,
                         "schema": {
                             "type": "string"
                         },
                         "style": "form"
                     }
                 ],
                 "requestBody": {
-                    "$ref": "#/components/requestBodies/payload_slices"
+                    "$ref": "#/components/requestBodies/payload_slices_create"
                 },
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "$ref": "#/components/schemas/slivers"
@@ -1124,15 +1255,15 @@
                         "schema": {
                             "type": "string"
                         },
                         "style": "simple"
                     }
                 ],
                 "requestBody": {
-                    "$ref": "#/components/requestBodies/payload_slices"
+                    "$ref": "#/components/requestBodies/payload_slices_modify"
                 },
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
                                     "$ref": "#/components/schemas/slivers"
@@ -1404,14 +1535,26 @@
                         "required": true,
                         "schema": {
                             "type": "string"
                         },
                         "style": "simple"
                     },
                     {
+                        "description": "GET object as Self",
+                        "explode": true,
+                        "in": "query",
+                        "name": "as_self",
+                        "required": false,
+                        "schema": {
+                            "default": true,
+                            "type": "boolean"
+                        },
+                        "style": "form"
+                    },
+                    {
                         "description": "graph format",
                         "explode": true,
                         "in": "query",
                         "name": "graph_format",
                         "required": true,
                         "schema": {
                             "default": "GRAPHML",
@@ -1508,14 +1651,26 @@
                         "in": "query",
                         "name": "slice_id",
                         "required": true,
                         "schema": {
                             "type": "string"
                         },
                         "style": "form"
+                    },
+                    {
+                        "description": "GET object as Self",
+                        "explode": true,
+                        "in": "query",
+                        "name": "as_self",
+                        "required": false,
+                        "schema": {
+                            "default": true,
+                            "type": "boolean"
+                        },
+                        "style": "form"
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
@@ -1583,14 +1738,284 @@
                 ],
                 "summary": "Retrieve a listing of user slivers",
                 "tags": [
                     "slivers"
                 ]
             }
         },
+        "/slivers/poa/{sliver_id}": {
+            "post": {
+                "description": "Request to perform an operation action on a sliver. Supported actions include - reboot a VM sliver, get cpu info, get numa info, pin vCPUs, pin memory to a numa node etc.  \n",
+                "parameters": [
+                    {
+                        "description": "Sliver identified by universally unique identifier",
+                        "explode": false,
+                        "in": "path",
+                        "name": "sliver_id",
+                        "required": true,
+                        "schema": {
+                            "type": "string"
+                        },
+                        "style": "simple"
+                    }
+                ],
+                "requestBody": {
+                    "$ref": "#/components/requestBodies/payload_poa"
+                },
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/poa"
+                                }
+                            }
+                        },
+                        "description": "OK"
+                    },
+                    "400": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_400_bad_request"
+                                }
+                            }
+                        },
+                        "description": "Bad Request"
+                    },
+                    "401": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_401_unauthorized"
+                                }
+                            }
+                        },
+                        "description": "Unauthorized"
+                    },
+                    "403": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_403_forbidden"
+                                }
+                            }
+                        },
+                        "description": "Forbidden"
+                    },
+                    "404": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_404_not_found"
+                                }
+                            }
+                        },
+                        "description": "Not Found"
+                    },
+                    "500": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_500_internal_server_error"
+                                }
+                            }
+                        },
+                        "description": "Internal Server Error"
+                    }
+                },
+                "security": [
+                    {
+                        "bearerAuth": []
+                    }
+                ],
+                "summary": "Perform an operational action on a sliver.",
+                "tags": [
+                    "slivers"
+                ]
+            }
+        },
+        "/slivers/poa_get/{poa_id}": {
+            "get": {
+                "description": "Request get the status of the POA identified by poa_id.  \n",
+                "parameters": [
+                    {
+                        "description": "Poa Id for the POA triggered",
+                        "explode": false,
+                        "in": "path",
+                        "name": "poa_id",
+                        "required": true,
+                        "schema": {
+                            "type": "string"
+                        },
+                        "style": "simple"
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/poa"
+                                }
+                            }
+                        },
+                        "description": "OK"
+                    },
+                    "400": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_400_bad_request"
+                                }
+                            }
+                        },
+                        "description": "Bad Request"
+                    },
+                    "401": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_401_unauthorized"
+                                }
+                            }
+                        },
+                        "description": "Unauthorized"
+                    },
+                    "403": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_403_forbidden"
+                                }
+                            }
+                        },
+                        "description": "Forbidden"
+                    },
+                    "404": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_404_not_found"
+                                }
+                            }
+                        },
+                        "description": "Not Found"
+                    },
+                    "500": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_500_internal_server_error"
+                                }
+                            }
+                        },
+                        "description": "Internal Server Error"
+                    }
+                },
+                "security": [
+                    {
+                        "bearerAuth": []
+                    }
+                ],
+                "summary": "Perform an operational action on a sliver.",
+                "tags": [
+                    "slivers"
+                ]
+            }
+        },
+        "/slivers/poa_get/{sliver_id}": {
+            "get": {
+                "description": "Request get the status of the POAs for a sliver identified by sliver_id.  \n",
+                "parameters": [
+                    {
+                        "description": "Sliver identified by universally unique identifier",
+                        "explode": false,
+                        "in": "path",
+                        "name": "sliver_id",
+                        "required": true,
+                        "schema": {
+                            "type": "string"
+                        },
+                        "style": "simple"
+                    }
+                ],
+                "responses": {
+                    "200": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/poa"
+                                }
+                            }
+                        },
+                        "description": "OK"
+                    },
+                    "400": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_400_bad_request"
+                                }
+                            }
+                        },
+                        "description": "Bad Request"
+                    },
+                    "401": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_401_unauthorized"
+                                }
+                            }
+                        },
+                        "description": "Unauthorized"
+                    },
+                    "403": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_403_forbidden"
+                                }
+                            }
+                        },
+                        "description": "Forbidden"
+                    },
+                    "404": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_404_not_found"
+                                }
+                            }
+                        },
+                        "description": "Not Found"
+                    },
+                    "500": {
+                        "content": {
+                            "application/json": {
+                                "schema": {
+                                    "$ref": "#/components/schemas/status_500_internal_server_error"
+                                }
+                            }
+                        },
+                        "description": "Internal Server Error"
+                    }
+                },
+                "security": [
+                    {
+                        "bearerAuth": []
+                    }
+                ],
+                "summary": "Perform an operational action on a sliver.",
+                "tags": [
+                    "slivers"
+                ]
+            }
+        },
         "/slivers/{sliver_id}": {
             "get": {
                 "description": "Retrieve Sliver properties",
                 "parameters": [
                     {
                         "description": "Slice identified by universally unique identifier",
                         "explode": true,
@@ -1608,14 +2033,26 @@
                         "in": "path",
                         "name": "sliver_id",
                         "required": true,
                         "schema": {
                             "type": "string"
                         },
                         "style": "simple"
+                    },
+                    {
+                        "description": "GET object as Self",
+                        "explode": true,
+                        "in": "query",
+                        "name": "as_self",
+                        "required": false,
+                        "schema": {
+                            "default": true,
+                            "type": "boolean"
+                        },
+                        "style": "form"
                     }
                 ],
                 "responses": {
                     "200": {
                         "content": {
                             "application/json": {
                                 "schema": {
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/orchestrator-yes.xml` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/orchestrator-yes.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/pdp.xml` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/pdp.xml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/setup.sh` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/setup.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/controllers/resources_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 
     :rtype: Resources
     """
     return rc.portalresources_get(graph_format)
 
 
 def resources_get(level, force_refresh):  # noqa: E501
-    """Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources.
+    """Retrieve a listing and description of available resources. By default, a cached available resource information
+    is returned. User can force to request the current available resources.
 
-    Retrieve a listing and description of available resources. By default, a cached available resource information is returned. User can force to request the current available resources. # noqa: E501
+    Retrieve a listing and description of available resources. By default, a cached available resource information is
+    returned. User can force to request the current available resources. # noqa: E501
 
     :param level: Level of details
     :type level: int
     :param force_refresh: Force to retrieve current available resource information.
     :type force_refresh: bool
 
     :rtype: Resources
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/controllers/slices_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,47 @@
+import connexion
+
+from fabric_cf.orchestrator.swagger_server.models import SlicesPost
 from fabric_cf.orchestrator.swagger_server.models.slice_details import SliceDetails  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.slices import Slices  # noqa: E501
+from fabric_cf.orchestrator.swagger_server.models.slices_post import SlicesPost  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.slivers import Slivers  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.status200_ok_no_content import Status200OkNoContent  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.response import slices_controller as rc
 
 
-def slices_create_post(body, name, ssh_key, lease_end_time=None):  # noqa: E501
+def slices_create_post(body, name, lease_end_time=None):  # noqa: E501
     """Create slice
 
     Request to create slice as described in the request. Request would be a graph ML describing the requested resources.
     Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing
     resources satisfying the request, and assigned to the given slice. This API returns list and description of the
     resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these
     resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke
     get slice API to get the latest state of the requested resources.   # noqa: E501
 
-    :param body: 
+    :param body: Create new Slice
     :type body: dict | bytes
     :param name: Slice Name
     :type name: str
-    :param ssh_key: User SSH Key
-    :type ssh_key: str
-    :param lease_end_time: New Lease End Time for the Slice
+    :param lease_end_time: Lease End Time for the Slice
     :type lease_end_time: str
 
     :rtype: Slivers
     """
-    return rc.slices_create_post(body, name, ssh_key, lease_end_time)
+    if connexion.request.is_json:
+        body = SlicesPost.from_dict(connexion.request.get_json())  # noqa: E501
+    return rc.slices_create_post(body, name, lease_end_time)
 
 
 def slices_delete_delete():  # noqa: E501
     """Delete all slices for a User within a project.
 
-    Delete all slices for a User within a project. User identity email and project id is available in the bearer token.  # noqa: E501
+    Delete all slices for a User within a project. User identity email and project id is available in the
+    bearer token.  # noqa: E501
 
 
     :rtype: Status200OkNoContent
     """
     return rc.slices_delete_delete()
 
 
@@ -50,52 +55,62 @@
     :type slice_id: str
 
     :rtype: Status200OkNoContent
     """
     return rc.slices_delete_slice_id_delete(slice_id)
 
 
-def slices_get(name=None, states=None, limit=None, offset=None):  # noqa: E501
+def slices_get(name=None, as_self=None, states=None, limit=None, offset=None):  # noqa: E501
     """Retrieve a listing of user slices
 
-    Retrieve a listing of user slices # noqa: E501
+    Retrieve a listing of user slices. It returns list of all slices belonging to all members in a project when
+    &#x27;as_self&#x27; is False otherwise returns only the all user&#x27;s slices in a project. # noqa: E501
 
     :param name: Search for Slices with the name
     :type name: str
+    :param as_self: GET object as Self
+    :type as_self: bool
     :param states: Search for Slices in the specified states
     :type states: List[str]
     :param limit: maximum number of results to return per page (1 or more)
     :type limit: int
     :param offset: number of items to skip before starting to collect the result set
     :type offset: int
 
     :rtype: Slices
     """
-    return rc.slices_get(name, states, limit, offset)
+    return rc.slices_get(name, states, limit, offset, as_self=as_self)
 
 
 def slices_modify_slice_id_accept_post(slice_id):  # noqa: E501
     """Accept the last modify an existing slice
 
-    Accept the last modify and prune any failed resources from the Slice. Also return the accepted slice model back to the user.   # noqa: E501
+    Accept the last modify and prune any failed resources from the Slice. Also return the accepted slice
+    model back to the user.   # noqa: E501
 
     :param slice_id: Slice identified by universally unique identifier
     :type slice_id: str
 
     :rtype: SliceDetails
     """
     return rc.slices_modify_slice_id_accept_post(slice_id)
 
 
 def slices_modify_slice_id_put(body, slice_id):  # noqa: E501
     """Modify an existing slice
 
-    Request to modify an existing slice as described in the request. Request would be a graph ML describing the experiment topolgy expected after a modify. The supported modify actions include adding or removing nodes, components, network services or interfaces of the slice. On success, one or more slivers are allocated, containing resources satisfying the request, and assigned to the given slice. This API returns list and description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can invoke get slice API to get the latest state of the requested resources.   # noqa: E501
+    Request to modify an existing slice as described in the request. Request would be a graph ML describing the
+    experiment topolgy expected after a modify. The supported modify actions include adding or removing nodes,
+    components, network services or interfaces of the slice. On success, one or more slivers are allocated,
+    containing resources satisfying the request, and assigned to the given slice. This API returns list and
+    description of the resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger
+    provisioning of these resources asynchronously on the appropriate sites either now or in the future as requested.
+    Experimenter can invoke get slice API to get the latest state of the requested resources.   # noqa: E501
 
-    :param body: 
+    :param body: Modify a Slice
     :type body: dict | bytes
     :param slice_id: Slice identified by universally unique identifier
     :type slice_id: str
 
     :rtype: Slivers
     """
     return rc.slices_modify_slice_id_put(body, slice_id)
@@ -113,20 +128,22 @@
     :type lease_end_time: str
 
     :rtype: Status200OkNoContent
     """
     return rc.slices_renew_slice_id_post(slice_id, lease_end_time)
 
 
-def slices_slice_id_get(slice_id, graph_format):  # noqa: E501
+def slices_slice_id_get(slice_id, graph_format, as_self=None):  # noqa: E501
     """slice properties
 
     Retrieve Slice properties # noqa: E501
 
     :param slice_id: Slice identified by universally unique identifier
     :type slice_id: str
     :param graph_format: graph format
     :type graph_format: str
+    :param as_self: GET object as Self
+    :type as_self: bool
 
     :rtype: SliceDetails
     """
-    return rc.slices_slice_id_get(slice_id, graph_format)
+    return rc.slices_slice_id_get(slice_id, graph_format, as_self=as_self)
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/encoder.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/encoder.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/__init__.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # coding: utf-8
 
 # flake8: noqa
 from __future__ import absolute_import
 # import models into model package
+from fabric_cf.orchestrator.swagger_server.models.poa import Poa
+from fabric_cf.orchestrator.swagger_server.models.poa_data import PoaData
+from fabric_cf.orchestrator.swagger_server.models.poa_post import PoaPost
+from fabric_cf.orchestrator.swagger_server.models.poa_post_data import PoaPostData
+from fabric_cf.orchestrator.swagger_server.models.poa_post_data_vcpu_cpu_map import PoaPostDataVcpuCpuMap
 from fabric_cf.orchestrator.swagger_server.models.resource import Resource
 from fabric_cf.orchestrator.swagger_server.models.resources import Resources
 from fabric_cf.orchestrator.swagger_server.models.slice import Slice
 from fabric_cf.orchestrator.swagger_server.models.slice_details import SliceDetails
 from fabric_cf.orchestrator.swagger_server.models.slices import Slices
+from fabric_cf.orchestrator.swagger_server.models.slices_post import SlicesPost
 from fabric_cf.orchestrator.swagger_server.models.sliver import Sliver
 from fabric_cf.orchestrator.swagger_server.models.slivers import Slivers
 from fabric_cf.orchestrator.swagger_server.models.status200_ok_no_content import Status200OkNoContent
 from fabric_cf.orchestrator.swagger_server.models.status200_ok_no_content_data import Status200OkNoContentData
 from fabric_cf.orchestrator.swagger_server.models.status200_ok_paginated import Status200OkPaginated
 from fabric_cf.orchestrator.swagger_server.models.status200_ok_single import Status200OkSingle
 from fabric_cf.orchestrator.swagger_server.models.status400_bad_request import Status400BadRequest
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/base_model_.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/resource.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/resources.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slice.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slice_details.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slices.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/sliver.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/slivers.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/version.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/models/version_data.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/constants.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,10 +41,12 @@
 SLICES_GET_SLICE_ID_PATH = '/slices/{slice_id}'
 SLICES_RENEW_PATH = '/slices/renew/{slice_id}'
 SLICE_STATUS_SLICE_ID_PATH = '/slices/status/{slice_id}'
 
 
 SLIVERS_GET_PATH = '/slivers'
 SLIVERS_GET_SLIVER_ID_PATH = '/slivers/{sliver_id}'
-SLIVERS_STATUS_SLIVER_ID_PATH = '/slivers/status/{sliver_id}'
+SLIVERS_POA_POST_SLIVER_ID_PATH = '/slivers/poa/{sliver_id}'
+SLIVERS_POA_GET_SLIVER_ID_PATH = '/slivers/poa_get/{sliver_id}'
+SLIVERS_POA_GET_POA_ID_PATH = '/slivers/poa_get/{poa_id}'
 
 VERSIONS_PATH = '/version'
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/cors_response.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/cors_response.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/resources_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/slices_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/slices_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,56 +22,54 @@
 # SOFTWARE.
 #
 #
 # Author: Komal Thareja (kthare10@renci.org)
 
 from fabric_cf.orchestrator.core.exceptions import OrchestratorException
 from fabric_cf.orchestrator.core.orchestrator_handler import OrchestratorHandler
-from fabric_cf.orchestrator.swagger_server.models import Status200OkNoContentData, Slice, Sliver
+from fabric_cf.orchestrator.swagger_server.models import Status200OkNoContentData, Slice, Sliver, SlicesPost
 from fabric_cf.orchestrator.swagger_server.models.slice_details import SliceDetails  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.slices import Slices  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.slivers import Slivers  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.status200_ok_no_content import Status200OkNoContent  # noqa: E501
 from fabric_cf.orchestrator.swagger_server import received_counter, success_counter, failure_counter
 from fabric_cf.orchestrator.swagger_server.response.constants import POST_METHOD, SLICES_CREATE_PATH, DELETE_METHOD, \
     SLICES_DELETE_PATH, GET_METHOD, SLICES_GET_PATH, SLICES_RENEW_PATH, SLICES_GET_SLICE_ID_PATH, SLICES_MODIFY_PATH, \
     SLICES_MODIFY_ACCEPT_PATH, SLICES_DELETE_SLICE_ID_PATH
 from fabric_cf.orchestrator.swagger_server.response.utils import get_token, cors_error_response, cors_success_response
 
 
-def slices_create_post(body, name, ssh_key, lease_end_time) -> Slivers:  # noqa: E501
+def slices_create_post(body: SlicesPost, name, lease_end_time) -> Slivers:  # noqa: E501
     """Create slice
 
     Request to create slice as described in the request. Request would be a graph ML describing the requested resources.
     Resources may be requested to be created now or in future. On success, one or more slivers are allocated, containing
     resources satisfying the request, and assigned to the given slice. This API returns list and description of the
     resources reserved for the slice in the form of Graph ML. Orchestrator would also trigger provisioning of these
     resources asynchronously on the appropriate sites either now or in the future as requested. Experimenter can
     invoke get slice API to get the latest state of the requested resources.   # noqa: E501
 
     :param body:
-    :type body: dict | bytes
+    :type body: SlicesPost
     :param name: Slice Name
     :type name: str
-    :param ssh_key: User SSH Key
-    :type ssh_key: str
     :param lease_end_time: New Lease End Time for the Slice
     :type lease_end_time: str
 
     :rtype: Slivers
     """
     handler = OrchestratorHandler()
     logger = handler.get_logger()
     received_counter.labels(POST_METHOD, SLICES_CREATE_PATH).inc()
 
     try:
         token = get_token()
-        slice_graph = body.decode("utf-8")
-        slivers_dict = handler.create_slice(token=token, slice_name=name, slice_graph=slice_graph,
-                                            ssh_key=ssh_key, lease_end_time=lease_end_time)
+        ssh_key = ','.join(body.ssh_keys)
+        slivers_dict = handler.create_slice(token=token, slice_name=name, slice_graph=body.graph_model,
+                                            lease_end_time=lease_end_time, ssh_key=ssh_key)
         response = Slivers()
         response.data = []
         for s in slivers_dict:
             sliver = Sliver().from_dict(s)
             response.data.append(sliver)
         response.size = len(response.data)
         response.type = "slivers"
@@ -156,36 +154,39 @@
         return cors_error_response(error=e)
     except Exception as e:
         logger.exception(e)
         failure_counter.labels(DELETE_METHOD, SLICES_DELETE_SLICE_ID_PATH).inc()
         return cors_error_response(error=e)
 
 
-def slices_get(name=None, states=None, limit=None, offset=None) -> Slices:  # noqa: E501
+def slices_get(name=None, states=None, limit=None, offset=None, as_self=True) -> Slices:  # noqa: E501
     """Retrieve a listing of user slices
 
     Retrieve a listing of user slices # noqa: E501
 
     :param name: Search for Slices with the name
     :type name: str
     :param states: Search for Slices in the specified states
     :type states: List[str]
     :param limit: maximum number of results to return per page (1 or more)
     :type limit: int
     :param offset: number of items to skip before starting to collect the result set
     :type offset: int
+    :param as_self: GET object as Self
+    :type as_self: bool
 
     :rtype: Slices
     """
     handler = OrchestratorHandler()
     logger = handler.get_logger()
     received_counter.labels(GET_METHOD, SLICES_GET_PATH).inc()
     try:
         token = get_token()
-        slices_dict = handler.get_slices(token=token, states=states, name=name, limit=limit, offset=offset)
+        slices_dict = handler.get_slices(token=token, states=states, name=name, limit=limit, offset=offset,
+                                         as_self=as_self)
         response = Slices()
         response.data = []
         response.type = 'slices'
         for s in slices_dict:
             slice_obj = Slice().from_dict(s)
             response.data.append(slice_obj)
         response.size = len(response.data)
@@ -315,32 +316,35 @@
         return cors_error_response(error=e)
     except Exception as e:
         logger.exception(e)
         failure_counter.labels(POST_METHOD, SLICES_RENEW_PATH).inc()
         return cors_error_response(error=e)
 
 
-def slices_slice_id_get(slice_id, graph_format) -> SliceDetails:  # noqa: E501
+def slices_slice_id_get(slice_id, graph_format, as_self=True) -> SliceDetails:  # noqa: E501
     """slice properties
 
     Retrieve Slice properties # noqa: E501
 
     :param slice_id: Slice identified by universally unique identifier
     :type slice_id: str
     :param graph_format: graph format
     :type graph_format: str
+    :param as_self: GET object as Self
+    :type as_self: bool
 
     :rtype: SliceDetails
     """
     handler = OrchestratorHandler()
     logger = handler.get_logger()
     received_counter.labels(GET_METHOD, SLICES_GET_SLICE_ID_PATH).inc()
     try:
         token = get_token()
-        value = handler.get_slice_graph(token=token, slice_id=slice_id, graph_format_str=graph_format)
+        value = handler.get_slice_graph(token=token, slice_id=slice_id, graph_format_str=graph_format,
+                                        as_self=as_self)
         slice_object = Slice().from_dict(value)
         response = SliceDetails(data=[slice_object], size=1)
         response.type = 'slice_details'
         success_counter.labels(GET_METHOD, SLICES_GET_SLICE_ID_PATH).inc()
         return cors_success_response(response_body=response)
     except OrchestratorException as e:
         logger.exception(e)
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/utils.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/utils.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/response/version_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/response/version_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/swagger/swagger.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -176,26 +176,37 @@
                 $ref: '#/components/schemas/status_500_internal_server_error'
       x-openapi-router-controller: fabric_cf.orchestrator.swagger_server.controllers.resources_controller
   /slices:
     get:
       tags:
       - slices
       summary: Retrieve a listing of user slices
-      description: Retrieve a listing of user slices
+      description: Retrieve a listing of user slices. It returns list of all slices
+        belonging to all members in a project when 'as_self' is False otherwise returns
+        only the all user's slices in a project.
       operationId: slices_get
       parameters:
       - name: name
         in: query
         description: Search for Slices with the name
         required: false
         style: form
         explode: true
         schema:
           minLength: 3
           type: string
+      - name: as_self
+        in: query
+        description: GET object as Self
+        required: false
+        style: form
+        explode: true
+        schema:
+          type: boolean
+          default: true
       - name: states
         in: query
         description: Search for Slices in the specified states
         required: false
         style: form
         explode: true
         schema:
@@ -289,14 +300,23 @@
         in: path
         description: Slice identified by universally unique identifier
         required: true
         style: simple
         explode: false
         schema:
           type: string
+      - name: as_self
+        in: query
+        description: GET object as Self
+        required: false
+        style: form
+        explode: true
+        schema:
+          type: boolean
+          default: true
       - name: graph_format
         in: query
         description: graph format
         required: true
         style: form
         explode: true
         schema:
@@ -367,32 +387,24 @@
         description: Slice Name
         required: true
         style: form
         explode: true
         schema:
           minLength: 3
           type: string
-      - name: ssh_key
-        in: query
-        description: User SSH Key
-        required: true
-        style: form
-        explode: true
-        schema:
-          type: string
       - name: lease_end_time
         in: query
-        description: New Lease End Time for the Slice
+        description: Lease End Time for the Slice
         required: false
         style: form
         explode: true
         schema:
           type: string
       requestBody:
-        $ref: '#/components/requestBodies/payload_slices'
+        $ref: '#/components/requestBodies/payload_slices_create'
       responses:
         "200":
           description: OK
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/slivers'
@@ -452,15 +464,15 @@
         description: Slice identified by universally unique identifier
         required: true
         style: simple
         explode: false
         schema:
           type: string
       requestBody:
-        $ref: '#/components/requestBodies/payload_slices'
+        $ref: '#/components/requestBodies/payload_slices_modify'
       responses:
         "200":
           description: OK
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/slivers'
@@ -738,14 +750,23 @@
         in: query
         description: Slice identifier as UUID
         required: true
         style: form
         explode: true
         schema:
           type: string
+      - name: as_self
+        in: query
+        description: GET object as Self
+        required: false
+        style: form
+        explode: true
+        schema:
+          type: boolean
+          default: true
       responses:
         "200":
           description: OK
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/slivers'
@@ -802,14 +823,23 @@
         in: path
         description: Sliver identified by universally unique identifier
         required: true
         style: simple
         explode: false
         schema:
           type: string
+      - name: as_self
+        in: query
+        description: GET object as Self
+        required: false
+        style: form
+        explode: true
+        schema:
+          type: boolean
+          default: true
       responses:
         "200":
           description: OK
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/slivers'
@@ -842,16 +872,217 @@
           content:
             application/json:
               schema:
                 $ref: '#/components/schemas/status_500_internal_server_error'
       security:
       - bearerAuth: []
       x-openapi-router-controller: fabric_cf.orchestrator.swagger_server.controllers.slivers_controller
+  /slivers/poa/{sliver_id}:
+    post:
+      tags:
+      - slivers
+      summary: Perform an operational action on a sliver.
+      description: "Request to perform an operation action on a sliver. Supported\
+        \ actions include - reboot a VM sliver, get cpu info, get numa info, pin vCPUs,\
+        \ pin memory to a numa node etc.  \n"
+      operationId: slivers_poa_sliver_id_post
+      parameters:
+      - name: sliver_id
+        in: path
+        description: Sliver identified by universally unique identifier
+        required: true
+        style: simple
+        explode: false
+        schema:
+          type: string
+      requestBody:
+        $ref: '#/components/requestBodies/payload_poa'
+      responses:
+        "200":
+          description: OK
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/poa'
+        "400":
+          description: Bad Request
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_400_bad_request'
+        "401":
+          description: Unauthorized
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_401_unauthorized'
+        "403":
+          description: Forbidden
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_403_forbidden'
+        "404":
+          description: Not Found
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_404_not_found'
+        "500":
+          description: Internal Server Error
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_500_internal_server_error'
+      security:
+      - bearerAuth: []
+      x-openapi-router-controller: fabric_cf.orchestrator.swagger_server.controllers.slivers_controller
+  /slivers/poa_get/{sliver_id}:
+    get:
+      tags:
+      - slivers
+      summary: Perform an operational action on a sliver.
+      description: "Request get the status of the POAs for a sliver identified by\
+        \ sliver_id.  \n"
+      operationId: slivers_poa_get_sliver_id_get
+      parameters:
+      - name: sliver_id
+        in: path
+        description: Sliver identified by universally unique identifier
+        required: true
+        style: simple
+        explode: false
+        schema:
+          type: string
+      responses:
+        "200":
+          description: OK
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/poa'
+        "400":
+          description: Bad Request
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_400_bad_request'
+        "401":
+          description: Unauthorized
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_401_unauthorized'
+        "403":
+          description: Forbidden
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_403_forbidden'
+        "404":
+          description: Not Found
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_404_not_found'
+        "500":
+          description: Internal Server Error
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_500_internal_server_error'
+      security:
+      - bearerAuth: []
+      x-openapi-router-controller: fabric_cf.orchestrator.swagger_server.controllers.slivers_controller
+  /slivers/poa_get/{poa_id}:
+    get:
+      tags:
+      - slivers
+      summary: Perform an operational action on a sliver.
+      description: "Request get the status of the POA identified by poa_id.  \n"
+      operationId: slivers_poa_get_poa_id_get
+      parameters:
+      - name: poa_id
+        in: path
+        description: Poa Id for the POA triggered
+        required: true
+        style: simple
+        explode: false
+        schema:
+          type: string
+      responses:
+        "200":
+          description: OK
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/poa'
+        "400":
+          description: Bad Request
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_400_bad_request'
+        "401":
+          description: Unauthorized
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_401_unauthorized'
+        "403":
+          description: Forbidden
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_403_forbidden'
+        "404":
+          description: Not Found
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_404_not_found'
+        "500":
+          description: Internal Server Error
+          content:
+            application/json:
+              schema:
+                $ref: '#/components/schemas/status_500_internal_server_error'
+      security:
+      - bearerAuth: []
+      x-openapi-router-controller: fabric_cf.orchestrator.swagger_server.controllers.slivers_controller
 components:
   schemas:
+    poa_post:
+      required:
+      - operation
+      type: object
+      properties:
+        operation:
+          type: string
+          enum:
+          - cpuinfo
+          - numainfo
+          - cpupin
+          - numatune
+          - reboot
+        data:
+          $ref: '#/components/schemas/poa_post_data'
+    slices_post:
+      required:
+      - graph_model
+      - ssh_keys
+      type: object
+      properties:
+        graph_model:
+          type: string
+        ssh_keys:
+          maxItems: 10
+          type: array
+          items:
+            type: string
     status_200_ok_single:
       type: object
       properties:
         size:
           type: integer
           default: 1
         status:
@@ -1149,21 +1380,77 @@
     resource:
       required:
       - model
       type: object
       properties:
         model:
           type: string
+    poa:
+      type: object
+      allOf:
+      - $ref: '#/components/schemas/status_200_ok_single'
+      - type: object
+        properties:
+          data:
+            type: array
+            items:
+              $ref: '#/components/schemas/poa_data'
+    poa_data:
+      type: object
+      properties:
+        operation:
+          type: string
+        poa_id:
+          type: string
+        sliver_id:
+          type: string
+        slice_id:
+          type: string
+        info:
+          type: object
+    poa_post_data_vcpu_cpu_map:
+      type: object
+      properties:
+        vcpu:
+          type: string
+        cpu:
+          type: string
+    poa_post_data:
+      type: object
+      properties:
+        vcpu_cpu_map:
+          type: array
+          items:
+            $ref: '#/components/schemas/poa_post_data_vcpu_cpu_map'
+        node_set:
+          type: array
+          items:
+            type: string
   requestBodies:
-    payload_slices:
+    payload_slices_modify:
+      description: Modify a Slice
       content:
         text/plain:
           schema:
             type: string
       required: true
+    payload_slices_create:
+      description: Create new Slice
+      content:
+        application/json:
+          schema:
+            $ref: '#/components/schemas/slices_post'
+      required: true
+    payload_poa:
+      description: Perform Operation Action
+      content:
+        application/json:
+          schema:
+            $ref: '#/components/schemas/poa_post'
+      required: true
   securitySchemes:
     bearerAuth:
       type: http
       scheme: bearer
       bearerFormat: JWT
       x-bearerInfoFunc: fabric_cf.orchestrator.swagger_server.controllers.authorization_controller.check_bearerAuth
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/test/test_resources_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/test/test_slices_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import absolute_import
 
 from flask import json
 from six import BytesIO
 
 from fabric_cf.orchestrator.swagger_server.models.slice_details import SliceDetails  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.slices import Slices  # noqa: E501
+from fabric_cf.orchestrator.swagger_server.models.slices_post import SlicesPost  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.slivers import Slivers  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.status200_ok_no_content import Status200OkNoContent  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.status400_bad_request import Status400BadRequest  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.status401_unauthorized import Status401Unauthorized  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.status403_forbidden import Status403Forbidden  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.status404_not_found import Status404NotFound  # noqa: E501
 from fabric_cf.orchestrator.swagger_server.models.status500_internal_server_error import Status500InternalServerError  # noqa: E501
@@ -21,23 +22,22 @@
     """SlicesController integration test stubs"""
 
     def test_slices_create_post(self):
         """Test case for slices_create_post
 
         Create slice
         """
-        body = 'body_example'
+        body = SlicesPost()
         query_string = [('name', 'name_example'),
-                        ('ssh_key', 'ssh_key_example'),
                         ('lease_end_time', 'lease_end_time_example')]
         response = self.client.open(
             '//slices/create',
             method='POST',
             data=json.dumps(body),
-            content_type='text/plain',
+            content_type='application/json',
             query_string=query_string)
         self.assert200(response,
                        'Response body is : ' + response.data.decode('utf-8'))
 
     def test_slices_delete_delete(self):
         """Test case for slices_delete_delete
 
@@ -62,14 +62,15 @@
 
     def test_slices_get(self):
         """Test case for slices_get
 
         Retrieve a listing of user slices
         """
         query_string = [('name', 'name_example'),
+                        ('as_self', true),
                         ('states', 'states_example'),
                         ('limit', 200),
                         ('offset', 1)]
         response = self.client.open(
             '//slices',
             method='GET',
             query_string=query_string)
@@ -115,15 +116,16 @@
                        'Response body is : ' + response.data.decode('utf-8'))
 
     def test_slices_slice_id_get(self):
         """Test case for slices_slice_id_get
 
         slice properties
         """
-        query_string = [('graph_format', 'GRAPHML')]
+        query_string = [('as_self', true),
+                        ('graph_format', 'GRAPHML')]
         response = self.client.open(
             '//slices/{slice_id}'.format(slice_id='slice_id_example'),
             method='GET',
             query_string=query_string)
         self.assert200(response,
                        'Response body is : ' + response.data.decode('utf-8'))
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/test/test_version_controller.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/type_util.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/type_util.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/swagger_server/util.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/swagger_server/util.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/orchestrator.py` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/test/orchestrator.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/test/test.yaml` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/test/test.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
   kafka-ssl-key-location:
   kafka-ssl-key-password:
   kafka-security-protocol: PLAINTEXT
   kafka-group-id: fabric-cf
   orchestrator.rest.port: 8700
   prometheus.port: 11002
   kafka.request.timeout.ms: 120000
-  rpc.request.timeout.seconds: 900
+  rpc.request.timeout.seconds: 120
   maint.project.id: 10c0094a-abaf-4ef9-a532-2be53e2a896b
   message.max.bytes: 1048588
   rpc.retries: 5
 
 logging:
   ## The directory in which actor should create log files.
   ## This directory will be automatically created if it does not exist.
```

### Comparing `fabric_cf-1.5.0b3/fabric_cf/orchestrator/update_swagger_stub.sh` & `fabric_cf-1.5.0b4/fabric_cf/orchestrator/update_swagger_stub.sh`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/images/am-pod.png` & `fabric_cf-1.5.0b4/images/am-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/images/am.png` & `fabric_cf-1.5.0b4/images/am.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/images/broker-pod.png` & `fabric_cf-1.5.0b4/images/broker-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/images/broker.png` & `fabric_cf-1.5.0b4/images/broker.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/images/cf.png` & `fabric_cf-1.5.0b4/images/cf.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/images/orchestrator-pod.png` & `fabric_cf-1.5.0b4/images/orchestrator-pod.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/images/orchestrator.png` & `fabric_cf-1.5.0b4/images/orchestrator.png`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/neo4j/AL2S.graphml` & `fabric_cf-1.5.0b4/neo4j/AL2S.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/neo4j/LBNL-ad.graphml` & `fabric_cf-1.5.0b4/neo4j/LBNL-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/neo4j/Network-ad.graphml` & `fabric_cf-1.5.0b4/neo4j/Network-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/neo4j/RENCI-ad.graphml` & `fabric_cf-1.5.0b4/neo4j/RENCI-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/neo4j/UKY-ad.graphml` & `fabric_cf-1.5.0b4/neo4j/UKY-ad.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/neo4j/UKY2.graphml` & `fabric_cf-1.5.0b4/neo4j/UKY2.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/neo4j/abqm.graphml` & `fabric_cf-1.5.0b4/neo4j/abqm.graphml`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/neo4j/certs/fullchain.pem` & `fabric_cf-1.5.0b4/neo4j/certs/fullchain.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/neo4j/certs/privkey.pem` & `fabric_cf-1.5.0b4/neo4j/certs/privkey.pem`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/psql.upgrade` & `fabric_cf-1.5.0b4/psql.upgrade`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/pyproject.toml` & `fabric_cf-1.5.0b4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     "sqlalchemy",
     "waitress",
     "prometheus_client",
     "connexion",
     "swagger-ui-bundle",
     "PyYAML",
     "fabric_fss_utils==1.5.0rc1",
-    "fabric-message-bus==1.5.0b1",
-    "fabric-fim==1.5.0b4"]
+    "fabric-message-bus==1.5.0b2",
+    "fabric-fim==1.5.0"]
 
 [project.optional-dependencies]
 test = ["pytest",
         "flask_testing",
         "coverage>=4.0.3",
         "nose>=1.3.7",
         "pluggy>=0.3.1",
```

### Comparing `fabric_cf-1.5.0b3/secrets/create-certs.sh` & `fabric_cf-1.5.0b4/secrets/create-certs.sh`

 * *Files 13% similar despite different names*

```diff
@@ -2,43 +2,44 @@
 
 set -o nounset \
     -o errexit \
     -o verbose \
     -o xtrace
 
 # Generate CA key
-openssl req -new -x509 -keyout snakeoil-ca-1.key -out snakeoil-ca-1.crt -days 365 -subj '/CN=ca1.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US' -passin pass:fabric -passout pass:fabric 
+openssl req -new -x509 -keyout snakeoil-ca-1.key -out snakeoil-ca-1.crt -days 365 -subj '/CN=ca1.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US' -passin pass:fabric -passout pass:fabric
 cp snakeoil-ca-1.crt snakeoil-ca-1-copy.crt
+# openssl req -new -x509 -keyout snakeoil-ca-2.key -out snakeoil-ca-2.crt -days 365 -subj '/CN=ca2.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US' -passin pass:fabric -passout pass:fabric
 
 # kafkacat1
 openssl genrsa -des3 -passout "pass:fabric" -out kafkacat1.client.key 2048
-openssl req -passin "pass:fabric" -passout "pass:fabric" -key kafkacat1.client.key -new -out kafkacat1.client.req -subj '/CN=kafkacat1.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US' 
-openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in kafkacat1.client.req -out kafkacat1-ca1-signed.pem -days 9999 -CAcreateserial -passin "pass:fabric"  -sha256
+openssl req -passin "pass:fabric" -passout "pass:fabric" -key kafkacat1.client.key -new -out kafkacat1.client.req -subj '/CN=kafkacat1.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US'
+openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in kafkacat1.client.req -out kafkacat1-ca1-signed.pem -days 9999 -CAcreateserial -passin "pass:fabric"
 
 openssl genrsa -des3 -passout "pass:fabric" -out kafkacat2.client.key 2048
-openssl req -passin "pass:fabric" -passout "pass:fabric" -key kafkacat2.client.key -new -out kafkacat2.client.req -subj '/CN=kafkacat2.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US' 
-openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in kafkacat2.client.req -out kafkacat2-ca1-signed.pem -days 9999 -CAcreateserial -passin "pass:fabric" -sha256
+openssl req -passin "pass:fabric" -passout "pass:fabric" -key kafkacat2.client.key -new -out kafkacat2.client.req -subj '/CN=kafkacat2.test.fabric.io/OU=TEST/O=FABRIC/L=ChapelHill/S=NC/C=US'
+openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in kafkacat2.client.req -out kafkacat2-ca1-signed.pem -days 9999 -CAcreateserial -passin "pass:fabric"
 
 
-for i in broker1 schemaregistry producer consumer zookeeper
+for i in broker1 schemaregistry producer consumer
 do
 	echo $i
 	# Create keystores
 	keytool -genkey -noprompt \
 				 -alias $i \
-				 -dname "CN=$i, OU=TEST, O=FABRIC, L=ChapelHill, S=NC, C=US" \
+				 -dname "CN=$i.test.fabric.io, OU=TEST, O=FABRIC, L=ChapelHill, S=NC, C=US" \
 				 -keystore kafka.$i.keystore.jks \
 				 -keyalg RSA \
 				 -storepass fabric \
 				 -keypass fabric
 
 	# Create CSR, sign the key and import back into keystore
 	keytool -keystore kafka.$i.keystore.jks -alias $i -certreq -file $i.csr -storepass fabric -keypass fabric
 
-	openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in $i.csr -out $i-ca1-signed.crt -days 9999 -CAcreateserial -passin pass:fabric -sha256
+	openssl x509 -req -CA snakeoil-ca-1.crt -CAkey snakeoil-ca-1.key -in $i.csr -out $i-ca1-signed.crt -days 9999 -CAcreateserial -passin pass:fabric
 
 	keytool -keystore kafka.$i.keystore.jks -alias CARoot -import -file snakeoil-ca-1.crt -storepass fabric -keypass fabric -noprompt
 
 	keytool -keystore kafka.$i.keystore.jks -alias $i -import -file $i-ca1-signed.crt -storepass fabric -keypass fabric
 
 	# Create truststore and import the CA cert.
 	keytool -keystore kafka.$i.truststore.jks -alias CARoot -import -file snakeoil-ca-1.crt -storepass fabric -keypass fabric -noprompt
```

### Comparing `fabric_cf-1.5.0b3/tools/audit.py` & `fabric_cf-1.5.0b4/tools/audit.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/tools/db_cli.py` & `fabric_cf-1.5.0b4/tools/db_cli.py`

 * *Files identical despite different names*

### Comparing `fabric_cf-1.5.0b3/PKG-INFO` & `fabric_cf-1.5.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric_cf
-Version: 1.5.0b3
+Version: 1.5.0b4
 Summary: Fabric Control Framework
 Keywords: Swagger,Fabric Control Framework
 Author-email: Komal Thareja <kthare10@renci.org>, Ilya Baldin <ibaldin@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,16 +15,16 @@
 Requires-Dist: sqlalchemy
 Requires-Dist: waitress
 Requires-Dist: prometheus_client
 Requires-Dist: connexion
 Requires-Dist: swagger-ui-bundle
 Requires-Dist: PyYAML
 Requires-Dist: fabric_fss_utils==1.5.0rc1
-Requires-Dist: fabric-message-bus==1.5.0b1
-Requires-Dist: fabric-fim==1.5.0b4
+Requires-Dist: fabric-message-bus==1.5.0b2
+Requires-Dist: fabric-fim==1.5.0
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: flask_testing ; extra == "test"
 Requires-Dist: coverage>=4.0.3 ; extra == "test"
 Requires-Dist: nose>=1.3.7 ; extra == "test"
 Requires-Dist: pluggy>=0.3.1 ; extra == "test"
 Requires-Dist: py>=1.4.31 ; extra == "test"
 Requires-Dist: randomize>=0.13 ; extra == "test"
```

