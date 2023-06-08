# Comparing `tmp/alibabacloud_oceanbasepro20190901-1.0.8.tar.gz` & `tmp/alibabacloud_oceanbasepro20190901-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901-1.0.8.tar", last modified: Fri May 19 10:09:54 2023, max compression
+gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901-1.0.9.tar", last modified: Thu Jun  8 02:58:36 2023, max compression
```

## Comparing `alibabacloud_oceanbasepro20190901-1.0.8.tar` & `alibabacloud_oceanbasepro20190901-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      288 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2382 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1049 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1134 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   268062 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/client.py
--rw-r--r--   0 root         (0) root         (0)   828724 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2382 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      492 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-19 10:09:54.000000 alibabacloud_oceanbasepro20190901-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2655 2023-05-19 10:09:53.000000 alibabacloud_oceanbasepro20190901-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      329 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   317978 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901/client.py
+-rw-r--r--   0 root         (0) root         (0)   996746 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2382 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      492 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2655 2023-06-08 02:58:36.000000 alibabacloud_oceanbasepro20190901-1.0.9/setup.py
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.8/LICENSE` & `alibabacloud_oceanbasepro20190901-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-1.0.8/PKG-INFO` & `alibabacloud_oceanbasepro20190901-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oceanbasepro20190901
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.8/README-CN.md` & `alibabacloud_oceanbasepro20190901-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-1.0.8/README.md` & `alibabacloud_oceanbasepro20190901-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/client.py` & `alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -789,14 +789,96 @@
     async def create_tenant_read_only_connection_async(
         self,
         request: ocean_base_pro_20190901_models.CreateTenantReadOnlyConnectionRequest,
     ) -> ocean_base_pro_20190901_models.CreateTenantReadOnlyConnectionResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_tenant_read_only_connection_with_options_async(request, runtime)
 
+    def create_tenant_security_ip_group_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.CreateTenantSecurityIpGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.CreateTenantSecurityIpGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_ip_group_name):
+            body['SecurityIpGroupName'] = request.security_ip_group_name
+        if not UtilClient.is_unset(request.security_ips):
+            body['SecurityIps'] = request.security_ips
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateTenantSecurityIpGroup',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.CreateTenantSecurityIpGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_tenant_security_ip_group_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.CreateTenantSecurityIpGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.CreateTenantSecurityIpGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_ip_group_name):
+            body['SecurityIpGroupName'] = request.security_ip_group_name
+        if not UtilClient.is_unset(request.security_ips):
+            body['SecurityIps'] = request.security_ips
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateTenantSecurityIpGroup',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.CreateTenantSecurityIpGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_tenant_security_ip_group(
+        self,
+        request: ocean_base_pro_20190901_models.CreateTenantSecurityIpGroupRequest,
+    ) -> ocean_base_pro_20190901_models.CreateTenantSecurityIpGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_tenant_security_ip_group_with_options(request, runtime)
+
+    async def create_tenant_security_ip_group_async(
+        self,
+        request: ocean_base_pro_20190901_models.CreateTenantSecurityIpGroupRequest,
+    ) -> ocean_base_pro_20190901_models.CreateTenantSecurityIpGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_tenant_security_ip_group_with_options_async(request, runtime)
+
     def create_tenant_user_with_options(
         self,
         request: ocean_base_pro_20190901_models.CreateTenantUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.CreateTenantUserResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -1221,14 +1303,92 @@
     async def delete_security_ip_group_async(
         self,
         request: ocean_base_pro_20190901_models.DeleteSecurityIpGroupRequest,
     ) -> ocean_base_pro_20190901_models.DeleteSecurityIpGroupResponse:
         runtime = util_models.RuntimeOptions()
         return await self.delete_security_ip_group_with_options_async(request, runtime)
 
+    def delete_tenant_security_ip_group_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.DeleteTenantSecurityIpGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DeleteTenantSecurityIpGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_ip_group_name):
+            body['SecurityIpGroupName'] = request.security_ip_group_name
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DeleteTenantSecurityIpGroup',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DeleteTenantSecurityIpGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def delete_tenant_security_ip_group_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.DeleteTenantSecurityIpGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DeleteTenantSecurityIpGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_ip_group_name):
+            body['SecurityIpGroupName'] = request.security_ip_group_name
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DeleteTenantSecurityIpGroup',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DeleteTenantSecurityIpGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def delete_tenant_security_ip_group(
+        self,
+        request: ocean_base_pro_20190901_models.DeleteTenantSecurityIpGroupRequest,
+    ) -> ocean_base_pro_20190901_models.DeleteTenantSecurityIpGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.delete_tenant_security_ip_group_with_options(request, runtime)
+
+    async def delete_tenant_security_ip_group_async(
+        self,
+        request: ocean_base_pro_20190901_models.DeleteTenantSecurityIpGroupRequest,
+    ) -> ocean_base_pro_20190901_models.DeleteTenantSecurityIpGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.delete_tenant_security_ip_group_with_options_async(request, runtime)
+
     def delete_tenant_users_with_options(
         self,
         request: ocean_base_pro_20190901_models.DeleteTenantUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.DeleteTenantUsersResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -2459,14 +2619,670 @@
     async def describe_node_metrics_async(
         self,
         request: ocean_base_pro_20190901_models.DescribeNodeMetricsRequest,
     ) -> ocean_base_pro_20190901_models.DescribeNodeMetricsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_node_metrics_with_options_async(request, runtime)
 
+    def describe_oas_anomaly_sqllist_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasAnomalySQLListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasAnomalySQLListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.accept_language):
+            body['AcceptLanguage'] = request.accept_language
+        if not UtilClient.is_unset(request.current):
+            body['Current'] = request.current
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.filter_condition):
+            body['FilterCondition'] = request.filter_condition
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_ip):
+            body['NodeIp'] = request.node_ip
+        if not UtilClient.is_unset(request.page_size):
+            body['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.search_key_word):
+            body['SearchKeyWord'] = request.search_key_word
+        if not UtilClient.is_unset(request.search_param):
+            body['SearchParam'] = request.search_param
+        if not UtilClient.is_unset(request.search_rule):
+            body['SearchRule'] = request.search_rule
+        if not UtilClient.is_unset(request.search_value):
+            body['SearchValue'] = request.search_value
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.sql_text_length):
+            body['SqlTextLength'] = request.sql_text_length
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasAnomalySQLList',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasAnomalySQLListResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_oas_anomaly_sqllist_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasAnomalySQLListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasAnomalySQLListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.accept_language):
+            body['AcceptLanguage'] = request.accept_language
+        if not UtilClient.is_unset(request.current):
+            body['Current'] = request.current
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.filter_condition):
+            body['FilterCondition'] = request.filter_condition
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_ip):
+            body['NodeIp'] = request.node_ip
+        if not UtilClient.is_unset(request.page_size):
+            body['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.search_key_word):
+            body['SearchKeyWord'] = request.search_key_word
+        if not UtilClient.is_unset(request.search_param):
+            body['SearchParam'] = request.search_param
+        if not UtilClient.is_unset(request.search_rule):
+            body['SearchRule'] = request.search_rule
+        if not UtilClient.is_unset(request.search_value):
+            body['SearchValue'] = request.search_value
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.sql_text_length):
+            body['SqlTextLength'] = request.sql_text_length
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasAnomalySQLList',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasAnomalySQLListResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_oas_anomaly_sqllist(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasAnomalySQLListRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasAnomalySQLListResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_anomaly_sqllist_with_options(request, runtime)
+
+    async def describe_oas_anomaly_sqllist_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasAnomalySQLListRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasAnomalySQLListResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_oas_anomaly_sqllist_with_options_async(request, runtime)
+
+    def describe_oas_sqldetails_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLDetailsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLDetailsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasSQLDetails',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasSQLDetailsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_oas_sqldetails_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLDetailsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLDetailsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasSQLDetails',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasSQLDetailsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_oas_sqldetails(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLDetailsRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLDetailsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_sqldetails_with_options(request, runtime)
+
+    async def describe_oas_sqldetails_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLDetailsRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLDetailsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_oas_sqldetails_with_options_async(request, runtime)
+
+    def describe_oas_sqlhistory_list_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLHistoryListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLHistoryListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.accept_language):
+            body['AcceptLanguage'] = request.accept_language
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_ip):
+            body['NodeIp'] = request.node_ip
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasSQLHistoryList',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasSQLHistoryListResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_oas_sqlhistory_list_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLHistoryListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLHistoryListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.accept_language):
+            body['AcceptLanguage'] = request.accept_language
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_ip):
+            body['NodeIp'] = request.node_ip
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasSQLHistoryList',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasSQLHistoryListResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_oas_sqlhistory_list(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLHistoryListRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLHistoryListResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_sqlhistory_list_with_options(request, runtime)
+
+    async def describe_oas_sqlhistory_list_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLHistoryListRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLHistoryListResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_oas_sqlhistory_list_with_options_async(request, runtime)
+
+    def describe_oas_sqlplans_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLPlansRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLPlansResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.accept_language):
+            body['AcceptLanguage'] = request.accept_language
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasSQLPlans',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasSQLPlansResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_oas_sqlplans_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLPlansRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLPlansResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.accept_language):
+            body['AcceptLanguage'] = request.accept_language
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasSQLPlans',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasSQLPlansResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_oas_sqlplans(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLPlansRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLPlansResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_sqlplans_with_options(request, runtime)
+
+    async def describe_oas_sqlplans_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSQLPlansRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSQLPlansResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_oas_sqlplans_with_options_async(request, runtime)
+
+    def describe_oas_slow_sqllist_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSlowSQLListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSlowSQLListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.accept_language):
+            body['AcceptLanguage'] = request.accept_language
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.filter_condition):
+            body['FilterCondition'] = request.filter_condition
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_ip):
+            body['NodeIp'] = request.node_ip
+        if not UtilClient.is_unset(request.search_key_word):
+            body['SearchKeyWord'] = request.search_key_word
+        if not UtilClient.is_unset(request.search_param):
+            body['SearchParam'] = request.search_param
+        if not UtilClient.is_unset(request.search_rule):
+            body['SearchRule'] = request.search_rule
+        if not UtilClient.is_unset(request.search_value):
+            body['SearchValue'] = request.search_value
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.sql_text_length):
+            body['SqlTextLength'] = request.sql_text_length
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasSlowSQLList',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasSlowSQLListResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_oas_slow_sqllist_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSlowSQLListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSlowSQLListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.accept_language):
+            body['AcceptLanguage'] = request.accept_language
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.filter_condition):
+            body['FilterCondition'] = request.filter_condition
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_ip):
+            body['NodeIp'] = request.node_ip
+        if not UtilClient.is_unset(request.search_key_word):
+            body['SearchKeyWord'] = request.search_key_word
+        if not UtilClient.is_unset(request.search_param):
+            body['SearchParam'] = request.search_param
+        if not UtilClient.is_unset(request.search_rule):
+            body['SearchRule'] = request.search_rule
+        if not UtilClient.is_unset(request.search_value):
+            body['SearchValue'] = request.search_value
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.sql_text_length):
+            body['SqlTextLength'] = request.sql_text_length
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasSlowSQLList',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasSlowSQLListResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_oas_slow_sqllist(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSlowSQLListRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSlowSQLListResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_slow_sqllist_with_options(request, runtime)
+
+    async def describe_oas_slow_sqllist_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasSlowSQLListRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasSlowSQLListResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_oas_slow_sqllist_with_options_async(request, runtime)
+
+    def describe_oas_top_sqllist_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasTopSQLListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasTopSQLListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.accept_language):
+            body['AcceptLanguage'] = request.accept_language
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.filter_condition):
+            body['FilterCondition'] = request.filter_condition
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_ip):
+            body['NodeIp'] = request.node_ip
+        if not UtilClient.is_unset(request.search_key_word):
+            body['SearchKeyWord'] = request.search_key_word
+        if not UtilClient.is_unset(request.search_param):
+            body['SearchParam'] = request.search_param
+        if not UtilClient.is_unset(request.search_rule):
+            body['SearchRule'] = request.search_rule
+        if not UtilClient.is_unset(request.search_value):
+            body['SearchValue'] = request.search_value
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.sql_text_length):
+            body['SqlTextLength'] = request.sql_text_length
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasTopSQLList',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasTopSQLListResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_oas_top_sqllist_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasTopSQLListRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeOasTopSQLListResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.accept_language):
+            body['AcceptLanguage'] = request.accept_language
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.filter_condition):
+            body['FilterCondition'] = request.filter_condition
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.node_ip):
+            body['NodeIp'] = request.node_ip
+        if not UtilClient.is_unset(request.search_key_word):
+            body['SearchKeyWord'] = request.search_key_word
+        if not UtilClient.is_unset(request.search_param):
+            body['SearchParam'] = request.search_param
+        if not UtilClient.is_unset(request.search_rule):
+            body['SearchRule'] = request.search_rule
+        if not UtilClient.is_unset(request.search_value):
+            body['SearchValue'] = request.search_value
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.sql_text_length):
+            body['SqlTextLength'] = request.sql_text_length
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeOasTopSQLList',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeOasTopSQLListResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_oas_top_sqllist(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasTopSQLListRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasTopSQLListResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_top_sqllist_with_options(request, runtime)
+
+    async def describe_oas_top_sqllist_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeOasTopSQLListRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeOasTopSQLListResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_oas_top_sqllist_with_options_async(request, runtime)
+
     def describe_oms_open_apiproject_with_options(
         self,
         request: ocean_base_pro_20190901_models.DescribeOmsOpenAPIProjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.DescribeOmsOpenAPIProjectResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -3201,14 +4017,104 @@
     async def describe_sqlplans_async(
         self,
         request: ocean_base_pro_20190901_models.DescribeSQLPlansRequest,
     ) -> ocean_base_pro_20190901_models.DescribeSQLPlansResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_sqlplans_with_options_async(request, runtime)
 
+    def describe_sqlsamples_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeSQLSamplesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeSQLSamplesResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSQLSamples',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeSQLSamplesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_sqlsamples_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeSQLSamplesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeSQLSamplesResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.db_name):
+            body['DbName'] = request.db_name
+        if not UtilClient.is_unset(request.end_time):
+            body['EndTime'] = request.end_time
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.sql_id):
+            body['SqlId'] = request.sql_id
+        if not UtilClient.is_unset(request.start_time):
+            body['StartTime'] = request.start_time
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeSQLSamples',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeSQLSamplesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_sqlsamples(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeSQLSamplesRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeSQLSamplesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_sqlsamples_with_options(request, runtime)
+
+    async def describe_sqlsamples_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeSQLSamplesRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeSQLSamplesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_sqlsamples_with_options_async(request, runtime)
+
     def describe_security_ip_groups_with_options(
         self,
         request: ocean_base_pro_20190901_models.DescribeSecurityIpGroupsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.DescribeSecurityIpGroupsResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -3745,14 +4651,88 @@
     async def describe_tenant_security_configs_async(
         self,
         request: ocean_base_pro_20190901_models.DescribeTenantSecurityConfigsRequest,
     ) -> ocean_base_pro_20190901_models.DescribeTenantSecurityConfigsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_tenant_security_configs_with_options_async(request, runtime)
 
+    def describe_tenant_security_ip_groups_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeTenantSecurityIpGroupsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeTenantSecurityIpGroupsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeTenantSecurityIpGroups',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeTenantSecurityIpGroupsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_tenant_security_ip_groups_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeTenantSecurityIpGroupsRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.DescribeTenantSecurityIpGroupsResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='DescribeTenantSecurityIpGroups',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.DescribeTenantSecurityIpGroupsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_tenant_security_ip_groups(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeTenantSecurityIpGroupsRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeTenantSecurityIpGroupsResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_tenant_security_ip_groups_with_options(request, runtime)
+
+    async def describe_tenant_security_ip_groups_async(
+        self,
+        request: ocean_base_pro_20190901_models.DescribeTenantSecurityIpGroupsRequest,
+    ) -> ocean_base_pro_20190901_models.DescribeTenantSecurityIpGroupsResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_tenant_security_ip_groups_with_options_async(request, runtime)
+
     def describe_tenant_tags_with_options(
         self,
         request: ocean_base_pro_20190901_models.DescribeTenantTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.DescribeTenantTagsResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -5259,14 +6239,96 @@
     async def modify_tenant_resource_async(
         self,
         request: ocean_base_pro_20190901_models.ModifyTenantResourceRequest,
     ) -> ocean_base_pro_20190901_models.ModifyTenantResourceResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_tenant_resource_with_options_async(request, runtime)
 
+    def modify_tenant_security_ip_group_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyTenantSecurityIpGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.ModifyTenantSecurityIpGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_ip_group_name):
+            body['SecurityIpGroupName'] = request.security_ip_group_name
+        if not UtilClient.is_unset(request.security_ips):
+            body['SecurityIps'] = request.security_ips
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ModifyTenantSecurityIpGroup',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.ModifyTenantSecurityIpGroupResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def modify_tenant_security_ip_group_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyTenantSecurityIpGroupRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.ModifyTenantSecurityIpGroupResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.security_ip_group_name):
+            body['SecurityIpGroupName'] = request.security_ip_group_name
+        if not UtilClient.is_unset(request.security_ips):
+            body['SecurityIps'] = request.security_ips
+        if not UtilClient.is_unset(request.tenant_id):
+            body['TenantId'] = request.tenant_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='ModifyTenantSecurityIpGroup',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.ModifyTenantSecurityIpGroupResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def modify_tenant_security_ip_group(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyTenantSecurityIpGroupRequest,
+    ) -> ocean_base_pro_20190901_models.ModifyTenantSecurityIpGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.modify_tenant_security_ip_group_with_options(request, runtime)
+
+    async def modify_tenant_security_ip_group_async(
+        self,
+        request: ocean_base_pro_20190901_models.ModifyTenantSecurityIpGroupRequest,
+    ) -> ocean_base_pro_20190901_models.ModifyTenantSecurityIpGroupResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.modify_tenant_security_ip_group_with_options_async(request, runtime)
+
     def modify_tenant_tags_with_options(
         self,
         request: ocean_base_pro_20190901_models.ModifyTenantTagsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocean_base_pro_20190901_models.ModifyTenantTagsResponse:
         UtilClient.validate_model(request)
         body = {}
@@ -6298,7 +7360,85 @@
 
     async def stop_oms_open_apiproject_async(
         self,
         request: ocean_base_pro_20190901_models.StopOmsOpenAPIProjectRequest,
     ) -> ocean_base_pro_20190901_models.StopOmsOpenAPIProjectResponse:
         runtime = util_models.RuntimeOptions()
         return await self.stop_oms_open_apiproject_with_options_async(request, runtime)
+
+    def switchover_instance_with_options(
+        self,
+        request: ocean_base_pro_20190901_models.SwitchoverInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.SwitchoverInstanceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.forced):
+            body['Forced'] = request.forced
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.target_instance_id):
+            body['TargetInstanceId'] = request.target_instance_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SwitchoverInstance',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.SwitchoverInstanceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def switchover_instance_with_options_async(
+        self,
+        request: ocean_base_pro_20190901_models.SwitchoverInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> ocean_base_pro_20190901_models.SwitchoverInstanceResponse:
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.forced):
+            body['Forced'] = request.forced
+        if not UtilClient.is_unset(request.instance_id):
+            body['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.target_instance_id):
+            body['TargetInstanceId'] = request.target_instance_id
+        req = open_api_models.OpenApiRequest(
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='SwitchoverInstance',
+            version='2019-09-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            ocean_base_pro_20190901_models.SwitchoverInstanceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def switchover_instance(
+        self,
+        request: ocean_base_pro_20190901_models.SwitchoverInstanceRequest,
+    ) -> ocean_base_pro_20190901_models.SwitchoverInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.switchover_instance_with_options(request, runtime)
+
+    async def switchover_instance_async(
+        self,
+        request: ocean_base_pro_20190901_models.SwitchoverInstanceRequest,
+    ) -> ocean_base_pro_20190901_models.SwitchoverInstanceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.switchover_instance_with_options_async(request, runtime)
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901/models.py` & `alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1957,14 +1957,183 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateTenantReadOnlyConnectionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateTenantSecurityIpGroupRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        security_ip_group_name: str = None,
+        security_ips: str = None,
+        tenant_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.security_ip_group_name = security_ip_group_name
+        self.security_ips = security_ips
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_ip_group_name is not None:
+            result['SecurityIpGroupName'] = self.security_ip_group_name
+        if self.security_ips is not None:
+            result['SecurityIps'] = self.security_ips
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityIpGroupName') is not None:
+            self.security_ip_group_name = m.get('SecurityIpGroupName')
+        if m.get('SecurityIps') is not None:
+            self.security_ips = m.get('SecurityIps')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class CreateTenantSecurityIpGroupResponseBodySecurityIpGroup(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        security_ip_group_name: str = None,
+        security_ips: str = None,
+        tenant_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.security_ip_group_name = security_ip_group_name
+        self.security_ips = security_ips
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_ip_group_name is not None:
+            result['SecurityIpGroupName'] = self.security_ip_group_name
+        if self.security_ips is not None:
+            result['SecurityIps'] = self.security_ips
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityIpGroupName') is not None:
+            self.security_ip_group_name = m.get('SecurityIpGroupName')
+        if m.get('SecurityIps') is not None:
+            self.security_ips = m.get('SecurityIps')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class CreateTenantSecurityIpGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        security_ip_group: CreateTenantSecurityIpGroupResponseBodySecurityIpGroup = None,
+    ):
+        self.request_id = request_id
+        self.security_ip_group = security_ip_group
+
+    def validate(self):
+        if self.security_ip_group:
+            self.security_ip_group.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.security_ip_group is not None:
+            result['SecurityIpGroup'] = self.security_ip_group.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SecurityIpGroup') is not None:
+            temp_model = CreateTenantSecurityIpGroupResponseBodySecurityIpGroup()
+            self.security_ip_group = temp_model.from_map(m['SecurityIpGroup'])
+        return self
+
+
+class CreateTenantSecurityIpGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateTenantSecurityIpGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateTenantSecurityIpGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class CreateTenantUserRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
         encryption_type: str = None,
         instance_id: str = None,
         roles: str = None,
@@ -2814,14 +2983,171 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteSecurityIpGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteTenantSecurityIpGroupRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        security_ip_group_name: str = None,
+        tenant_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.security_ip_group_name = security_ip_group_name
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_ip_group_name is not None:
+            result['SecurityIpGroupName'] = self.security_ip_group_name
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityIpGroupName') is not None:
+            self.security_ip_group_name = m.get('SecurityIpGroupName')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DeleteTenantSecurityIpGroupResponseBodySecurityIpGroup(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        security_ip_group_name: str = None,
+        tenant_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.security_ip_group_name = security_ip_group_name
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_ip_group_name is not None:
+            result['SecurityIpGroupName'] = self.security_ip_group_name
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityIpGroupName') is not None:
+            self.security_ip_group_name = m.get('SecurityIpGroupName')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DeleteTenantSecurityIpGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        security_ip_group: DeleteTenantSecurityIpGroupResponseBodySecurityIpGroup = None,
+    ):
+        self.request_id = request_id
+        self.security_ip_group = security_ip_group
+
+    def validate(self):
+        if self.security_ip_group:
+            self.security_ip_group.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.security_ip_group is not None:
+            result['SecurityIpGroup'] = self.security_ip_group.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SecurityIpGroup') is not None:
+            temp_model = DeleteTenantSecurityIpGroupResponseBodySecurityIpGroup()
+            self.security_ip_group = temp_model.from_map(m['SecurityIpGroup'])
+        return self
+
+
+class DeleteTenantSecurityIpGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DeleteTenantSecurityIpGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DeleteTenantSecurityIpGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteTenantUsersRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         tenant_id: str = None,
         users: str = None,
     ):
@@ -7151,14 +7477,2945 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeNodeMetricsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeOasAnomalySQLListRequest(TeaModel):
+    def __init__(
+        self,
+        accept_language: str = None,
+        current: int = None,
+        db_name: str = None,
+        end_time: str = None,
+        filter_condition: str = None,
+        instance_id: str = None,
+        node_ip: str = None,
+        page_size: int = None,
+        search_key_word: str = None,
+        search_param: str = None,
+        search_rule: str = None,
+        search_value: str = None,
+        sql_id: str = None,
+        sql_text_length: int = None,
+        start_time: str = None,
+        tenant_id: str = None,
+    ):
+        self.accept_language = accept_language
+        self.current = current
+        self.db_name = db_name
+        self.end_time = end_time
+        self.filter_condition = filter_condition
+        self.instance_id = instance_id
+        self.node_ip = node_ip
+        self.page_size = page_size
+        self.search_key_word = search_key_word
+        self.search_param = search_param
+        self.search_rule = search_rule
+        self.search_value = search_value
+        # SQL ID。
+        self.sql_id = sql_id
+        self.sql_text_length = sql_text_length
+        self.start_time = start_time
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.accept_language is not None:
+            result['AcceptLanguage'] = self.accept_language
+        if self.current is not None:
+            result['Current'] = self.current
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.filter_condition is not None:
+            result['FilterCondition'] = self.filter_condition
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_ip is not None:
+            result['NodeIp'] = self.node_ip
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.search_key_word is not None:
+            result['SearchKeyWord'] = self.search_key_word
+        if self.search_param is not None:
+            result['SearchParam'] = self.search_param
+        if self.search_rule is not None:
+            result['SearchRule'] = self.search_rule
+        if self.search_value is not None:
+            result['SearchValue'] = self.search_value
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_text_length is not None:
+            result['SqlTextLength'] = self.sql_text_length
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AcceptLanguage') is not None:
+            self.accept_language = m.get('AcceptLanguage')
+        if m.get('Current') is not None:
+            self.current = m.get('Current')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('FilterCondition') is not None:
+            self.filter_condition = m.get('FilterCondition')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeIp') is not None:
+            self.node_ip = m.get('NodeIp')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('SearchKeyWord') is not None:
+            self.search_key_word = m.get('SearchKeyWord')
+        if m.get('SearchParam') is not None:
+            self.search_param = m.get('SearchParam')
+        if m.get('SearchRule') is not None:
+            self.search_rule = m.get('SearchRule')
+        if m.get('SearchValue') is not None:
+            self.search_value = m.get('SearchValue')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlTextLength') is not None:
+            self.sql_text_length = m.get('SqlTextLength')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DescribeOasAnomalySQLListResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        avg_cpu_time: float = None,
+        avg_elapsed_time: float = None,
+        avg_get_plan_time: float = None,
+        cpu_time: float = None,
+        db_name: str = None,
+        diag_types: List[str] = None,
+        diagnosis: str = None,
+        executions: float = None,
+        last_executed_time: float = None,
+        risk_level: str = None,
+        sql_id: str = None,
+        sql_text_short: str = None,
+        suggestion: str = None,
+        sum_elapsed_time: str = None,
+        user_name: str = None,
+    ):
+        self.avg_cpu_time = avg_cpu_time
+        self.avg_elapsed_time = avg_elapsed_time
+        self.avg_get_plan_time = avg_get_plan_time
+        self.cpu_time = cpu_time
+        self.db_name = db_name
+        self.diag_types = diag_types
+        self.diagnosis = diagnosis
+        self.executions = executions
+        self.last_executed_time = last_executed_time
+        self.risk_level = risk_level
+        # SQL ID。
+        self.sql_id = sql_id
+        self.sql_text_short = sql_text_short
+        self.suggestion = suggestion
+        self.sum_elapsed_time = sum_elapsed_time
+        self.user_name = user_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.avg_cpu_time is not None:
+            result['AvgCpuTime'] = self.avg_cpu_time
+        if self.avg_elapsed_time is not None:
+            result['AvgElapsedTime'] = self.avg_elapsed_time
+        if self.avg_get_plan_time is not None:
+            result['AvgGetPlanTime'] = self.avg_get_plan_time
+        if self.cpu_time is not None:
+            result['CpuTime'] = self.cpu_time
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.diag_types is not None:
+            result['DiagTypes'] = self.diag_types
+        if self.diagnosis is not None:
+            result['Diagnosis'] = self.diagnosis
+        if self.executions is not None:
+            result['Executions'] = self.executions
+        if self.last_executed_time is not None:
+            result['LastExecutedTime'] = self.last_executed_time
+        if self.risk_level is not None:
+            result['RiskLevel'] = self.risk_level
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_text_short is not None:
+            result['SqlTextShort'] = self.sql_text_short
+        if self.suggestion is not None:
+            result['Suggestion'] = self.suggestion
+        if self.sum_elapsed_time is not None:
+            result['SumElapsedTime'] = self.sum_elapsed_time
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AvgCpuTime') is not None:
+            self.avg_cpu_time = m.get('AvgCpuTime')
+        if m.get('AvgElapsedTime') is not None:
+            self.avg_elapsed_time = m.get('AvgElapsedTime')
+        if m.get('AvgGetPlanTime') is not None:
+            self.avg_get_plan_time = m.get('AvgGetPlanTime')
+        if m.get('CpuTime') is not None:
+            self.cpu_time = m.get('CpuTime')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('DiagTypes') is not None:
+            self.diag_types = m.get('DiagTypes')
+        if m.get('Diagnosis') is not None:
+            self.diagnosis = m.get('Diagnosis')
+        if m.get('Executions') is not None:
+            self.executions = m.get('Executions')
+        if m.get('LastExecutedTime') is not None:
+            self.last_executed_time = m.get('LastExecutedTime')
+        if m.get('RiskLevel') is not None:
+            self.risk_level = m.get('RiskLevel')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlTextShort') is not None:
+            self.sql_text_short = m.get('SqlTextShort')
+        if m.get('Suggestion') is not None:
+            self.suggestion = m.get('Suggestion')
+        if m.get('SumElapsedTime') is not None:
+            self.sum_elapsed_time = m.get('SumElapsedTime')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        return self
+
+
+class DescribeOasAnomalySQLListResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: List[DescribeOasAnomalySQLListResponseBodyData] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+        self.total_count = total_count
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = DescribeOasAnomalySQLListResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeOasAnomalySQLListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeOasAnomalySQLListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeOasAnomalySQLListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeOasSQLDetailsRequest(TeaModel):
+    def __init__(
+        self,
+        db_name: str = None,
+        end_time: str = None,
+        instance_id: str = None,
+        sql_id: str = None,
+        start_time: str = None,
+        tenant_id: str = None,
+    ):
+        self.db_name = db_name
+        self.end_time = end_time
+        self.instance_id = instance_id
+        # SQL ID。
+        self.sql_id = sql_id
+        self.start_time = start_time
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DescribeOasSQLDetailsResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        db_name: str = None,
+        fulltext: str = None,
+        statement: str = None,
+        tables: List[str] = None,
+        user_name: str = None,
+    ):
+        self.db_name = db_name
+        self.fulltext = fulltext
+        self.statement = statement
+        self.tables = tables
+        self.user_name = user_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.fulltext is not None:
+            result['Fulltext'] = self.fulltext
+        if self.statement is not None:
+            result['Statement'] = self.statement
+        if self.tables is not None:
+            result['Tables'] = self.tables
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('Fulltext') is not None:
+            self.fulltext = m.get('Fulltext')
+        if m.get('Statement') is not None:
+            self.statement = m.get('Statement')
+        if m.get('Tables') is not None:
+            self.tables = m.get('Tables')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        return self
+
+
+class DescribeOasSQLDetailsResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: DescribeOasSQLDetailsResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = DescribeOasSQLDetailsResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeOasSQLDetailsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeOasSQLDetailsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeOasSQLDetailsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeOasSQLHistoryListRequest(TeaModel):
+    def __init__(
+        self,
+        accept_language: str = None,
+        db_name: str = None,
+        end_time: str = None,
+        instance_id: str = None,
+        node_ip: str = None,
+        sql_id: str = None,
+        start_time: str = None,
+        tenant_id: str = None,
+    ):
+        self.accept_language = accept_language
+        self.db_name = db_name
+        self.end_time = end_time
+        self.instance_id = instance_id
+        self.node_ip = node_ip
+        # SQL ID。
+        self.sql_id = sql_id
+        self.start_time = start_time
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.accept_language is not None:
+            result['AcceptLanguage'] = self.accept_language
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_ip is not None:
+            result['NodeIp'] = self.node_ip
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AcceptLanguage') is not None:
+            self.accept_language = m.get('AcceptLanguage')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeIp') is not None:
+            self.node_ip = m.get('NodeIp')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DescribeOasSQLHistoryListResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        avg_affected_rows: int = None,
+        avg_application_wait_time: float = None,
+        avg_block_cache_hit: int = None,
+        avg_block_index_cache_hit: int = None,
+        avg_bloom_filter_cache_hit: int = None,
+        avg_concurrency_wait_time: float = None,
+        avg_cpu_time: float = None,
+        avg_decode_time: float = None,
+        avg_disk_reads: int = None,
+        avg_elapsed_time: float = None,
+        avg_execute_time: float = None,
+        avg_executor_rpc_count: float = None,
+        avg_expected_worker_count: float = None,
+        avg_get_plan_time: float = None,
+        avg_logical_reads: int = None,
+        avg_memstore_read_rows: int = None,
+        avg_net_time: float = None,
+        avg_net_wait_time: float = None,
+        avg_partition_count: float = None,
+        avg_queue_time: float = None,
+        avg_return_rows: int = None,
+        avg_row_cache_hit: int = None,
+        avg_rpc_count: int = None,
+        avg_schedule_time: float = None,
+        avg_ssstore_read_rows: int = None,
+        avg_used_worker_count: float = None,
+        avg_user_io_wait_time: float = None,
+        avg_wait_count: float = None,
+        avg_wait_time: float = None,
+        db_name: str = None,
+        dist_plan_percentage: float = None,
+        exec_ps: float = None,
+        executions: int = None,
+        fail_count: int = None,
+        fail_percentage: float = None,
+        local_plan_percentage: float = None,
+        max_affected_rows: float = None,
+        max_application_wait_time: float = None,
+        max_concurrency_wait_time: float = None,
+        max_cpu_time: float = None,
+        max_disk_reads: float = None,
+        max_elapsed_time: float = None,
+        max_return_rows: float = None,
+        max_user_io_wait_time: float = None,
+        max_wait_time: float = None,
+        miss_plan_percentage: float = None,
+        miss_plans: int = None,
+        remote_plan_percentage: float = None,
+        remote_plans: int = None,
+        ret_code_4012count: float = None,
+        ret_code_4013count: float = None,
+        ret_code_5001count: float = None,
+        ret_code_5024count: float = None,
+        ret_code_5167count: float = None,
+        ret_code_5217count: float = None,
+        ret_code_6002count: float = None,
+        retry_count: int = None,
+        sqlid: str = None,
+        server: str = None,
+        strong_consistency_percentage: float = None,
+        sum_elapsed_time: float = None,
+        sum_logical_reads: float = None,
+        sum_wait_time: float = None,
+        table_scan_percentage: float = None,
+        timestamp: str = None,
+        user_name: str = None,
+        weak_consistency_percentage: float = None,
+    ):
+        self.avg_affected_rows = avg_affected_rows
+        self.avg_application_wait_time = avg_application_wait_time
+        self.avg_block_cache_hit = avg_block_cache_hit
+        self.avg_block_index_cache_hit = avg_block_index_cache_hit
+        self.avg_bloom_filter_cache_hit = avg_bloom_filter_cache_hit
+        self.avg_concurrency_wait_time = avg_concurrency_wait_time
+        self.avg_cpu_time = avg_cpu_time
+        self.avg_decode_time = avg_decode_time
+        self.avg_disk_reads = avg_disk_reads
+        self.avg_elapsed_time = avg_elapsed_time
+        self.avg_execute_time = avg_execute_time
+        self.avg_executor_rpc_count = avg_executor_rpc_count
+        self.avg_expected_worker_count = avg_expected_worker_count
+        self.avg_get_plan_time = avg_get_plan_time
+        self.avg_logical_reads = avg_logical_reads
+        self.avg_memstore_read_rows = avg_memstore_read_rows
+        self.avg_net_time = avg_net_time
+        self.avg_net_wait_time = avg_net_wait_time
+        self.avg_partition_count = avg_partition_count
+        self.avg_queue_time = avg_queue_time
+        self.avg_return_rows = avg_return_rows
+        self.avg_row_cache_hit = avg_row_cache_hit
+        self.avg_rpc_count = avg_rpc_count
+        self.avg_schedule_time = avg_schedule_time
+        self.avg_ssstore_read_rows = avg_ssstore_read_rows
+        self.avg_used_worker_count = avg_used_worker_count
+        self.avg_user_io_wait_time = avg_user_io_wait_time
+        self.avg_wait_count = avg_wait_count
+        self.avg_wait_time = avg_wait_time
+        self.db_name = db_name
+        self.dist_plan_percentage = dist_plan_percentage
+        self.exec_ps = exec_ps
+        self.executions = executions
+        self.fail_count = fail_count
+        self.fail_percentage = fail_percentage
+        self.local_plan_percentage = local_plan_percentage
+        self.max_affected_rows = max_affected_rows
+        self.max_application_wait_time = max_application_wait_time
+        self.max_concurrency_wait_time = max_concurrency_wait_time
+        self.max_cpu_time = max_cpu_time
+        self.max_disk_reads = max_disk_reads
+        self.max_elapsed_time = max_elapsed_time
+        self.max_return_rows = max_return_rows
+        self.max_user_io_wait_time = max_user_io_wait_time
+        self.max_wait_time = max_wait_time
+        self.miss_plan_percentage = miss_plan_percentage
+        self.miss_plans = miss_plans
+        self.remote_plan_percentage = remote_plan_percentage
+        self.remote_plans = remote_plans
+        self.ret_code_4012count = ret_code_4012count
+        self.ret_code_4013count = ret_code_4013count
+        self.ret_code_5001count = ret_code_5001count
+        self.ret_code_5024count = ret_code_5024count
+        self.ret_code_5167count = ret_code_5167count
+        self.ret_code_5217count = ret_code_5217count
+        self.ret_code_6002count = ret_code_6002count
+        self.retry_count = retry_count
+        # SQL ID
+        self.sqlid = sqlid
+        self.server = server
+        self.strong_consistency_percentage = strong_consistency_percentage
+        self.sum_elapsed_time = sum_elapsed_time
+        self.sum_logical_reads = sum_logical_reads
+        self.sum_wait_time = sum_wait_time
+        self.table_scan_percentage = table_scan_percentage
+        self.timestamp = timestamp
+        self.user_name = user_name
+        self.weak_consistency_percentage = weak_consistency_percentage
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.avg_affected_rows is not None:
+            result['AvgAffectedRows'] = self.avg_affected_rows
+        if self.avg_application_wait_time is not None:
+            result['AvgApplicationWaitTime'] = self.avg_application_wait_time
+        if self.avg_block_cache_hit is not None:
+            result['AvgBlockCacheHit'] = self.avg_block_cache_hit
+        if self.avg_block_index_cache_hit is not None:
+            result['AvgBlockIndexCacheHit'] = self.avg_block_index_cache_hit
+        if self.avg_bloom_filter_cache_hit is not None:
+            result['AvgBloomFilterCacheHit'] = self.avg_bloom_filter_cache_hit
+        if self.avg_concurrency_wait_time is not None:
+            result['AvgConcurrencyWaitTime'] = self.avg_concurrency_wait_time
+        if self.avg_cpu_time is not None:
+            result['AvgCpuTime'] = self.avg_cpu_time
+        if self.avg_decode_time is not None:
+            result['AvgDecodeTime'] = self.avg_decode_time
+        if self.avg_disk_reads is not None:
+            result['AvgDiskReads'] = self.avg_disk_reads
+        if self.avg_elapsed_time is not None:
+            result['AvgElapsedTime'] = self.avg_elapsed_time
+        if self.avg_execute_time is not None:
+            result['AvgExecuteTime'] = self.avg_execute_time
+        if self.avg_executor_rpc_count is not None:
+            result['AvgExecutorRpcCount'] = self.avg_executor_rpc_count
+        if self.avg_expected_worker_count is not None:
+            result['AvgExpectedWorkerCount'] = self.avg_expected_worker_count
+        if self.avg_get_plan_time is not None:
+            result['AvgGetPlanTime'] = self.avg_get_plan_time
+        if self.avg_logical_reads is not None:
+            result['AvgLogicalReads'] = self.avg_logical_reads
+        if self.avg_memstore_read_rows is not None:
+            result['AvgMemstoreReadRows'] = self.avg_memstore_read_rows
+        if self.avg_net_time is not None:
+            result['AvgNetTime'] = self.avg_net_time
+        if self.avg_net_wait_time is not None:
+            result['AvgNetWaitTime'] = self.avg_net_wait_time
+        if self.avg_partition_count is not None:
+            result['AvgPartitionCount'] = self.avg_partition_count
+        if self.avg_queue_time is not None:
+            result['AvgQueueTime'] = self.avg_queue_time
+        if self.avg_return_rows is not None:
+            result['AvgReturnRows'] = self.avg_return_rows
+        if self.avg_row_cache_hit is not None:
+            result['AvgRowCacheHit'] = self.avg_row_cache_hit
+        if self.avg_rpc_count is not None:
+            result['AvgRpcCount'] = self.avg_rpc_count
+        if self.avg_schedule_time is not None:
+            result['AvgScheduleTime'] = self.avg_schedule_time
+        if self.avg_ssstore_read_rows is not None:
+            result['AvgSsstoreReadRows'] = self.avg_ssstore_read_rows
+        if self.avg_used_worker_count is not None:
+            result['AvgUsedWorkerCount'] = self.avg_used_worker_count
+        if self.avg_user_io_wait_time is not None:
+            result['AvgUserIoWaitTime'] = self.avg_user_io_wait_time
+        if self.avg_wait_count is not None:
+            result['AvgWaitCount'] = self.avg_wait_count
+        if self.avg_wait_time is not None:
+            result['AvgWaitTime'] = self.avg_wait_time
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.dist_plan_percentage is not None:
+            result['DistPlanPercentage'] = self.dist_plan_percentage
+        if self.exec_ps is not None:
+            result['ExecPs'] = self.exec_ps
+        if self.executions is not None:
+            result['Executions'] = self.executions
+        if self.fail_count is not None:
+            result['FailCount'] = self.fail_count
+        if self.fail_percentage is not None:
+            result['FailPercentage'] = self.fail_percentage
+        if self.local_plan_percentage is not None:
+            result['LocalPlanPercentage'] = self.local_plan_percentage
+        if self.max_affected_rows is not None:
+            result['MaxAffectedRows'] = self.max_affected_rows
+        if self.max_application_wait_time is not None:
+            result['MaxApplicationWaitTime'] = self.max_application_wait_time
+        if self.max_concurrency_wait_time is not None:
+            result['MaxConcurrencyWaitTime'] = self.max_concurrency_wait_time
+        if self.max_cpu_time is not None:
+            result['MaxCpuTime'] = self.max_cpu_time
+        if self.max_disk_reads is not None:
+            result['MaxDiskReads'] = self.max_disk_reads
+        if self.max_elapsed_time is not None:
+            result['MaxElapsedTime'] = self.max_elapsed_time
+        if self.max_return_rows is not None:
+            result['MaxReturnRows'] = self.max_return_rows
+        if self.max_user_io_wait_time is not None:
+            result['MaxUserIoWaitTime'] = self.max_user_io_wait_time
+        if self.max_wait_time is not None:
+            result['MaxWaitTime'] = self.max_wait_time
+        if self.miss_plan_percentage is not None:
+            result['MissPlanPercentage'] = self.miss_plan_percentage
+        if self.miss_plans is not None:
+            result['MissPlans'] = self.miss_plans
+        if self.remote_plan_percentage is not None:
+            result['RemotePlanPercentage'] = self.remote_plan_percentage
+        if self.remote_plans is not None:
+            result['RemotePlans'] = self.remote_plans
+        if self.ret_code_4012count is not None:
+            result['RetCode4012Count'] = self.ret_code_4012count
+        if self.ret_code_4013count is not None:
+            result['RetCode4013Count'] = self.ret_code_4013count
+        if self.ret_code_5001count is not None:
+            result['RetCode5001Count'] = self.ret_code_5001count
+        if self.ret_code_5024count is not None:
+            result['RetCode5024Count'] = self.ret_code_5024count
+        if self.ret_code_5167count is not None:
+            result['RetCode5167Count'] = self.ret_code_5167count
+        if self.ret_code_5217count is not None:
+            result['RetCode5217Count'] = self.ret_code_5217count
+        if self.ret_code_6002count is not None:
+            result['RetCode6002Count'] = self.ret_code_6002count
+        if self.retry_count is not None:
+            result['RetryCount'] = self.retry_count
+        if self.sqlid is not None:
+            result['SQLId'] = self.sqlid
+        if self.server is not None:
+            result['Server'] = self.server
+        if self.strong_consistency_percentage is not None:
+            result['StrongConsistencyPercentage'] = self.strong_consistency_percentage
+        if self.sum_elapsed_time is not None:
+            result['SumElapsedTime'] = self.sum_elapsed_time
+        if self.sum_logical_reads is not None:
+            result['SumLogicalReads'] = self.sum_logical_reads
+        if self.sum_wait_time is not None:
+            result['SumWaitTime'] = self.sum_wait_time
+        if self.table_scan_percentage is not None:
+            result['TableScanPercentage'] = self.table_scan_percentage
+        if self.timestamp is not None:
+            result['Timestamp'] = self.timestamp
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        if self.weak_consistency_percentage is not None:
+            result['WeakConsistencyPercentage'] = self.weak_consistency_percentage
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AvgAffectedRows') is not None:
+            self.avg_affected_rows = m.get('AvgAffectedRows')
+        if m.get('AvgApplicationWaitTime') is not None:
+            self.avg_application_wait_time = m.get('AvgApplicationWaitTime')
+        if m.get('AvgBlockCacheHit') is not None:
+            self.avg_block_cache_hit = m.get('AvgBlockCacheHit')
+        if m.get('AvgBlockIndexCacheHit') is not None:
+            self.avg_block_index_cache_hit = m.get('AvgBlockIndexCacheHit')
+        if m.get('AvgBloomFilterCacheHit') is not None:
+            self.avg_bloom_filter_cache_hit = m.get('AvgBloomFilterCacheHit')
+        if m.get('AvgConcurrencyWaitTime') is not None:
+            self.avg_concurrency_wait_time = m.get('AvgConcurrencyWaitTime')
+        if m.get('AvgCpuTime') is not None:
+            self.avg_cpu_time = m.get('AvgCpuTime')
+        if m.get('AvgDecodeTime') is not None:
+            self.avg_decode_time = m.get('AvgDecodeTime')
+        if m.get('AvgDiskReads') is not None:
+            self.avg_disk_reads = m.get('AvgDiskReads')
+        if m.get('AvgElapsedTime') is not None:
+            self.avg_elapsed_time = m.get('AvgElapsedTime')
+        if m.get('AvgExecuteTime') is not None:
+            self.avg_execute_time = m.get('AvgExecuteTime')
+        if m.get('AvgExecutorRpcCount') is not None:
+            self.avg_executor_rpc_count = m.get('AvgExecutorRpcCount')
+        if m.get('AvgExpectedWorkerCount') is not None:
+            self.avg_expected_worker_count = m.get('AvgExpectedWorkerCount')
+        if m.get('AvgGetPlanTime') is not None:
+            self.avg_get_plan_time = m.get('AvgGetPlanTime')
+        if m.get('AvgLogicalReads') is not None:
+            self.avg_logical_reads = m.get('AvgLogicalReads')
+        if m.get('AvgMemstoreReadRows') is not None:
+            self.avg_memstore_read_rows = m.get('AvgMemstoreReadRows')
+        if m.get('AvgNetTime') is not None:
+            self.avg_net_time = m.get('AvgNetTime')
+        if m.get('AvgNetWaitTime') is not None:
+            self.avg_net_wait_time = m.get('AvgNetWaitTime')
+        if m.get('AvgPartitionCount') is not None:
+            self.avg_partition_count = m.get('AvgPartitionCount')
+        if m.get('AvgQueueTime') is not None:
+            self.avg_queue_time = m.get('AvgQueueTime')
+        if m.get('AvgReturnRows') is not None:
+            self.avg_return_rows = m.get('AvgReturnRows')
+        if m.get('AvgRowCacheHit') is not None:
+            self.avg_row_cache_hit = m.get('AvgRowCacheHit')
+        if m.get('AvgRpcCount') is not None:
+            self.avg_rpc_count = m.get('AvgRpcCount')
+        if m.get('AvgScheduleTime') is not None:
+            self.avg_schedule_time = m.get('AvgScheduleTime')
+        if m.get('AvgSsstoreReadRows') is not None:
+            self.avg_ssstore_read_rows = m.get('AvgSsstoreReadRows')
+        if m.get('AvgUsedWorkerCount') is not None:
+            self.avg_used_worker_count = m.get('AvgUsedWorkerCount')
+        if m.get('AvgUserIoWaitTime') is not None:
+            self.avg_user_io_wait_time = m.get('AvgUserIoWaitTime')
+        if m.get('AvgWaitCount') is not None:
+            self.avg_wait_count = m.get('AvgWaitCount')
+        if m.get('AvgWaitTime') is not None:
+            self.avg_wait_time = m.get('AvgWaitTime')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('DistPlanPercentage') is not None:
+            self.dist_plan_percentage = m.get('DistPlanPercentage')
+        if m.get('ExecPs') is not None:
+            self.exec_ps = m.get('ExecPs')
+        if m.get('Executions') is not None:
+            self.executions = m.get('Executions')
+        if m.get('FailCount') is not None:
+            self.fail_count = m.get('FailCount')
+        if m.get('FailPercentage') is not None:
+            self.fail_percentage = m.get('FailPercentage')
+        if m.get('LocalPlanPercentage') is not None:
+            self.local_plan_percentage = m.get('LocalPlanPercentage')
+        if m.get('MaxAffectedRows') is not None:
+            self.max_affected_rows = m.get('MaxAffectedRows')
+        if m.get('MaxApplicationWaitTime') is not None:
+            self.max_application_wait_time = m.get('MaxApplicationWaitTime')
+        if m.get('MaxConcurrencyWaitTime') is not None:
+            self.max_concurrency_wait_time = m.get('MaxConcurrencyWaitTime')
+        if m.get('MaxCpuTime') is not None:
+            self.max_cpu_time = m.get('MaxCpuTime')
+        if m.get('MaxDiskReads') is not None:
+            self.max_disk_reads = m.get('MaxDiskReads')
+        if m.get('MaxElapsedTime') is not None:
+            self.max_elapsed_time = m.get('MaxElapsedTime')
+        if m.get('MaxReturnRows') is not None:
+            self.max_return_rows = m.get('MaxReturnRows')
+        if m.get('MaxUserIoWaitTime') is not None:
+            self.max_user_io_wait_time = m.get('MaxUserIoWaitTime')
+        if m.get('MaxWaitTime') is not None:
+            self.max_wait_time = m.get('MaxWaitTime')
+        if m.get('MissPlanPercentage') is not None:
+            self.miss_plan_percentage = m.get('MissPlanPercentage')
+        if m.get('MissPlans') is not None:
+            self.miss_plans = m.get('MissPlans')
+        if m.get('RemotePlanPercentage') is not None:
+            self.remote_plan_percentage = m.get('RemotePlanPercentage')
+        if m.get('RemotePlans') is not None:
+            self.remote_plans = m.get('RemotePlans')
+        if m.get('RetCode4012Count') is not None:
+            self.ret_code_4012count = m.get('RetCode4012Count')
+        if m.get('RetCode4013Count') is not None:
+            self.ret_code_4013count = m.get('RetCode4013Count')
+        if m.get('RetCode5001Count') is not None:
+            self.ret_code_5001count = m.get('RetCode5001Count')
+        if m.get('RetCode5024Count') is not None:
+            self.ret_code_5024count = m.get('RetCode5024Count')
+        if m.get('RetCode5167Count') is not None:
+            self.ret_code_5167count = m.get('RetCode5167Count')
+        if m.get('RetCode5217Count') is not None:
+            self.ret_code_5217count = m.get('RetCode5217Count')
+        if m.get('RetCode6002Count') is not None:
+            self.ret_code_6002count = m.get('RetCode6002Count')
+        if m.get('RetryCount') is not None:
+            self.retry_count = m.get('RetryCount')
+        if m.get('SQLId') is not None:
+            self.sqlid = m.get('SQLId')
+        if m.get('Server') is not None:
+            self.server = m.get('Server')
+        if m.get('StrongConsistencyPercentage') is not None:
+            self.strong_consistency_percentage = m.get('StrongConsistencyPercentage')
+        if m.get('SumElapsedTime') is not None:
+            self.sum_elapsed_time = m.get('SumElapsedTime')
+        if m.get('SumLogicalReads') is not None:
+            self.sum_logical_reads = m.get('SumLogicalReads')
+        if m.get('SumWaitTime') is not None:
+            self.sum_wait_time = m.get('SumWaitTime')
+        if m.get('TableScanPercentage') is not None:
+            self.table_scan_percentage = m.get('TableScanPercentage')
+        if m.get('Timestamp') is not None:
+            self.timestamp = m.get('Timestamp')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        if m.get('WeakConsistencyPercentage') is not None:
+            self.weak_consistency_percentage = m.get('WeakConsistencyPercentage')
+        return self
+
+
+class DescribeOasSQLHistoryListResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: List[DescribeOasSQLHistoryListResponseBodyData] = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = DescribeOasSQLHistoryListResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeOasSQLHistoryListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeOasSQLHistoryListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeOasSQLHistoryListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeOasSQLPlansRequest(TeaModel):
+    def __init__(
+        self,
+        accept_language: str = None,
+        db_name: str = None,
+        end_time: str = None,
+        instance_id: str = None,
+        sql_id: str = None,
+        start_time: str = None,
+        tenant_id: str = None,
+    ):
+        self.accept_language = accept_language
+        self.db_name = db_name
+        self.end_time = end_time
+        self.instance_id = instance_id
+        # SQL ID。
+        self.sql_id = sql_id
+        self.start_time = start_time
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.accept_language is not None:
+            result['AcceptLanguage'] = self.accept_language
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AcceptLanguage') is not None:
+            self.accept_language = m.get('AcceptLanguage')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DescribeOasSQLPlansResponseBodyDataPlanExplain(TeaModel):
+    def __init__(
+        self,
+        plan_json_string: str = None,
+    ):
+        self.plan_json_string = plan_json_string
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.plan_json_string is not None:
+            result['PlanJsonString'] = self.plan_json_string
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('PlanJsonString') is not None:
+            self.plan_json_string = m.get('PlanJsonString')
+        return self
+
+
+class DescribeOasSQLPlansResponseBodyDataPlans(TeaModel):
+    def __init__(
+        self,
+        avg_application_wait_time: float = None,
+        avg_buffer_gets: float = None,
+        avg_concurrency_wait_time: float = None,
+        avg_cpu_time: float = None,
+        avg_disk_reads: float = None,
+        avg_disk_writes: float = None,
+        avg_elapsed_time: float = None,
+        avg_row_processed: float = None,
+        avg_user_io_wait_time: float = None,
+        collect_time_us: int = None,
+        delayed_large_query_percentage: float = None,
+        exec_ps: float = None,
+        executions: int = None,
+        first_load_time: str = None,
+        first_load_time_us: int = None,
+        hit_diagnosis: bool = None,
+        hit_percentage: float = None,
+        large_query_percentage: float = None,
+        merged_version: int = None,
+        ob_db_id: int = None,
+        ob_server_id: int = None,
+        outline_data: str = None,
+        outline_id: int = None,
+        plan_hash: str = None,
+        plan_id: int = None,
+        plan_size: int = None,
+        plan_type: str = None,
+        plan_union_hash: str = None,
+        schema_version: int = None,
+        server: str = None,
+        server_id: int = None,
+        table_scan: bool = None,
+        timeout_percentage: float = None,
+        uid: str = None,
+    ):
+        self.avg_application_wait_time = avg_application_wait_time
+        self.avg_buffer_gets = avg_buffer_gets
+        self.avg_concurrency_wait_time = avg_concurrency_wait_time
+        self.avg_cpu_time = avg_cpu_time
+        self.avg_disk_reads = avg_disk_reads
+        self.avg_disk_writes = avg_disk_writes
+        self.avg_elapsed_time = avg_elapsed_time
+        self.avg_row_processed = avg_row_processed
+        self.avg_user_io_wait_time = avg_user_io_wait_time
+        self.collect_time_us = collect_time_us
+        self.delayed_large_query_percentage = delayed_large_query_percentage
+        self.exec_ps = exec_ps
+        self.executions = executions
+        self.first_load_time = first_load_time
+        self.first_load_time_us = first_load_time_us
+        self.hit_diagnosis = hit_diagnosis
+        self.hit_percentage = hit_percentage
+        self.large_query_percentage = large_query_percentage
+        self.merged_version = merged_version
+        self.ob_db_id = ob_db_id
+        # server  ID。
+        self.ob_server_id = ob_server_id
+        self.outline_data = outline_data
+        # Outline ID。
+        self.outline_id = outline_id
+        self.plan_hash = plan_hash
+        self.plan_id = plan_id
+        self.plan_size = plan_size
+        self.plan_type = plan_type
+        self.plan_union_hash = plan_union_hash
+        self.schema_version = schema_version
+        self.server = server
+        self.server_id = server_id
+        self.table_scan = table_scan
+        self.timeout_percentage = timeout_percentage
+        self.uid = uid
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.avg_application_wait_time is not None:
+            result['AvgApplicationWaitTime'] = self.avg_application_wait_time
+        if self.avg_buffer_gets is not None:
+            result['AvgBufferGets'] = self.avg_buffer_gets
+        if self.avg_concurrency_wait_time is not None:
+            result['AvgConcurrencyWaitTime'] = self.avg_concurrency_wait_time
+        if self.avg_cpu_time is not None:
+            result['AvgCpuTime'] = self.avg_cpu_time
+        if self.avg_disk_reads is not None:
+            result['AvgDiskReads'] = self.avg_disk_reads
+        if self.avg_disk_writes is not None:
+            result['AvgDiskWrites'] = self.avg_disk_writes
+        if self.avg_elapsed_time is not None:
+            result['AvgElapsedTime'] = self.avg_elapsed_time
+        if self.avg_row_processed is not None:
+            result['AvgRowProcessed'] = self.avg_row_processed
+        if self.avg_user_io_wait_time is not None:
+            result['AvgUserIoWaitTime'] = self.avg_user_io_wait_time
+        if self.collect_time_us is not None:
+            result['CollectTimeUs'] = self.collect_time_us
+        if self.delayed_large_query_percentage is not None:
+            result['DelayedLargeQueryPercentage'] = self.delayed_large_query_percentage
+        if self.exec_ps is not None:
+            result['ExecPs'] = self.exec_ps
+        if self.executions is not None:
+            result['Executions'] = self.executions
+        if self.first_load_time is not None:
+            result['FirstLoadTime'] = self.first_load_time
+        if self.first_load_time_us is not None:
+            result['FirstLoadTimeUs'] = self.first_load_time_us
+        if self.hit_diagnosis is not None:
+            result['HitDiagnosis'] = self.hit_diagnosis
+        if self.hit_percentage is not None:
+            result['HitPercentage'] = self.hit_percentage
+        if self.large_query_percentage is not None:
+            result['LargeQueryPercentage'] = self.large_query_percentage
+        if self.merged_version is not None:
+            result['MergedVersion'] = self.merged_version
+        if self.ob_db_id is not None:
+            result['ObDbId'] = self.ob_db_id
+        if self.ob_server_id is not None:
+            result['ObServerId'] = self.ob_server_id
+        if self.outline_data is not None:
+            result['OutlineData'] = self.outline_data
+        if self.outline_id is not None:
+            result['OutlineId'] = self.outline_id
+        if self.plan_hash is not None:
+            result['PlanHash'] = self.plan_hash
+        if self.plan_id is not None:
+            result['PlanId'] = self.plan_id
+        if self.plan_size is not None:
+            result['PlanSize'] = self.plan_size
+        if self.plan_type is not None:
+            result['PlanType'] = self.plan_type
+        if self.plan_union_hash is not None:
+            result['PlanUnionHash'] = self.plan_union_hash
+        if self.schema_version is not None:
+            result['SchemaVersion'] = self.schema_version
+        if self.server is not None:
+            result['Server'] = self.server
+        if self.server_id is not None:
+            result['ServerId'] = self.server_id
+        if self.table_scan is not None:
+            result['TableScan'] = self.table_scan
+        if self.timeout_percentage is not None:
+            result['TimeoutPercentage'] = self.timeout_percentage
+        if self.uid is not None:
+            result['Uid'] = self.uid
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AvgApplicationWaitTime') is not None:
+            self.avg_application_wait_time = m.get('AvgApplicationWaitTime')
+        if m.get('AvgBufferGets') is not None:
+            self.avg_buffer_gets = m.get('AvgBufferGets')
+        if m.get('AvgConcurrencyWaitTime') is not None:
+            self.avg_concurrency_wait_time = m.get('AvgConcurrencyWaitTime')
+        if m.get('AvgCpuTime') is not None:
+            self.avg_cpu_time = m.get('AvgCpuTime')
+        if m.get('AvgDiskReads') is not None:
+            self.avg_disk_reads = m.get('AvgDiskReads')
+        if m.get('AvgDiskWrites') is not None:
+            self.avg_disk_writes = m.get('AvgDiskWrites')
+        if m.get('AvgElapsedTime') is not None:
+            self.avg_elapsed_time = m.get('AvgElapsedTime')
+        if m.get('AvgRowProcessed') is not None:
+            self.avg_row_processed = m.get('AvgRowProcessed')
+        if m.get('AvgUserIoWaitTime') is not None:
+            self.avg_user_io_wait_time = m.get('AvgUserIoWaitTime')
+        if m.get('CollectTimeUs') is not None:
+            self.collect_time_us = m.get('CollectTimeUs')
+        if m.get('DelayedLargeQueryPercentage') is not None:
+            self.delayed_large_query_percentage = m.get('DelayedLargeQueryPercentage')
+        if m.get('ExecPs') is not None:
+            self.exec_ps = m.get('ExecPs')
+        if m.get('Executions') is not None:
+            self.executions = m.get('Executions')
+        if m.get('FirstLoadTime') is not None:
+            self.first_load_time = m.get('FirstLoadTime')
+        if m.get('FirstLoadTimeUs') is not None:
+            self.first_load_time_us = m.get('FirstLoadTimeUs')
+        if m.get('HitDiagnosis') is not None:
+            self.hit_diagnosis = m.get('HitDiagnosis')
+        if m.get('HitPercentage') is not None:
+            self.hit_percentage = m.get('HitPercentage')
+        if m.get('LargeQueryPercentage') is not None:
+            self.large_query_percentage = m.get('LargeQueryPercentage')
+        if m.get('MergedVersion') is not None:
+            self.merged_version = m.get('MergedVersion')
+        if m.get('ObDbId') is not None:
+            self.ob_db_id = m.get('ObDbId')
+        if m.get('ObServerId') is not None:
+            self.ob_server_id = m.get('ObServerId')
+        if m.get('OutlineData') is not None:
+            self.outline_data = m.get('OutlineData')
+        if m.get('OutlineId') is not None:
+            self.outline_id = m.get('OutlineId')
+        if m.get('PlanHash') is not None:
+            self.plan_hash = m.get('PlanHash')
+        if m.get('PlanId') is not None:
+            self.plan_id = m.get('PlanId')
+        if m.get('PlanSize') is not None:
+            self.plan_size = m.get('PlanSize')
+        if m.get('PlanType') is not None:
+            self.plan_type = m.get('PlanType')
+        if m.get('PlanUnionHash') is not None:
+            self.plan_union_hash = m.get('PlanUnionHash')
+        if m.get('SchemaVersion') is not None:
+            self.schema_version = m.get('SchemaVersion')
+        if m.get('Server') is not None:
+            self.server = m.get('Server')
+        if m.get('ServerId') is not None:
+            self.server_id = m.get('ServerId')
+        if m.get('TableScan') is not None:
+            self.table_scan = m.get('TableScan')
+        if m.get('TimeoutPercentage') is not None:
+            self.timeout_percentage = m.get('TimeoutPercentage')
+        if m.get('Uid') is not None:
+            self.uid = m.get('Uid')
+        return self
+
+
+class DescribeOasSQLPlansResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        avg_cpu_time: float = None,
+        bounded: bool = None,
+        executions: int = None,
+        first_load_time: str = None,
+        hit_diagnosis: bool = None,
+        hit_percentage: float = None,
+        merged_version: int = None,
+        plan_explain: DescribeOasSQLPlansResponseBodyDataPlanExplain = None,
+        plan_hash: str = None,
+        plan_type: str = None,
+        plan_union_hash: str = None,
+        plans: List[DescribeOasSQLPlansResponseBodyDataPlans] = None,
+        query_sql: str = None,
+    ):
+        self.avg_cpu_time = avg_cpu_time
+        self.bounded = bounded
+        self.executions = executions
+        self.first_load_time = first_load_time
+        self.hit_diagnosis = hit_diagnosis
+        self.hit_percentage = hit_percentage
+        self.merged_version = merged_version
+        self.plan_explain = plan_explain
+        self.plan_hash = plan_hash
+        self.plan_type = plan_type
+        self.plan_union_hash = plan_union_hash
+        self.plans = plans
+        self.query_sql = query_sql
+
+    def validate(self):
+        if self.plan_explain:
+            self.plan_explain.validate()
+        if self.plans:
+            for k in self.plans:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.avg_cpu_time is not None:
+            result['AvgCpuTime'] = self.avg_cpu_time
+        if self.bounded is not None:
+            result['Bounded'] = self.bounded
+        if self.executions is not None:
+            result['Executions'] = self.executions
+        if self.first_load_time is not None:
+            result['FirstLoadTime'] = self.first_load_time
+        if self.hit_diagnosis is not None:
+            result['HitDiagnosis'] = self.hit_diagnosis
+        if self.hit_percentage is not None:
+            result['HitPercentage'] = self.hit_percentage
+        if self.merged_version is not None:
+            result['MergedVersion'] = self.merged_version
+        if self.plan_explain is not None:
+            result['PlanExplain'] = self.plan_explain.to_map()
+        if self.plan_hash is not None:
+            result['PlanHash'] = self.plan_hash
+        if self.plan_type is not None:
+            result['PlanType'] = self.plan_type
+        if self.plan_union_hash is not None:
+            result['PlanUnionHash'] = self.plan_union_hash
+        result['Plans'] = []
+        if self.plans is not None:
+            for k in self.plans:
+                result['Plans'].append(k.to_map() if k else None)
+        if self.query_sql is not None:
+            result['QuerySql'] = self.query_sql
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AvgCpuTime') is not None:
+            self.avg_cpu_time = m.get('AvgCpuTime')
+        if m.get('Bounded') is not None:
+            self.bounded = m.get('Bounded')
+        if m.get('Executions') is not None:
+            self.executions = m.get('Executions')
+        if m.get('FirstLoadTime') is not None:
+            self.first_load_time = m.get('FirstLoadTime')
+        if m.get('HitDiagnosis') is not None:
+            self.hit_diagnosis = m.get('HitDiagnosis')
+        if m.get('HitPercentage') is not None:
+            self.hit_percentage = m.get('HitPercentage')
+        if m.get('MergedVersion') is not None:
+            self.merged_version = m.get('MergedVersion')
+        if m.get('PlanExplain') is not None:
+            temp_model = DescribeOasSQLPlansResponseBodyDataPlanExplain()
+            self.plan_explain = temp_model.from_map(m['PlanExplain'])
+        if m.get('PlanHash') is not None:
+            self.plan_hash = m.get('PlanHash')
+        if m.get('PlanType') is not None:
+            self.plan_type = m.get('PlanType')
+        if m.get('PlanUnionHash') is not None:
+            self.plan_union_hash = m.get('PlanUnionHash')
+        self.plans = []
+        if m.get('Plans') is not None:
+            for k in m.get('Plans'):
+                temp_model = DescribeOasSQLPlansResponseBodyDataPlans()
+                self.plans.append(temp_model.from_map(k))
+        if m.get('QuerySql') is not None:
+            self.query_sql = m.get('QuerySql')
+        return self
+
+
+class DescribeOasSQLPlansResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: List[DescribeOasSQLPlansResponseBodyData] = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = DescribeOasSQLPlansResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeOasSQLPlansResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeOasSQLPlansResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeOasSQLPlansResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeOasSlowSQLListRequest(TeaModel):
+    def __init__(
+        self,
+        accept_language: str = None,
+        db_name: str = None,
+        end_time: str = None,
+        filter_condition: str = None,
+        instance_id: str = None,
+        node_ip: str = None,
+        search_key_word: str = None,
+        search_param: str = None,
+        search_rule: str = None,
+        search_value: str = None,
+        sql_id: str = None,
+        sql_text_length: int = None,
+        start_time: str = None,
+        tenant_id: str = None,
+    ):
+        self.accept_language = accept_language
+        self.db_name = db_name
+        self.end_time = end_time
+        self.filter_condition = filter_condition
+        self.instance_id = instance_id
+        self.node_ip = node_ip
+        self.search_key_word = search_key_word
+        self.search_param = search_param
+        self.search_rule = search_rule
+        self.search_value = search_value
+        self.sql_id = sql_id
+        self.sql_text_length = sql_text_length
+        self.start_time = start_time
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.accept_language is not None:
+            result['AcceptLanguage'] = self.accept_language
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.filter_condition is not None:
+            result['FilterCondition'] = self.filter_condition
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_ip is not None:
+            result['NodeIp'] = self.node_ip
+        if self.search_key_word is not None:
+            result['SearchKeyWord'] = self.search_key_word
+        if self.search_param is not None:
+            result['SearchParam'] = self.search_param
+        if self.search_rule is not None:
+            result['SearchRule'] = self.search_rule
+        if self.search_value is not None:
+            result['SearchValue'] = self.search_value
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_text_length is not None:
+            result['SqlTextLength'] = self.sql_text_length
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AcceptLanguage') is not None:
+            self.accept_language = m.get('AcceptLanguage')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('FilterCondition') is not None:
+            self.filter_condition = m.get('FilterCondition')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeIp') is not None:
+            self.node_ip = m.get('NodeIp')
+        if m.get('SearchKeyWord') is not None:
+            self.search_key_word = m.get('SearchKeyWord')
+        if m.get('SearchParam') is not None:
+            self.search_param = m.get('SearchParam')
+        if m.get('SearchRule') is not None:
+            self.search_rule = m.get('SearchRule')
+        if m.get('SearchValue') is not None:
+            self.search_value = m.get('SearchValue')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlTextLength') is not None:
+            self.sql_text_length = m.get('SqlTextLength')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DescribeOasSlowSQLListResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        avg_affected_rows: float = None,
+        avg_application_wait_time: float = None,
+        avg_block_cache_hit: float = None,
+        avg_block_index_cache_hit: float = None,
+        avg_bloom_filter_cache_hit: float = None,
+        avg_concurrency_wait_time: float = None,
+        avg_cpu_time: float = None,
+        avg_decode_time: float = None,
+        avg_disk_reads: float = None,
+        avg_elapsed_time: float = None,
+        avg_execute_time: float = None,
+        avg_executor_rpc_count: float = None,
+        avg_expected_worker_count: float = None,
+        avg_get_plan_time: float = None,
+        avg_logical_reads: float = None,
+        avg_memstore_read_rows: float = None,
+        avg_net_time: float = None,
+        avg_net_wait_time: float = None,
+        avg_partition_count: float = None,
+        avg_queue_time: float = None,
+        avg_return_rows: float = None,
+        avg_row_cache_hit: float = None,
+        avg_rpc_count: float = None,
+        avg_schedule_time: float = None,
+        avg_ssstore_read_rows: float = None,
+        avg_used_worker_count: float = None,
+        avg_user_io_wait_time: float = None,
+        avg_wait_count: float = None,
+        avg_wait_time: float = None,
+        client_ip: str = None,
+        db_name: str = None,
+        dist_plan_percentage: float = None,
+        exec_ps: float = None,
+        executions: float = None,
+        fail_count: float = None,
+        fail_percentage: float = None,
+        inner: bool = None,
+        local_plan_percentage: float = None,
+        max_affected_rows: float = None,
+        max_application_wait_time: float = None,
+        max_concurrency_wait_time: float = None,
+        max_cpu_time: float = None,
+        max_disk_reads: float = None,
+        max_elapsed_time: float = None,
+        max_return_rows: float = None,
+        max_user_io_wait_time: float = None,
+        max_wait_time: float = None,
+        miss_plan_percentage: float = None,
+        miss_plans: float = None,
+        remote_plan_percentage: float = None,
+        remote_plans: float = None,
+        ret_code_4012count: int = None,
+        ret_code_4013count: int = None,
+        ret_code_5001count: int = None,
+        ret_code_5024count: int = None,
+        ret_code_5167count: int = None,
+        ret_code_5217count: int = None,
+        ret_code_6002count: int = None,
+        retry_count: float = None,
+        rpc_count: float = None,
+        server: str = None,
+        server_ip: str = None,
+        server_port: int = None,
+        sql_id: str = None,
+        sql_text_short: str = None,
+        sql_type: str = None,
+        strong_consistency_percentage: float = None,
+        sum_elapsed_time: float = None,
+        sum_logical_reads: float = None,
+        sum_wait_time: float = None,
+        table_scan_percentage: float = None,
+        total_wait_time: float = None,
+        user_name: str = None,
+        wait_event: str = None,
+        weak_consistency_percentage: float = None,
+    ):
+        self.avg_affected_rows = avg_affected_rows
+        self.avg_application_wait_time = avg_application_wait_time
+        self.avg_block_cache_hit = avg_block_cache_hit
+        self.avg_block_index_cache_hit = avg_block_index_cache_hit
+        self.avg_bloom_filter_cache_hit = avg_bloom_filter_cache_hit
+        self.avg_concurrency_wait_time = avg_concurrency_wait_time
+        self.avg_cpu_time = avg_cpu_time
+        self.avg_decode_time = avg_decode_time
+        self.avg_disk_reads = avg_disk_reads
+        self.avg_elapsed_time = avg_elapsed_time
+        self.avg_execute_time = avg_execute_time
+        self.avg_executor_rpc_count = avg_executor_rpc_count
+        self.avg_expected_worker_count = avg_expected_worker_count
+        self.avg_get_plan_time = avg_get_plan_time
+        self.avg_logical_reads = avg_logical_reads
+        self.avg_memstore_read_rows = avg_memstore_read_rows
+        self.avg_net_time = avg_net_time
+        self.avg_net_wait_time = avg_net_wait_time
+        self.avg_partition_count = avg_partition_count
+        self.avg_queue_time = avg_queue_time
+        self.avg_return_rows = avg_return_rows
+        self.avg_row_cache_hit = avg_row_cache_hit
+        self.avg_rpc_count = avg_rpc_count
+        self.avg_schedule_time = avg_schedule_time
+        self.avg_ssstore_read_rows = avg_ssstore_read_rows
+        self.avg_used_worker_count = avg_used_worker_count
+        self.avg_user_io_wait_time = avg_user_io_wait_time
+        self.avg_wait_count = avg_wait_count
+        self.avg_wait_time = avg_wait_time
+        self.client_ip = client_ip
+        self.db_name = db_name
+        self.dist_plan_percentage = dist_plan_percentage
+        self.exec_ps = exec_ps
+        self.executions = executions
+        self.fail_count = fail_count
+        self.fail_percentage = fail_percentage
+        self.inner = inner
+        self.local_plan_percentage = local_plan_percentage
+        self.max_affected_rows = max_affected_rows
+        self.max_application_wait_time = max_application_wait_time
+        self.max_concurrency_wait_time = max_concurrency_wait_time
+        self.max_cpu_time = max_cpu_time
+        self.max_disk_reads = max_disk_reads
+        self.max_elapsed_time = max_elapsed_time
+        self.max_return_rows = max_return_rows
+        self.max_user_io_wait_time = max_user_io_wait_time
+        self.max_wait_time = max_wait_time
+        self.miss_plan_percentage = miss_plan_percentage
+        self.miss_plans = miss_plans
+        self.remote_plan_percentage = remote_plan_percentage
+        self.remote_plans = remote_plans
+        self.ret_code_4012count = ret_code_4012count
+        self.ret_code_4013count = ret_code_4013count
+        self.ret_code_5001count = ret_code_5001count
+        self.ret_code_5024count = ret_code_5024count
+        self.ret_code_5167count = ret_code_5167count
+        self.ret_code_5217count = ret_code_5217count
+        self.ret_code_6002count = ret_code_6002count
+        self.retry_count = retry_count
+        self.rpc_count = rpc_count
+        self.server = server
+        self.server_ip = server_ip
+        self.server_port = server_port
+        # SQL ID。
+        self.sql_id = sql_id
+        self.sql_text_short = sql_text_short
+        self.sql_type = sql_type
+        self.strong_consistency_percentage = strong_consistency_percentage
+        self.sum_elapsed_time = sum_elapsed_time
+        self.sum_logical_reads = sum_logical_reads
+        self.sum_wait_time = sum_wait_time
+        self.table_scan_percentage = table_scan_percentage
+        self.total_wait_time = total_wait_time
+        self.user_name = user_name
+        self.wait_event = wait_event
+        self.weak_consistency_percentage = weak_consistency_percentage
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.avg_affected_rows is not None:
+            result['AvgAffectedRows'] = self.avg_affected_rows
+        if self.avg_application_wait_time is not None:
+            result['AvgApplicationWaitTime'] = self.avg_application_wait_time
+        if self.avg_block_cache_hit is not None:
+            result['AvgBlockCacheHit'] = self.avg_block_cache_hit
+        if self.avg_block_index_cache_hit is not None:
+            result['AvgBlockIndexCacheHit'] = self.avg_block_index_cache_hit
+        if self.avg_bloom_filter_cache_hit is not None:
+            result['AvgBloomFilterCacheHit'] = self.avg_bloom_filter_cache_hit
+        if self.avg_concurrency_wait_time is not None:
+            result['AvgConcurrencyWaitTime'] = self.avg_concurrency_wait_time
+        if self.avg_cpu_time is not None:
+            result['AvgCpuTime'] = self.avg_cpu_time
+        if self.avg_decode_time is not None:
+            result['AvgDecodeTime'] = self.avg_decode_time
+        if self.avg_disk_reads is not None:
+            result['AvgDiskReads'] = self.avg_disk_reads
+        if self.avg_elapsed_time is not None:
+            result['AvgElapsedTime'] = self.avg_elapsed_time
+        if self.avg_execute_time is not None:
+            result['AvgExecuteTime'] = self.avg_execute_time
+        if self.avg_executor_rpc_count is not None:
+            result['AvgExecutorRpcCount'] = self.avg_executor_rpc_count
+        if self.avg_expected_worker_count is not None:
+            result['AvgExpectedWorkerCount'] = self.avg_expected_worker_count
+        if self.avg_get_plan_time is not None:
+            result['AvgGetPlanTime'] = self.avg_get_plan_time
+        if self.avg_logical_reads is not None:
+            result['AvgLogicalReads'] = self.avg_logical_reads
+        if self.avg_memstore_read_rows is not None:
+            result['AvgMemstoreReadRows'] = self.avg_memstore_read_rows
+        if self.avg_net_time is not None:
+            result['AvgNetTime'] = self.avg_net_time
+        if self.avg_net_wait_time is not None:
+            result['AvgNetWaitTime'] = self.avg_net_wait_time
+        if self.avg_partition_count is not None:
+            result['AvgPartitionCount'] = self.avg_partition_count
+        if self.avg_queue_time is not None:
+            result['AvgQueueTime'] = self.avg_queue_time
+        if self.avg_return_rows is not None:
+            result['AvgReturnRows'] = self.avg_return_rows
+        if self.avg_row_cache_hit is not None:
+            result['AvgRowCacheHit'] = self.avg_row_cache_hit
+        if self.avg_rpc_count is not None:
+            result['AvgRpcCount'] = self.avg_rpc_count
+        if self.avg_schedule_time is not None:
+            result['AvgScheduleTime'] = self.avg_schedule_time
+        if self.avg_ssstore_read_rows is not None:
+            result['AvgSsstoreReadRows'] = self.avg_ssstore_read_rows
+        if self.avg_used_worker_count is not None:
+            result['AvgUsedWorkerCount'] = self.avg_used_worker_count
+        if self.avg_user_io_wait_time is not None:
+            result['AvgUserIoWaitTime'] = self.avg_user_io_wait_time
+        if self.avg_wait_count is not None:
+            result['AvgWaitCount'] = self.avg_wait_count
+        if self.avg_wait_time is not None:
+            result['AvgWaitTime'] = self.avg_wait_time
+        if self.client_ip is not None:
+            result['ClientIp'] = self.client_ip
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.dist_plan_percentage is not None:
+            result['DistPlanPercentage'] = self.dist_plan_percentage
+        if self.exec_ps is not None:
+            result['ExecPs'] = self.exec_ps
+        if self.executions is not None:
+            result['Executions'] = self.executions
+        if self.fail_count is not None:
+            result['FailCount'] = self.fail_count
+        if self.fail_percentage is not None:
+            result['FailPercentage'] = self.fail_percentage
+        if self.inner is not None:
+            result['Inner'] = self.inner
+        if self.local_plan_percentage is not None:
+            result['LocalPlanPercentage'] = self.local_plan_percentage
+        if self.max_affected_rows is not None:
+            result['MaxAffectedRows'] = self.max_affected_rows
+        if self.max_application_wait_time is not None:
+            result['MaxApplicationWaitTime'] = self.max_application_wait_time
+        if self.max_concurrency_wait_time is not None:
+            result['MaxConcurrencyWaitTime'] = self.max_concurrency_wait_time
+        if self.max_cpu_time is not None:
+            result['MaxCpuTime'] = self.max_cpu_time
+        if self.max_disk_reads is not None:
+            result['MaxDiskReads'] = self.max_disk_reads
+        if self.max_elapsed_time is not None:
+            result['MaxElapsedTime'] = self.max_elapsed_time
+        if self.max_return_rows is not None:
+            result['MaxReturnRows'] = self.max_return_rows
+        if self.max_user_io_wait_time is not None:
+            result['MaxUserIoWaitTime'] = self.max_user_io_wait_time
+        if self.max_wait_time is not None:
+            result['MaxWaitTime'] = self.max_wait_time
+        if self.miss_plan_percentage is not None:
+            result['MissPlanPercentage'] = self.miss_plan_percentage
+        if self.miss_plans is not None:
+            result['MissPlans'] = self.miss_plans
+        if self.remote_plan_percentage is not None:
+            result['RemotePlanPercentage'] = self.remote_plan_percentage
+        if self.remote_plans is not None:
+            result['RemotePlans'] = self.remote_plans
+        if self.ret_code_4012count is not None:
+            result['RetCode4012Count'] = self.ret_code_4012count
+        if self.ret_code_4013count is not None:
+            result['RetCode4013Count'] = self.ret_code_4013count
+        if self.ret_code_5001count is not None:
+            result['RetCode5001Count'] = self.ret_code_5001count
+        if self.ret_code_5024count is not None:
+            result['RetCode5024Count'] = self.ret_code_5024count
+        if self.ret_code_5167count is not None:
+            result['RetCode5167Count'] = self.ret_code_5167count
+        if self.ret_code_5217count is not None:
+            result['RetCode5217Count'] = self.ret_code_5217count
+        if self.ret_code_6002count is not None:
+            result['RetCode6002Count'] = self.ret_code_6002count
+        if self.retry_count is not None:
+            result['RetryCount'] = self.retry_count
+        if self.rpc_count is not None:
+            result['RpcCount'] = self.rpc_count
+        if self.server is not None:
+            result['Server'] = self.server
+        if self.server_ip is not None:
+            result['ServerIp'] = self.server_ip
+        if self.server_port is not None:
+            result['ServerPort'] = self.server_port
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_text_short is not None:
+            result['SqlTextShort'] = self.sql_text_short
+        if self.sql_type is not None:
+            result['SqlType'] = self.sql_type
+        if self.strong_consistency_percentage is not None:
+            result['StrongConsistencyPercentage'] = self.strong_consistency_percentage
+        if self.sum_elapsed_time is not None:
+            result['SumElapsedTime'] = self.sum_elapsed_time
+        if self.sum_logical_reads is not None:
+            result['SumLogicalReads'] = self.sum_logical_reads
+        if self.sum_wait_time is not None:
+            result['SumWaitTime'] = self.sum_wait_time
+        if self.table_scan_percentage is not None:
+            result['TableScanPercentage'] = self.table_scan_percentage
+        if self.total_wait_time is not None:
+            result['TotalWaitTime'] = self.total_wait_time
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        if self.wait_event is not None:
+            result['WaitEvent'] = self.wait_event
+        if self.weak_consistency_percentage is not None:
+            result['WeakConsistencyPercentage'] = self.weak_consistency_percentage
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AvgAffectedRows') is not None:
+            self.avg_affected_rows = m.get('AvgAffectedRows')
+        if m.get('AvgApplicationWaitTime') is not None:
+            self.avg_application_wait_time = m.get('AvgApplicationWaitTime')
+        if m.get('AvgBlockCacheHit') is not None:
+            self.avg_block_cache_hit = m.get('AvgBlockCacheHit')
+        if m.get('AvgBlockIndexCacheHit') is not None:
+            self.avg_block_index_cache_hit = m.get('AvgBlockIndexCacheHit')
+        if m.get('AvgBloomFilterCacheHit') is not None:
+            self.avg_bloom_filter_cache_hit = m.get('AvgBloomFilterCacheHit')
+        if m.get('AvgConcurrencyWaitTime') is not None:
+            self.avg_concurrency_wait_time = m.get('AvgConcurrencyWaitTime')
+        if m.get('AvgCpuTime') is not None:
+            self.avg_cpu_time = m.get('AvgCpuTime')
+        if m.get('AvgDecodeTime') is not None:
+            self.avg_decode_time = m.get('AvgDecodeTime')
+        if m.get('AvgDiskReads') is not None:
+            self.avg_disk_reads = m.get('AvgDiskReads')
+        if m.get('AvgElapsedTime') is not None:
+            self.avg_elapsed_time = m.get('AvgElapsedTime')
+        if m.get('AvgExecuteTime') is not None:
+            self.avg_execute_time = m.get('AvgExecuteTime')
+        if m.get('AvgExecutorRpcCount') is not None:
+            self.avg_executor_rpc_count = m.get('AvgExecutorRpcCount')
+        if m.get('AvgExpectedWorkerCount') is not None:
+            self.avg_expected_worker_count = m.get('AvgExpectedWorkerCount')
+        if m.get('AvgGetPlanTime') is not None:
+            self.avg_get_plan_time = m.get('AvgGetPlanTime')
+        if m.get('AvgLogicalReads') is not None:
+            self.avg_logical_reads = m.get('AvgLogicalReads')
+        if m.get('AvgMemstoreReadRows') is not None:
+            self.avg_memstore_read_rows = m.get('AvgMemstoreReadRows')
+        if m.get('AvgNetTime') is not None:
+            self.avg_net_time = m.get('AvgNetTime')
+        if m.get('AvgNetWaitTime') is not None:
+            self.avg_net_wait_time = m.get('AvgNetWaitTime')
+        if m.get('AvgPartitionCount') is not None:
+            self.avg_partition_count = m.get('AvgPartitionCount')
+        if m.get('AvgQueueTime') is not None:
+            self.avg_queue_time = m.get('AvgQueueTime')
+        if m.get('AvgReturnRows') is not None:
+            self.avg_return_rows = m.get('AvgReturnRows')
+        if m.get('AvgRowCacheHit') is not None:
+            self.avg_row_cache_hit = m.get('AvgRowCacheHit')
+        if m.get('AvgRpcCount') is not None:
+            self.avg_rpc_count = m.get('AvgRpcCount')
+        if m.get('AvgScheduleTime') is not None:
+            self.avg_schedule_time = m.get('AvgScheduleTime')
+        if m.get('AvgSsstoreReadRows') is not None:
+            self.avg_ssstore_read_rows = m.get('AvgSsstoreReadRows')
+        if m.get('AvgUsedWorkerCount') is not None:
+            self.avg_used_worker_count = m.get('AvgUsedWorkerCount')
+        if m.get('AvgUserIoWaitTime') is not None:
+            self.avg_user_io_wait_time = m.get('AvgUserIoWaitTime')
+        if m.get('AvgWaitCount') is not None:
+            self.avg_wait_count = m.get('AvgWaitCount')
+        if m.get('AvgWaitTime') is not None:
+            self.avg_wait_time = m.get('AvgWaitTime')
+        if m.get('ClientIp') is not None:
+            self.client_ip = m.get('ClientIp')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('DistPlanPercentage') is not None:
+            self.dist_plan_percentage = m.get('DistPlanPercentage')
+        if m.get('ExecPs') is not None:
+            self.exec_ps = m.get('ExecPs')
+        if m.get('Executions') is not None:
+            self.executions = m.get('Executions')
+        if m.get('FailCount') is not None:
+            self.fail_count = m.get('FailCount')
+        if m.get('FailPercentage') is not None:
+            self.fail_percentage = m.get('FailPercentage')
+        if m.get('Inner') is not None:
+            self.inner = m.get('Inner')
+        if m.get('LocalPlanPercentage') is not None:
+            self.local_plan_percentage = m.get('LocalPlanPercentage')
+        if m.get('MaxAffectedRows') is not None:
+            self.max_affected_rows = m.get('MaxAffectedRows')
+        if m.get('MaxApplicationWaitTime') is not None:
+            self.max_application_wait_time = m.get('MaxApplicationWaitTime')
+        if m.get('MaxConcurrencyWaitTime') is not None:
+            self.max_concurrency_wait_time = m.get('MaxConcurrencyWaitTime')
+        if m.get('MaxCpuTime') is not None:
+            self.max_cpu_time = m.get('MaxCpuTime')
+        if m.get('MaxDiskReads') is not None:
+            self.max_disk_reads = m.get('MaxDiskReads')
+        if m.get('MaxElapsedTime') is not None:
+            self.max_elapsed_time = m.get('MaxElapsedTime')
+        if m.get('MaxReturnRows') is not None:
+            self.max_return_rows = m.get('MaxReturnRows')
+        if m.get('MaxUserIoWaitTime') is not None:
+            self.max_user_io_wait_time = m.get('MaxUserIoWaitTime')
+        if m.get('MaxWaitTime') is not None:
+            self.max_wait_time = m.get('MaxWaitTime')
+        if m.get('MissPlanPercentage') is not None:
+            self.miss_plan_percentage = m.get('MissPlanPercentage')
+        if m.get('MissPlans') is not None:
+            self.miss_plans = m.get('MissPlans')
+        if m.get('RemotePlanPercentage') is not None:
+            self.remote_plan_percentage = m.get('RemotePlanPercentage')
+        if m.get('RemotePlans') is not None:
+            self.remote_plans = m.get('RemotePlans')
+        if m.get('RetCode4012Count') is not None:
+            self.ret_code_4012count = m.get('RetCode4012Count')
+        if m.get('RetCode4013Count') is not None:
+            self.ret_code_4013count = m.get('RetCode4013Count')
+        if m.get('RetCode5001Count') is not None:
+            self.ret_code_5001count = m.get('RetCode5001Count')
+        if m.get('RetCode5024Count') is not None:
+            self.ret_code_5024count = m.get('RetCode5024Count')
+        if m.get('RetCode5167Count') is not None:
+            self.ret_code_5167count = m.get('RetCode5167Count')
+        if m.get('RetCode5217Count') is not None:
+            self.ret_code_5217count = m.get('RetCode5217Count')
+        if m.get('RetCode6002Count') is not None:
+            self.ret_code_6002count = m.get('RetCode6002Count')
+        if m.get('RetryCount') is not None:
+            self.retry_count = m.get('RetryCount')
+        if m.get('RpcCount') is not None:
+            self.rpc_count = m.get('RpcCount')
+        if m.get('Server') is not None:
+            self.server = m.get('Server')
+        if m.get('ServerIp') is not None:
+            self.server_ip = m.get('ServerIp')
+        if m.get('ServerPort') is not None:
+            self.server_port = m.get('ServerPort')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlTextShort') is not None:
+            self.sql_text_short = m.get('SqlTextShort')
+        if m.get('SqlType') is not None:
+            self.sql_type = m.get('SqlType')
+        if m.get('StrongConsistencyPercentage') is not None:
+            self.strong_consistency_percentage = m.get('StrongConsistencyPercentage')
+        if m.get('SumElapsedTime') is not None:
+            self.sum_elapsed_time = m.get('SumElapsedTime')
+        if m.get('SumLogicalReads') is not None:
+            self.sum_logical_reads = m.get('SumLogicalReads')
+        if m.get('SumWaitTime') is not None:
+            self.sum_wait_time = m.get('SumWaitTime')
+        if m.get('TableScanPercentage') is not None:
+            self.table_scan_percentage = m.get('TableScanPercentage')
+        if m.get('TotalWaitTime') is not None:
+            self.total_wait_time = m.get('TotalWaitTime')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        if m.get('WaitEvent') is not None:
+            self.wait_event = m.get('WaitEvent')
+        if m.get('WeakConsistencyPercentage') is not None:
+            self.weak_consistency_percentage = m.get('WeakConsistencyPercentage')
+        return self
+
+
+class DescribeOasSlowSQLListResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: List[DescribeOasSlowSQLListResponseBodyData] = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = DescribeOasSlowSQLListResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeOasSlowSQLListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeOasSlowSQLListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeOasSlowSQLListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
+class DescribeOasTopSQLListRequest(TeaModel):
+    def __init__(
+        self,
+        accept_language: str = None,
+        db_name: str = None,
+        end_time: str = None,
+        filter_condition: str = None,
+        instance_id: str = None,
+        node_ip: str = None,
+        search_key_word: str = None,
+        search_param: str = None,
+        search_rule: str = None,
+        search_value: str = None,
+        sql_id: str = None,
+        sql_text_length: int = None,
+        start_time: str = None,
+        tenant_id: str = None,
+    ):
+        self.accept_language = accept_language
+        self.db_name = db_name
+        self.end_time = end_time
+        self.filter_condition = filter_condition
+        self.instance_id = instance_id
+        self.node_ip = node_ip
+        self.search_key_word = search_key_word
+        self.search_param = search_param
+        self.search_rule = search_rule
+        self.search_value = search_value
+        self.sql_id = sql_id
+        self.sql_text_length = sql_text_length
+        self.start_time = start_time
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.accept_language is not None:
+            result['AcceptLanguage'] = self.accept_language
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.filter_condition is not None:
+            result['FilterCondition'] = self.filter_condition
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.node_ip is not None:
+            result['NodeIp'] = self.node_ip
+        if self.search_key_word is not None:
+            result['SearchKeyWord'] = self.search_key_word
+        if self.search_param is not None:
+            result['SearchParam'] = self.search_param
+        if self.search_rule is not None:
+            result['SearchRule'] = self.search_rule
+        if self.search_value is not None:
+            result['SearchValue'] = self.search_value
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_text_length is not None:
+            result['SqlTextLength'] = self.sql_text_length
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AcceptLanguage') is not None:
+            self.accept_language = m.get('AcceptLanguage')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('FilterCondition') is not None:
+            self.filter_condition = m.get('FilterCondition')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('NodeIp') is not None:
+            self.node_ip = m.get('NodeIp')
+        if m.get('SearchKeyWord') is not None:
+            self.search_key_word = m.get('SearchKeyWord')
+        if m.get('SearchParam') is not None:
+            self.search_param = m.get('SearchParam')
+        if m.get('SearchRule') is not None:
+            self.search_rule = m.get('SearchRule')
+        if m.get('SearchValue') is not None:
+            self.search_value = m.get('SearchValue')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlTextLength') is not None:
+            self.sql_text_length = m.get('SqlTextLength')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DescribeOasTopSQLListResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        avg_affected_rows: float = None,
+        avg_application_wait_time: float = None,
+        avg_block_cache_hit: float = None,
+        avg_block_index_cache_hit: float = None,
+        avg_bloom_filter_cache_hit: float = None,
+        avg_concurrency_wait_time: float = None,
+        avg_cpu_time: float = None,
+        avg_decode_time: float = None,
+        avg_disk_reads: float = None,
+        avg_elapsed_time: float = None,
+        avg_execute_time: float = None,
+        avg_executor_rpc_count: float = None,
+        avg_expected_worker_count: float = None,
+        avg_get_plan_time: float = None,
+        avg_logical_reads: float = None,
+        avg_memstore_read_rows: float = None,
+        avg_net_time: float = None,
+        avg_net_wait_time: float = None,
+        avg_partition_count: float = None,
+        avg_queue_time: float = None,
+        avg_return_rows: float = None,
+        avg_row_cache_hit: float = None,
+        avg_rpc_count: float = None,
+        avg_schedule_time: float = None,
+        avg_ssstore_read_rows: float = None,
+        avg_used_worker_count: float = None,
+        avg_user_io_wait_time: float = None,
+        avg_wait_count: float = None,
+        avg_wait_time: float = None,
+        client_ip: str = None,
+        cpu_percentage: float = None,
+        db_name: str = None,
+        dist_plan_percentage: float = None,
+        exec_ps: float = None,
+        executions: float = None,
+        fail_count: float = None,
+        fail_percentage: float = None,
+        inner: bool = None,
+        local_plan_percentage: float = None,
+        max_affected_rows: float = None,
+        max_application_wait_time: float = None,
+        max_concurrency_wait_time: float = None,
+        max_cpu_time: float = None,
+        max_disk_reads: float = None,
+        max_elapsed_time: float = None,
+        max_return_rows: float = None,
+        max_user_io_wait_time: float = None,
+        max_wait_time: float = None,
+        miss_plan_percentage: float = None,
+        miss_plans: float = None,
+        remote_plan_percentage: float = None,
+        remote_plans: float = None,
+        ret_code_4012count: int = None,
+        ret_code_4013count: int = None,
+        ret_code_5001count: int = None,
+        ret_code_5024count: int = None,
+        ret_code_5167count: int = None,
+        ret_code_5217count: int = None,
+        ret_code_6002count: int = None,
+        retry_count: float = None,
+        rpc_count: float = None,
+        server: str = None,
+        server_ip: str = None,
+        server_port: int = None,
+        sql_id: str = None,
+        sql_text_short: str = None,
+        sql_type: str = None,
+        strong_consistency_percentage: float = None,
+        sum_elapsed_time: float = None,
+        sum_logical_reads: float = None,
+        sum_wait_time: float = None,
+        table_scan_percentage: float = None,
+        total_wait_time: float = None,
+        user_name: str = None,
+        wait_event: str = None,
+        weak_consistency_percentage: float = None,
+    ):
+        self.avg_affected_rows = avg_affected_rows
+        self.avg_application_wait_time = avg_application_wait_time
+        self.avg_block_cache_hit = avg_block_cache_hit
+        self.avg_block_index_cache_hit = avg_block_index_cache_hit
+        self.avg_bloom_filter_cache_hit = avg_bloom_filter_cache_hit
+        self.avg_concurrency_wait_time = avg_concurrency_wait_time
+        self.avg_cpu_time = avg_cpu_time
+        self.avg_decode_time = avg_decode_time
+        self.avg_disk_reads = avg_disk_reads
+        self.avg_elapsed_time = avg_elapsed_time
+        self.avg_execute_time = avg_execute_time
+        self.avg_executor_rpc_count = avg_executor_rpc_count
+        self.avg_expected_worker_count = avg_expected_worker_count
+        self.avg_get_plan_time = avg_get_plan_time
+        self.avg_logical_reads = avg_logical_reads
+        self.avg_memstore_read_rows = avg_memstore_read_rows
+        self.avg_net_time = avg_net_time
+        self.avg_net_wait_time = avg_net_wait_time
+        self.avg_partition_count = avg_partition_count
+        self.avg_queue_time = avg_queue_time
+        self.avg_return_rows = avg_return_rows
+        self.avg_row_cache_hit = avg_row_cache_hit
+        self.avg_rpc_count = avg_rpc_count
+        self.avg_schedule_time = avg_schedule_time
+        self.avg_ssstore_read_rows = avg_ssstore_read_rows
+        self.avg_used_worker_count = avg_used_worker_count
+        self.avg_user_io_wait_time = avg_user_io_wait_time
+        self.avg_wait_count = avg_wait_count
+        self.avg_wait_time = avg_wait_time
+        self.client_ip = client_ip
+        self.cpu_percentage = cpu_percentage
+        self.db_name = db_name
+        self.dist_plan_percentage = dist_plan_percentage
+        self.exec_ps = exec_ps
+        self.executions = executions
+        self.fail_count = fail_count
+        self.fail_percentage = fail_percentage
+        self.inner = inner
+        self.local_plan_percentage = local_plan_percentage
+        self.max_affected_rows = max_affected_rows
+        self.max_application_wait_time = max_application_wait_time
+        self.max_concurrency_wait_time = max_concurrency_wait_time
+        self.max_cpu_time = max_cpu_time
+        self.max_disk_reads = max_disk_reads
+        self.max_elapsed_time = max_elapsed_time
+        self.max_return_rows = max_return_rows
+        self.max_user_io_wait_time = max_user_io_wait_time
+        self.max_wait_time = max_wait_time
+        self.miss_plan_percentage = miss_plan_percentage
+        self.miss_plans = miss_plans
+        self.remote_plan_percentage = remote_plan_percentage
+        self.remote_plans = remote_plans
+        self.ret_code_4012count = ret_code_4012count
+        self.ret_code_4013count = ret_code_4013count
+        self.ret_code_5001count = ret_code_5001count
+        self.ret_code_5024count = ret_code_5024count
+        self.ret_code_5167count = ret_code_5167count
+        self.ret_code_5217count = ret_code_5217count
+        self.ret_code_6002count = ret_code_6002count
+        self.retry_count = retry_count
+        self.rpc_count = rpc_count
+        self.server = server
+        self.server_ip = server_ip
+        self.server_port = server_port
+        # SQL ID。
+        self.sql_id = sql_id
+        self.sql_text_short = sql_text_short
+        self.sql_type = sql_type
+        self.strong_consistency_percentage = strong_consistency_percentage
+        self.sum_elapsed_time = sum_elapsed_time
+        self.sum_logical_reads = sum_logical_reads
+        self.sum_wait_time = sum_wait_time
+        self.table_scan_percentage = table_scan_percentage
+        self.total_wait_time = total_wait_time
+        self.user_name = user_name
+        self.wait_event = wait_event
+        self.weak_consistency_percentage = weak_consistency_percentage
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.avg_affected_rows is not None:
+            result['AvgAffectedRows'] = self.avg_affected_rows
+        if self.avg_application_wait_time is not None:
+            result['AvgApplicationWaitTime'] = self.avg_application_wait_time
+        if self.avg_block_cache_hit is not None:
+            result['AvgBlockCacheHit'] = self.avg_block_cache_hit
+        if self.avg_block_index_cache_hit is not None:
+            result['AvgBlockIndexCacheHit'] = self.avg_block_index_cache_hit
+        if self.avg_bloom_filter_cache_hit is not None:
+            result['AvgBloomFilterCacheHit'] = self.avg_bloom_filter_cache_hit
+        if self.avg_concurrency_wait_time is not None:
+            result['AvgConcurrencyWaitTime'] = self.avg_concurrency_wait_time
+        if self.avg_cpu_time is not None:
+            result['AvgCpuTime'] = self.avg_cpu_time
+        if self.avg_decode_time is not None:
+            result['AvgDecodeTime'] = self.avg_decode_time
+        if self.avg_disk_reads is not None:
+            result['AvgDiskReads'] = self.avg_disk_reads
+        if self.avg_elapsed_time is not None:
+            result['AvgElapsedTime'] = self.avg_elapsed_time
+        if self.avg_execute_time is not None:
+            result['AvgExecuteTime'] = self.avg_execute_time
+        if self.avg_executor_rpc_count is not None:
+            result['AvgExecutorRpcCount'] = self.avg_executor_rpc_count
+        if self.avg_expected_worker_count is not None:
+            result['AvgExpectedWorkerCount'] = self.avg_expected_worker_count
+        if self.avg_get_plan_time is not None:
+            result['AvgGetPlanTime'] = self.avg_get_plan_time
+        if self.avg_logical_reads is not None:
+            result['AvgLogicalReads'] = self.avg_logical_reads
+        if self.avg_memstore_read_rows is not None:
+            result['AvgMemstoreReadRows'] = self.avg_memstore_read_rows
+        if self.avg_net_time is not None:
+            result['AvgNetTime'] = self.avg_net_time
+        if self.avg_net_wait_time is not None:
+            result['AvgNetWaitTime'] = self.avg_net_wait_time
+        if self.avg_partition_count is not None:
+            result['AvgPartitionCount'] = self.avg_partition_count
+        if self.avg_queue_time is not None:
+            result['AvgQueueTime'] = self.avg_queue_time
+        if self.avg_return_rows is not None:
+            result['AvgReturnRows'] = self.avg_return_rows
+        if self.avg_row_cache_hit is not None:
+            result['AvgRowCacheHit'] = self.avg_row_cache_hit
+        if self.avg_rpc_count is not None:
+            result['AvgRpcCount'] = self.avg_rpc_count
+        if self.avg_schedule_time is not None:
+            result['AvgScheduleTime'] = self.avg_schedule_time
+        if self.avg_ssstore_read_rows is not None:
+            result['AvgSsstoreReadRows'] = self.avg_ssstore_read_rows
+        if self.avg_used_worker_count is not None:
+            result['AvgUsedWorkerCount'] = self.avg_used_worker_count
+        if self.avg_user_io_wait_time is not None:
+            result['AvgUserIoWaitTime'] = self.avg_user_io_wait_time
+        if self.avg_wait_count is not None:
+            result['AvgWaitCount'] = self.avg_wait_count
+        if self.avg_wait_time is not None:
+            result['AvgWaitTime'] = self.avg_wait_time
+        if self.client_ip is not None:
+            result['ClientIp'] = self.client_ip
+        if self.cpu_percentage is not None:
+            result['CpuPercentage'] = self.cpu_percentage
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.dist_plan_percentage is not None:
+            result['DistPlanPercentage'] = self.dist_plan_percentage
+        if self.exec_ps is not None:
+            result['ExecPs'] = self.exec_ps
+        if self.executions is not None:
+            result['Executions'] = self.executions
+        if self.fail_count is not None:
+            result['FailCount'] = self.fail_count
+        if self.fail_percentage is not None:
+            result['FailPercentage'] = self.fail_percentage
+        if self.inner is not None:
+            result['Inner'] = self.inner
+        if self.local_plan_percentage is not None:
+            result['LocalPlanPercentage'] = self.local_plan_percentage
+        if self.max_affected_rows is not None:
+            result['MaxAffectedRows'] = self.max_affected_rows
+        if self.max_application_wait_time is not None:
+            result['MaxApplicationWaitTime'] = self.max_application_wait_time
+        if self.max_concurrency_wait_time is not None:
+            result['MaxConcurrencyWaitTime'] = self.max_concurrency_wait_time
+        if self.max_cpu_time is not None:
+            result['MaxCpuTime'] = self.max_cpu_time
+        if self.max_disk_reads is not None:
+            result['MaxDiskReads'] = self.max_disk_reads
+        if self.max_elapsed_time is not None:
+            result['MaxElapsedTime'] = self.max_elapsed_time
+        if self.max_return_rows is not None:
+            result['MaxReturnRows'] = self.max_return_rows
+        if self.max_user_io_wait_time is not None:
+            result['MaxUserIoWaitTime'] = self.max_user_io_wait_time
+        if self.max_wait_time is not None:
+            result['MaxWaitTime'] = self.max_wait_time
+        if self.miss_plan_percentage is not None:
+            result['MissPlanPercentage'] = self.miss_plan_percentage
+        if self.miss_plans is not None:
+            result['MissPlans'] = self.miss_plans
+        if self.remote_plan_percentage is not None:
+            result['RemotePlanPercentage'] = self.remote_plan_percentage
+        if self.remote_plans is not None:
+            result['RemotePlans'] = self.remote_plans
+        if self.ret_code_4012count is not None:
+            result['RetCode4012Count'] = self.ret_code_4012count
+        if self.ret_code_4013count is not None:
+            result['RetCode4013Count'] = self.ret_code_4013count
+        if self.ret_code_5001count is not None:
+            result['RetCode5001Count'] = self.ret_code_5001count
+        if self.ret_code_5024count is not None:
+            result['RetCode5024Count'] = self.ret_code_5024count
+        if self.ret_code_5167count is not None:
+            result['RetCode5167Count'] = self.ret_code_5167count
+        if self.ret_code_5217count is not None:
+            result['RetCode5217Count'] = self.ret_code_5217count
+        if self.ret_code_6002count is not None:
+            result['RetCode6002Count'] = self.ret_code_6002count
+        if self.retry_count is not None:
+            result['RetryCount'] = self.retry_count
+        if self.rpc_count is not None:
+            result['RpcCount'] = self.rpc_count
+        if self.server is not None:
+            result['Server'] = self.server
+        if self.server_ip is not None:
+            result['ServerIp'] = self.server_ip
+        if self.server_port is not None:
+            result['ServerPort'] = self.server_port
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.sql_text_short is not None:
+            result['SqlTextShort'] = self.sql_text_short
+        if self.sql_type is not None:
+            result['SqlType'] = self.sql_type
+        if self.strong_consistency_percentage is not None:
+            result['StrongConsistencyPercentage'] = self.strong_consistency_percentage
+        if self.sum_elapsed_time is not None:
+            result['SumElapsedTime'] = self.sum_elapsed_time
+        if self.sum_logical_reads is not None:
+            result['SumLogicalReads'] = self.sum_logical_reads
+        if self.sum_wait_time is not None:
+            result['SumWaitTime'] = self.sum_wait_time
+        if self.table_scan_percentage is not None:
+            result['TableScanPercentage'] = self.table_scan_percentage
+        if self.total_wait_time is not None:
+            result['TotalWaitTime'] = self.total_wait_time
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        if self.wait_event is not None:
+            result['WaitEvent'] = self.wait_event
+        if self.weak_consistency_percentage is not None:
+            result['WeakConsistencyPercentage'] = self.weak_consistency_percentage
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AvgAffectedRows') is not None:
+            self.avg_affected_rows = m.get('AvgAffectedRows')
+        if m.get('AvgApplicationWaitTime') is not None:
+            self.avg_application_wait_time = m.get('AvgApplicationWaitTime')
+        if m.get('AvgBlockCacheHit') is not None:
+            self.avg_block_cache_hit = m.get('AvgBlockCacheHit')
+        if m.get('AvgBlockIndexCacheHit') is not None:
+            self.avg_block_index_cache_hit = m.get('AvgBlockIndexCacheHit')
+        if m.get('AvgBloomFilterCacheHit') is not None:
+            self.avg_bloom_filter_cache_hit = m.get('AvgBloomFilterCacheHit')
+        if m.get('AvgConcurrencyWaitTime') is not None:
+            self.avg_concurrency_wait_time = m.get('AvgConcurrencyWaitTime')
+        if m.get('AvgCpuTime') is not None:
+            self.avg_cpu_time = m.get('AvgCpuTime')
+        if m.get('AvgDecodeTime') is not None:
+            self.avg_decode_time = m.get('AvgDecodeTime')
+        if m.get('AvgDiskReads') is not None:
+            self.avg_disk_reads = m.get('AvgDiskReads')
+        if m.get('AvgElapsedTime') is not None:
+            self.avg_elapsed_time = m.get('AvgElapsedTime')
+        if m.get('AvgExecuteTime') is not None:
+            self.avg_execute_time = m.get('AvgExecuteTime')
+        if m.get('AvgExecutorRpcCount') is not None:
+            self.avg_executor_rpc_count = m.get('AvgExecutorRpcCount')
+        if m.get('AvgExpectedWorkerCount') is not None:
+            self.avg_expected_worker_count = m.get('AvgExpectedWorkerCount')
+        if m.get('AvgGetPlanTime') is not None:
+            self.avg_get_plan_time = m.get('AvgGetPlanTime')
+        if m.get('AvgLogicalReads') is not None:
+            self.avg_logical_reads = m.get('AvgLogicalReads')
+        if m.get('AvgMemstoreReadRows') is not None:
+            self.avg_memstore_read_rows = m.get('AvgMemstoreReadRows')
+        if m.get('AvgNetTime') is not None:
+            self.avg_net_time = m.get('AvgNetTime')
+        if m.get('AvgNetWaitTime') is not None:
+            self.avg_net_wait_time = m.get('AvgNetWaitTime')
+        if m.get('AvgPartitionCount') is not None:
+            self.avg_partition_count = m.get('AvgPartitionCount')
+        if m.get('AvgQueueTime') is not None:
+            self.avg_queue_time = m.get('AvgQueueTime')
+        if m.get('AvgReturnRows') is not None:
+            self.avg_return_rows = m.get('AvgReturnRows')
+        if m.get('AvgRowCacheHit') is not None:
+            self.avg_row_cache_hit = m.get('AvgRowCacheHit')
+        if m.get('AvgRpcCount') is not None:
+            self.avg_rpc_count = m.get('AvgRpcCount')
+        if m.get('AvgScheduleTime') is not None:
+            self.avg_schedule_time = m.get('AvgScheduleTime')
+        if m.get('AvgSsstoreReadRows') is not None:
+            self.avg_ssstore_read_rows = m.get('AvgSsstoreReadRows')
+        if m.get('AvgUsedWorkerCount') is not None:
+            self.avg_used_worker_count = m.get('AvgUsedWorkerCount')
+        if m.get('AvgUserIoWaitTime') is not None:
+            self.avg_user_io_wait_time = m.get('AvgUserIoWaitTime')
+        if m.get('AvgWaitCount') is not None:
+            self.avg_wait_count = m.get('AvgWaitCount')
+        if m.get('AvgWaitTime') is not None:
+            self.avg_wait_time = m.get('AvgWaitTime')
+        if m.get('ClientIp') is not None:
+            self.client_ip = m.get('ClientIp')
+        if m.get('CpuPercentage') is not None:
+            self.cpu_percentage = m.get('CpuPercentage')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('DistPlanPercentage') is not None:
+            self.dist_plan_percentage = m.get('DistPlanPercentage')
+        if m.get('ExecPs') is not None:
+            self.exec_ps = m.get('ExecPs')
+        if m.get('Executions') is not None:
+            self.executions = m.get('Executions')
+        if m.get('FailCount') is not None:
+            self.fail_count = m.get('FailCount')
+        if m.get('FailPercentage') is not None:
+            self.fail_percentage = m.get('FailPercentage')
+        if m.get('Inner') is not None:
+            self.inner = m.get('Inner')
+        if m.get('LocalPlanPercentage') is not None:
+            self.local_plan_percentage = m.get('LocalPlanPercentage')
+        if m.get('MaxAffectedRows') is not None:
+            self.max_affected_rows = m.get('MaxAffectedRows')
+        if m.get('MaxApplicationWaitTime') is not None:
+            self.max_application_wait_time = m.get('MaxApplicationWaitTime')
+        if m.get('MaxConcurrencyWaitTime') is not None:
+            self.max_concurrency_wait_time = m.get('MaxConcurrencyWaitTime')
+        if m.get('MaxCpuTime') is not None:
+            self.max_cpu_time = m.get('MaxCpuTime')
+        if m.get('MaxDiskReads') is not None:
+            self.max_disk_reads = m.get('MaxDiskReads')
+        if m.get('MaxElapsedTime') is not None:
+            self.max_elapsed_time = m.get('MaxElapsedTime')
+        if m.get('MaxReturnRows') is not None:
+            self.max_return_rows = m.get('MaxReturnRows')
+        if m.get('MaxUserIoWaitTime') is not None:
+            self.max_user_io_wait_time = m.get('MaxUserIoWaitTime')
+        if m.get('MaxWaitTime') is not None:
+            self.max_wait_time = m.get('MaxWaitTime')
+        if m.get('MissPlanPercentage') is not None:
+            self.miss_plan_percentage = m.get('MissPlanPercentage')
+        if m.get('MissPlans') is not None:
+            self.miss_plans = m.get('MissPlans')
+        if m.get('RemotePlanPercentage') is not None:
+            self.remote_plan_percentage = m.get('RemotePlanPercentage')
+        if m.get('RemotePlans') is not None:
+            self.remote_plans = m.get('RemotePlans')
+        if m.get('RetCode4012Count') is not None:
+            self.ret_code_4012count = m.get('RetCode4012Count')
+        if m.get('RetCode4013Count') is not None:
+            self.ret_code_4013count = m.get('RetCode4013Count')
+        if m.get('RetCode5001Count') is not None:
+            self.ret_code_5001count = m.get('RetCode5001Count')
+        if m.get('RetCode5024Count') is not None:
+            self.ret_code_5024count = m.get('RetCode5024Count')
+        if m.get('RetCode5167Count') is not None:
+            self.ret_code_5167count = m.get('RetCode5167Count')
+        if m.get('RetCode5217Count') is not None:
+            self.ret_code_5217count = m.get('RetCode5217Count')
+        if m.get('RetCode6002Count') is not None:
+            self.ret_code_6002count = m.get('RetCode6002Count')
+        if m.get('RetryCount') is not None:
+            self.retry_count = m.get('RetryCount')
+        if m.get('RpcCount') is not None:
+            self.rpc_count = m.get('RpcCount')
+        if m.get('Server') is not None:
+            self.server = m.get('Server')
+        if m.get('ServerIp') is not None:
+            self.server_ip = m.get('ServerIp')
+        if m.get('ServerPort') is not None:
+            self.server_port = m.get('ServerPort')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('SqlTextShort') is not None:
+            self.sql_text_short = m.get('SqlTextShort')
+        if m.get('SqlType') is not None:
+            self.sql_type = m.get('SqlType')
+        if m.get('StrongConsistencyPercentage') is not None:
+            self.strong_consistency_percentage = m.get('StrongConsistencyPercentage')
+        if m.get('SumElapsedTime') is not None:
+            self.sum_elapsed_time = m.get('SumElapsedTime')
+        if m.get('SumLogicalReads') is not None:
+            self.sum_logical_reads = m.get('SumLogicalReads')
+        if m.get('SumWaitTime') is not None:
+            self.sum_wait_time = m.get('SumWaitTime')
+        if m.get('TableScanPercentage') is not None:
+            self.table_scan_percentage = m.get('TableScanPercentage')
+        if m.get('TotalWaitTime') is not None:
+            self.total_wait_time = m.get('TotalWaitTime')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        if m.get('WaitEvent') is not None:
+            self.wait_event = m.get('WaitEvent')
+        if m.get('WeakConsistencyPercentage') is not None:
+            self.weak_consistency_percentage = m.get('WeakConsistencyPercentage')
+        return self
+
+
+class DescribeOasTopSQLListResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: List[DescribeOasTopSQLListResponseBodyData] = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = DescribeOasTopSQLListResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeOasTopSQLListResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeOasTopSQLListResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeOasTopSQLListResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeOmsOpenAPIProjectRequest(TeaModel):
     def __init__(
         self,
         page_number: int = None,
         page_size: int = None,
         project_id: str = None,
         worker_grade_id: str = None,
@@ -11058,14 +14315,486 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSQLPlansResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeSQLSamplesRequest(TeaModel):
+    def __init__(
+        self,
+        db_name: str = None,
+        end_time: str = None,
+        instance_id: str = None,
+        sql_id: str = None,
+        start_time: str = None,
+        tenant_id: str = None,
+    ):
+        self.db_name = db_name
+        self.end_time = end_time
+        self.instance_id = instance_id
+        # SQL ID。
+        self.sql_id = sql_id
+        self.start_time = start_time
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.end_time is not None:
+            result['EndTime'] = self.end_time
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.sql_id is not None:
+            result['SqlId'] = self.sql_id
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('EndTime') is not None:
+            self.end_time = m.get('EndTime')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SqlId') is not None:
+            self.sql_id = m.get('SqlId')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DescribeSQLSamplesResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        affected_rows: float = None,
+        application_wait_time: float = None,
+        block_cache_hit: float = None,
+        block_index_cache_hit: float = None,
+        bloom_filter_cache_hit: float = None,
+        client_ip: str = None,
+        client_port: str = None,
+        concurrency_wait_time: float = None,
+        consistency_level: str = None,
+        cpu_time: float = None,
+        db_name: str = None,
+        decode_time: float = None,
+        disk_reads: float = None,
+        elapsed_time: float = None,
+        execute_time: float = None,
+        executor_rpc: float = None,
+        expected_worker_count: float = None,
+        get_plan_time: float = None,
+        hit_plan: float = None,
+        inner: bool = None,
+        memstore_read_rows: float = None,
+        net_time: float = None,
+        net_wait_time: float = None,
+        ob_db_id: float = None,
+        ob_server_id: float = None,
+        ob_user_id: float = None,
+        partition_count: float = None,
+        plan_id: float = None,
+        plan_type: str = None,
+        queue_time: float = None,
+        request_id: str = None,
+        request_time: str = None,
+        ret_code: float = None,
+        retry_count: float = None,
+        return_rows: float = None,
+        row_cache_hit: float = None,
+        rpc_count: float = None,
+        schedule_time: float = None,
+        server: str = None,
+        sql_type: str = None,
+        ssstore_read_rows: float = None,
+        statement: str = None,
+        table_scan: float = None,
+        trace_id: str = None,
+        trans_hash: str = None,
+        used_worker_count: float = None,
+        user_io_wait_time: float = None,
+        user_name: str = None,
+        wait_count: float = None,
+        wait_event: str = None,
+        wait_time: float = None,
+    ):
+        self.affected_rows = affected_rows
+        self.application_wait_time = application_wait_time
+        self.block_cache_hit = block_cache_hit
+        self.block_index_cache_hit = block_index_cache_hit
+        self.bloom_filter_cache_hit = bloom_filter_cache_hit
+        self.client_ip = client_ip
+        self.client_port = client_port
+        self.concurrency_wait_time = concurrency_wait_time
+        self.consistency_level = consistency_level
+        self.cpu_time = cpu_time
+        self.db_name = db_name
+        self.decode_time = decode_time
+        self.disk_reads = disk_reads
+        self.elapsed_time = elapsed_time
+        self.execute_time = execute_time
+        self.executor_rpc = executor_rpc
+        self.expected_worker_count = expected_worker_count
+        self.get_plan_time = get_plan_time
+        self.hit_plan = hit_plan
+        self.inner = inner
+        self.memstore_read_rows = memstore_read_rows
+        self.net_time = net_time
+        self.net_wait_time = net_wait_time
+        self.ob_db_id = ob_db_id
+        # server  ID。
+        self.ob_server_id = ob_server_id
+        self.ob_user_id = ob_user_id
+        self.partition_count = partition_count
+        self.plan_id = plan_id
+        self.plan_type = plan_type
+        self.queue_time = queue_time
+        self.request_id = request_id
+        self.request_time = request_time
+        self.ret_code = ret_code
+        self.retry_count = retry_count
+        self.return_rows = return_rows
+        self.row_cache_hit = row_cache_hit
+        self.rpc_count = rpc_count
+        self.schedule_time = schedule_time
+        self.server = server
+        self.sql_type = sql_type
+        self.ssstore_read_rows = ssstore_read_rows
+        self.statement = statement
+        self.table_scan = table_scan
+        self.trace_id = trace_id
+        # transaction hash。
+        self.trans_hash = trans_hash
+        self.used_worker_count = used_worker_count
+        self.user_io_wait_time = user_io_wait_time
+        self.user_name = user_name
+        self.wait_count = wait_count
+        self.wait_event = wait_event
+        self.wait_time = wait_time
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.affected_rows is not None:
+            result['AffectedRows'] = self.affected_rows
+        if self.application_wait_time is not None:
+            result['ApplicationWaitTime'] = self.application_wait_time
+        if self.block_cache_hit is not None:
+            result['BlockCacheHit'] = self.block_cache_hit
+        if self.block_index_cache_hit is not None:
+            result['BlockIndexCacheHit'] = self.block_index_cache_hit
+        if self.bloom_filter_cache_hit is not None:
+            result['BloomFilterCacheHit'] = self.bloom_filter_cache_hit
+        if self.client_ip is not None:
+            result['ClientIp'] = self.client_ip
+        if self.client_port is not None:
+            result['ClientPort'] = self.client_port
+        if self.concurrency_wait_time is not None:
+            result['ConcurrencyWaitTime'] = self.concurrency_wait_time
+        if self.consistency_level is not None:
+            result['ConsistencyLevel'] = self.consistency_level
+        if self.cpu_time is not None:
+            result['CpuTime'] = self.cpu_time
+        if self.db_name is not None:
+            result['DbName'] = self.db_name
+        if self.decode_time is not None:
+            result['DecodeTime'] = self.decode_time
+        if self.disk_reads is not None:
+            result['DiskReads'] = self.disk_reads
+        if self.elapsed_time is not None:
+            result['ElapsedTime'] = self.elapsed_time
+        if self.execute_time is not None:
+            result['ExecuteTime'] = self.execute_time
+        if self.executor_rpc is not None:
+            result['ExecutorRpc'] = self.executor_rpc
+        if self.expected_worker_count is not None:
+            result['ExpectedWorkerCount'] = self.expected_worker_count
+        if self.get_plan_time is not None:
+            result['GetPlanTime'] = self.get_plan_time
+        if self.hit_plan is not None:
+            result['HitPlan'] = self.hit_plan
+        if self.inner is not None:
+            result['Inner'] = self.inner
+        if self.memstore_read_rows is not None:
+            result['MemstoreReadRows'] = self.memstore_read_rows
+        if self.net_time is not None:
+            result['NetTime'] = self.net_time
+        if self.net_wait_time is not None:
+            result['NetWaitTime'] = self.net_wait_time
+        if self.ob_db_id is not None:
+            result['ObDbId'] = self.ob_db_id
+        if self.ob_server_id is not None:
+            result['ObServerId'] = self.ob_server_id
+        if self.ob_user_id is not None:
+            result['ObUserId'] = self.ob_user_id
+        if self.partition_count is not None:
+            result['PartitionCount'] = self.partition_count
+        if self.plan_id is not None:
+            result['PlanId'] = self.plan_id
+        if self.plan_type is not None:
+            result['PlanType'] = self.plan_type
+        if self.queue_time is not None:
+            result['QueueTime'] = self.queue_time
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.request_time is not None:
+            result['RequestTime'] = self.request_time
+        if self.ret_code is not None:
+            result['RetCode'] = self.ret_code
+        if self.retry_count is not None:
+            result['RetryCount'] = self.retry_count
+        if self.return_rows is not None:
+            result['ReturnRows'] = self.return_rows
+        if self.row_cache_hit is not None:
+            result['RowCacheHit'] = self.row_cache_hit
+        if self.rpc_count is not None:
+            result['RpcCount'] = self.rpc_count
+        if self.schedule_time is not None:
+            result['ScheduleTime'] = self.schedule_time
+        if self.server is not None:
+            result['Server'] = self.server
+        if self.sql_type is not None:
+            result['SqlType'] = self.sql_type
+        if self.ssstore_read_rows is not None:
+            result['SsstoreReadRows'] = self.ssstore_read_rows
+        if self.statement is not None:
+            result['Statement'] = self.statement
+        if self.table_scan is not None:
+            result['TableScan'] = self.table_scan
+        if self.trace_id is not None:
+            result['TraceId'] = self.trace_id
+        if self.trans_hash is not None:
+            result['TransHash'] = self.trans_hash
+        if self.used_worker_count is not None:
+            result['UsedWorkerCount'] = self.used_worker_count
+        if self.user_io_wait_time is not None:
+            result['UserIoWaitTime'] = self.user_io_wait_time
+        if self.user_name is not None:
+            result['UserName'] = self.user_name
+        if self.wait_count is not None:
+            result['WaitCount'] = self.wait_count
+        if self.wait_event is not None:
+            result['WaitEvent'] = self.wait_event
+        if self.wait_time is not None:
+            result['WaitTime'] = self.wait_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AffectedRows') is not None:
+            self.affected_rows = m.get('AffectedRows')
+        if m.get('ApplicationWaitTime') is not None:
+            self.application_wait_time = m.get('ApplicationWaitTime')
+        if m.get('BlockCacheHit') is not None:
+            self.block_cache_hit = m.get('BlockCacheHit')
+        if m.get('BlockIndexCacheHit') is not None:
+            self.block_index_cache_hit = m.get('BlockIndexCacheHit')
+        if m.get('BloomFilterCacheHit') is not None:
+            self.bloom_filter_cache_hit = m.get('BloomFilterCacheHit')
+        if m.get('ClientIp') is not None:
+            self.client_ip = m.get('ClientIp')
+        if m.get('ClientPort') is not None:
+            self.client_port = m.get('ClientPort')
+        if m.get('ConcurrencyWaitTime') is not None:
+            self.concurrency_wait_time = m.get('ConcurrencyWaitTime')
+        if m.get('ConsistencyLevel') is not None:
+            self.consistency_level = m.get('ConsistencyLevel')
+        if m.get('CpuTime') is not None:
+            self.cpu_time = m.get('CpuTime')
+        if m.get('DbName') is not None:
+            self.db_name = m.get('DbName')
+        if m.get('DecodeTime') is not None:
+            self.decode_time = m.get('DecodeTime')
+        if m.get('DiskReads') is not None:
+            self.disk_reads = m.get('DiskReads')
+        if m.get('ElapsedTime') is not None:
+            self.elapsed_time = m.get('ElapsedTime')
+        if m.get('ExecuteTime') is not None:
+            self.execute_time = m.get('ExecuteTime')
+        if m.get('ExecutorRpc') is not None:
+            self.executor_rpc = m.get('ExecutorRpc')
+        if m.get('ExpectedWorkerCount') is not None:
+            self.expected_worker_count = m.get('ExpectedWorkerCount')
+        if m.get('GetPlanTime') is not None:
+            self.get_plan_time = m.get('GetPlanTime')
+        if m.get('HitPlan') is not None:
+            self.hit_plan = m.get('HitPlan')
+        if m.get('Inner') is not None:
+            self.inner = m.get('Inner')
+        if m.get('MemstoreReadRows') is not None:
+            self.memstore_read_rows = m.get('MemstoreReadRows')
+        if m.get('NetTime') is not None:
+            self.net_time = m.get('NetTime')
+        if m.get('NetWaitTime') is not None:
+            self.net_wait_time = m.get('NetWaitTime')
+        if m.get('ObDbId') is not None:
+            self.ob_db_id = m.get('ObDbId')
+        if m.get('ObServerId') is not None:
+            self.ob_server_id = m.get('ObServerId')
+        if m.get('ObUserId') is not None:
+            self.ob_user_id = m.get('ObUserId')
+        if m.get('PartitionCount') is not None:
+            self.partition_count = m.get('PartitionCount')
+        if m.get('PlanId') is not None:
+            self.plan_id = m.get('PlanId')
+        if m.get('PlanType') is not None:
+            self.plan_type = m.get('PlanType')
+        if m.get('QueueTime') is not None:
+            self.queue_time = m.get('QueueTime')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('RequestTime') is not None:
+            self.request_time = m.get('RequestTime')
+        if m.get('RetCode') is not None:
+            self.ret_code = m.get('RetCode')
+        if m.get('RetryCount') is not None:
+            self.retry_count = m.get('RetryCount')
+        if m.get('ReturnRows') is not None:
+            self.return_rows = m.get('ReturnRows')
+        if m.get('RowCacheHit') is not None:
+            self.row_cache_hit = m.get('RowCacheHit')
+        if m.get('RpcCount') is not None:
+            self.rpc_count = m.get('RpcCount')
+        if m.get('ScheduleTime') is not None:
+            self.schedule_time = m.get('ScheduleTime')
+        if m.get('Server') is not None:
+            self.server = m.get('Server')
+        if m.get('SqlType') is not None:
+            self.sql_type = m.get('SqlType')
+        if m.get('SsstoreReadRows') is not None:
+            self.ssstore_read_rows = m.get('SsstoreReadRows')
+        if m.get('Statement') is not None:
+            self.statement = m.get('Statement')
+        if m.get('TableScan') is not None:
+            self.table_scan = m.get('TableScan')
+        if m.get('TraceId') is not None:
+            self.trace_id = m.get('TraceId')
+        if m.get('TransHash') is not None:
+            self.trans_hash = m.get('TransHash')
+        if m.get('UsedWorkerCount') is not None:
+            self.used_worker_count = m.get('UsedWorkerCount')
+        if m.get('UserIoWaitTime') is not None:
+            self.user_io_wait_time = m.get('UserIoWaitTime')
+        if m.get('UserName') is not None:
+            self.user_name = m.get('UserName')
+        if m.get('WaitCount') is not None:
+            self.wait_count = m.get('WaitCount')
+        if m.get('WaitEvent') is not None:
+            self.wait_event = m.get('WaitEvent')
+        if m.get('WaitTime') is not None:
+            self.wait_time = m.get('WaitTime')
+        return self
+
+
+class DescribeSQLSamplesResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: List[DescribeSQLSamplesResponseBodyData] = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Data'] = []
+        if self.data is not None:
+            for k in self.data:
+                result['Data'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.data = []
+        if m.get('Data') is not None:
+            for k in m.get('Data'):
+                temp_model = DescribeSQLSamplesResponseBodyData()
+                self.data.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribeSQLSamplesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeSQLSamplesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeSQLSamplesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeSecurityIpGroupsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id
@@ -13624,14 +17353,183 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeTenantSecurityConfigsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeTenantSecurityIpGroupsRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        tenant_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DescribeTenantSecurityIpGroupsResponseBodySecurityIpGroups(TeaModel):
+    def __init__(
+        self,
+        security_ip_group_name: str = None,
+        security_ip_group_type: str = None,
+        security_ips: str = None,
+        tenant_id: str = None,
+    ):
+        self.security_ip_group_name = security_ip_group_name
+        self.security_ip_group_type = security_ip_group_type
+        self.security_ips = security_ips
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.security_ip_group_name is not None:
+            result['SecurityIpGroupName'] = self.security_ip_group_name
+        if self.security_ip_group_type is not None:
+            result['SecurityIpGroupType'] = self.security_ip_group_type
+        if self.security_ips is not None:
+            result['SecurityIps'] = self.security_ips
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('SecurityIpGroupName') is not None:
+            self.security_ip_group_name = m.get('SecurityIpGroupName')
+        if m.get('SecurityIpGroupType') is not None:
+            self.security_ip_group_type = m.get('SecurityIpGroupType')
+        if m.get('SecurityIps') is not None:
+            self.security_ips = m.get('SecurityIps')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DescribeTenantSecurityIpGroupsResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        security_ip_groups: List[DescribeTenantSecurityIpGroupsResponseBodySecurityIpGroups] = None,
+        total_count: int = None,
+    ):
+        self.request_id = request_id
+        self.security_ip_groups = security_ip_groups
+        self.total_count = total_count
+
+    def validate(self):
+        if self.security_ip_groups:
+            for k in self.security_ip_groups:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['SecurityIpGroups'] = []
+        if self.security_ip_groups is not None:
+            for k in self.security_ip_groups:
+                result['SecurityIpGroups'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.security_ip_groups = []
+        if m.get('SecurityIpGroups') is not None:
+            for k in m.get('SecurityIpGroups'):
+                temp_model = DescribeTenantSecurityIpGroupsResponseBodySecurityIpGroups()
+                self.security_ip_groups.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeTenantSecurityIpGroupsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeTenantSecurityIpGroupsResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeTenantSecurityIpGroupsResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeTenantTagsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         tags: str = None,
         tenant_ids: str = None,
     ):
@@ -17323,14 +21221,183 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyTenantResourceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyTenantSecurityIpGroupRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        security_ip_group_name: str = None,
+        security_ips: str = None,
+        tenant_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.security_ip_group_name = security_ip_group_name
+        self.security_ips = security_ips
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_ip_group_name is not None:
+            result['SecurityIpGroupName'] = self.security_ip_group_name
+        if self.security_ips is not None:
+            result['SecurityIps'] = self.security_ips
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityIpGroupName') is not None:
+            self.security_ip_group_name = m.get('SecurityIpGroupName')
+        if m.get('SecurityIps') is not None:
+            self.security_ips = m.get('SecurityIps')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class ModifyTenantSecurityIpGroupResponseBodySecurityIpGroup(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        security_ip_group_name: str = None,
+        security_ips: str = None,
+        tenant_id: str = None,
+    ):
+        self.instance_id = instance_id
+        self.security_ip_group_name = security_ip_group_name
+        self.security_ips = security_ips
+        self.tenant_id = tenant_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.security_ip_group_name is not None:
+            result['SecurityIpGroupName'] = self.security_ip_group_name
+        if self.security_ips is not None:
+            result['SecurityIps'] = self.security_ips
+        if self.tenant_id is not None:
+            result['TenantId'] = self.tenant_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('SecurityIpGroupName') is not None:
+            self.security_ip_group_name = m.get('SecurityIpGroupName')
+        if m.get('SecurityIps') is not None:
+            self.security_ips = m.get('SecurityIps')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class ModifyTenantSecurityIpGroupResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        security_ip_group: ModifyTenantSecurityIpGroupResponseBodySecurityIpGroup = None,
+    ):
+        self.request_id = request_id
+        self.security_ip_group = security_ip_group
+
+    def validate(self):
+        if self.security_ip_group:
+            self.security_ip_group.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.security_ip_group is not None:
+            result['SecurityIpGroup'] = self.security_ip_group.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('SecurityIpGroup') is not None:
+            temp_model = ModifyTenantSecurityIpGroupResponseBodySecurityIpGroup()
+            self.security_ip_group = temp_model.from_map(m['SecurityIpGroup'])
+        return self
+
+
+class ModifyTenantSecurityIpGroupResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ModifyTenantSecurityIpGroupResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ModifyTenantSecurityIpGroupResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ModifyTenantTagsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         tags: str = None,
         tenant_id: str = None,
     ):
@@ -21184,7 +25251,158 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = StopOmsOpenAPIProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SwitchoverInstanceRequest(TeaModel):
+    def __init__(
+        self,
+        forced: bool = None,
+        instance_id: str = None,
+        target_instance_id: str = None,
+    ):
+        self.forced = forced
+        self.instance_id = instance_id
+        self.target_instance_id = target_instance_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.forced is not None:
+            result['Forced'] = self.forced
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.target_instance_id is not None:
+            result['TargetInstanceId'] = self.target_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Forced') is not None:
+            self.forced = m.get('Forced')
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('TargetInstanceId') is not None:
+            self.target_instance_id = m.get('TargetInstanceId')
+        return self
+
+
+class SwitchoverInstanceResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        message: str = None,
+        success: bool = None,
+    ):
+        self.message = message
+        self.success = success
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.success is not None:
+            result['Success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class SwitchoverInstanceResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: SwitchoverInstanceResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Data') is not None:
+            temp_model = SwitchoverInstanceResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SwitchoverInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SwitchoverInstanceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SwitchoverInstanceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.8/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO` & `alibabacloud_oceanbasepro20190901-1.0.9/alibabacloud_oceanbasepro20190901.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oceanbasepro20190901
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901-1.0.8/setup.py` & `alibabacloud_oceanbasepro20190901-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oceanbasepro20190901.
 
-Created on 19/05/2023
+Created on 08/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oceanbasepro20190901"
 NAME = "alibabacloud_oceanbasepro20190901" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OceanBasePro (20190901) SDK Library for Python"
```

