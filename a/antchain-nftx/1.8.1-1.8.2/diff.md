# Comparing `tmp/antchain_nftx-1.8.1.tar.gz` & `tmp/antchain_nftx-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_nftx-1.8.1.tar", last modified: Tue Jun  6 09:43:07 2023, max compression
+gzip compressed data, was "dist/antchain_nftx-1.8.2.tar", last modified: Thu Jun  8 03:51:06 2023, max compression
```

## Comparing `antchain_nftx-1.8.1.tar` & `antchain_nftx-1.8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_nftx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_sdk_nftx/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_sdk_nftx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50083 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_sdk_nftx/client.py
--rw-r--r--   0 root         (0) root         (0)    99666 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/antchain_sdk_nftx/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-06-06 09:43:07.000000 antchain_nftx-1.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_nftx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_sdk_nftx/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_sdk_nftx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52197 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_sdk_nftx/client.py
+-rw-r--r--   0 root         (0) root         (0)   105809 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/antchain_sdk_nftx/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-08 03:51:06.000000 antchain_nftx-1.8.2/setup.py
```

### Comparing `antchain_nftx-1.8.1/LICENSE` & `antchain_nftx-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.1/PKG-INFO` & `antchain_nftx-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_nftx
-Version: 1.8.1
+Version: 1.8.2
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.8.1/README-CN.md` & `antchain_nftx-1.8.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.1/README.md` & `antchain_nftx-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_nftx-1.8.1/antchain_nftx.egg-info/PKG-INFO` & `antchain_nftx-1.8.2/antchain_nftx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-nftx
-Version: 1.8.1
+Version: 1.8.2
 Summary: Ant Chain NFTX SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_nftx-1.8.1/antchain_sdk_nftx/client.py` & `antchain_nftx-1.8.2/antchain_sdk_nftx/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.8.1',
+                    'sdk_version': '1.8.2',
                     '_prod_code': 'NFTX',
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
-                    'sdk_version': '1.8.1',
+                    'sdk_version': '1.8.2',
                     '_prod_code': 'NFTX',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1111,14 +1111,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             nftx_models.SyncOrderDataResponse(),
             await self.do_request_async('1.0', 'antchain.nftx.order.data.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def query_resource_image(
+        self,
+        request: nftx_models.QueryResourceImageRequest,
+    ) -> nftx_models.QueryResourceImageResponse:
+        """
+        Description: 查询实物定制图片
+        Summary: 查询实物定制图片
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_resource_image_ex(request, headers, runtime)
+
+    async def query_resource_image_async(
+        self,
+        request: nftx_models.QueryResourceImageRequest,
+    ) -> nftx_models.QueryResourceImageResponse:
+        """
+        Description: 查询实物定制图片
+        Summary: 查询实物定制图片
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_resource_image_ex_async(request, headers, runtime)
+
+    def query_resource_image_ex(
+        self,
+        request: nftx_models.QueryResourceImageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> nftx_models.QueryResourceImageResponse:
+        """
+        Description: 查询实物定制图片
+        Summary: 查询实物定制图片
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            nftx_models.QueryResourceImageResponse(),
+            self.do_request('1.0', 'antchain.nftx.resource.image.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_resource_image_ex_async(
+        self,
+        request: nftx_models.QueryResourceImageRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> nftx_models.QueryResourceImageResponse:
+        """
+        Description: 查询实物定制图片
+        Summary: 查询实物定制图片
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            nftx_models.QueryResourceImageResponse(),
+            await self.do_request_async('1.0', 'antchain.nftx.resource.image.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def apply_oauth_token(
         self,
         request: nftx_models.ApplyOauthTokenRequest,
     ) -> nftx_models.ApplyOauthTokenResponse:
         """
         Description: 拿authcode换token
         Summary: 拿authcode换token
```

### Comparing `antchain_nftx-1.8.1/antchain_sdk_nftx/models.py` & `antchain_nftx-1.8.2/antchain_sdk_nftx/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2488,14 +2488,173 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
+class QueryResourceImageRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        access_token: str = None,
+        type: str = None,
+        resource_id: str = None,
+        nft_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # access_token
+        self.access_token = access_token
+        # 素材的类型（AIGC/NFT）
+        self.type = type
+        # 资源ID
+        self.resource_id = resource_id
+        # type为NFT必填
+        self.nft_id = nft_id
+
+    def validate(self):
+        self.validate_required(self.access_token, 'access_token')
+        self.validate_required(self.type, 'type')
+        self.validate_required(self.resource_id, 'resource_id')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.access_token is not None:
+            result['access_token'] = self.access_token
+        if self.type is not None:
+            result['type'] = self.type
+        if self.resource_id is not None:
+            result['resource_id'] = self.resource_id
+        if self.nft_id is not None:
+            result['nft_id'] = self.nft_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('access_token') is not None:
+            self.access_token = m.get('access_token')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('resource_id') is not None:
+            self.resource_id = m.get('resource_id')
+        if m.get('nft_id') is not None:
+            self.nft_id = m.get('nft_id')
+        return self
+
+
+class QueryResourceImageResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        nft_id: str = None,
+        sku_name: str = None,
+        uni_hash: str = None,
+        creation_time: str = None,
+        thumbnail_urls: List[str] = None,
+        high_definition_status: int = None,
+        high_definition_urls: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # nftID 藏品素材nftId，type为NFT时有值
+        self.nft_id = nft_id
+        # 具体藏品名称，type为NFT时有值
+        self.sku_name = sku_name
+        # nftId 的 算法计算的hash，该藏品唯一标识，type为NFT时有值
+        self.uni_hash = uni_hash
+        # Date	藏品铸造上链生成时间，例如2021.09.22 20:22:19，type为NFT时有值
+        self.creation_time = creation_time
+        # 缩略图url列表
+        self.thumbnail_urls = thumbnail_urls
+        # int	高清图状态
+        # 0 需要等待
+        # 1 已完成
+        self.high_definition_status = high_definition_status
+        # 在highDefinitionStatus为1时有值
+        # 高清图列表
+        self.high_definition_urls = high_definition_urls
+
+    def validate(self):
+        if self.creation_time is not None:
+            self.validate_pattern(self.creation_time, 'creation_time', '\\d{4}[-]\\d{1,2}[-]\\d{1,2}[T]\\d{2}:\\d{2}:\\d{2}([Z]|([\\.]\\d{1,9})?[\\+]\\d{2}[\\:]?\\d{2})')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.nft_id is not None:
+            result['nft_id'] = self.nft_id
+        if self.sku_name is not None:
+            result['sku_name'] = self.sku_name
+        if self.uni_hash is not None:
+            result['uni_hash'] = self.uni_hash
+        if self.creation_time is not None:
+            result['creation_time'] = self.creation_time
+        if self.thumbnail_urls is not None:
+            result['thumbnail_urls'] = self.thumbnail_urls
+        if self.high_definition_status is not None:
+            result['high_definition_status'] = self.high_definition_status
+        if self.high_definition_urls is not None:
+            result['high_definition_urls'] = self.high_definition_urls
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('nft_id') is not None:
+            self.nft_id = m.get('nft_id')
+        if m.get('sku_name') is not None:
+            self.sku_name = m.get('sku_name')
+        if m.get('uni_hash') is not None:
+            self.uni_hash = m.get('uni_hash')
+        if m.get('creation_time') is not None:
+            self.creation_time = m.get('creation_time')
+        if m.get('thumbnail_urls') is not None:
+            self.thumbnail_urls = m.get('thumbnail_urls')
+        if m.get('high_definition_status') is not None:
+            self.high_definition_status = m.get('high_definition_status')
+        if m.get('high_definition_urls') is not None:
+            self.high_definition_urls = m.get('high_definition_urls')
+        return self
+
+
 class ApplyOauthTokenRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         grant_type: str = None,
         auth_code: str = None,
```

### Comparing `antchain_nftx-1.8.1/setup.py` & `antchain_nftx-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_nftx.
 
-Created on 06/06/2023
+Created on 08/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_nftx"
 NAME = "antchain_nftx" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain NFTX SDK Library for Python"
```

