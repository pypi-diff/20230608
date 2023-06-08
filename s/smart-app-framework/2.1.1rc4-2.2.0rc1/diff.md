# Comparing `tmp/smart_app_framework-2.1.1rc4-py3-none-any.whl.zip` & `tmp/smart_app_framework-2.2.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 307044 bytes, number of entries: 334
+Zip file size: 307125 bytes, number of entries: 334
 -rw-r--r--  2.0 unx      113 b- defN 80-Jan-01 00:00 core/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/basic_models/actions/__init__.py
 -rw-r--r--  2.0 unx    10756 b- defN 80-Jan-01 00:00 core/basic_models/actions/basic_actions.py
 -rw-r--r--  2.0 unx     6265 b- defN 80-Jan-01 00:00 core/basic_models/actions/client_profile_actions.py
 -rw-r--r--  2.0 unx     1203 b- defN 80-Jan-01 00:00 core/basic_models/actions/command.py
 -rw-r--r--  2.0 unx     3083 b- defN 80-Jan-01 00:00 core/basic_models/actions/counter_actions.py
@@ -62,15 +62,15 @@
 -rw-r--r--  2.0 unx      568 b- defN 80-Jan-01 00:00 core/logging/logger_constants.py
 -rw-r--r--  2.0 unx      937 b- defN 80-Jan-01 00:00 core/logging/logger_formatter.py
 -rw-r--r--  2.0 unx      386 b- defN 80-Jan-01 00:00 core/logging/logger_handlers.py
 -rw-r--r--  2.0 unx     5264 b- defN 80-Jan-01 00:00 core/logging/logger_utils.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/message/__init__.py
 -rw-r--r--  2.0 unx      765 b- defN 80-Jan-01 00:00 core/message/app_info.py
 -rw-r--r--  2.0 unx     1370 b- defN 80-Jan-01 00:00 core/message/device.py
--rw-r--r--  2.0 unx     9237 b- defN 80-Jan-01 00:00 core/message/from_message.py
+-rw-r--r--  2.0 unx     9475 b- defN 80-Jan-01 00:00 core/message/from_message.py
 -rw-r--r--  2.0 unx      120 b- defN 80-Jan-01 00:00 core/message/message_constants.py
 -rw-r--r--  2.0 unx      179 b- defN 80-Jan-01 00:00 core/message/msg_validator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/model/__init__.py
 -rw-r--r--  2.0 unx     3159 b- defN 80-Jan-01 00:00 core/model/base_user.py
 -rw-r--r--  2.0 unx     2817 b- defN 80-Jan-01 00:00 core/model/factory.py
 -rw-r--r--  2.0 unx      209 b- defN 80-Jan-01 00:00 core/model/field.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 core/model/heapq/__init__.py
@@ -326,11 +326,11 @@
 -rw-r--r--  2.0 unx     1325 b- defN 80-Jan-01 00:00 smart_kit/utils/cache.py
 -rw-r--r--  2.0 unx     2899 b- defN 80-Jan-01 00:00 smart_kit/utils/diff.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/__init__.py
 -rw-r--r--  2.0 unx     3385 b- defN 80-Jan-01 00:00 smart_kit/utils/logger_writer/logger_formatter.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 smart_kit/utils/monitoring.py
 -rw-r--r--  2.0 unx      332 b- defN 80-Jan-01 00:00 smart_kit/utils/object_location.py
 -rw-r--r--  2.0 unx      320 b- defN 80-Jan-01 00:00 smart_kit/utils/picklable_mock.py
--rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.1.1rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.1.1rc4.dist-info/WHEEL
-?rw-r--r--  2.0 unx    32375 b- defN 16-Jan-01 00:00 smart_app_framework-2.1.1rc4.dist-info/RECORD
-334 files, 987734 bytes uncompressed, 254262 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx    10823 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 smart_app_framework-2.2.0rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    32375 b- defN 16-Jan-01 00:00 smart_app_framework-2.2.0rc1.dist-info/RECORD
+334 files, 987972 bytes uncompressed, 254343 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -987,17 +987,17 @@
 
 Filename: smart_kit/utils/object_location.py
 Comment: 
 
 Filename: smart_kit/utils/picklable_mock.py
 Comment: 
 
-Filename: smart_app_framework-2.1.1rc4.dist-info/METADATA
+Filename: smart_app_framework-2.2.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: smart_app_framework-2.1.1rc4.dist-info/WHEEL
+Filename: smart_app_framework-2.2.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: smart_app_framework-2.1.1rc4.dist-info/RECORD
+Filename: smart_app_framework-2.2.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## core/message/from_message.py

```diff
@@ -40,14 +40,20 @@
     MESSAGE_NAME = "messageName"
     MESSAGE_ID = "messageId"
     UUID = "uuid"
     PAYLOAD = "payload"
     SESSION_ID = "sessionId"
     CALLBACK_ID_HEADER_NAME = CALLBACK_ID_HEADER
 
+    _REQUIRED_FIELDS_MAP = {
+        None: {MESSAGE_ID, UUID, PAYLOAD, SESSION_ID, MESSAGE_NAME},  # default
+        "PUSH_RESULT": {MESSAGE_ID, MESSAGE_NAME},
+        "PUSH_SENDING_RESULT": {MESSAGE_ID, MESSAGE_NAME}
+    }
+
     # following fields are used for validation
     incremental_id: int
     message_name: str
     payload: dict
     uuid: dict
 
     def __init__(self, value: Dict[str, Any], topic_key: str = None, creation_time: Optional[int] = None,
@@ -74,15 +80,17 @@
                 return False
 
         if self._headers_required and not self.headers:
             log("Message headers is empty", level="ERROR")
             return False
 
         try:
-            for r_field in self._required_fields:
+            message_name = self.as_dict.get(self.MESSAGE_NAME)
+            required_fields = self._REQUIRED_FIELDS_MAP.get(message_name) or self._REQUIRED_FIELDS_MAP[None]
+            for r_field in required_fields:
                 if r_field not in self.as_dict:
                     self.print_validation_error(r_field)
                     return False
 
                 if r_field not in self.__annotations__:
                     continue
 
@@ -143,18 +151,14 @@
             log("Message validation error: Message is empty", level="ERROR")
 
     @property
     def _callback_id_header_name(self) -> str:
         return CALLBACK_ID_HEADER
 
     @property
-    def _required_fields(self) -> Set[str]:
-        return {self.MESSAGE_ID, self.UUID, self.PAYLOAD, self.SESSION_ID, self.MESSAGE_NAME}
-
-    @property
     def session_id(self) -> Optional[str]:
         return self.as_dict.get(self.SESSION_ID)
 
     # database user_id
     @property
     def db_uid(self) -> str:
         return "{}_{}".format(self.uid, self.channel)
```

## Comparing `smart_app_framework-2.1.1rc4.dist-info/METADATA` & `smart_app_framework-2.2.0rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart-app-framework
-Version: 2.1.1rc4
+Version: 2.2.0rc1
 Summary: Python-фреймворк, который позволяет создавать смартапы для виртуальных ассистентов Салют.
 Author: Salute Developers
 Author-email: developer@sberdevices.ru
 Requires-Python: >=3.8.1,<3.12
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
```

## Comparing `smart_app_framework-2.1.1rc4.dist-info/RECORD` & `smart_app_framework-2.2.0rc1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 core/logging/logger_constants.py,sha256=hn56NJa4uT94uZ56W7nVFxV8rJp2fczrBHJLhh2XFPM,568
 core/logging/logger_formatter.py,sha256=3gBZq87MQIj2f45MF5AcsJNAoLJVM6aUYE7C2hd-6p0,937
 core/logging/logger_handlers.py,sha256=RWetoI6jCU7UUnZrxKol0kPxOLRaMSv-h0VhzUSC5y8,386
 core/logging/logger_utils.py,sha256=gwbCzCFmdtxj0RfKOXG4HfW--YOPttHWKf8GycFvBF8,5264
 core/message/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/message/app_info.py,sha256=N35Q5NIuwi7CADWt8DqLcg97h0IVt9Up6WhQhwmdeZ4,765
 core/message/device.py,sha256=u7XbFgDDx7n8vScd_KgMySt_ztrYnoRzwmfr4ukMOFo,1370
-core/message/from_message.py,sha256=acy1FzQr8WdfOGXzkk-h-Ck1NmM1a5dKWjiFkbs579Q,9237
+core/message/from_message.py,sha256=b3-5-uOrFCU1xJ2EChW5lh7fQHGgJjyNE5lPaQkt7A4,9475
 core/message/message_constants.py,sha256=K_ZvW_IvW7bBDo5PrrWFBlfPGq9WJQuz5a4O9YWmEsc,120
 core/message/msg_validator.py,sha256=tFm5A9yTE5HoPntYPS5057c43viDuODNLryeL2mRzUI,179
 core/model/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 core/model/base_user.py,sha256=m2vtxxan7ow1JLo6BHIKsGsqXOUGR3WCztHyfNXJ10w,3159
 core/model/factory.py,sha256=7OlLQPmiEv0Gcaa13eahwN6WJ14hxii6tgRxUu--fNA,2817
 core/model/field.py,sha256=D2YvHG_9NnLS1uU5PaMPFUrFhypgv9FD1JfoAOk5fEw,209
 core/model/heapq/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -325,10 +325,10 @@
 smart_kit/utils/cache.py,sha256=Lut5HMkfoeiRwCCnZoSHw7srWYn3Y0fD-hUJWckDBf8,1325
 smart_kit/utils/diff.py,sha256=rUdzi6f8mtXacNL6HvVYVoOnXD_M3FEMHFsMhPo0YL0,2899
 smart_kit/utils/logger_writer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/logger_writer/logger_formatter.py,sha256=bC7tdYW480irANhxaFxiKgnAsvmz-luf52WSu7ZjnIU,3385
 smart_kit/utils/monitoring.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 smart_kit/utils/object_location.py,sha256=uJmTxBBeeyvwahiA1TMKr2rzDW9R1bh-FwK663zoBe4,332
 smart_kit/utils/picklable_mock.py,sha256=PxrgnKue58GFpVZMBGIQq36LPnITFzfNA21euCbfViE,320
-smart_app_framework-2.1.1rc4.dist-info/METADATA,sha256=BR-Ks-GN_SVRhIdY3XtG-kKAZS_wYF5fTCXxUZ_2Bho,10823
-smart_app_framework-2.1.1rc4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-smart_app_framework-2.1.1rc4.dist-info/RECORD,,
+smart_app_framework-2.2.0rc1.dist-info/METADATA,sha256=ffzo1oCWUmHOEcHICAuwfw-WfJAUk92gr_ukg-JR15E,10823
+smart_app_framework-2.2.0rc1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+smart_app_framework-2.2.0rc1.dist-info/RECORD,,
```

