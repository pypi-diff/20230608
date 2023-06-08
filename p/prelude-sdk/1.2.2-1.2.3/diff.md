# Comparing `tmp/prelude-sdk-1.2.2.tar.gz` & `tmp/prelude-sdk-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-sdk-1.2.2.tar", last modified: Fri Jun  2 17:12:33 2023, max compression
+gzip compressed data, was "prelude-sdk-1.2.3.tar", last modified: Wed Jun  7 21:03:27 2023, max compression
```

## Comparing `prelude-sdk-1.2.2.tar` & `prelude-sdk-1.2.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.154370 prelude-sdk-1.2.2/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.2.2/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-02 17:12:33.154420 prelude-sdk-1.2.2/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.2.2/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.150192 prelude-sdk-1.2.2/prelude_sdk/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.2/prelude_sdk/__init__.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.151974 prelude-sdk-1.2.2/prelude_sdk/controllers/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1587 2023-06-02 13:58:42.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4923 2023-05-22 15:57:51.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3266 2023-05-12 13:56:19.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     2057 2023-05-23 21:42:11.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/partner_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.2.2/prelude_sdk/controllers/probe_controller.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.152640 prelude-sdk-1.2.2/prelude_sdk/models/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.2/prelude_sdk/models/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.2.2/prelude_sdk/models/account.py
--rw-r--r--   0 pack       (501) staff       (20)     2555 2023-05-22 15:57:51.000000 prelude-sdk-1.2.2/prelude_sdk/models/codes.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.150769 prelude-sdk-1.2.2/prelude_sdk.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-02 17:12:33.000000 prelude-sdk-1.2.2/prelude_sdk.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      773 2023-06-02 17:12:33.000000 prelude-sdk-1.2.2/prelude_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-02 17:12:33.000000 prelude-sdk-1.2.2/prelude_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)        9 2023-06-02 17:12:33.000000 prelude-sdk-1.2.2/prelude_sdk.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       18 2023-06-02 17:12:33.000000 prelude-sdk-1.2.2/prelude_sdk.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.2.2/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      532 2023-06-02 17:12:33.154626 prelude-sdk-1.2.2/setup.cfg
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.154086 prelude-sdk-1.2.2/tests/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.2/tests/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.2.2/tests/conftest.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-02 17:12:33.154287 prelude-sdk-1.2.2/tests/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.2/tests/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1662 2023-06-01 16:01:25.000000 prelude-sdk-1.2.2/tests/test_build_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     4623 2023-05-23 21:42:11.000000 prelude-sdk-1.2.2/tests/test_detect_controller.py
--rw-r--r--   0 pack       (501) staff       (20)     3223 2023-05-23 21:42:11.000000 prelude-sdk-1.2.2/tests/test_iam_controller.py
--rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.2.2/tests/test_probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:03:27.981855 prelude-sdk-1.2.3/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-sdk-1.2.3/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-07 21:03:27.981917 prelude-sdk-1.2.3/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      697 2023-04-11 22:16:02.000000 prelude-sdk-1.2.3/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:03:27.977612 prelude-sdk-1.2.3/prelude_sdk/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.3/prelude_sdk/__init__.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:03:27.979654 prelude-sdk-1.2.3/prelude_sdk/controllers/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.3/prelude_sdk/controllers/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2248 2023-06-06 22:22:58.000000 prelude-sdk-1.2.3/prelude_sdk/controllers/build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5438 2023-06-06 22:22:58.000000 prelude-sdk-1.2.3/prelude_sdk/controllers/detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3703 2023-06-07 20:52:19.000000 prelude-sdk-1.2.3/prelude_sdk/controllers/iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     2057 2023-05-23 21:42:11.000000 prelude-sdk-1.2.3/prelude_sdk/controllers/partner_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      443 2023-05-03 13:30:52.000000 prelude-sdk-1.2.3/prelude_sdk/controllers/probe_controller.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:03:27.980334 prelude-sdk-1.2.3/prelude_sdk/models/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-sdk-1.2.3/prelude_sdk/models/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2816 2023-04-07 19:23:14.000000 prelude-sdk-1.2.3/prelude_sdk/models/account.py
+-rw-r--r--   0 pack       (501) staff       (20)     2555 2023-05-22 15:57:51.000000 prelude-sdk-1.2.3/prelude_sdk/models/codes.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:03:27.978249 prelude-sdk-1.2.3/prelude_sdk.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-06-07 21:03:27.000000 prelude-sdk-1.2.3/prelude_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      773 2023-06-07 21:03:27.000000 prelude-sdk-1.2.3/prelude_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-07 21:03:27.000000 prelude-sdk-1.2.3/prelude_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)        9 2023-06-07 21:03:27.000000 prelude-sdk-1.2.3/prelude_sdk.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       18 2023-06-07 21:03:27.000000 prelude-sdk-1.2.3/prelude_sdk.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-sdk-1.2.3/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      532 2023-06-07 21:03:27.982142 prelude-sdk-1.2.3/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:03:27.981513 prelude-sdk-1.2.3/tests/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.3/tests/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1097 2023-05-17 16:29:25.000000 prelude-sdk-1.2.3/tests/conftest.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-07 21:03:27.981721 prelude-sdk-1.2.3/tests/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-04-07 19:23:14.000000 prelude-sdk-1.2.3/tests/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     2075 2023-06-06 22:22:58.000000 prelude-sdk-1.2.3/tests/test_build_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     5045 2023-06-06 22:22:58.000000 prelude-sdk-1.2.3/tests/test_detect_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)     3350 2023-06-07 19:10:37.000000 prelude-sdk-1.2.3/tests/test_iam_controller.py
+-rw-r--r--   0 pack       (501) staff       (20)      682 2023-04-07 19:23:14.000000 prelude-sdk-1.2.3/tests/test_probe_controller.py
```

### Comparing `prelude-sdk-1.2.2/LICENSE` & `prelude-sdk-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.2/PKG-INFO` & `prelude-sdk-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.2.2
+Version: 1.2.3
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.2.2/README.md` & `prelude-sdk-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.2/prelude_sdk/controllers/build_controller.py` & `prelude-sdk-1.2.3/prelude_sdk/controllers/build_controller.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,52 @@
 
 class BuildController:
 
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
-    def create_test(self, test_id, name, unit, advisory=None):
+    def create_test(self, name, unit, advisory=None, test_id=None):
         """ Create or update a test """
         body = dict(name=name, unit=unit)
+        if advisory:
+            body['advisory'] = advisory
+        if test_id:
+            body['id'] = test_id
 
+        res = requests.post(
+            f'{self.account.hq}/build/tests',
+            json=body,
+            headers=self.account.headers,
+            timeout=10
+        )
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
+
+    @verify_credentials
+    def update_test(self, test_id, name=None, unit=None, advisory=None):
+        """ Update a test """
+        body = dict()
+        if name:
+            body['name'] = name
+        if unit:
+            body['unit'] = unit
         if advisory:
             body['advisory'] = advisory
 
         res = requests.post(
             f'{self.account.hq}/build/tests/{test_id}',
             json=body,
             headers=self.account.headers,
             timeout=10
         )
-        if not res.status_code == 200:
-            raise Exception(res.text)
+        if res.status_code == 200:
+            return res.json()
+        raise Exception(res.text)
 
     @verify_credentials
     def delete_test(self, test_id):
         """ Delete an existing test """
         res = requests.delete(
             f'{self.account.hq}/build/tests/{test_id}',
             headers=self.account.headers,
```

### Comparing `prelude-sdk-1.2.2/prelude_sdk/controllers/detect_controller.py` & `prelude-sdk-1.2.3/prelude_sdk/controllers/detect_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,51 @@
 
 class DetectController:
 
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
-    def register_endpoint(self, host, serial_num, edr_id, tags, endpoint_id=None):
+    def register_endpoint(self, host, serial_num, edr_id='', tags=None):
         """ Register (or re-register) an endpoint to your account """
-        params = dict(id=f'{host}:{serial_num}:{edr_id}', tags=tags) if not endpoint_id else \
-            dict(endpoint_id=endpoint_id, tags=tags, edr_id=edr_id, host=host)
+        body = dict(id=f'{host}:{serial_num}:{edr_id}')
+        if tags:
+            body['tags'] = tags
+
         res = requests.post(
             f'{self.account.hq}/detect/endpoint',
             headers=self.account.headers,
-            json=params,
+            json=body,
             timeout=10
         )
         if res.status_code == 200:
             return res.text
         raise Exception(res.text)
 
     @verify_credentials
+    def update_endpoint(self, endpoint_id, host=None, edr_id=None, tags=None):
+        """ Update an endpoint in your account """
+        body = dict()
+        if host:
+            body['host'] = host
+        if edr_id:
+            body['edr_id'] = edr_id
+        if tags:
+            body['tags'] = tags
+
+        res = requests.post(
+            f'{self.account.hq}/detect/endpoint/{endpoint_id}',
+            headers=self.account.headers,
+            json=body,
+            timeout=10
+        )
+        if res.status_code != 200:
+            raise Exception(res.text)
+
+    @verify_credentials
     def delete_endpoint(self, ident: str):
         """ Delete an endpoint from your account """
         params = dict(id=ident)
         res = requests.delete(
             f'{self.account.hq}/detect/endpoint',
             headers=self.account.headers,
             json=params,
```

### Comparing `prelude-sdk-1.2.2/prelude_sdk/controllers/iam_controller.py` & `prelude-sdk-1.2.3/prelude_sdk/controllers/partner_controller.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,62 @@
 import requests
-import datetime
 
 from prelude_sdk.models.account import verify_credentials
 
 
-class IAMController:
+class PartnerController:
 
     def __init__(self, account):
         self.account = account
 
     @verify_credentials
-    def new_account(self, user_email: str, user_name: str):
+    def attach(self, name: str, api: str, user: str, secret: str):
+        """ Attach a partner to your account """
+        params = dict(api=api, user=user, secret=secret)
         res = requests.post(
-            url=f'{self.account.hq}/iam/account',
-            json=dict(handle=user_email, user_name=user_name),
-            headers=self.account.headers,
-            timeout=10
-        )
-        if res.status_code != 200:
-            raise Exception(res.text)
-
-        cfg = self.account.read_keychain_config()
-        res_json = res.json()
-        cfg[self.account.profile]['account'] = res_json['account_id']
-        cfg[self.account.profile]['token'] = res_json['token']
-        self.account.write_keychain_config(cfg)
-        return res_json
-
-    @verify_credentials
-    def purge_account(self):
-        """ Delete an account and all things in it """
-        res = requests.delete(
-            f'{self.account.hq}/iam/account',
-            headers=self.account.headers,
-            timeout=10
-        )
-        if not res.status_code == 200:
-            raise Exception(res.text)
-        return res.text
-
-    @verify_credentials
-    def update_account(self, mode: int):
-        """ Update properties on an account """
-        res = requests.put(
-            f'{self.account.hq}/iam/account',
-            headers=self.account.headers,
-            json=dict(mode=mode),
-            timeout=10
-        )
-        if res.status_code != 200:
-            raise Exception(res.text)
-
-    @verify_credentials
-    def get_account(self):
-        """ Get account properties """
-        res = requests.get(
-            f'{self.account.hq}/iam/account',
-            headers=self.account.headers,
-            timeout=10
-        )
-        if res.status_code == 200:
-            return res.json()
-        raise Exception(res.text)
-
-    @verify_credentials
-    def create_user(self, permission: int, email: str, name: str, expires: datetime):
-        """ Create a new user inside an account """
-        res = requests.post(
-            url=f'{self.account.hq}/iam/user',
-            json=dict(permission=permission, handle=email, name=name, expires=expires.isoformat()),
+            f'{self.account.hq}/partner/{name}',
             headers=self.account.headers,
+            json=params,
             timeout=10
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
 
     @verify_credentials
-    def delete_user(self, handle):
-        """ Delete a user from an account """
+    def detach(self, name: str):
+        """ Detach a partner from your Detect account """
         res = requests.delete(
-            f'{self.account.hq}/iam/user',
-            json=dict(handle=handle),
+            f'{self.account.hq}/partner/{name}',
             headers=self.account.headers,
             timeout=10
         )
         if res.status_code == 200:
-            return True
+            return res.text
         raise Exception(res.text)
-
+        
     @verify_credentials
-    def audit_logs(self, days: int = 7, limit: int = 1000):
-        """ Get audit logs from the last X days """
-        params = dict(days=days, limit=limit)
+    def endpoints(self, partner_name: str, platform: str, hostname: str = '', offset: int = 0, count: int = 100):
+        """ Get a list of endpoints from all partners """
+        params = dict(platform=platform, hostname=hostname, offset=offset, count=count)
         res = requests.get(
-            f'{self.account.hq}/iam/audit',
+            f'{self.account.hq}/partner/endpoints/{partner_name}',
             headers=self.account.headers,
             params=params,
             timeout=30
         )
         if res.status_code == 200:
             return res.json()
         raise Exception(res.text)
+
+    @verify_credentials
+    def deploy(self, partner_name: str, host_ids: list):
+        """ Deploy probes on all specified partner endpoints """
+        params = dict(host_ids=host_ids)
+        res = requests.post(
+            f'{self.account.hq}/partner/deploy/{partner_name}',
+            headers=self.account.headers,
+            json=params,
+            timeout=30
+        )
+        if not res.status_code == 200:
+            raise Exception(res.text)
```

### Comparing `prelude-sdk-1.2.2/prelude_sdk/models/account.py` & `prelude-sdk-1.2.3/prelude_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.2/prelude_sdk/models/codes.py` & `prelude-sdk-1.2.3/prelude_sdk/models/codes.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.2/prelude_sdk.egg-info/PKG-INFO` & `prelude-sdk-1.2.3/prelude_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-sdk
-Version: 1.2.2
+Version: 1.2.3
 Summary: For interacting with the Prelude API
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-sdk-1.2.2/prelude_sdk.egg-info/SOURCES.txt` & `prelude-sdk-1.2.3/prelude_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.2/setup.cfg` & `prelude-sdk-1.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-sdk
-version = 1.2.2
+version = 1.2.3
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers =
```

### Comparing `prelude-sdk-1.2.2/tests/conftest.py` & `prelude-sdk-1.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prelude-sdk-1.2.2/tests/test_build_controller.py` & `prelude-sdk-1.2.3/tests/test_build_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import time
 import uuid
 import pytest
 
 from datetime import datetime
 from importlib.resources import files
 
 from tests import templates as templates
@@ -12,31 +13,40 @@
 
 class TestBuildController:
 
     def setup_class(self):
         """Setup the test class"""
         self.test_id = str(uuid.uuid4())
         self.test_name = 'test'
+        self.test_updated_name = 'updated_test'
+        self.test_unit = 'AV'
         self.build = BuildController(pytest.account)
         self.detect = DetectController(pytest.account)
 
     def test_create_test(self, unwrap):
         """Test create_test method"""
         unwrap(self.build.create_test)(self.build, test_id=self.test_id, name=self.test_name, unit='bulletin')
         pytest.test_id = self.test_id
         assert True
 
     def test_upload(self, unwrap):
         """Test upload method"""
         template = files(templates).joinpath('template.go').read_text()
         template = template.replace('$ID', self.test_id)
         template = template.replace('$NAME', self.test_name)
+        template = template.replace('$UNIT', self.test_unit)
         template = template.replace('$CREATED', str(datetime.utcnow()))
         unwrap(self.build.upload)(self.build, test_id=self.test_id, filename=f'{self.test_id}.go', data=template)
+        time.sleep(5)
         res = unwrap(self.detect.get_test)(self.detect, test_id=self.test_id)
         assert f'{self.test_id}.go' in res['attachments']
 
+    def test_update_test(self, unwrap):
+        """Test update_test method"""
+        res = unwrap(self.build.update_test)(self.build, test_id=self.test_id, name=self.test_updated_name)
+        assert res['name'] == self.test_updated_name
+
     @pytest.mark.order(after='test_detect_controller.py::TestDetectController::test_disable_test')
     def test_delete_test(self, unwrap):
         """Test delete_test method"""
         unwrap(self.build.delete_test)(self.build, test_id=pytest.test_id)
         assert True
```

### Comparing `prelude-sdk-1.2.2/tests/test_detect_controller.py` & `prelude-sdk-1.2.3/tests/test_detect_controller.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     def setup_class(self):
         """Setup the test class"""
         self.host = 'test_host'
         self.serial = 'test_serial'
         self.edr_id = 'test_edr_id'
         self.tags = 'test_tag'
+        self.updated_tags = 'updated_test_tag'
         self.health_check = '39de298a-911d-4a3b-aed4-1e8281010a9a'
         self.recommendation = 'Test'
         self.detect = DetectController(pytest.account)
         self.iam = IAMController(pytest.account)
 
     def test_list_advisories(self, unwrap):
         """Test list_advisories method"""
@@ -83,14 +84,21 @@
                 start=datetime.utcnow() - timedelta(days=7),
                 finish=datetime.utcnow() + timedelta(days=1)
             )
             describe_activity = unwrap(self.detect.describe_activity)(self.detect, filters=filters | {'endpoint_id': pytest.endpoint_id})
             assert len(describe_activity) == 2
         finally:
             os.remove(pytest.probe)
+    
+    @pytest.mark.order(after='test_describe_activity')
+    def test_update_endpoint(self, unwrap):
+        """Test update_endpoint method"""
+        unwrap(self.detect.update_endpoint)(self.detect, endpoint_id=pytest.endpoint_id, tags=self.updated_tags)
+        res = unwrap(self.detect.list_endpoints)(self.detect)
+        assert res[0]['tags'][0] == self.updated_tags
 
     @pytest.mark.order(after='test_describe_activity')
     def test_disable_test(self, unwrap):
         """Test disable_test method"""
         unwrap(self.detect.disable_test)(self.detect, ident=pytest.test_id, tags=self.tags)
         queue = unwrap(self.iam.get_account)(self.iam)['queue']
         assert len([test for test in queue if test['test'] == pytest.test_id]) == 0
```

### Comparing `prelude-sdk-1.2.2/tests/test_iam_controller.py` & `prelude-sdk-1.2.3/tests/test_iam_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,18 @@
         return True
     except ValueError:
         return False
 
 
 class TestIAMController:
 
+    def setup_class(self):
+        """Setup the test class"""
+        self.company = 'prelude'
+
     @pytest.mark.order(1)
     def test_new_account(self, unwrap, pause_for_manual_action, email, api):
         """Test new_account method"""
         pytest.account = Account(hq=api)
         iam = IAMController(pytest.account)
         res = unwrap(iam.new_account)(iam, user_email=email, user_name='Bob')
         if email.endswith('@auto-accept.developer.preludesecurity.com'):
@@ -73,17 +77,17 @@
         res = unwrap(iam.get_account)(iam)
         assert len([user for user in res['users'] if user['handle'] == 'registration']) == 0
 
     @pytest.mark.order(after='test_detect_controller.py::TestDetectController::test_delete_endpoint')
     def test_update_account(self, unwrap):
         """Test update_account method"""
         iam = IAMController(pytest.account)
-        unwrap(iam.update_account)(iam, mode=Mode.FROZEN.value)
-        res = unwrap(iam.get_account)(iam)
+        res = unwrap(iam.update_account)(iam, mode=Mode.FROZEN.value, company=self.company)
         assert res['mode'] == Mode.FROZEN.value
+        assert res['company'] == self.company
 
     @pytest.mark.order(after='test_update_account')
     def test_purge_account(self, unwrap):
         """Test purge_account method"""
         iam = IAMController(pytest.account)
         res = unwrap(iam.purge_account)(iam)
         assert res is not None
```

### Comparing `prelude-sdk-1.2.2/tests/test_probe_controller.py` & `prelude-sdk-1.2.3/tests/test_probe_controller.py`

 * *Files identical despite different names*

