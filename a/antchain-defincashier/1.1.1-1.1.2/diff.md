# Comparing `tmp/antchain_defincashier-1.1.1.tar.gz` & `tmp/antchain_defincashier-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_defincashier-1.1.1.tar", last modified: Wed Jun  7 09:23:19 2023, max compression
+gzip compressed data, was "dist/antchain_defincashier-1.1.2.tar", last modified: Thu Jun  8 03:09:50 2023, max compression
```

## Comparing `antchain_defincashier-1.1.1.tar` & `antchain_defincashier-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2216 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2216 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_defincashier.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_sdk_defincashier/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_sdk_defincashier/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39521 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_sdk_defincashier/client.py
--rw-r--r--   0 root         (0) root         (0)    76711 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/antchain_sdk_defincashier/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2533 2023-06-07 09:23:19.000000 antchain_defincashier-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/antchain_defincashier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/antchain_defincashier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/antchain_defincashier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/antchain_defincashier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/antchain_defincashier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/antchain_defincashier.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/antchain_sdk_defincashier/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/antchain_sdk_defincashier/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39521 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/antchain_sdk_defincashier/client.py
+-rw-r--r--   0 root         (0) root         (0)    77183 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/antchain_sdk_defincashier/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-06-08 03:09:50.000000 antchain_defincashier-1.1.2/setup.py
```

### Comparing `antchain_defincashier-1.1.1/LICENSE` & `antchain_defincashier-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_defincashier-1.1.1/PKG-INFO` & `antchain_defincashier-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_defincashier
-Version: 1.1.1
+Version: 1.1.2
 Summary: Ant Chain DEFINCASHIER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_defincashier-1.1.1/README-CN.md` & `antchain_defincashier-1.1.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_defincashier-1.1.1/README.md` & `antchain_defincashier-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_defincashier-1.1.1/antchain_defincashier.egg-info/PKG-INFO` & `antchain_defincashier-1.1.2/antchain_defincashier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-defincashier
-Version: 1.1.1
+Version: 1.1.2
 Summary: Ant Chain DEFINCASHIER SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_defincashier-1.1.1/antchain_sdk_defincashier/client.py` & `antchain_defincashier-1.1.2/antchain_sdk_defincashier/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.1',
+                    'sdk_version': '1.1.2',
                     '_prod_code': 'DEFINCASHIER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.1',
+                    'sdk_version': '1.1.2',
                     '_prod_code': 'DEFINCASHIER',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_defincashier-1.1.1/antchain_sdk_defincashier/models.py` & `antchain_defincashier-1.1.2/antchain_sdk_defincashier/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,42 +155,50 @@
 
 
 class AmountItem(TeaModel):
     def __init__(
         self,
         balance_amount: str = None,
         currency: str = None,
+        frozen_balance_amount: str = None,
     ):
         # 余额，单位元
         self.balance_amount = balance_amount
         # 币种，CNY-人民币
         self.currency = currency
+        # 冻结余额，单位元
+        self.frozen_balance_amount = frozen_balance_amount
 
     def validate(self):
         self.validate_required(self.balance_amount, 'balance_amount')
         self.validate_required(self.currency, 'currency')
+        self.validate_required(self.frozen_balance_amount, 'frozen_balance_amount')
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.balance_amount is not None:
             result['balance_amount'] = self.balance_amount
         if self.currency is not None:
             result['currency'] = self.currency
+        if self.frozen_balance_amount is not None:
+            result['frozen_balance_amount'] = self.frozen_balance_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('balance_amount') is not None:
             self.balance_amount = m.get('balance_amount')
         if m.get('currency') is not None:
             self.currency = m.get('currency')
+        if m.get('frozen_balance_amount') is not None:
+            self.frozen_balance_amount = m.get('frozen_balance_amount')
         return self
 
 
 class AccountDTO(TeaModel):
     def __init__(
         self,
         account_no: str = None,
```

### Comparing `antchain_defincashier-1.1.1/setup.py` & `antchain_defincashier-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_defincashier.
 
-Created on 07/06/2023
+Created on 08/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_defincashier"
 NAME = "antchain_defincashier" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain DEFINCASHIER SDK Library for Python"
```

