# Comparing `tmp/fabric-message-bus-1.5.0b1.tar.gz` & `tmp/fabric-message-bus-1.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-message-bus-1.5.0b1.tar", last modified: Thu Feb  9 15:48:31 2023, max compression
+gzip compressed data, was "fabric-message-bus-1.5.0b2.tar", last modified: Thu Jun  8 14:59:29 2023, max compression
```

## Comparing `fabric-message-bus-1.5.0b1.tar` & `fabric-message-bus-1.5.0b2.tar`

### file list

```diff
@@ -1,101 +1,105 @@
--rw-r--r--   0        0        0     1856 2023-02-03 22:42:24.554591 fabric-message-bus-1.5.0b1/.gitignore
--rw-r--r--   0        0        0     1071 2023-02-03 22:42:24.554732 fabric-message-bus-1.5.0b1/LICENSE
--rw-r--r--   0        0        0     3990 2023-02-09 15:32:52.228236 fabric-message-bus-1.5.0b1/README.md
--rwxr-xr-x   0        0        0      203 2023-02-03 22:42:24.555067 fabric-message-bus-1.5.0b1/clean.sh
--rw-r--r--   0        0        0     2857 2023-02-03 22:42:24.555163 fabric-message-bus-1.5.0b1/docker-compose.yml
--rw-r--r--   0        0        0       24 2023-02-09 15:48:09.369938 fabric-message-bus-1.5.0b1/fabric_mb/__init__.py
--rw-r--r--   0        0        0        0 2023-02-03 22:42:24.555446 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/__init__.py
--rw-r--r--   0        0        0     2089 2023-02-03 22:42:24.555616 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/abc_mb_api.py
--rw-r--r--   0        0        0     5899 2023-02-03 22:42:24.555774 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/admin.py
--rw-r--r--   0        0        0     5881 2023-02-03 22:42:24.555969 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/consumer.py
--rw-r--r--   0        0        0     1301 2023-02-03 22:42:24.556095 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/message_bus_exception.py
--rw-r--r--   0        0        0        0 2023-02-03 22:42:24.556192 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/__init__.py
--rw-r--r--   0        0        0     8017 2023-02-03 22:42:24.556330 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/abc_message_avro.py
--rw-r--r--   0        0        0     3663 2023-02-03 22:42:24.556471 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/abc_object_avro.py
--rw-r--r--   0        0        0     6737 2023-02-03 22:42:24.556633 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/actor_avro.py
--rw-r--r--   0        0        0     2306 2023-02-03 22:42:24.556810 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_peer_avro.py
--rw-r--r--   0        0        0     1620 2023-02-03 22:42:24.556975 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_reservation_avro.py
--rw-r--r--   0        0        0     3647 2023-02-03 22:42:24.557068 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_reservations_avro.py
--rw-r--r--   0        0        0     1578 2023-02-03 22:42:24.557180 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_slice_avro.py
--rw-r--r--   0        0        0     3815 2023-02-03 22:42:24.557296 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_update_reservation_record.py
--rw-r--r--   0        0        0     3068 2023-02-03 22:42:24.557391 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_update_slice_record.py
--rw-r--r--   0        0        0     2077 2023-02-03 22:42:24.557497 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/auth_avro.py
--rw-r--r--   0        0        0     2275 2023-02-03 22:42:24.557753 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/broker_query_model_avro.py
--rw-r--r--   0        0        0     1965 2023-02-03 22:42:24.557902 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/claim_delegation_avro.py
--rw-r--r--   0        0        0     2036 2023-02-03 22:42:24.558266 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/claim_resources_avro.py
--rw-r--r--   0        0        0     1924 2023-02-03 22:42:24.558501 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/close_avro.py
--rw-r--r--   0        0        0     2025 2023-02-03 22:42:24.558808 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/close_delegations_avro.py
--rw-r--r--   0        0        0     2029 2023-02-03 22:42:24.559036 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/close_reservations_avro.py
--rw-r--r--   0        0        0     3008 2023-02-03 22:42:24.559238 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/constants.py
--rw-r--r--   0        0        0     3790 2023-02-03 22:42:24.559434 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/delegation_avro.py
--rw-r--r--   0        0        0     2063 2023-02-03 22:42:24.559631 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/demand_reservation_avro.py
--rw-r--r--   0        0        0     1950 2023-02-03 22:42:24.559815 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/extend_lease_avro.py
--rw-r--r--   0        0        0     3384 2023-02-03 22:42:24.560021 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/extend_reservation_avro.py
--rw-r--r--   0        0        0     1977 2023-02-03 22:42:24.560198 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/extend_ticket_avro.py
--rw-r--r--   0        0        0     2199 2023-02-03 22:42:24.560427 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/failed_rpc_avro.py
--rw-r--r--   0        0        0     1593 2023-02-03 22:42:24.560624 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_actors_request_avro.py
--rw-r--r--   0        0        0     1628 2023-02-03 22:42:24.560825 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py
--rw-r--r--   0        0        0     1591 2023-02-03 22:42:24.560986 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_delegations_avro.py
--rw-r--r--   0        0        0     2016 2023-02-03 22:42:24.561162 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py
--rw-r--r--   0        0        0     1967 2023-02-03 22:42:24.561317 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_reservations_request_avro.py
--rw-r--r--   0        0        0     2544 2023-02-03 22:42:24.561504 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py
--rw-r--r--   0        0        0     1939 2023-02-03 22:42:24.561643 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_sites_request_avro.py
--rw-r--r--   0        0        0     1943 2023-02-03 22:42:24.561812 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_slices_request_avro.py
--rw-r--r--   0        0        0     1959 2023-02-03 22:42:24.562066 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_unit_request_avro.py
--rw-r--r--   0        0        0     5914 2023-02-03 22:42:24.562294 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/lease_reservation_avro.py
--rw-r--r--   0        0        0     1891 2023-02-03 22:42:24.562527 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/lease_reservation_state_avro.py
--rw-r--r--   0        0        0     3444 2023-02-03 22:42:24.562787 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/maintenance_request_avro.py
--rw-r--r--   0        0        0     1970 2023-02-03 22:42:24.563033 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/modify_lease_avro.py
--rw-r--r--   0        0        0     3103 2023-02-03 22:42:24.563271 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/proxy_avro.py
--rw-r--r--   0        0        0     2020 2023-02-03 22:42:24.563455 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/query_avro.py
--rw-r--r--   0        0        0     1904 2023-02-03 22:42:24.563669 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/query_result_avro.py
--rw-r--r--   0        0        0     1972 2023-02-03 22:42:24.563923 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reclaim_delegation_avro.py
--rw-r--r--   0        0        0     2043 2023-02-03 22:42:24.564129 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reclaim_resources_avro.py
--rw-r--r--   0        0        0     1948 2023-02-03 22:42:24.564348 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/redeem_avro.py
--rw-r--r--   0        0        0     1964 2023-02-03 22:42:24.564628 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/relinquish_avro.py
--rw-r--r--   0        0        0     1995 2023-02-03 22:42:24.564953 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/remove_delegation_avro.py
--rw-r--r--   0        0        0     1982 2023-02-03 22:42:24.565172 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/remove_reservation_avro.py
--rw-r--r--   0        0        0     1952 2023-02-03 22:42:24.565371 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/remove_slice_avro.py
--rw-r--r--   0        0        0     4120 2023-02-03 22:42:24.565651 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/request_by_id_record.py
--rw-r--r--   0        0        0     3019 2023-02-03 22:42:24.565914 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reservation_avro.py
--rw-r--r--   0        0        0     7721 2023-02-03 22:42:24.566157 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reservation_mng.py
--rw-r--r--   0        0        0     3126 2023-02-03 22:42:24.566387 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reservation_or_delegation_record.py
--rw-r--r--   0        0        0     2059 2023-02-03 22:42:24.566595 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reservation_predecessor_avro.py
--rw-r--r--   0        0        0     2513 2023-02-03 22:42:24.566842 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reservation_state_avro.py
--rw-r--r--   0        0        0     3193 2023-02-03 22:42:24.567210 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/resource_set_avro.py
--rw-r--r--   0        0        0     3431 2023-02-03 22:42:24.567594 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/resource_ticket_avro.py
--rw-r--r--   0        0        0     1587 2023-02-03 22:42:24.567904 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_actor_avro.py
--rw-r--r--   0        0        0     2550 2023-02-03 22:42:24.568148 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_avro.py
--rw-r--r--   0        0        0     1625 2023-02-03 22:42:24.568378 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_broker_query_model_avro.py
--rw-r--r--   0        0        0     1607 2023-02-03 22:42:24.568551 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_delegation_avro.py
--rw-r--r--   0        0        0     1588 2023-02-03 22:42:24.568710 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_proxy_avro.py
--rw-r--r--   0        0        0    11205 2023-02-03 22:42:24.568915 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_record_list.py
--rw-r--r--   0        0        0     1611 2023-02-03 22:42:24.569168 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_reservation_avro.py
--rw-r--r--   0        0        0     1633 2023-02-03 22:42:24.569556 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_reservation_state_avro.py
--rw-r--r--   0        0        0     1662 2023-02-03 22:42:24.570103 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_sites_avro.py
--rw-r--r--   0        0        0     1587 2023-02-03 22:42:24.570347 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_slice_avro.py
--rw-r--r--   0        0        0     3167 2023-02-03 22:42:24.570534 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_string_avro.py
--rw-r--r--   0        0        0     3191 2023-02-03 22:42:24.570719 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_strings_avro.py
--rw-r--r--   0        0        0     1662 2023-02-03 22:42:24.570874 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_units_avro.py
--rw-r--r--   0        0        0     1900 2023-02-03 22:42:24.571062 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/site_avro.py
--rw-r--r--   0        0        0     8670 2023-02-03 22:42:24.571248 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/slice_avro.py
--rw-r--r--   0        0        0     1844 2023-02-03 22:42:24.571460 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/term_avro.py
--rw-r--r--   0        0        0     3474 2023-02-03 22:42:24.571662 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/ticket.py
--rw-r--r--   0        0        0     2810 2023-02-03 22:42:24.571880 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/ticket_avro.py
--rw-r--r--   0        0        0     4436 2023-02-03 22:42:24.572065 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/ticket_reservation_avro.py
--rw-r--r--   0        0        0     3512 2023-02-03 22:42:24.572264 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/unit_avro.py
--rw-r--r--   0        0        0     1759 2023-02-03 22:42:24.572486 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_data_avro.py
--rw-r--r--   0        0        0     1969 2023-02-03 22:42:24.572648 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_delegation_avro.py
--rw-r--r--   0        0        0     1971 2023-02-03 22:42:24.572811 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_lease_avro.py
--rw-r--r--   0        0        0     1631 2023-02-03 22:42:24.572971 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_reservation_avro.py
--rw-r--r--   0        0        0     1588 2023-02-03 22:42:24.573133 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_slice_avro.py
--rw-r--r--   0        0        0     1975 2023-02-03 22:42:24.573299 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_ticket_avro.py
--rw-r--r--   0        0        0     7894 2023-02-03 22:42:24.573498 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/producer.py
--rw-r--r--   0        0        0       92 2023-02-03 22:42:24.573750 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/schema/key.avsc
--rw-r--r--   0        0        0    27389 2023-02-03 22:42:24.574159 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/schema/message.avsc
--rw-r--r--   0        0        0        0 2023-02-03 22:42:24.574374 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/test/__init__.py
--rw-r--r--   0        0        0    15232 2023-02-03 22:42:24.574593 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/test/abqm.graphml
--rw-r--r--   0        0        0    42658 2023-02-03 22:42:24.574984 fabric-message-bus-1.5.0b1/fabric_mb/message_bus/test/message_bus_test.py
--rw-r--r--   0        0        0      747 2023-02-09 15:46:30.298154 fabric-message-bus-1.5.0b1/pyproject.toml
--rwxr-xr-x   0        0        0     2190 2023-02-03 22:42:24.575420 fabric-message-bus-1.5.0b1/secrets/create-certs.sh
--rw-r--r--   0        0        0     4553 1970-01-01 00:00:00.000000 fabric-message-bus-1.5.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1856 2023-05-25 14:23:12.456470 fabric-message-bus-1.5.0b2/.gitignore
+-rw-r--r--   0        0        0     1071 2023-05-25 14:23:12.456641 fabric-message-bus-1.5.0b2/LICENSE
+-rw-r--r--   0        0        0     3990 2023-05-25 14:24:41.685533 fabric-message-bus-1.5.0b2/README.md
+-rwxr-xr-x   0        0        0      203 2023-05-25 14:23:12.456973 fabric-message-bus-1.5.0b2/clean.sh
+-rw-r--r--   0        0        0     1560 2023-06-01 19:59:30.435322 fabric-message-bus-1.5.0b2/docker-compose-no-ssl-kafka.yaml
+-rw-r--r--   0        0        0     2857 2023-05-25 14:23:12.457153 fabric-message-bus-1.5.0b2/docker-compose.yml
+-rw-r--r--   0        0        0       24 2023-06-08 14:58:55.799244 fabric-message-bus-1.5.0b2/fabric_mb/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-25 14:23:12.457626 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-25 14:23:12.457824 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/abc_mb_api.py
+-rw-r--r--   0        0        0     5899 2023-05-25 14:23:12.458029 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/admin.py
+-rw-r--r--   0        0        0     5881 2023-06-02 19:00:21.506228 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/consumer.py
+-rw-r--r--   0        0        0     1301 2023-05-25 14:23:12.458360 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/message_bus_exception.py
+-rw-r--r--   0        0        0        0 2023-05-25 14:23:12.458458 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/__init__.py
+-rw-r--r--   0        0        0     8062 2023-06-02 18:49:03.390770 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/abc_message_avro.py
+-rw-r--r--   0        0        0     3915 2023-06-07 20:36:42.802978 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/abc_object_avro.py
+-rw-r--r--   0        0        0     6737 2023-05-25 14:23:12.458921 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/actor_avro.py
+-rw-r--r--   0        0        0     2306 2023-05-25 14:23:12.459252 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_peer_avro.py
+-rw-r--r--   0        0        0     1620 2023-05-25 14:23:12.459510 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_reservation_avro.py
+-rw-r--r--   0        0        0     3647 2023-05-25 14:23:12.459637 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_reservations_avro.py
+-rw-r--r--   0        0        0     1578 2023-05-25 14:23:12.459736 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_slice_avro.py
+-rw-r--r--   0        0        0     3815 2023-05-25 14:23:12.459867 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_update_reservation_record.py
+-rw-r--r--   0        0        0     3068 2023-05-25 14:23:12.459981 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_update_slice_record.py
+-rw-r--r--   0        0        0     2077 2023-05-25 14:23:12.460090 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/auth_avro.py
+-rw-r--r--   0        0        0     2275 2023-05-25 14:23:12.460193 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/broker_query_model_avro.py
+-rw-r--r--   0        0        0     1965 2023-05-25 14:23:12.460399 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/claim_delegation_avro.py
+-rw-r--r--   0        0        0     2036 2023-05-25 14:23:12.460571 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/claim_resources_avro.py
+-rw-r--r--   0        0        0     1924 2023-05-25 14:23:12.460710 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/close_avro.py
+-rw-r--r--   0        0        0     2025 2023-05-25 14:23:12.460895 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/close_delegations_avro.py
+-rw-r--r--   0        0        0     2029 2023-05-25 14:23:12.461073 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/close_reservations_avro.py
+-rw-r--r--   0        0        0     3044 2023-06-07 20:36:50.400191 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/constants.py
+-rw-r--r--   0        0        0     3946 2023-06-04 21:13:21.833540 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/delegation_avro.py
+-rw-r--r--   0        0        0     2063 2023-05-25 14:23:12.461627 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/demand_reservation_avro.py
+-rw-r--r--   0        0        0     1950 2023-05-25 14:23:12.461780 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/extend_lease_avro.py
+-rw-r--r--   0        0        0     3384 2023-05-25 14:23:12.461942 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/extend_reservation_avro.py
+-rw-r--r--   0        0        0     1977 2023-05-25 14:23:12.462053 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/extend_ticket_avro.py
+-rw-r--r--   0        0        0     2199 2023-05-25 14:23:12.462166 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/failed_rpc_avro.py
+-rw-r--r--   0        0        0     1593 2023-05-25 14:23:12.462307 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_actors_request_avro.py
+-rw-r--r--   0        0        0     1628 2023-05-25 14:23:12.462527 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py
+-rw-r--r--   0        0        0     1591 2023-05-25 14:23:12.462698 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_delegations_avro.py
+-rw-r--r--   0        0        0     2016 2023-05-25 14:23:12.462860 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py
+-rw-r--r--   0        0        0     1967 2023-05-25 14:23:12.463021 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_reservations_request_avro.py
+-rw-r--r--   0        0        0     2544 2023-05-25 14:23:12.463335 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py
+-rw-r--r--   0        0        0     1939 2023-05-25 14:23:12.463597 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_sites_request_avro.py
+-rw-r--r--   0        0        0     1943 2023-05-25 14:23:12.463894 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_slices_request_avro.py
+-rw-r--r--   0        0        0     1959 2023-05-25 14:23:12.464127 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_unit_request_avro.py
+-rw-r--r--   0        0        0     5914 2023-05-25 14:23:12.464377 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/lease_reservation_avro.py
+-rw-r--r--   0        0        0     1891 2023-05-25 14:23:12.464631 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/lease_reservation_state_avro.py
+-rw-r--r--   0        0        0     3444 2023-05-25 14:23:12.464856 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/maintenance_request_avro.py
+-rw-r--r--   0        0        0     1970 2023-05-25 14:23:12.465020 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/modify_lease_avro.py
+-rw-r--r--   0        0        0     3263 2023-06-08 03:34:35.573911 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/poa_avro.py
+-rw-r--r--   0        0        0     2734 2023-06-08 13:02:17.482566 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/poa_info_avro.py
+-rw-r--r--   0        0        0     3103 2023-05-25 14:23:12.465213 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/proxy_avro.py
+-rw-r--r--   0        0        0     2020 2023-05-25 14:23:12.465372 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/query_avro.py
+-rw-r--r--   0        0        0     1904 2023-05-25 14:23:12.465547 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/query_result_avro.py
+-rw-r--r--   0        0        0     1972 2023-05-25 14:23:12.465826 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reclaim_delegation_avro.py
+-rw-r--r--   0        0        0     2043 2023-05-25 14:23:12.466002 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reclaim_resources_avro.py
+-rw-r--r--   0        0        0     1948 2023-05-25 14:23:12.466176 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/redeem_avro.py
+-rw-r--r--   0        0        0     1964 2023-05-25 14:23:12.466351 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/relinquish_avro.py
+-rw-r--r--   0        0        0     1995 2023-05-25 14:23:12.466510 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/remove_delegation_avro.py
+-rw-r--r--   0        0        0     1982 2023-05-25 14:23:12.466651 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/remove_reservation_avro.py
+-rw-r--r--   0        0        0     1952 2023-05-25 14:23:12.466787 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/remove_slice_avro.py
+-rw-r--r--   0        0        0     4120 2023-05-25 14:23:12.467038 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/request_by_id_record.py
+-rw-r--r--   0        0        0     3019 2023-05-25 14:23:12.467342 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reservation_avro.py
+-rw-r--r--   0        0        0     7721 2023-05-25 14:23:12.467592 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reservation_mng.py
+-rw-r--r--   0        0        0     3126 2023-05-25 14:23:12.467825 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reservation_or_delegation_record.py
+-rw-r--r--   0        0        0     2059 2023-05-25 14:23:12.468069 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reservation_predecessor_avro.py
+-rw-r--r--   0        0        0     2513 2023-05-25 14:23:12.468350 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reservation_state_avro.py
+-rw-r--r--   0        0        0     3193 2023-05-25 14:23:12.468583 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/resource_set_avro.py
+-rw-r--r--   0        0        0     3431 2023-05-25 14:23:12.468776 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/resource_ticket_avro.py
+-rw-r--r--   0        0        0     1587 2023-05-25 14:23:12.468942 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_actor_avro.py
+-rw-r--r--   0        0        0     2550 2023-05-25 14:23:12.469128 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_avro.py
+-rw-r--r--   0        0        0     1625 2023-05-25 14:23:12.469377 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_broker_query_model_avro.py
+-rw-r--r--   0        0        0     1607 2023-05-25 14:23:12.469563 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_delegation_avro.py
+-rw-r--r--   0        0        0     1581 2023-06-02 18:48:46.680999 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_poa_avro.py
+-rw-r--r--   0        0        0     1588 2023-05-25 14:23:12.469767 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_proxy_avro.py
+-rw-r--r--   0        0        0    11980 2023-06-07 16:42:49.661850 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_record_list.py
+-rw-r--r--   0        0        0     1611 2023-05-25 14:23:12.470157 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_reservation_avro.py
+-rw-r--r--   0        0        0     1633 2023-05-25 14:23:12.470304 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_reservation_state_avro.py
+-rw-r--r--   0        0        0     1662 2023-05-25 14:23:12.470471 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_sites_avro.py
+-rw-r--r--   0        0        0     1587 2023-05-25 14:23:12.470680 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_slice_avro.py
+-rw-r--r--   0        0        0     3167 2023-05-25 14:23:12.470890 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_string_avro.py
+-rw-r--r--   0        0        0     3191 2023-05-25 14:23:12.471165 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_strings_avro.py
+-rw-r--r--   0        0        0     1662 2023-05-25 14:23:12.471387 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_units_avro.py
+-rw-r--r--   0        0        0     1900 2023-05-25 14:23:12.471588 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/site_avro.py
+-rw-r--r--   0        0        0     8670 2023-05-25 14:23:12.471759 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/slice_avro.py
+-rw-r--r--   0        0        0     1844 2023-05-25 14:23:12.471938 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/term_avro.py
+-rw-r--r--   0        0        0     3474 2023-05-25 14:23:12.472208 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/ticket.py
+-rw-r--r--   0        0        0     2810 2023-05-25 14:23:12.472453 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/ticket_avro.py
+-rw-r--r--   0        0        0     4436 2023-05-25 14:23:12.472668 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/ticket_reservation_avro.py
+-rw-r--r--   0        0        0     3512 2023-05-25 14:23:12.472946 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/unit_avro.py
+-rw-r--r--   0        0        0     1759 2023-05-25 14:23:12.473229 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_data_avro.py
+-rw-r--r--   0        0        0     1969 2023-05-25 14:23:12.473537 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_delegation_avro.py
+-rw-r--r--   0        0        0     1971 2023-05-25 14:23:12.473754 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_lease_avro.py
+-rw-r--r--   0        0        0     1631 2023-05-25 14:23:12.473942 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_reservation_avro.py
+-rw-r--r--   0        0        0     1588 2023-05-25 14:23:12.474164 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_slice_avro.py
+-rw-r--r--   0        0        0     1975 2023-05-25 14:23:12.474363 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_ticket_avro.py
+-rw-r--r--   0        0        0     7894 2023-05-25 14:23:12.474547 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/producer.py
+-rw-r--r--   0        0        0       92 2023-05-25 14:23:12.474798 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/schema/key.avsc
+-rw-r--r--   0        0        0    30539 2023-06-08 03:34:35.566814 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/schema/message.avsc
+-rw-r--r--   0        0        0        0 2023-05-25 14:23:12.475455 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/test/__init__.py
+-rw-r--r--   0        0        0    15232 2023-05-25 14:23:12.475842 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/test/abqm.graphml
+-rw-r--r--   0        0        0    44737 2023-06-04 23:16:17.979513 fabric-message-bus-1.5.0b2/fabric_mb/message_bus/test/message_bus_test.py
+-rw-r--r--   0        0        0      747 2023-05-25 14:24:41.685910 fabric-message-bus-1.5.0b2/pyproject.toml
+-rwxr-xr-x   0        0        0     2190 2023-05-25 14:23:12.476803 fabric-message-bus-1.5.0b2/secrets/create-certs.sh
+-rw-r--r--   0        0        0     4553 1970-01-01 00:00:00.000000 fabric-message-bus-1.5.0b2/PKG-INFO
```

### Comparing `fabric-message-bus-1.5.0b1/.gitignore` & `fabric-message-bus-1.5.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/LICENSE` & `fabric-message-bus-1.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/README.md` & `fabric-message-bus-1.5.0b2/README.md`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/docker-compose.yml` & `fabric-message-bus-1.5.0b2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/abc_mb_api.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/abc_mb_api.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/admin.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/admin.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/consumer.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/consumer.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/message_bus_exception.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/message_bus_exception.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/abc_message_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/abc_message_avro.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     claim_delegation = "ClaimDelegation"
     reclaim_delegation = "ReclaimDelegation"
     close = "Close"
     extend_lease = "ExtendLease"
     extend_ticket = "ExtendTicket"
     failed_rpc = "FailedRpc"
     modify_lease = "ModifyLease"
+    poa = "Poa"
     query = "Query"
     query_result = "QueryResult"
     redeem = "Redeem"
     relinquish = "Relinquish"
     update_lease = "UpdateLease"
     update_ticket = "UpdateTicket"
     ticket = "Ticket"
@@ -92,14 +93,15 @@
     result_strings = "ResultStrings"
     result_string = "ResultString"
     result_units = "ResultUnits"
     result_sites = "ResultSites"
     result_proxy = "ResultProxy"
     result_broker_query_model = "ResultBrokerQueryModel"
     result_actor = "ResultActor"
+    result_poa = "ResultPoa"
 
     def __init__(self, *, message_id: str = None, name: str = None, callback_topic: str = None, kafka_error: str = None,
                  id_token: str = None):
         # Unique id used to track produce request success/failures.
         # Do *not* include in the serialized object.
         self.id = uuid4()
         self.message_id = message_id
```

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/abc_object_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/abc_object_avro.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             raise MessageBusException(Constants.ERROR_INVALID_ARGUMENTS)
 
         result = self.__dict__.copy()
 
         for k in self.__dict__:
             if result[k] is None:
                 result.pop(k)
-            elif k == Constants.SLIVER or k == Constants.MAINT_INFO:
+            elif k in [Constants.SLIVER, Constants.MAINT_INFO, Constants.INFO]:
                 v = result[k]
                 if v is not None:
                     result[k] = pickle.dumps(v)
             elif isinstance(result[k], AbcObjectAvro):
                 result[k] = result[k].to_dict()
             elif isinstance(result[k], list):
                 temp = []
@@ -62,16 +62,20 @@
         """
         The Avro Python library does not support code generation.
         For this reason we must provide conversion from dict to our class for de-serialization
         :param value: incoming message dictionary
         """
         for k, v in value.items():
             if k in self.__dict__:
-                if (k == Constants.SLIVER or k == Constants.MAINT_INFO) and v is not None:
+                if (k in [Constants.SLIVER, Constants.MAINT_INFO, Constants.INFO]) and v is not None:
                     self.__dict__[k] = pickle.loads(v)
+                elif k == Constants.AUTH:
+                    from fabric_mb.message_bus.messages.auth_avro import AuthAvro
+                    self.__dict__[k] = AuthAvro()
+                    self.__dict__[k].from_dict(value=v)
                 else:
                     self.__dict__[k] = v
 
     def __str__(self):
         d = self.__dict__.copy()
         for k in self.__dict__:
             if d[k] is None:
```

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/actor_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/actor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_peer_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_peer_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_reservation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_reservations_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_reservations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_slice_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_update_reservation_record.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_update_reservation_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/add_update_slice_record.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/add_update_slice_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/auth_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/auth_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/broker_query_model_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/broker_query_model_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/claim_delegation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/claim_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/claim_resources_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/claim_resources_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/close_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/close_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/close_delegations_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/close_delegations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/close_reservations_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/close_reservations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/constants.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,16 @@
     SEQUENCE = "sequence"
     RESERVATION_ID = "reservation_id"
     SLICE_ID = "slice_id"
     ACTOR_ID = "actor_id"
     PROPERTIES = "properties"
     SLIVER = "sliver"
     MAINT_INFO = "maint_info"
+    POAS = "poas"
+    INFO = "info"
     BROKER = "broker"
     TICKET = "ticket"
     RENEWABLE = "renewable"
     RENEW_TIME = "renew_time"
     UNIT_SET = "unit_set"
     UNITS = "units"
     PROXIES = "proxies"
```

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/delegation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/delegation_avro.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     def __init__(self):
         self.delegation_id = None
         self.slice = None
         self.graph = None
         self.sequence = 0
         self.state = None
         self.delegation_name = None
+        self.site = None
 
     def from_dict(self, value: dict):
         """
         The Avro Python library does not support code generation.
         For this reason we must provide conversion from dict to our class for de-serialization
         :param value: incoming message dictionary
         """
@@ -90,22 +91,27 @@
 
     def get_state(self) -> int:
         return self.state
 
     def get_name(self) -> str:
         return self.delegation_name
 
+    def get_site(self) -> str:
+        return self.site
+
     def print(self):
         """
         Print on console
         """
         print("")
         print("Delegation ID: {} Slice ID: {}".format(self.delegation_id, self.slice.get_slice_id()))
         if self.delegation_name is not None:
             print("Delegation Name: {}".format(self.delegation_name))
         if self.sequence is not None:
             print("Sequence: {}".format(self.sequence))
         if self.state is not None:
             print(f"State: {self.state}")
+        if self.site is not None:
+            print(f"Site: {self.site}")
         if self.graph is not None:
             print("Graph: {}".format(self.graph))
         print("")
```

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/demand_reservation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/demand_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/extend_lease_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/extend_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/extend_reservation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/extend_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/extend_ticket_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/extend_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/failed_rpc_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/failed_rpc_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_actors_request_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_actors_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_broker_query_model_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_delegations_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_delegations_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_reservation_units_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_reservations_request_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_reservations_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_reservations_state_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_sites_request_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_sites_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_slices_request_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_slices_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/get_unit_request_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/get_unit_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/lease_reservation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/lease_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/lease_reservation_state_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/lease_reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/maintenance_request_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/maintenance_request_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/modify_lease_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/modify_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/proxy_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/proxy_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/query_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/query_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/query_result_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/query_result_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reclaim_delegation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reclaim_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reclaim_resources_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reclaim_resources_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/redeem_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/redeem_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/relinquish_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/relinquish_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/remove_delegation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/remove_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/remove_reservation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/remove_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/remove_slice_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/remove_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/request_by_id_record.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/request_by_id_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reservation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reservation_mng.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reservation_mng.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reservation_or_delegation_record.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reservation_or_delegation_record.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reservation_predecessor_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reservation_predecessor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/reservation_state_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/resource_set_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/resource_set_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/resource_ticket_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/resource_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_actor_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_actor_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_broker_query_model_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_broker_query_model_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_delegation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_proxy_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_proxy_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_record_list.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_record_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from fabric_mb.message_bus.message_bus_exception import MessageBusException
 from fabric_mb.message_bus.messages.actor_avro import ActorAvro
 from fabric_mb.message_bus.messages.constants import Constants
 from fabric_mb.message_bus.messages.delegation_avro import DelegationAvro
 from fabric_mb.message_bus.messages.lease_reservation_avro import LeaseReservationAvro
 from fabric_mb.message_bus.messages.lease_reservation_state_avro import LeaseReservationStateAvro
 from fabric_mb.message_bus.messages.broker_query_model_avro import BrokerQueryModelAvro
+from fabric_mb.message_bus.messages.poa_info_avro import PoaInfoAvro
 from fabric_mb.message_bus.messages.proxy_avro import ProxyAvro
 from fabric_mb.message_bus.messages.reservation_mng import ReservationMng
 from fabric_mb.message_bus.messages.reservation_state_avro import ReservationStateAvro
 from fabric_mb.message_bus.messages.result_avro import ResultAvro
 from fabric_mb.message_bus.messages.abc_message_avro import AbcMessageAvro
 from fabric_mb.message_bus.messages.site_avro import SiteAvro
 from fabric_mb.message_bus.messages.slice_avro import SliceAvro
@@ -56,14 +57,15 @@
         self.reservation_states = None
         self.units = None
         self.proxies = None
         self.model = None
         self.actors = None
         self.delegations = None
         self.sites = None
+        self.poas = None
 
     def from_dict_slices(self, value: list):
         """
         The Avro Python library does not support code generation.
         For this reason we must provide conversion from dict to our class for de-serialization
         :param value: incoming message dictionary
         """
@@ -186,14 +188,27 @@
         if value is not None:
             self.sites = []
             for s in value:
                 site = SiteAvro()
                 site.from_dict(s)
                 self.sites.append(site)
 
+    def from_dict_poas(self, value: dict):
+        """
+        The Avro Python library does not support code generation.
+        For this reason we must provide conversion from dict to our class for de-serialization
+        :param value: incoming message dictionary
+        """
+        if value is not None:
+            self.poas = []
+            for p in value:
+                poa = PoaInfoAvro()
+                poa.from_dict(p)
+                self.poas.append(poa)
+
     def from_dict(self, value: dict):
         """
         The Avro Python library does not support code generation.
         For this reason we must provide conversion from dict to our class for de-serialization
         :param value: incoming message dictionary
         """
         for k, v in value.items():
@@ -215,14 +230,16 @@
                     self.from_dict_model(value=v)
                 elif k == Constants.ACTORS:
                     self.from_dict_actors(value=v)
                 elif k == Constants.DELEGATIONS:
                     self.from_dict_delegations(value=v)
                 elif k == Constants.SITES:
                     self.from_dict_sites(value=v)
+                elif k == Constants.POAS:
+                    self.from_dict_poas(value=v)
                 else:
                     self.__dict__[k] = v
 
     def set_status(self, status: ResultAvro):
         """
         Set status
         """
@@ -284,14 +301,20 @@
 
     def get_sites(self) -> List[SiteAvro]:
         """
         Return sites
         """
         return self.sites
 
+    def get_poas(self) -> List[PoaInfoAvro]:
+        """
+        Return Poa Info
+        """
+        return self.poas
+
     def validate(self) -> bool:
         """
         Check if the object is valid and contains all mandatory fields
         :return True on success; False on failure
         """
         ret_val = super().validate()
         if self.status is None:
```

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_reservation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_reservation_state_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_reservation_state_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_sites_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_sites_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_slice_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_string_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_string_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_strings_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_strings_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/result_units_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/result_units_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/site_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/site_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/slice_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/term_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/term_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/ticket.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/ticket.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/ticket_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/ticket_reservation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/ticket_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/unit_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/unit_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_data_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_data_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_delegation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_delegation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_lease_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_lease_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_reservation_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_reservation_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_slice_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_slice_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/messages/update_ticket_avro.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/messages/update_ticket_avro.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/producer.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/producer.py`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/schema/message.avsc` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/schema/message.avsc`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9385614385614386%*

 * *Differences: {'15': "{'fields': {insert: [(2, OrderedDict([('name', 'site'), ('type', ['null', 'string']), "*

 * *       "('default', None)]))]}}",*

 * * '22': "{'fields': {insert: [(10, OrderedDict([('name', 'poas'), ('type', ['null', "*

 * *       "OrderedDict([('type', 'array'), ('items', 'fabric.cf.model.PoaInInfoRecord')])]), "*

 * *       "('default', None)]))]}}",*

 * * 'insert': "[(20, OrderedDict([('namespace', 'fabric.cf.model'), ('name', 'PoaRequest'), ('type', "*

 * *           "'record'), ('fields', [OrderedDict([('name', 'name'), ('typ […]*

```diff
@@ -843,14 +843,22 @@
                 "type": [
                     "null",
                     "string"
                 ]
             },
             {
                 "default": null,
+                "name": "site",
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            {
+                "default": null,
                 "name": "sequence",
                 "type": [
                     "null",
                     "int"
                 ]
             },
             {
@@ -1084,14 +1092,133 @@
     {
         "fields": [
             {
                 "name": "name",
                 "type": "string"
             },
             {
+                "name": "callback_topic",
+                "type": "string"
+            },
+            {
+                "name": "message_id",
+                "type": "string"
+            },
+            {
+                "name": "poa_id",
+                "type": "string"
+            },
+            {
+                "name": "project_id",
+                "type": "string"
+            },
+            {
+                "name": "operation",
+                "type": "string"
+            },
+            {
+                "name": "rid",
+                "type": "string"
+            },
+            {
+                "name": "slice_id",
+                "type": "string"
+            },
+            {
+                "name": "sequence",
+                "type": "int"
+            },
+            {
+                "name": "auth",
+                "type": "fabric.cf.model.AuthRecord"
+            },
+            {
+                "default": null,
+                "name": "id_token",
+                "type": [
+                    "null",
+                    "string"
+                ]
+            },
+            {
+                "default": null,
+                "name": "vcpu_cpu_map",
+                "type": [
+                    "null",
+                    {
+                        "items": {
+                            "type": "map",
+                            "values": "string"
+                        },
+                        "type": "array"
+                    }
+                ]
+            },
+            {
+                "default": null,
+                "name": "node_set",
+                "type": [
+                    "null",
+                    {
+                        "items": "string",
+                        "type": "array"
+                    }
+                ]
+            }
+        ],
+        "name": "PoaRequest",
+        "namespace": "fabric.cf.model",
+        "type": "record"
+    },
+    {
+        "fields": [
+            {
+                "name": "operation",
+                "type": "string"
+            },
+            {
+                "name": "poa_id",
+                "type": "string"
+            },
+            {
+                "name": "rid",
+                "type": "string"
+            },
+            {
+                "name": "slice_id",
+                "type": "string"
+            },
+            {
+                "name": "project_id",
+                "type": "string"
+            },
+            {
+                "name": "auth",
+                "type": "fabric.cf.model.AuthRecord"
+            },
+            {
+                "default": null,
+                "name": "info",
+                "type": [
+                    "null",
+                    "bytes"
+                ]
+            }
+        ],
+        "name": "PoaInInfoRecord",
+        "namespace": "fabric.cf.model",
+        "type": "record"
+    },
+    {
+        "fields": [
+            {
+                "name": "name",
+                "type": "string"
+            },
+            {
                 "name": "message_id",
                 "type": "string"
             },
             {
                 "name": "status",
                 "type": "fabric.cf.model.ResultRecord"
             },
@@ -1167,14 +1294,25 @@
                 "type": [
                     "null",
                     "fabric.cf.model.BrokerQueryModelRecord"
                 ]
             },
             {
                 "default": null,
+                "name": "poas",
+                "type": [
+                    "null",
+                    {
+                        "items": "fabric.cf.model.PoaInInfoRecord",
+                        "type": "array"
+                    }
+                ]
+            },
+            {
+                "default": null,
                 "name": "delegations",
                 "type": [
                     "null",
                     {
                         "items": "fabric.cf.model.DelegationRecord",
                         "type": "array"
                     }
```

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/test/abqm.graphml` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/test/abqm.graphml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/fabric_mb/message_bus/test/message_bus_test.py` & `fabric-message-bus-1.5.0b2/fabric_mb/message_bus/test/message_bus_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,21 +56,24 @@
 from fabric_mb.message_bus.messages.get_reservation_units_request_avro import GetReservationUnitsRequestAvro
 from fabric_mb.message_bus.messages.get_reservations_request_avro import GetReservationsRequestAvro
 from fabric_mb.message_bus.messages.get_reservations_state_request_avro import GetReservationsStateRequestAvro
 from fabric_mb.message_bus.messages.get_unit_request_avro import GetUnitRequestAvro
 from fabric_mb.message_bus.messages.maintenance_request_avro import MaintenanceRequestAvro
 from fabric_mb.message_bus.messages.modify_lease_avro import ModifyLeaseAvro
 from fabric_mb.message_bus.messages.broker_query_model_avro import BrokerQueryModelAvro
+from fabric_mb.message_bus.messages.poa_avro import PoaAvro
+from fabric_mb.message_bus.messages.poa_info_avro import PoaInfoAvro
 from fabric_mb.message_bus.messages.proxy_avro import ProxyAvro
 from fabric_mb.message_bus.messages.request_by_id_record import RequestByIdRecord
 from fabric_mb.message_bus.messages.reservation_or_delegation_record import ReservationOrDelegationRecord
 from fabric_mb.message_bus.messages.reservation_state_avro import ReservationStateAvro
 from fabric_mb.message_bus.messages.resource_ticket_avro import ResourceTicketAvro
 from fabric_mb.message_bus.messages.result_actor_avro import ResultActorAvro
 from fabric_mb.message_bus.messages.result_broker_query_model_avro import ResultBrokerQueryModelAvro
+from fabric_mb.message_bus.messages.result_poa_avro import ResultPoaAvro
 from fabric_mb.message_bus.messages.result_proxy_avro import ResultProxyAvro
 from fabric_mb.message_bus.messages.result_record_list import ResultRecordList
 from fabric_mb.message_bus.messages.result_reservation_avro import ResultReservationAvro
 from fabric_mb.message_bus.messages.get_slices_request_avro import GetSlicesRequestAvro
 from fabric_mb.message_bus.messages.result_reservation_state_avro import ResultReservationStateAvro
 from fabric_mb.message_bus.messages.result_slice_avro import ResultSliceAvro
 from fabric_mb.message_bus.messages.query_avro import QueryAvro
@@ -81,14 +84,15 @@
 from fabric_mb.message_bus.messages.reservation_avro import ReservationAvro
 from fabric_mb.message_bus.messages.reservation_mng import ReservationMng
 from fabric_mb.message_bus.messages.resource_set_avro import ResourceSetAvro
 from fabric_mb.message_bus.messages.result_avro import ResultAvro
 from fabric_mb.message_bus.messages.result_string_avro import ResultStringAvro
 from fabric_mb.message_bus.messages.result_strings_avro import ResultStringsAvro
 from fabric_mb.message_bus.messages.result_units_avro import ResultUnitsAvro
+from fabric_mb.message_bus.messages.site_avro import SiteAvro
 from fabric_mb.message_bus.messages.slice_avro import SliceAvro
 from fabric_mb.message_bus.messages.term_avro import TermAvro
 from fabric_mb.message_bus.messages.ticket import Ticket
 from fabric_mb.message_bus.messages.ticket_avro import TicketAvro
 from fabric_mb.message_bus.messages.ticket_reservation_avro import TicketReservationAvro
 from fabric_mb.message_bus.messages.unit_avro import UnitAvro
 from fabric_mb.message_bus.messages.update_data_avro import UpdateDataAvro
@@ -104,21 +108,23 @@
 class MessageBusTest(unittest.TestCase):
     """
     Implements test functions
     """
     def test_consumer_producer(self):
         from threading import Thread
         import time
-
+        '''
         conf = {'metadata.broker.list': 'localhost:19092',
                 'security.protocol': 'SSL',
                 'ssl.ca.location': '../../../secrets/snakeoil-ca-1.crt',
                 'ssl.key.location': '../../../secrets/kafkacat.client.key',
                 'ssl.key.password': 'confluent',
                 'ssl.certificate.location': '../../../secrets/kafkacat-ca1-signed.pem'}
+        '''
+        conf = {'metadata.broker.list': 'localhost:9092'}
         # Create Admin API object
         api = AdminApi(conf=conf)
 
         for a in api.list_topics():
             print("Topic {}".format(a))
 
         topics = ['fabric_mb-mb-public-test1', 'fabric_mb-mb-public-test2']
@@ -324,14 +330,21 @@
         slice_res.slices = []
         slice_res.slices.append(s1)
 
         #print(slice_res.to_dict())
 
         producer.produce("fabric_mb-mb-public-test2", slice_res)
 
+        poa_res = ResultPoaAvro()
+        poa_res.message_id = "msg12"
+        poa_res.status = result
+        poa_res.poas = PoaInfoAvro(operation="reboot")
+
+        producer.produce("fabric_mb-mb-public-test2", poa_res)
+
         res_req = GetReservationsRequestAvro()
         res_req.message_id = "abc123"
         res_req.callback_topic = "test"
         res_req.guid = "guid"
         res_req.reservation_id = "res123"
         res_req.reservation_type = "broker"
         res_req.auth = auth
@@ -673,21 +686,28 @@
         result_actor.status = result
         result_actor.actors = []
         result_actor.actors.append(actor)
 
         producer.produce("fabric_mb-mb-public-test2", result_actor)
 
         props = {"mode": "True"}
+        site = SiteAvro(name="renc")
         maint_req = MaintenanceRequestAvro(properties=props, actor_guid="am", callback_topic="test", id_token="id_token",
-                                           message_id="mesg-id-1")
+                                           message_id="mesg-id-1", sites=[site])
+
         producer.produce("fabric_mb-mb-public-test2", maint_req)
 
         #add_peer_req = AddPeerAvro(peer=proxy, callback_topic="test", id_token="token", message_id="mg-1")
         #producer.produce("fabric_mb-mb-public-test2", add_peer_req)
 
+        vcpu_cpu_map = [{"vcpu": "1", "cpu": "11"}, {"vcpu": "0", "cpu": "10"}]
+        poa = PoaAvro(operation="cpupin", vcpu_cpu_map=vcpu_cpu_map, callback_topic="test",
+                      id_token="id_token", auth=auth, rid="rid", message_id="mesg-id-1")
+        producer.produce("fabric_mb-mb-public-test2", poa)
+
         # Fallback to earliest to ensure all messages are consumed
         conf['auto.offset.reset'] = "earliest"
 
         print("+++++++++++++++++++++++++++++++++++++++++++++++++++++++++")
         print("++++++++++++++++++++++CONSUMER+++++++++++++++++++++")
         print("+++++++++++++++++++++++++++++++++++++++++++++++++++++++++")
 
@@ -722,14 +742,17 @@
 
                 elif message.get_message_name() == AbcMessageAvro.get_slices_request:
                     self.parent.validate_request_by_id(message, get_slice)
 
                 elif message.get_message_name() == AbcMessageAvro.result_slice:
                     self.parent.validate_result_record(message, slice_res)
 
+                elif message.get_message_name() == AbcMessageAvro.result_poa:
+                    self.parent.validate_result_record(message, poa_res)
+
                 elif message.get_message_name() == AbcMessageAvro.get_reservations_request:
                     self.parent.validate_request_by_id(message, res_req)
 
                 elif message.get_message_name() == AbcMessageAvro.get_delegations:
                     self.parent.validate_request_by_id(message, del_req)
 
                 elif message.get_message_name() == AbcMessageAvro.result_reservation:
@@ -821,14 +844,17 @@
 
                 elif message.get_message_name() == AbcMessageAvro.result_actor:
                     self.parent.validate_result_record(message, result_actor)
 
                 elif message.get_message_name() == AbcMessageAvro.maintenance_request:
                     self.parent.assertEqual(message, maint_req)
 
+                elif message.get_message_name() == AbcMessageAvro.poa:
+                    self.parent.validate_poa(message, poa)
+
                 #elif message.get_message_name() == AbcMessageAvro.add_peer:
                 #    self.parent.assertEqual(message, add_peer_req)
 
         # create a consumer
         conf['group.id'] = 'ssl-host'
         consumer = TestConsumer(consumer_conf=conf, key_schema_location=key_schema,
                                 value_schema_location=value_schema, topics=topics)
@@ -899,26 +925,41 @@
     def validate_ticket(self, incoming: TicketAvro, outgoing: TicketAvro):
         self.assertEqual(incoming.name, outgoing.name)
         self.assertEqual(incoming.message_id, outgoing.message_id)
         self.assertEqual(incoming.reservation, outgoing.reservation)
         self.assertEqual(incoming.auth, outgoing.auth)
         self.assertEqual(incoming.callback_topic, outgoing.callback_topic)
 
+    def validate_poa(self, incoming: PoaAvro, outgoing: PoaAvro):
+        self.assertEqual(incoming.name, outgoing.name)
+        self.assertEqual(incoming.message_id, outgoing.message_id)
+        self.assertEqual(incoming.callback_topic, outgoing.callback_topic)
+        self.assertEqual(incoming.operation, outgoing.operation)
+        self.assertEqual(len(incoming.vcpu_cpu_map), len(outgoing.vcpu_cpu_map))
+        idx = 0
+        for v_c_pair in incoming.vcpu_cpu_map:
+            self.assertEqual(v_c_pair.get("vcpu"), outgoing.vcpu_cpu_map[idx].get("vcpu"))
+            self.assertEqual(v_c_pair.get("cpu"), outgoing.vcpu_cpu_map[idx].get("cpu"))
+            idx += 1
+        self.assertEqual(incoming.node_set, outgoing.node_set)
+        self.assertEqual(incoming.id_token, outgoing.id_token)
+
     def validate_result_record(self, incoming: ResultRecordList, outgoing: ResultRecordList):
         self.assertEqual(incoming.name, outgoing.name)
         self.assertEqual(incoming.message_id, outgoing.message_id)
         self.assertEqual(incoming.status, outgoing.status)
         self.assertEqual(incoming.slices, outgoing.slices)
         self.assertEqual(incoming.reservations, outgoing.reservations)
         self.assertEqual(incoming.reservation_states, outgoing.reservation_states)
         self.assertEqual(incoming.units, outgoing.units)
         self.assertEqual(incoming.proxies, outgoing.proxies)
         self.assertEqual(incoming.model, outgoing.model)
         self.assertEqual(incoming.actors, outgoing.actors)
         self.assertEqual(incoming.delegations, outgoing.delegations)
+        self.assertEqual(incoming.poas, outgoing.poas)
 
     def validate_get_reservations_state_request(self, incoming: GetReservationsStateRequestAvro,
                                                 outgoing: GetReservationsStateRequestAvro):
         self.assertEqual(incoming.name, outgoing.name)
         self.assertEqual(incoming.guid, outgoing.guid)
         self.assertEqual(incoming.message_id, outgoing.message_id)
         self.assertEqual(incoming.reservation_ids, outgoing.reservation_ids)
```

### Comparing `fabric-message-bus-1.5.0b1/pyproject.toml` & `fabric-message-bus-1.5.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/secrets/create-certs.sh` & `fabric-message-bus-1.5.0b2/secrets/create-certs.sh`

 * *Files identical despite different names*

### Comparing `fabric-message-bus-1.5.0b1/PKG-INFO` & `fabric-message-bus-1.5.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-message-bus
-Version: 1.5.0b1
+Version: 1.5.0b2
 Summary: Fabric Message Bus Schema
 Keywords: Kafka,Fabric Message Bus Schema,Avro
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

