# Comparing `tmp/intellect_core-0.1.0.tar.gz` & `tmp/intellect_core-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intellect_core-0.1.0.tar", max compression
+gzip compressed data, was "intellect_core-0.1.1.tar", max compression
```

## Comparing `intellect_core-0.1.0.tar` & `intellect_core-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.1.0/LICENSE
--rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.1.0/intellect_core/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.1.0/intellect_core/dto/__init__.py
--rw-r--r--   0        0        0     2256 2023-05-31 10:07:28.656329 intellect_core-0.1.0/intellect_core/dto/dto.py
--rw-r--r--   0        0        0     1023 2023-05-29 14:54:49.902384 intellect_core-0.1.0/intellect_core/handler.py
--rw-r--r--   0        0        0     5209 2023-06-07 15:02:30.337406 intellect_core-0.1.0/intellect_core/intelletct_server.py
--rw-r--r--   0        0        0      307 2023-06-07 15:03:10.172964 intellect_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-05-29 14:14:55.721473 intellect_core-0.1.1/LICENSE
+-rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 intellect_core-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 14:10:28.656955 intellect_core-0.1.1/intellect_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:57:45.552839 intellect_core-0.1.1/intellect_core/dto/__init__.py
+-rw-r--r--   0        0        0     2256 2023-05-31 10:07:28.656329 intellect_core-0.1.1/intellect_core/dto/dto.py
+-rw-r--r--   0        0        0     1023 2023-05-29 14:54:49.902384 intellect_core-0.1.1/intellect_core/handler.py
+-rw-r--r--   0        0        0     5324 2023-06-08 13:06:35.268211 intellect_core-0.1.1/intellect_core/intelletct_server.py
+-rw-r--r--   0        0        0      307 2023-06-08 13:06:35.264211 intellect_core-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 intellect_core-0.1.1/PKG-INFO
```

### Comparing `intellect_core-0.1.0/intellect_core/dto/dto.py` & `intellect_core-0.1.1/intellect_core/dto/dto.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.1.0/intellect_core/handler.py` & `intellect_core-0.1.1/intellect_core/handler.py`

 * *Files identical despite different names*

### Comparing `intellect_core-0.1.0/intellect_core/intelletct_server.py` & `intellect_core-0.1.1/intellect_core/intelletct_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import json
+
+from asyncio import TimeoutError
 from datetime import datetime, timedelta
 from aiohttp import ClientSession, ClientTimeout, ClientResponse
 from loguru import logger
 
 from intellect_core.dto.dto import IntellectConfigDto, \
     CoreCommand, \
     ObjectType, \
@@ -13,14 +15,15 @@
 
 
 class IntellectWebServer:
     log_debug: bool = False
     config: IntellectConfigDto
     autarization_info: AutarizationInfo
     expire_token_date: str
+
     # =====================================================================================================================
 
     async def _wrap_response(self, response: ClientResponse):
         await response.read()
         if (await response.json()).get("Status") == "ERROR":
             logger.error(await response.json())
         if self.log_debug:
@@ -39,32 +42,32 @@
             return url[0:-1]
         else:
             url = url + f"objid<{objid}>"
             return url
 
     # =====================================================================================================================
     async def autorization(self):
-        session = ClientSession()
-        url = f"http://{self.config.host_user}:{self.config.host_password}@{self.config.intellect_host}:{self.config.intellect_port}/token?expires_in={self.config.token_expires}"
-        try:
-            async with session.request(method="GET", url=url) as response:
-                string = "{" + (await response.text()).replace("\n", ",")[2:-2] + "}"
-                self.autarization_info = AutarizationInfo(**json.loads(string))
-                self.expire_token_date = datetime.now() + timedelta(seconds=self.autarization_info.expires_in)
-                await session.close()
-                if self.log_debug:
-                    logger.debug(f"\nresponse_body: {bytes(await response.read()).decode()}\nresponse: {response}")
-        except OSError as e:
-            await session.close()
-            logger.error(f"Intellect connection error: {e}")
+        timeout = ClientTimeout(total=5)
+        async with ClientSession(timeout=timeout) as session:
+            url = f"http://{self.config.host_user}:{self.config.host_password}@{self.config.intellect_host}:{self.config.intellect_port}/token?expires_in={self.config.token_expires}"
+            logger.debug(url)
+            try:
+                async with session.request(method="GET", url=url) as response:
+                    string = "{" + (await response.text()).replace("\n", ",")[2:-2] + "}"
+                    self.autarization_info = AutarizationInfo(**json.loads(string))
+                    self.expire_token_date = datetime.now() + timedelta(seconds=self.autarization_info.expires_in)
+                    if self.log_debug:
+                        logger.debug(f"\nresponse_body: {bytes(await response.read()).decode()}\nresponse: {response}")
+            except TimeoutError as e:
+                logger.error(f"Intellect connection error timeout: {e}")
+
     # =====================================================================================================================
     async def init(self, intellect_config: IntellectConfigDto):
         self.config = intellect_config
 
-
     async def logic(self, object_type: ObjectType,
                     command: CoreCommand,
                     dto: IntellectVisitDto.Create |
                          IntellectVisitDto.Update |
                          IntellectDepartmentDto.Create |
                          IntellectDepartmentDto.Update = None,
                     objid: int = None) -> None:
```

### Comparing `intellect_core-0.1.0/PKG-INFO` & `intellect_core-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intellect-core
-Version: 0.1.0
+Version: 0.1.1
 Summary: Модуль интеграции с Интеллект
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

