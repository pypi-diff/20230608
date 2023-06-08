# Comparing `tmp/pyxplora_api-2.8.0.tar.gz` & `tmp/pyxplora_api-2.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxplora_api-2.8.0.tar", last modified: Wed Jun  7 18:09:39 2023, max compression
+gzip compressed data, was "pyxplora_api-2.8.2.tar", last modified: Thu Jun  8 02:40:44 2023, max compression
```

## Comparing `pyxplora_api-2.8.0.tar` & `pyxplora_api-2.8.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:09:39.757193 pyxplora_api-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    35587 2023-06-07 18:09:39.757193 pyxplora_api-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:09:39.757193 pyxplora_api-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:09:39.745193 pyxplora_api-2.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:09:39.753193 pyxplora_api-2.8.0/src/pyxplora_api/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 18:09:26.000000 pyxplora_api-2.8.0/src/pyxplora_api/const_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/exception_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    44320 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/gql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/gql_handler_async.py
--rw-r--r--   0 runner    (1001) docker     (123)   118669 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (123)    64798 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/gql_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/graphql_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/handler_gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/pyxplora.py
--rw-r--r--   0 runner    (1001) docker     (123)    27431 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/pyxplora_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30113 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/pyxplora_api_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-07 18:09:23.000000 pyxplora_api-2.8.0/src/pyxplora_api/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:09:39.757193 pyxplora_api-2.8.0/src/pyxplora_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35587 2023-06-07 18:09:39.000000 pyxplora_api-2.8.0/src/pyxplora_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 18:09:39.000000 pyxplora_api-2.8.0/src/pyxplora_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:09:39.000000 pyxplora_api-2.8.0/src/pyxplora_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-07 18:09:39.000000 pyxplora_api-2.8.0/src/pyxplora_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 18:09:39.000000 pyxplora_api-2.8.0/src/pyxplora_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:40:44.771526 pyxplora_api-2.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    35587 2023-06-08 02:40:44.771526 pyxplora_api-2.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34609 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 02:40:44.771526 pyxplora_api-2.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:40:44.767526 pyxplora_api-2.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:40:44.767526 pyxplora_api-2.8.2/src/pyxplora_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/const_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/exception_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44320 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/gql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24786 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/gql_handler_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118669 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64798 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/gql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/graphql_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/handler_gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16180 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/pyxplora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27431 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/pyxplora_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30154 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/pyxplora_api_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-06-08 02:40:30.000000 pyxplora_api-2.8.2/src/pyxplora_api/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:40:44.767526 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35587 2023-06-08 02:40:44.000000 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-08 02:40:44.000000 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 02:40:44.000000 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 02:40:44.000000 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 02:40:44.000000 pyxplora_api-2.8.2/src/pyxplora_api.egg-info/top_level.txt
```

### Comparing `pyxplora_api-2.8.0/LICENSE` & `pyxplora_api-2.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/PKG-INFO` & `pyxplora_api-2.8.2/src/pyxplora_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyxplora_api
-Version: 2.8.0
+Name: pyxplora-api
+Version: 2.8.2
 Summary: Python Xplora® Api
 Home-page: https://github.com/Ludy87/pyxplora_api
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyxplora_api/issues
 Keywords: api xplora watch
@@ -198,15 +198,15 @@
 | watchesDynamic()                                                                              | dict[str, any]:       |
 | watchGroups(id: str)                                                                          | dict[str, any]:       |
 | familyInfo(wuid: str, watchId: str, tz: str, date: int)                                       | dict[str, any]:       |
 | avatars(id: str)                                                                              | dict[str, any]:       |
 | submitIncorrectLocationData(wuid: str, lat: str, lng: str, timestamp: str)                    | bool:                 |
 | getAppVersion()                                                                               | dict[str, any]:       |
 | checkEmailOrPhoneExist(type: UserContactType, email: str, countryCode: str, phoneNumber: str) | bool:                 | [2.2.2](https://github.com/Ludy87/pyxplora_api/releases/tag/2.2.2) |
-| refresh_token(wuid: str, refresh_token: str)                                                  | str:                  | [2.8.0](https://github.com/Ludy87/pyxplora_api/releases/tag/2.8.0) |
+| refresh_token(wuid: str, refresh_token: str)                                                  | str:                  | [2.8.0](https://github.com/Ludy87/pyxplora_api/releases/tag/2.8.2) |
 
 ---
 
 ## Country Support
 
 | country name                                 | country code |
 | -------------------------------------------- | ------------ |
```

### Comparing `pyxplora_api-2.8.0/README.md` & `pyxplora_api-2.8.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 | watchesDynamic()                                                                              | dict[str, any]:       |
 | watchGroups(id: str)                                                                          | dict[str, any]:       |
 | familyInfo(wuid: str, watchId: str, tz: str, date: int)                                       | dict[str, any]:       |
 | avatars(id: str)                                                                              | dict[str, any]:       |
 | submitIncorrectLocationData(wuid: str, lat: str, lng: str, timestamp: str)                    | bool:                 |
 | getAppVersion()                                                                               | dict[str, any]:       |
 | checkEmailOrPhoneExist(type: UserContactType, email: str, countryCode: str, phoneNumber: str) | bool:                 | [2.2.2](https://github.com/Ludy87/pyxplora_api/releases/tag/2.2.2) |
-| refresh_token(wuid: str, refresh_token: str)                                                  | str:                  | [2.8.0](https://github.com/Ludy87/pyxplora_api/releases/tag/2.8.0) |
+| refresh_token(wuid: str, refresh_token: str)                                                  | str:                  | [2.8.0](https://github.com/Ludy87/pyxplora_api/releases/tag/2.8.2) |
 
 ---
 
 ## Country Support
 
 | country name                                 | country code |
 | -------------------------------------------- | ------------ |
```

### Comparing `pyxplora_api-2.8.0/setup.py` & `pyxplora_api-2.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/exception_classes.py` & `pyxplora_api-2.8.2/src/pyxplora_api/exception_classes.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/gql_handler.py` & `pyxplora_api-2.8.2/src/pyxplora_api/gql_handler.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/gql_handler_async.py` & `pyxplora_api-2.8.2/src/pyxplora_api/gql_handler_async.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/gql_mutations.py` & `pyxplora_api-2.8.2/src/pyxplora_api/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/gql_queries.py` & `pyxplora_api-2.8.2/src/pyxplora_api/gql_queries.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/graphql_client.py` & `pyxplora_api-2.8.2/src/pyxplora_api/graphql_client.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/handler_gql.py` & `pyxplora_api-2.8.2/src/pyxplora_api/handler_gql.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/model.py` & `pyxplora_api-2.8.2/src/pyxplora_api/model.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/pyxplora.py` & `pyxplora_api-2.8.2/src/pyxplora_api/pyxplora.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/pyxplora_api.py` & `pyxplora_api-2.8.2/src/pyxplora_api/pyxplora_api.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/pyxplora_api_async.py` & `pyxplora_api-2.8.2/src/pyxplora_api/pyxplora_api_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         )
 
     async def _login(self, force_login: bool = False, key=None, sec=None) -> Dict[str, Any]:
         if not self._isConnected() or self._hasTokenExpired() or force_login:
             retryCounter = 0
             while not self._isConnected() and (retryCounter < self.maxRetries + 2):
                 retryCounter += 1
+                self._refresh_token = ""
 
                 # Try to login
                 try:
                     self._issueToken, self._refresh_token = await self._gql_handler.login_a(key, sec)
                 except LoginError as error:
                     self.error_message = error.error_message
                     await asyncio.sleep(self.retryDelay)
```

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api/status.py` & `pyxplora_api-2.8.2/src/pyxplora_api/status.py`

 * *Files identical despite different names*

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api.egg-info/PKG-INFO` & `pyxplora_api-2.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyxplora-api
-Version: 2.8.0
+Name: pyxplora_api
+Version: 2.8.2
 Summary: Python Xplora® Api
 Home-page: https://github.com/Ludy87/pyxplora_api
 Author: Ludy87
 Author-email: android@astra-g.org
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Ludy87/pyxplora_api/issues
 Keywords: api xplora watch
@@ -198,15 +198,15 @@
 | watchesDynamic()                                                                              | dict[str, any]:       |
 | watchGroups(id: str)                                                                          | dict[str, any]:       |
 | familyInfo(wuid: str, watchId: str, tz: str, date: int)                                       | dict[str, any]:       |
 | avatars(id: str)                                                                              | dict[str, any]:       |
 | submitIncorrectLocationData(wuid: str, lat: str, lng: str, timestamp: str)                    | bool:                 |
 | getAppVersion()                                                                               | dict[str, any]:       |
 | checkEmailOrPhoneExist(type: UserContactType, email: str, countryCode: str, phoneNumber: str) | bool:                 | [2.2.2](https://github.com/Ludy87/pyxplora_api/releases/tag/2.2.2) |
-| refresh_token(wuid: str, refresh_token: str)                                                  | str:                  | [2.8.0](https://github.com/Ludy87/pyxplora_api/releases/tag/2.8.0) |
+| refresh_token(wuid: str, refresh_token: str)                                                  | str:                  | [2.8.0](https://github.com/Ludy87/pyxplora_api/releases/tag/2.8.2) |
 
 ---
 
 ## Country Support
 
 | country name                                 | country code |
 | -------------------------------------------- | ------------ |
```

### Comparing `pyxplora_api-2.8.0/src/pyxplora_api.egg-info/SOURCES.txt` & `pyxplora_api-2.8.2/src/pyxplora_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

