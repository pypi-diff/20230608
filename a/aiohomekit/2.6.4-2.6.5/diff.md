# Comparing `tmp/aiohomekit-2.6.4.tar.gz` & `tmp/aiohomekit-2.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohomekit-2.6.4.tar", max compression
+gzip compressed data, was "aiohomekit-2.6.5.tar", max compression
```

## Comparing `aiohomekit-2.6.4.tar` & `aiohomekit-2.6.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0    11537 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/LICENSE.md
--rw-r--r--   0        0        0     5841 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/README.md
--rw-r--r--   0        0        0     1867 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/__init__.py
--rw-r--r--   0        0        0    18829 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/__main__.py
--rw-r--r--   0        0        0     4465 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/characteristic_cache.py
--rw-r--r--   0        0        0     1162 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/const.py
--rw-r--r--   0        0        0      697 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/__init__.py
--rw-r--r--   0        0        0    15767 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/abstract.py
--rw-r--r--   0        0        0      704 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/__init__.py
--rw-r--r--   0        0        0     6832 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/bleak.py
--rw-r--r--   0        0        0     7819 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/client.py
--rw-r--r--   0        0        0     2017 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/connection.py
--rw-r--r--   0        0        0     1310 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/const.py
--rw-r--r--   0        0        0     7024 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/controller.py
--rw-r--r--   0        0        0     7614 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/discovery.py
--rw-r--r--   0        0        0     1894 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/key.py
--rw-r--r--   0        0        0     3749 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/manufacturer_data.py
--rw-r--r--   0        0        0    68500 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/pairing.py
--rw-r--r--   0        0        0    11737 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/structs.py
--rw-r--r--   0        0        0     2140 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ble/values.py
--rw-r--r--   0        0        0      708 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/__init__.py
--rw-r--r--   0        0        0    25705 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/connection.py
--rw-r--r--   0        0        0     1182 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/controller.py
--rw-r--r--   0        0        0     2422 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/discovery.py
--rw-r--r--   0        0        0     9972 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/pairing.py
--rw-r--r--   0        0        0     3433 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/pdu.py
--rw-r--r--   0        0        0    12547 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/coap/structs.py
--rw-r--r--   0        0        0     9288 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/controller.py
--rw-r--r--   0        0        0      757 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ip/__init__.py
--rw-r--r--   0        0        0    22040 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ip/connection.py
--rw-r--r--   0        0        0     1120 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ip/controller.py
--rw-r--r--   0        0        0     4108 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ip/discovery.py
--rw-r--r--   0        0        0    20914 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/controller/ip/pairing.py
--rw-r--r--   0        0        0      868 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/crypto/__init__.py
--rw-r--r--   0        0        0     4789 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/crypto/chacha20poly1305.py
--rw-r--r--   0        0        0     1036 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/crypto/hkdf.py
--rw-r--r--   0        0        0    10728 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/crypto/srp.py
--rw-r--r--   0        0        0     4060 2023-06-01 21:57:55.262368 aiohomekit-2.6.4/aiohomekit/debounce.py
--rw-r--r--   0        0        0      985 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/enum.py
--rw-r--r--   0        0        0     7746 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/exceptions.py
--rw-r--r--   0        0        0     2116 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/hkjson.py
--rw-r--r--   0        0        0     2049 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/http/__init__.py
--rw-r--r--   0        0        0     5265 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/http/response.py
--rw-r--r--   0        0        0     2609 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/meshcop.py
--rw-r--r--   0        0        0    12582 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/__init__.py
--rw-r--r--   0        0        0     1245 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/categories.py
--rw-r--r--   0        0        0     1892 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/__init__.py
--rw-r--r--   0        0        0    14170 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic.py
--rw-r--r--   0        0        0     1815 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic_formats.py
--rw-r--r--   0        0        0    22463 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic_types.py
--rw-r--r--   0        0        0     4956 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/const.py
--rw-r--r--   0        0        0    29366 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/data.py
--rw-r--r--   0        0        0      800 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/permissions.py
--rw-r--r--   0        0        0     4410 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/structs.py
--rw-r--r--   0        0        0      731 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/types.py
--rw-r--r--   0        0        0     1067 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/characteristics/units.py
--rw-r--r--   0        0        0     1439 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/entity_map.py
--rw-r--r--   0        0        0      723 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/feature_flags.py
--rw-r--r--   0        0        0      685 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/mixin.py
--rw-r--r--   0        0        0      796 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/services/__init__.py
--rw-r--r--   0        0        0    19993 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/services/data.py
--rw-r--r--   0        0        0     5021 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/services/service.py
--rw-r--r--   0        0        0     5380 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/services/service_types.py
--rw-r--r--   0        0        0      703 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/services/types.py
--rw-r--r--   0        0        0      717 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/model/status_flags.py
--rw-r--r--   0        0        0     4067 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/pdu.py
--rw-r--r--   0        0        0    20539 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/protocol/__init__.py
--rw-r--r--   0        0        0     3494 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/protocol/statuscodes.py
--rw-r--r--   0        0        0     8483 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/protocol/tlv.py
--rw-r--r--   0        0        0        0 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/py.typed
--rw-r--r--   0        0        0    12836 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/testing.py
--rw-r--r--   0        0        0     8265 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/tlv8.py
--rw-r--r--   0        0        0     3581 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/utils.py
--rw-r--r--   0        0        0     1662 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/uuid.py
--rw-r--r--   0        0        0    11606 2023-06-01 21:57:55.266368 aiohomekit-2.6.4/aiohomekit/zeroconf.py
--rw-r--r--   0        0        0     1809 2023-06-01 21:57:55.270367 aiohomekit-2.6.4/pyproject.toml
--rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 aiohomekit-2.6.4/PKG-INFO
+-rw-r--r--   0        0        0    11537 2023-06-08 11:57:27.219518 aiohomekit-2.6.5/LICENSE.md
+-rw-r--r--   0        0        0     5841 2023-06-08 11:57:27.219518 aiohomekit-2.6.5/README.md
+-rw-r--r--   0        0        0     1867 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/__init__.py
+-rw-r--r--   0        0        0    18829 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/__main__.py
+-rw-r--r--   0        0        0     4465 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/characteristic_cache.py
+-rw-r--r--   0        0        0     1162 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/const.py
+-rw-r--r--   0        0        0      697 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/__init__.py
+-rw-r--r--   0        0        0    15767 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/abstract.py
+-rw-r--r--   0        0        0      704 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/__init__.py
+-rw-r--r--   0        0        0     6832 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/bleak.py
+-rw-r--r--   0        0        0     7819 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/client.py
+-rw-r--r--   0        0        0     2017 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/connection.py
+-rw-r--r--   0        0        0     1310 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/const.py
+-rw-r--r--   0        0        0     7024 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/controller.py
+-rw-r--r--   0        0        0     7614 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/discovery.py
+-rw-r--r--   0        0        0     1894 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/key.py
+-rw-r--r--   0        0        0     3749 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/manufacturer_data.py
+-rw-r--r--   0        0        0    68500 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/pairing.py
+-rw-r--r--   0        0        0    11737 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/structs.py
+-rw-r--r--   0        0        0     2140 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ble/values.py
+-rw-r--r--   0        0        0      708 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/__init__.py
+-rw-r--r--   0        0        0    25705 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/connection.py
+-rw-r--r--   0        0        0     1182 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/controller.py
+-rw-r--r--   0        0        0     2422 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/discovery.py
+-rw-r--r--   0        0        0     9972 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/pairing.py
+-rw-r--r--   0        0        0     3433 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/pdu.py
+-rw-r--r--   0        0        0    12547 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/coap/structs.py
+-rw-r--r--   0        0        0     9288 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/controller.py
+-rw-r--r--   0        0        0      757 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ip/__init__.py
+-rw-r--r--   0        0        0    22146 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ip/connection.py
+-rw-r--r--   0        0        0     1120 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ip/controller.py
+-rw-r--r--   0        0        0     4108 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ip/discovery.py
+-rw-r--r--   0        0        0    20914 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/controller/ip/pairing.py
+-rw-r--r--   0        0        0      868 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/crypto/__init__.py
+-rw-r--r--   0        0        0     4789 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/crypto/chacha20poly1305.py
+-rw-r--r--   0        0        0     1036 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/crypto/hkdf.py
+-rw-r--r--   0        0        0    10728 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/crypto/srp.py
+-rw-r--r--   0        0        0     4060 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/debounce.py
+-rw-r--r--   0        0        0      985 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/enum.py
+-rw-r--r--   0        0        0     7746 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/exceptions.py
+-rw-r--r--   0        0        0     2116 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/hkjson.py
+-rw-r--r--   0        0        0     2044 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/http/__init__.py
+-rw-r--r--   0        0        0     5265 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/http/response.py
+-rw-r--r--   0        0        0     2609 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/meshcop.py
+-rw-r--r--   0        0        0    12839 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/__init__.py
+-rw-r--r--   0        0        0     1245 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/categories.py
+-rw-r--r--   0        0        0     1892 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/__init__.py
+-rw-r--r--   0        0        0    14170 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic.py
+-rw-r--r--   0        0        0     1815 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic_formats.py
+-rw-r--r--   0        0        0    22463 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic_types.py
+-rw-r--r--   0        0        0     4956 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/const.py
+-rw-r--r--   0        0        0    29366 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/data.py
+-rw-r--r--   0        0        0      800 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/permissions.py
+-rw-r--r--   0        0        0     4410 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/structs.py
+-rw-r--r--   0        0        0      731 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/types.py
+-rw-r--r--   0        0        0     1067 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/characteristics/units.py
+-rw-r--r--   0        0        0     1439 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/entity_map.py
+-rw-r--r--   0        0        0      723 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/feature_flags.py
+-rw-r--r--   0        0        0      685 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/mixin.py
+-rw-r--r--   0        0        0      796 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/services/__init__.py
+-rw-r--r--   0        0        0    19993 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/services/data.py
+-rw-r--r--   0        0        0     5021 2023-06-08 11:57:27.223518 aiohomekit-2.6.5/aiohomekit/model/services/service.py
+-rw-r--r--   0        0        0     5380 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/model/services/service_types.py
+-rw-r--r--   0        0        0      703 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/model/services/types.py
+-rw-r--r--   0        0        0      717 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/model/status_flags.py
+-rw-r--r--   0        0        0     4067 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/pdu.py
+-rw-r--r--   0        0        0    20539 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/protocol/__init__.py
+-rw-r--r--   0        0        0     3494 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/protocol/statuscodes.py
+-rw-r--r--   0        0        0     8483 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/protocol/tlv.py
+-rw-r--r--   0        0        0        0 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/py.typed
+-rw-r--r--   0        0        0    12836 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/testing.py
+-rw-r--r--   0        0        0     8265 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/tlv8.py
+-rw-r--r--   0        0        0     3581 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/utils.py
+-rw-r--r--   0        0        0     1662 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/uuid.py
+-rw-r--r--   0        0        0    11606 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/aiohomekit/zeroconf.py
+-rw-r--r--   0        0        0     1809 2023-06-08 11:57:27.227518 aiohomekit-2.6.5/pyproject.toml
+-rw-r--r--   0        0        0     7021 1970-01-01 00:00:00.000000 aiohomekit-2.6.5/PKG-INFO
```

### Comparing `aiohomekit-2.6.4/LICENSE.md` & `aiohomekit-2.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/README.md` & `aiohomekit-2.6.5/README.md`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/__init__.py` & `aiohomekit-2.6.5/aiohomekit/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/__main__.py` & `aiohomekit-2.6.5/aiohomekit/__main__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/characteristic_cache.py` & `aiohomekit-2.6.5/aiohomekit/characteristic_cache.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/const.py` & `aiohomekit-2.6.5/aiohomekit/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/__init__.py` & `aiohomekit-2.6.5/aiohomekit/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/abstract.py` & `aiohomekit-2.6.5/aiohomekit/controller/abstract.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/__init__.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/bleak.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/bleak.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/client.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/client.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/connection.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/const.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/controller.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/discovery.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/key.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/key.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/manufacturer_data.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/manufacturer_data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/pairing.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/structs.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ble/values.py` & `aiohomekit-2.6.5/aiohomekit/controller/ble/values.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/coap/__init__.py` & `aiohomekit-2.6.5/aiohomekit/controller/coap/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/coap/connection.py` & `aiohomekit-2.6.5/aiohomekit/controller/coap/connection.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/coap/controller.py` & `aiohomekit-2.6.5/aiohomekit/controller/coap/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/coap/discovery.py` & `aiohomekit-2.6.5/aiohomekit/controller/coap/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/coap/pairing.py` & `aiohomekit-2.6.5/aiohomekit/controller/coap/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/coap/pdu.py` & `aiohomekit-2.6.5/aiohomekit/controller/coap/pdu.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/coap/structs.py` & `aiohomekit-2.6.5/aiohomekit/controller/coap/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/controller.py` & `aiohomekit-2.6.5/aiohomekit/controller/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ip/__init__.py` & `aiohomekit-2.6.5/aiohomekit/controller/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ip/connection.py` & `aiohomekit-2.6.5/aiohomekit/controller/ip/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -318,15 +318,18 @@
         """
         Sends a HTTP POST request to the current transport and returns an awaitable
         that can be used to wait for a response.
         """
         return await self.request(
             method="PUT",
             target=target,
-            headers=[("Content-Length", len(body)), ("Content-Type", content_type)],
+            headers=[
+                ("Content-Length", len(body)),
+                ("Content-Type", content_type.value),
+            ],
             body=body,
         )
 
     async def put_json(self, target, body):
         response = await self.put(
             target,
             hkjson.dump_bytes(body),
@@ -358,15 +361,18 @@
         """
         Sends a HTTP POST request to the current transport and returns an awaitable
         that can be used to wait for a response.
         """
         return await self.request(
             method="POST",
             target=target,
-            headers=[("Content-Length", len(body)), ("Content-Type", content_type)],
+            headers=[
+                ("Content-Length", len(body)),
+                ("Content-Type", content_type.value),
+            ],
             body=body,
         )
 
     async def post_json(self, target, body):
         response = await self.post(
             target,
             hkjson.dump_bytes(body),
```

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ip/controller.py` & `aiohomekit-2.6.5/aiohomekit/controller/ip/controller.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ip/discovery.py` & `aiohomekit-2.6.5/aiohomekit/controller/ip/discovery.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/controller/ip/pairing.py` & `aiohomekit-2.6.5/aiohomekit/controller/ip/pairing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/crypto/__init__.py` & `aiohomekit-2.6.5/aiohomekit/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/crypto/chacha20poly1305.py` & `aiohomekit-2.6.5/aiohomekit/crypto/chacha20poly1305.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/crypto/hkdf.py` & `aiohomekit-2.6.5/aiohomekit/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/crypto/srp.py` & `aiohomekit-2.6.5/aiohomekit/crypto/srp.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/debounce.py` & `aiohomekit-2.6.5/aiohomekit/debounce.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/enum.py` & `aiohomekit-2.6.5/aiohomekit/enum.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/exceptions.py` & `aiohomekit-2.6.5/aiohomekit/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/hkjson.py` & `aiohomekit-2.6.5/aiohomekit/hkjson.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/http/__init__.py` & `aiohomekit-2.6.5/aiohomekit/http/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 #
 
 import enum
 
 __all__ = ["HttpContentTypes", "HttpStatusCodes"]
 
 
-class HttpContentTypes(str, enum.Enum):
+class HttpContentTypes(enum.Enum):
     """
     Collection of HTTP content types as used in HTTP headers
     """
 
     JSON = "application/hap+json"
     TLV = "application/pairing+tlv8"
```

### Comparing `aiohomekit-2.6.4/aiohomekit/http/response.py` & `aiohomekit-2.6.5/aiohomekit/http/response.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/meshcop.py` & `aiohomekit-2.6.5/aiohomekit/meshcop.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/__init__.py` & `aiohomekit-2.6.5/aiohomekit/model/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -156,19 +156,21 @@
         self._services = services
 
     def iid(self, iid: int) -> Characteristic | None:
         return self._services.get_char_by_iid(iid)
 
 
 class Accessory:
-    def __init__(self):
+    def __init__(self) -> None:
+        """Initialize a new accessory."""
         self.aid = get_id()
         self._next_id = 0
         self.services = Services()
         self.characteristics = Characteristics(self.services)
+        self._accessory_information: Service | None = None
 
     @classmethod
     def create_with_info(
         cls,
         name: str,
         manufacturer: str,
         model: str,
@@ -193,15 +195,19 @@
         )
 
         return self
 
     @property
     def accessory_information(self) -> Service:
         """Returns the ACCESSORY_INFORMATION service for this accessory."""
-        return self.services.first(service_type=ServicesTypes.ACCESSORY_INFORMATION)
+        if self._accessory_information is None:
+            self._accessory_information = self.services.first(
+                service_type=ServicesTypes.ACCESSORY_INFORMATION
+            )
+        return self._accessory_information
 
     @property
     def name(self) -> str:
         return self.accessory_information.value(CharacteristicsTypes.NAME, "")
 
     @property
     def manufacturer(self) -> str:
```

### Comparing `aiohomekit-2.6.4/aiohomekit/model/categories.py` & `aiohomekit-2.6.5/aiohomekit/model/categories.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/characteristics/__init__.py` & `aiohomekit-2.6.5/aiohomekit/model/characteristics/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic.py` & `aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic_formats.py` & `aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic_formats.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/characteristics/characteristic_types.py` & `aiohomekit-2.6.5/aiohomekit/model/characteristics/characteristic_types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/characteristics/const.py` & `aiohomekit-2.6.5/aiohomekit/model/characteristics/const.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/characteristics/data.py` & `aiohomekit-2.6.5/aiohomekit/model/characteristics/data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/characteristics/permissions.py` & `aiohomekit-2.6.5/aiohomekit/model/characteristics/permissions.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/characteristics/structs.py` & `aiohomekit-2.6.5/aiohomekit/model/characteristics/structs.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/characteristics/types.py` & `aiohomekit-2.6.5/aiohomekit/model/characteristics/types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/characteristics/units.py` & `aiohomekit-2.6.5/aiohomekit/model/characteristics/units.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/entity_map.py` & `aiohomekit-2.6.5/aiohomekit/model/entity_map.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/feature_flags.py` & `aiohomekit-2.6.5/aiohomekit/model/feature_flags.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/mixin.py` & `aiohomekit-2.6.5/aiohomekit/model/mixin.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/services/__init__.py` & `aiohomekit-2.6.5/aiohomekit/model/services/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/services/data.py` & `aiohomekit-2.6.5/aiohomekit/model/services/data.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/services/service.py` & `aiohomekit-2.6.5/aiohomekit/model/services/service.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/services/service_types.py` & `aiohomekit-2.6.5/aiohomekit/model/services/service_types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/services/types.py` & `aiohomekit-2.6.5/aiohomekit/model/services/types.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/model/status_flags.py` & `aiohomekit-2.6.5/aiohomekit/model/status_flags.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/pdu.py` & `aiohomekit-2.6.5/aiohomekit/pdu.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/protocol/__init__.py` & `aiohomekit-2.6.5/aiohomekit/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/protocol/statuscodes.py` & `aiohomekit-2.6.5/aiohomekit/protocol/statuscodes.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/protocol/tlv.py` & `aiohomekit-2.6.5/aiohomekit/protocol/tlv.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/testing.py` & `aiohomekit-2.6.5/aiohomekit/testing.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/tlv8.py` & `aiohomekit-2.6.5/aiohomekit/tlv8.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/utils.py` & `aiohomekit-2.6.5/aiohomekit/utils.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/uuid.py` & `aiohomekit-2.6.5/aiohomekit/uuid.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/aiohomekit/zeroconf.py` & `aiohomekit-2.6.5/aiohomekit/zeroconf.py`

 * *Files identical despite different names*

### Comparing `aiohomekit-2.6.4/pyproject.toml` & `aiohomekit-2.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiohomekit"
-version = "2.6.4"
+version = "2.6.5"
 description = "An asyncio HomeKit client"
 authors = ["John Carr <john.carr@unrouted.co.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/Jc2k/aiohomekit"
 repository = "https://github.com/Jc2k/aiohomekit"
 keywords = ["HomeKit", "home", "automation"]
```

### Comparing `aiohomekit-2.6.4/PKG-INFO` & `aiohomekit-2.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohomekit
-Version: 2.6.4
+Version: 2.6.5
 Summary: An asyncio HomeKit client
 Home-page: https://github.com/Jc2k/aiohomekit
 License: Apache-2.0
 Keywords: HomeKit,home,automation
 Author: John Carr
 Author-email: john.carr@unrouted.co.uk
 Requires-Python: >=3.9,<4.0
```

