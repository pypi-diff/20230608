# Comparing `tmp/alibabacloud_oceanbasepro20190901_py2-1.0.3.tar.gz` & `tmp/alibabacloud_oceanbasepro20190901_py2-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901_py2-1.0.3.tar", last modified: Fri May 19 10:09:23 2023, max compression
+gzip compressed data, was "dist/alibabacloud_oceanbasepro20190901_py2-1.0.4.tar", last modified: Thu Jun  8 02:58:03 2023, max compression
```

## Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.3.tar` & `alibabacloud_oceanbasepro20190901_py2-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      124 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2526 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1060 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1143 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   109067 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/client.py
--rw-r--r--   0 root         (0) root         (0)   835668 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2526 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2948 2023-05-19 10:09:23.000000 alibabacloud_oceanbasepro20190901_py2-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   129641 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901/client.py
+-rw-r--r--   0 root         (0) root         (0)  1004910 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-06-08 02:58:03.000000 alibabacloud_oceanbasepro20190901_py2-1.0.4/setup.py
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.3/LICENSE` & `alibabacloud_oceanbasepro20190901_py2-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.3/PKG-INFO` & `alibabacloud_oceanbasepro20190901_py2-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_oceanbasepro20190901_py2
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.3/README-CN.md` & `alibabacloud_oceanbasepro20190901_py2-1.0.4/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.3/README.md` & `alibabacloud_oceanbasepro20190901_py2-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/client.py` & `alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -358,14 +358,48 @@
             self.call_api(params, req, runtime)
         )
 
     def create_tenant_read_only_connection(self, request):
         runtime = util_models.RuntimeOptions()
         return self.create_tenant_read_only_connection_with_options(request, runtime)
 
+    def create_tenant_security_ip_group_with_options(self, request, runtime):
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
+    def create_tenant_security_ip_group(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.create_tenant_security_ip_group_with_options(request, runtime)
+
     def create_tenant_user_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.description):
             body['Description'] = request.description
         if not UtilClient.is_unset(request.encryption_type):
             body['EncryptionType'] = request.encryption_type
@@ -544,14 +578,46 @@
             self.call_api(params, req, runtime)
         )
 
     def delete_security_ip_group(self, request):
         runtime = util_models.RuntimeOptions()
         return self.delete_security_ip_group_with_options(request, runtime)
 
+    def delete_tenant_security_ip_group_with_options(self, request, runtime):
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
+    def delete_tenant_security_ip_group(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.delete_tenant_security_ip_group_with_options(request, runtime)
+
     def delete_tenant_users_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.instance_id):
             body['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.tenant_id):
             body['TenantId'] = request.tenant_id
@@ -1058,14 +1124,300 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_node_metrics(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_node_metrics_with_options(request, runtime)
 
+    def describe_oas_anomaly_sqllist_with_options(self, request, runtime):
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
+    def describe_oas_anomaly_sqllist(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_anomaly_sqllist_with_options(request, runtime)
+
+    def describe_oas_sqldetails_with_options(self, request, runtime):
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
+    def describe_oas_sqldetails(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_sqldetails_with_options(request, runtime)
+
+    def describe_oas_sqlhistory_list_with_options(self, request, runtime):
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
+    def describe_oas_sqlhistory_list(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_sqlhistory_list_with_options(request, runtime)
+
+    def describe_oas_sqlplans_with_options(self, request, runtime):
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
+    def describe_oas_sqlplans(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_sqlplans_with_options(request, runtime)
+
+    def describe_oas_slow_sqllist_with_options(self, request, runtime):
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
+    def describe_oas_slow_sqllist(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_slow_sqllist_with_options(request, runtime)
+
+    def describe_oas_top_sqllist_with_options(self, request, runtime):
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
+    def describe_oas_top_sqllist(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_oas_top_sqllist_with_options(request, runtime)
+
     def describe_oms_open_apiproject_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.page_number):
             body['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
             body['PageSize'] = request.page_size
@@ -1366,14 +1718,52 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_sqlplans(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_sqlplans_with_options(request, runtime)
 
+    def describe_sqlsamples_with_options(self, request, runtime):
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
+    def describe_sqlsamples(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_sqlsamples_with_options(request, runtime)
+
     def describe_security_ip_groups_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.instance_id):
             body['InstanceId'] = request.instance_id
         req = open_api_models.OpenApiRequest(
             body=OpenApiUtilClient.parse_to_map(body)
@@ -1596,14 +1986,44 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_tenant_security_configs(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_tenant_security_configs_with_options(request, runtime)
 
+    def describe_tenant_security_ip_groups_with_options(self, request, runtime):
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
+    def describe_tenant_security_ip_groups(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_tenant_security_ip_groups_with_options(request, runtime)
+
     def describe_tenant_tags_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.instance_id):
             body['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.tags):
             body['Tags'] = request.tags
@@ -2228,14 +2648,48 @@
             self.call_api(params, req, runtime)
         )
 
     def modify_tenant_resource(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_tenant_resource_with_options(request, runtime)
 
+    def modify_tenant_security_ip_group_with_options(self, request, runtime):
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
+    def modify_tenant_security_ip_group(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.modify_tenant_security_ip_group_with_options(request, runtime)
+
     def modify_tenant_tags_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.instance_id):
             body['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.tags):
             body['Tags'] = request.tags
@@ -2663,7 +3117,39 @@
             ocean_base_pro_20190901_models.StopOmsOpenAPIProjectResponse(),
             self.call_api(params, req, runtime)
         )
 
     def stop_oms_open_apiproject(self, request):
         runtime = util_models.RuntimeOptions()
         return self.stop_oms_open_apiproject_with_options(request, runtime)
+
+    def switchover_instance_with_options(self, request, runtime):
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
+    def switchover_instance(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.switchover_instance_with_options(request, runtime)
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901/models.py` & `alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1730,14 +1730,162 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateTenantReadOnlyConnectionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateTenantSecurityIpGroupRequest(TeaModel):
+    def __init__(self, instance_id=None, security_ip_group_name=None, security_ips=None, tenant_id=None):
+        self.instance_id = instance_id  # type: str
+        self.security_ip_group_name = security_ip_group_name  # type: str
+        self.security_ips = security_ips  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateTenantSecurityIpGroupRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_id=None, security_ip_group_name=None, security_ips=None, tenant_id=None):
+        self.instance_id = instance_id  # type: str
+        self.security_ip_group_name = security_ip_group_name  # type: str
+        self.security_ips = security_ips  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(CreateTenantSecurityIpGroupResponseBodySecurityIpGroup, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, security_ip_group=None):
+        self.request_id = request_id  # type: str
+        self.security_ip_group = security_ip_group  # type: CreateTenantSecurityIpGroupResponseBodySecurityIpGroup
+
+    def validate(self):
+        if self.security_ip_group:
+            self.security_ip_group.validate()
+
+    def to_map(self):
+        _map = super(CreateTenantSecurityIpGroupResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: CreateTenantSecurityIpGroupResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(CreateTenantSecurityIpGroupResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, description=None, encryption_type=None, instance_id=None, roles=None, tenant_id=None,
                  user_name=None, user_password=None, user_type=None):
         # The description of the database.
         self.description = description  # type: str
         # 加密方式。
         self.encryption_type = encryption_type  # type: str
@@ -2488,14 +2636,152 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DeleteSecurityIpGroupResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DeleteTenantSecurityIpGroupRequest(TeaModel):
+    def __init__(self, instance_id=None, security_ip_group_name=None, tenant_id=None):
+        self.instance_id = instance_id  # type: str
+        self.security_ip_group_name = security_ip_group_name  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteTenantSecurityIpGroupRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_id=None, security_ip_group_name=None, tenant_id=None):
+        self.instance_id = instance_id  # type: str
+        self.security_ip_group_name = security_ip_group_name  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DeleteTenantSecurityIpGroupResponseBodySecurityIpGroup, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, security_ip_group=None):
+        self.request_id = request_id  # type: str
+        self.security_ip_group = security_ip_group  # type: DeleteTenantSecurityIpGroupResponseBodySecurityIpGroup
+
+    def validate(self):
+        if self.security_ip_group:
+            self.security_ip_group.validate()
+
+    def to_map(self):
+        _map = super(DeleteTenantSecurityIpGroupResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DeleteTenantSecurityIpGroupResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DeleteTenantSecurityIpGroupResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, tenant_id=None, users=None):
         # Example 1
         self.instance_id = instance_id  # type: str
         # $.parameters[4].schema.enumValueTitles
         self.tenant_id = tenant_id  # type: str
         # $.parameters[2].schema.example
@@ -6353,14 +6639,2576 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeNodeMetricsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeOasAnomalySQLListRequest(TeaModel):
+    def __init__(self, accept_language=None, current=None, db_name=None, end_time=None, filter_condition=None,
+                 instance_id=None, node_ip=None, page_size=None, search_key_word=None, search_param=None, search_rule=None,
+                 search_value=None, sql_id=None, sql_text_length=None, start_time=None, tenant_id=None):
+        self.accept_language = accept_language  # type: str
+        self.current = current  # type: long
+        self.db_name = db_name  # type: str
+        self.end_time = end_time  # type: str
+        self.filter_condition = filter_condition  # type: str
+        self.instance_id = instance_id  # type: str
+        self.node_ip = node_ip  # type: str
+        self.page_size = page_size  # type: long
+        self.search_key_word = search_key_word  # type: str
+        self.search_param = search_param  # type: str
+        self.search_rule = search_rule  # type: str
+        self.search_value = search_value  # type: str
+        # SQL ID。
+        self.sql_id = sql_id  # type: str
+        self.sql_text_length = sql_text_length  # type: long
+        self.start_time = start_time  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasAnomalySQLListRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, avg_cpu_time=None, avg_elapsed_time=None, avg_get_plan_time=None, cpu_time=None,
+                 db_name=None, diag_types=None, diagnosis=None, executions=None, last_executed_time=None, risk_level=None,
+                 sql_id=None, sql_text_short=None, suggestion=None, sum_elapsed_time=None, user_name=None):
+        self.avg_cpu_time = avg_cpu_time  # type: float
+        self.avg_elapsed_time = avg_elapsed_time  # type: float
+        self.avg_get_plan_time = avg_get_plan_time  # type: float
+        self.cpu_time = cpu_time  # type: float
+        self.db_name = db_name  # type: str
+        self.diag_types = diag_types  # type: list[str]
+        self.diagnosis = diagnosis  # type: str
+        self.executions = executions  # type: float
+        self.last_executed_time = last_executed_time  # type: float
+        self.risk_level = risk_level  # type: str
+        # SQL ID。
+        self.sql_id = sql_id  # type: str
+        self.sql_text_short = sql_text_short  # type: str
+        self.suggestion = suggestion  # type: str
+        self.sum_elapsed_time = sum_elapsed_time  # type: str
+        self.user_name = user_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasAnomalySQLListResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, data=None, request_id=None, total_count=None):
+        self.data = data  # type: list[DescribeOasAnomalySQLListResponseBodyData]
+        self.request_id = request_id  # type: str
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasAnomalySQLListResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeOasAnomalySQLListResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasAnomalySQLListResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, db_name=None, end_time=None, instance_id=None, sql_id=None, start_time=None, tenant_id=None):
+        self.db_name = db_name  # type: str
+        self.end_time = end_time  # type: str
+        self.instance_id = instance_id  # type: str
+        # SQL ID。
+        self.sql_id = sql_id  # type: str
+        self.start_time = start_time  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasSQLDetailsRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, db_name=None, fulltext=None, statement=None, tables=None, user_name=None):
+        self.db_name = db_name  # type: str
+        self.fulltext = fulltext  # type: str
+        self.statement = statement  # type: str
+        self.tables = tables  # type: list[str]
+        self.user_name = user_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasSQLDetailsResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: DescribeOasSQLDetailsResponseBodyData
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasSQLDetailsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeOasSQLDetailsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasSQLDetailsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, accept_language=None, db_name=None, end_time=None, instance_id=None, node_ip=None,
+                 sql_id=None, start_time=None, tenant_id=None):
+        self.accept_language = accept_language  # type: str
+        self.db_name = db_name  # type: str
+        self.end_time = end_time  # type: str
+        self.instance_id = instance_id  # type: str
+        self.node_ip = node_ip  # type: str
+        # SQL ID。
+        self.sql_id = sql_id  # type: str
+        self.start_time = start_time  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasSQLHistoryListRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, avg_affected_rows=None, avg_application_wait_time=None, avg_block_cache_hit=None,
+                 avg_block_index_cache_hit=None, avg_bloom_filter_cache_hit=None, avg_concurrency_wait_time=None, avg_cpu_time=None,
+                 avg_decode_time=None, avg_disk_reads=None, avg_elapsed_time=None, avg_execute_time=None,
+                 avg_executor_rpc_count=None, avg_expected_worker_count=None, avg_get_plan_time=None, avg_logical_reads=None,
+                 avg_memstore_read_rows=None, avg_net_time=None, avg_net_wait_time=None, avg_partition_count=None, avg_queue_time=None,
+                 avg_return_rows=None, avg_row_cache_hit=None, avg_rpc_count=None, avg_schedule_time=None,
+                 avg_ssstore_read_rows=None, avg_used_worker_count=None, avg_user_io_wait_time=None, avg_wait_count=None,
+                 avg_wait_time=None, db_name=None, dist_plan_percentage=None, exec_ps=None, executions=None, fail_count=None,
+                 fail_percentage=None, local_plan_percentage=None, max_affected_rows=None, max_application_wait_time=None,
+                 max_concurrency_wait_time=None, max_cpu_time=None, max_disk_reads=None, max_elapsed_time=None, max_return_rows=None,
+                 max_user_io_wait_time=None, max_wait_time=None, miss_plan_percentage=None, miss_plans=None, remote_plan_percentage=None,
+                 remote_plans=None, ret_code_4012count=None, ret_code_4013count=None, ret_code_5001count=None,
+                 ret_code_5024count=None, ret_code_5167count=None, ret_code_5217count=None, ret_code_6002count=None, retry_count=None,
+                 sqlid=None, server=None, strong_consistency_percentage=None, sum_elapsed_time=None,
+                 sum_logical_reads=None, sum_wait_time=None, table_scan_percentage=None, timestamp=None, user_name=None,
+                 weak_consistency_percentage=None):
+        self.avg_affected_rows = avg_affected_rows  # type: long
+        self.avg_application_wait_time = avg_application_wait_time  # type: float
+        self.avg_block_cache_hit = avg_block_cache_hit  # type: long
+        self.avg_block_index_cache_hit = avg_block_index_cache_hit  # type: long
+        self.avg_bloom_filter_cache_hit = avg_bloom_filter_cache_hit  # type: long
+        self.avg_concurrency_wait_time = avg_concurrency_wait_time  # type: float
+        self.avg_cpu_time = avg_cpu_time  # type: float
+        self.avg_decode_time = avg_decode_time  # type: float
+        self.avg_disk_reads = avg_disk_reads  # type: long
+        self.avg_elapsed_time = avg_elapsed_time  # type: float
+        self.avg_execute_time = avg_execute_time  # type: float
+        self.avg_executor_rpc_count = avg_executor_rpc_count  # type: float
+        self.avg_expected_worker_count = avg_expected_worker_count  # type: float
+        self.avg_get_plan_time = avg_get_plan_time  # type: float
+        self.avg_logical_reads = avg_logical_reads  # type: long
+        self.avg_memstore_read_rows = avg_memstore_read_rows  # type: long
+        self.avg_net_time = avg_net_time  # type: float
+        self.avg_net_wait_time = avg_net_wait_time  # type: float
+        self.avg_partition_count = avg_partition_count  # type: float
+        self.avg_queue_time = avg_queue_time  # type: float
+        self.avg_return_rows = avg_return_rows  # type: long
+        self.avg_row_cache_hit = avg_row_cache_hit  # type: long
+        self.avg_rpc_count = avg_rpc_count  # type: long
+        self.avg_schedule_time = avg_schedule_time  # type: float
+        self.avg_ssstore_read_rows = avg_ssstore_read_rows  # type: long
+        self.avg_used_worker_count = avg_used_worker_count  # type: float
+        self.avg_user_io_wait_time = avg_user_io_wait_time  # type: float
+        self.avg_wait_count = avg_wait_count  # type: float
+        self.avg_wait_time = avg_wait_time  # type: float
+        self.db_name = db_name  # type: str
+        self.dist_plan_percentage = dist_plan_percentage  # type: float
+        self.exec_ps = exec_ps  # type: float
+        self.executions = executions  # type: long
+        self.fail_count = fail_count  # type: long
+        self.fail_percentage = fail_percentage  # type: float
+        self.local_plan_percentage = local_plan_percentage  # type: float
+        self.max_affected_rows = max_affected_rows  # type: float
+        self.max_application_wait_time = max_application_wait_time  # type: float
+        self.max_concurrency_wait_time = max_concurrency_wait_time  # type: float
+        self.max_cpu_time = max_cpu_time  # type: float
+        self.max_disk_reads = max_disk_reads  # type: float
+        self.max_elapsed_time = max_elapsed_time  # type: float
+        self.max_return_rows = max_return_rows  # type: float
+        self.max_user_io_wait_time = max_user_io_wait_time  # type: float
+        self.max_wait_time = max_wait_time  # type: float
+        self.miss_plan_percentage = miss_plan_percentage  # type: float
+        self.miss_plans = miss_plans  # type: long
+        self.remote_plan_percentage = remote_plan_percentage  # type: float
+        self.remote_plans = remote_plans  # type: long
+        self.ret_code_4012count = ret_code_4012count  # type: float
+        self.ret_code_4013count = ret_code_4013count  # type: float
+        self.ret_code_5001count = ret_code_5001count  # type: float
+        self.ret_code_5024count = ret_code_5024count  # type: float
+        self.ret_code_5167count = ret_code_5167count  # type: float
+        self.ret_code_5217count = ret_code_5217count  # type: float
+        self.ret_code_6002count = ret_code_6002count  # type: float
+        self.retry_count = retry_count  # type: long
+        # SQL ID
+        self.sqlid = sqlid  # type: str
+        self.server = server  # type: str
+        self.strong_consistency_percentage = strong_consistency_percentage  # type: float
+        self.sum_elapsed_time = sum_elapsed_time  # type: float
+        self.sum_logical_reads = sum_logical_reads  # type: float
+        self.sum_wait_time = sum_wait_time  # type: float
+        self.table_scan_percentage = table_scan_percentage  # type: float
+        self.timestamp = timestamp  # type: str
+        self.user_name = user_name  # type: str
+        self.weak_consistency_percentage = weak_consistency_percentage  # type: float
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasSQLHistoryListResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: list[DescribeOasSQLHistoryListResponseBodyData]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasSQLHistoryListResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeOasSQLHistoryListResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasSQLHistoryListResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, accept_language=None, db_name=None, end_time=None, instance_id=None, sql_id=None,
+                 start_time=None, tenant_id=None):
+        self.accept_language = accept_language  # type: str
+        self.db_name = db_name  # type: str
+        self.end_time = end_time  # type: str
+        self.instance_id = instance_id  # type: str
+        # SQL ID。
+        self.sql_id = sql_id  # type: str
+        self.start_time = start_time  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasSQLPlansRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, plan_json_string=None):
+        self.plan_json_string = plan_json_string  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasSQLPlansResponseBodyDataPlanExplain, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.plan_json_string is not None:
+            result['PlanJsonString'] = self.plan_json_string
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('PlanJsonString') is not None:
+            self.plan_json_string = m.get('PlanJsonString')
+        return self
+
+
+class DescribeOasSQLPlansResponseBodyDataPlans(TeaModel):
+    def __init__(self, avg_application_wait_time=None, avg_buffer_gets=None, avg_concurrency_wait_time=None,
+                 avg_cpu_time=None, avg_disk_reads=None, avg_disk_writes=None, avg_elapsed_time=None, avg_row_processed=None,
+                 avg_user_io_wait_time=None, collect_time_us=None, delayed_large_query_percentage=None, exec_ps=None, executions=None,
+                 first_load_time=None, first_load_time_us=None, hit_diagnosis=None, hit_percentage=None,
+                 large_query_percentage=None, merged_version=None, ob_db_id=None, ob_server_id=None, outline_data=None, outline_id=None,
+                 plan_hash=None, plan_id=None, plan_size=None, plan_type=None, plan_union_hash=None, schema_version=None,
+                 server=None, server_id=None, table_scan=None, timeout_percentage=None, uid=None):
+        self.avg_application_wait_time = avg_application_wait_time  # type: float
+        self.avg_buffer_gets = avg_buffer_gets  # type: float
+        self.avg_concurrency_wait_time = avg_concurrency_wait_time  # type: float
+        self.avg_cpu_time = avg_cpu_time  # type: float
+        self.avg_disk_reads = avg_disk_reads  # type: float
+        self.avg_disk_writes = avg_disk_writes  # type: float
+        self.avg_elapsed_time = avg_elapsed_time  # type: float
+        self.avg_row_processed = avg_row_processed  # type: float
+        self.avg_user_io_wait_time = avg_user_io_wait_time  # type: float
+        self.collect_time_us = collect_time_us  # type: long
+        self.delayed_large_query_percentage = delayed_large_query_percentage  # type: float
+        self.exec_ps = exec_ps  # type: float
+        self.executions = executions  # type: long
+        self.first_load_time = first_load_time  # type: str
+        self.first_load_time_us = first_load_time_us  # type: long
+        self.hit_diagnosis = hit_diagnosis  # type: bool
+        self.hit_percentage = hit_percentage  # type: float
+        self.large_query_percentage = large_query_percentage  # type: float
+        self.merged_version = merged_version  # type: long
+        self.ob_db_id = ob_db_id  # type: long
+        # server  ID。
+        self.ob_server_id = ob_server_id  # type: long
+        self.outline_data = outline_data  # type: str
+        # Outline ID。
+        self.outline_id = outline_id  # type: long
+        self.plan_hash = plan_hash  # type: str
+        self.plan_id = plan_id  # type: long
+        self.plan_size = plan_size  # type: long
+        self.plan_type = plan_type  # type: str
+        self.plan_union_hash = plan_union_hash  # type: str
+        self.schema_version = schema_version  # type: long
+        self.server = server  # type: str
+        self.server_id = server_id  # type: long
+        self.table_scan = table_scan  # type: bool
+        self.timeout_percentage = timeout_percentage  # type: float
+        self.uid = uid  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasSQLPlansResponseBodyDataPlans, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, avg_cpu_time=None, bounded=None, executions=None, first_load_time=None, hit_diagnosis=None,
+                 hit_percentage=None, merged_version=None, plan_explain=None, plan_hash=None, plan_type=None, plan_union_hash=None,
+                 plans=None, query_sql=None):
+        self.avg_cpu_time = avg_cpu_time  # type: float
+        self.bounded = bounded  # type: bool
+        self.executions = executions  # type: long
+        self.first_load_time = first_load_time  # type: str
+        self.hit_diagnosis = hit_diagnosis  # type: bool
+        self.hit_percentage = hit_percentage  # type: float
+        self.merged_version = merged_version  # type: long
+        self.plan_explain = plan_explain  # type: DescribeOasSQLPlansResponseBodyDataPlanExplain
+        self.plan_hash = plan_hash  # type: str
+        self.plan_type = plan_type  # type: str
+        self.plan_union_hash = plan_union_hash  # type: str
+        self.plans = plans  # type: list[DescribeOasSQLPlansResponseBodyDataPlans]
+        self.query_sql = query_sql  # type: str
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
+        _map = super(DescribeOasSQLPlansResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: list[DescribeOasSQLPlansResponseBodyData]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasSQLPlansResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeOasSQLPlansResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasSQLPlansResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, accept_language=None, db_name=None, end_time=None, filter_condition=None, instance_id=None,
+                 node_ip=None, search_key_word=None, search_param=None, search_rule=None, search_value=None, sql_id=None,
+                 sql_text_length=None, start_time=None, tenant_id=None):
+        self.accept_language = accept_language  # type: str
+        self.db_name = db_name  # type: str
+        self.end_time = end_time  # type: str
+        self.filter_condition = filter_condition  # type: str
+        self.instance_id = instance_id  # type: str
+        self.node_ip = node_ip  # type: str
+        self.search_key_word = search_key_word  # type: str
+        self.search_param = search_param  # type: str
+        self.search_rule = search_rule  # type: str
+        self.search_value = search_value  # type: str
+        self.sql_id = sql_id  # type: str
+        self.sql_text_length = sql_text_length  # type: long
+        self.start_time = start_time  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasSlowSQLListRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, avg_affected_rows=None, avg_application_wait_time=None, avg_block_cache_hit=None,
+                 avg_block_index_cache_hit=None, avg_bloom_filter_cache_hit=None, avg_concurrency_wait_time=None, avg_cpu_time=None,
+                 avg_decode_time=None, avg_disk_reads=None, avg_elapsed_time=None, avg_execute_time=None,
+                 avg_executor_rpc_count=None, avg_expected_worker_count=None, avg_get_plan_time=None, avg_logical_reads=None,
+                 avg_memstore_read_rows=None, avg_net_time=None, avg_net_wait_time=None, avg_partition_count=None, avg_queue_time=None,
+                 avg_return_rows=None, avg_row_cache_hit=None, avg_rpc_count=None, avg_schedule_time=None,
+                 avg_ssstore_read_rows=None, avg_used_worker_count=None, avg_user_io_wait_time=None, avg_wait_count=None,
+                 avg_wait_time=None, client_ip=None, db_name=None, dist_plan_percentage=None, exec_ps=None, executions=None,
+                 fail_count=None, fail_percentage=None, inner=None, local_plan_percentage=None, max_affected_rows=None,
+                 max_application_wait_time=None, max_concurrency_wait_time=None, max_cpu_time=None, max_disk_reads=None,
+                 max_elapsed_time=None, max_return_rows=None, max_user_io_wait_time=None, max_wait_time=None,
+                 miss_plan_percentage=None, miss_plans=None, remote_plan_percentage=None, remote_plans=None, ret_code_4012count=None,
+                 ret_code_4013count=None, ret_code_5001count=None, ret_code_5024count=None, ret_code_5167count=None,
+                 ret_code_5217count=None, ret_code_6002count=None, retry_count=None, rpc_count=None, server=None, server_ip=None,
+                 server_port=None, sql_id=None, sql_text_short=None, sql_type=None, strong_consistency_percentage=None,
+                 sum_elapsed_time=None, sum_logical_reads=None, sum_wait_time=None, table_scan_percentage=None,
+                 total_wait_time=None, user_name=None, wait_event=None, weak_consistency_percentage=None):
+        self.avg_affected_rows = avg_affected_rows  # type: float
+        self.avg_application_wait_time = avg_application_wait_time  # type: float
+        self.avg_block_cache_hit = avg_block_cache_hit  # type: float
+        self.avg_block_index_cache_hit = avg_block_index_cache_hit  # type: float
+        self.avg_bloom_filter_cache_hit = avg_bloom_filter_cache_hit  # type: float
+        self.avg_concurrency_wait_time = avg_concurrency_wait_time  # type: float
+        self.avg_cpu_time = avg_cpu_time  # type: float
+        self.avg_decode_time = avg_decode_time  # type: float
+        self.avg_disk_reads = avg_disk_reads  # type: float
+        self.avg_elapsed_time = avg_elapsed_time  # type: float
+        self.avg_execute_time = avg_execute_time  # type: float
+        self.avg_executor_rpc_count = avg_executor_rpc_count  # type: float
+        self.avg_expected_worker_count = avg_expected_worker_count  # type: float
+        self.avg_get_plan_time = avg_get_plan_time  # type: float
+        self.avg_logical_reads = avg_logical_reads  # type: float
+        self.avg_memstore_read_rows = avg_memstore_read_rows  # type: float
+        self.avg_net_time = avg_net_time  # type: float
+        self.avg_net_wait_time = avg_net_wait_time  # type: float
+        self.avg_partition_count = avg_partition_count  # type: float
+        self.avg_queue_time = avg_queue_time  # type: float
+        self.avg_return_rows = avg_return_rows  # type: float
+        self.avg_row_cache_hit = avg_row_cache_hit  # type: float
+        self.avg_rpc_count = avg_rpc_count  # type: float
+        self.avg_schedule_time = avg_schedule_time  # type: float
+        self.avg_ssstore_read_rows = avg_ssstore_read_rows  # type: float
+        self.avg_used_worker_count = avg_used_worker_count  # type: float
+        self.avg_user_io_wait_time = avg_user_io_wait_time  # type: float
+        self.avg_wait_count = avg_wait_count  # type: float
+        self.avg_wait_time = avg_wait_time  # type: float
+        self.client_ip = client_ip  # type: str
+        self.db_name = db_name  # type: str
+        self.dist_plan_percentage = dist_plan_percentage  # type: float
+        self.exec_ps = exec_ps  # type: float
+        self.executions = executions  # type: float
+        self.fail_count = fail_count  # type: float
+        self.fail_percentage = fail_percentage  # type: float
+        self.inner = inner  # type: bool
+        self.local_plan_percentage = local_plan_percentage  # type: float
+        self.max_affected_rows = max_affected_rows  # type: float
+        self.max_application_wait_time = max_application_wait_time  # type: float
+        self.max_concurrency_wait_time = max_concurrency_wait_time  # type: float
+        self.max_cpu_time = max_cpu_time  # type: float
+        self.max_disk_reads = max_disk_reads  # type: float
+        self.max_elapsed_time = max_elapsed_time  # type: float
+        self.max_return_rows = max_return_rows  # type: float
+        self.max_user_io_wait_time = max_user_io_wait_time  # type: float
+        self.max_wait_time = max_wait_time  # type: float
+        self.miss_plan_percentage = miss_plan_percentage  # type: float
+        self.miss_plans = miss_plans  # type: float
+        self.remote_plan_percentage = remote_plan_percentage  # type: float
+        self.remote_plans = remote_plans  # type: float
+        self.ret_code_4012count = ret_code_4012count  # type: long
+        self.ret_code_4013count = ret_code_4013count  # type: long
+        self.ret_code_5001count = ret_code_5001count  # type: long
+        self.ret_code_5024count = ret_code_5024count  # type: long
+        self.ret_code_5167count = ret_code_5167count  # type: long
+        self.ret_code_5217count = ret_code_5217count  # type: long
+        self.ret_code_6002count = ret_code_6002count  # type: long
+        self.retry_count = retry_count  # type: float
+        self.rpc_count = rpc_count  # type: float
+        self.server = server  # type: str
+        self.server_ip = server_ip  # type: str
+        self.server_port = server_port  # type: long
+        # SQL ID。
+        self.sql_id = sql_id  # type: str
+        self.sql_text_short = sql_text_short  # type: str
+        self.sql_type = sql_type  # type: str
+        self.strong_consistency_percentage = strong_consistency_percentage  # type: float
+        self.sum_elapsed_time = sum_elapsed_time  # type: float
+        self.sum_logical_reads = sum_logical_reads  # type: float
+        self.sum_wait_time = sum_wait_time  # type: float
+        self.table_scan_percentage = table_scan_percentage  # type: float
+        self.total_wait_time = total_wait_time  # type: float
+        self.user_name = user_name  # type: str
+        self.wait_event = wait_event  # type: str
+        self.weak_consistency_percentage = weak_consistency_percentage  # type: float
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasSlowSQLListResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: list[DescribeOasSlowSQLListResponseBodyData]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasSlowSQLListResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeOasSlowSQLListResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasSlowSQLListResponse, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, accept_language=None, db_name=None, end_time=None, filter_condition=None, instance_id=None,
+                 node_ip=None, search_key_word=None, search_param=None, search_rule=None, search_value=None, sql_id=None,
+                 sql_text_length=None, start_time=None, tenant_id=None):
+        self.accept_language = accept_language  # type: str
+        self.db_name = db_name  # type: str
+        self.end_time = end_time  # type: str
+        self.filter_condition = filter_condition  # type: str
+        self.instance_id = instance_id  # type: str
+        self.node_ip = node_ip  # type: str
+        self.search_key_word = search_key_word  # type: str
+        self.search_param = search_param  # type: str
+        self.search_rule = search_rule  # type: str
+        self.search_value = search_value  # type: str
+        self.sql_id = sql_id  # type: str
+        self.sql_text_length = sql_text_length  # type: long
+        self.start_time = start_time  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasTopSQLListRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, avg_affected_rows=None, avg_application_wait_time=None, avg_block_cache_hit=None,
+                 avg_block_index_cache_hit=None, avg_bloom_filter_cache_hit=None, avg_concurrency_wait_time=None, avg_cpu_time=None,
+                 avg_decode_time=None, avg_disk_reads=None, avg_elapsed_time=None, avg_execute_time=None,
+                 avg_executor_rpc_count=None, avg_expected_worker_count=None, avg_get_plan_time=None, avg_logical_reads=None,
+                 avg_memstore_read_rows=None, avg_net_time=None, avg_net_wait_time=None, avg_partition_count=None, avg_queue_time=None,
+                 avg_return_rows=None, avg_row_cache_hit=None, avg_rpc_count=None, avg_schedule_time=None,
+                 avg_ssstore_read_rows=None, avg_used_worker_count=None, avg_user_io_wait_time=None, avg_wait_count=None,
+                 avg_wait_time=None, client_ip=None, cpu_percentage=None, db_name=None, dist_plan_percentage=None, exec_ps=None,
+                 executions=None, fail_count=None, fail_percentage=None, inner=None, local_plan_percentage=None,
+                 max_affected_rows=None, max_application_wait_time=None, max_concurrency_wait_time=None, max_cpu_time=None,
+                 max_disk_reads=None, max_elapsed_time=None, max_return_rows=None, max_user_io_wait_time=None, max_wait_time=None,
+                 miss_plan_percentage=None, miss_plans=None, remote_plan_percentage=None, remote_plans=None, ret_code_4012count=None,
+                 ret_code_4013count=None, ret_code_5001count=None, ret_code_5024count=None, ret_code_5167count=None,
+                 ret_code_5217count=None, ret_code_6002count=None, retry_count=None, rpc_count=None, server=None, server_ip=None,
+                 server_port=None, sql_id=None, sql_text_short=None, sql_type=None, strong_consistency_percentage=None,
+                 sum_elapsed_time=None, sum_logical_reads=None, sum_wait_time=None, table_scan_percentage=None,
+                 total_wait_time=None, user_name=None, wait_event=None, weak_consistency_percentage=None):
+        self.avg_affected_rows = avg_affected_rows  # type: float
+        self.avg_application_wait_time = avg_application_wait_time  # type: float
+        self.avg_block_cache_hit = avg_block_cache_hit  # type: float
+        self.avg_block_index_cache_hit = avg_block_index_cache_hit  # type: float
+        self.avg_bloom_filter_cache_hit = avg_bloom_filter_cache_hit  # type: float
+        self.avg_concurrency_wait_time = avg_concurrency_wait_time  # type: float
+        self.avg_cpu_time = avg_cpu_time  # type: float
+        self.avg_decode_time = avg_decode_time  # type: float
+        self.avg_disk_reads = avg_disk_reads  # type: float
+        self.avg_elapsed_time = avg_elapsed_time  # type: float
+        self.avg_execute_time = avg_execute_time  # type: float
+        self.avg_executor_rpc_count = avg_executor_rpc_count  # type: float
+        self.avg_expected_worker_count = avg_expected_worker_count  # type: float
+        self.avg_get_plan_time = avg_get_plan_time  # type: float
+        self.avg_logical_reads = avg_logical_reads  # type: float
+        self.avg_memstore_read_rows = avg_memstore_read_rows  # type: float
+        self.avg_net_time = avg_net_time  # type: float
+        self.avg_net_wait_time = avg_net_wait_time  # type: float
+        self.avg_partition_count = avg_partition_count  # type: float
+        self.avg_queue_time = avg_queue_time  # type: float
+        self.avg_return_rows = avg_return_rows  # type: float
+        self.avg_row_cache_hit = avg_row_cache_hit  # type: float
+        self.avg_rpc_count = avg_rpc_count  # type: float
+        self.avg_schedule_time = avg_schedule_time  # type: float
+        self.avg_ssstore_read_rows = avg_ssstore_read_rows  # type: float
+        self.avg_used_worker_count = avg_used_worker_count  # type: float
+        self.avg_user_io_wait_time = avg_user_io_wait_time  # type: float
+        self.avg_wait_count = avg_wait_count  # type: float
+        self.avg_wait_time = avg_wait_time  # type: float
+        self.client_ip = client_ip  # type: str
+        self.cpu_percentage = cpu_percentage  # type: float
+        self.db_name = db_name  # type: str
+        self.dist_plan_percentage = dist_plan_percentage  # type: float
+        self.exec_ps = exec_ps  # type: float
+        self.executions = executions  # type: float
+        self.fail_count = fail_count  # type: float
+        self.fail_percentage = fail_percentage  # type: float
+        self.inner = inner  # type: bool
+        self.local_plan_percentage = local_plan_percentage  # type: float
+        self.max_affected_rows = max_affected_rows  # type: float
+        self.max_application_wait_time = max_application_wait_time  # type: float
+        self.max_concurrency_wait_time = max_concurrency_wait_time  # type: float
+        self.max_cpu_time = max_cpu_time  # type: float
+        self.max_disk_reads = max_disk_reads  # type: float
+        self.max_elapsed_time = max_elapsed_time  # type: float
+        self.max_return_rows = max_return_rows  # type: float
+        self.max_user_io_wait_time = max_user_io_wait_time  # type: float
+        self.max_wait_time = max_wait_time  # type: float
+        self.miss_plan_percentage = miss_plan_percentage  # type: float
+        self.miss_plans = miss_plans  # type: float
+        self.remote_plan_percentage = remote_plan_percentage  # type: float
+        self.remote_plans = remote_plans  # type: float
+        self.ret_code_4012count = ret_code_4012count  # type: long
+        self.ret_code_4013count = ret_code_4013count  # type: long
+        self.ret_code_5001count = ret_code_5001count  # type: long
+        self.ret_code_5024count = ret_code_5024count  # type: long
+        self.ret_code_5167count = ret_code_5167count  # type: long
+        self.ret_code_5217count = ret_code_5217count  # type: long
+        self.ret_code_6002count = ret_code_6002count  # type: long
+        self.retry_count = retry_count  # type: float
+        self.rpc_count = rpc_count  # type: float
+        self.server = server  # type: str
+        self.server_ip = server_ip  # type: str
+        self.server_port = server_port  # type: long
+        # SQL ID。
+        self.sql_id = sql_id  # type: str
+        self.sql_text_short = sql_text_short  # type: str
+        self.sql_type = sql_type  # type: str
+        self.strong_consistency_percentage = strong_consistency_percentage  # type: float
+        self.sum_elapsed_time = sum_elapsed_time  # type: float
+        self.sum_logical_reads = sum_logical_reads  # type: float
+        self.sum_wait_time = sum_wait_time  # type: float
+        self.table_scan_percentage = table_scan_percentage  # type: float
+        self.total_wait_time = total_wait_time  # type: float
+        self.user_name = user_name  # type: str
+        self.wait_event = wait_event  # type: str
+        self.weak_consistency_percentage = weak_consistency_percentage  # type: float
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeOasTopSQLListResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: list[DescribeOasTopSQLListResponseBodyData]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasTopSQLListResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeOasTopSQLListResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeOasTopSQLListResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, page_number=None, page_size=None, project_id=None, worker_grade_id=None):
         # The page number, which takes effect in a pagination query.
         self.page_number = page_number  # type: int
         # The page size, which takes effect in a pagination query.
         self.page_size = page_size  # type: int
         # The project ID.
@@ -9828,14 +12676,425 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeSQLPlansResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeSQLSamplesRequest(TeaModel):
+    def __init__(self, db_name=None, end_time=None, instance_id=None, sql_id=None, start_time=None, tenant_id=None):
+        self.db_name = db_name  # type: str
+        self.end_time = end_time  # type: str
+        self.instance_id = instance_id  # type: str
+        # SQL ID。
+        self.sql_id = sql_id  # type: str
+        self.start_time = start_time  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeSQLSamplesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, affected_rows=None, application_wait_time=None, block_cache_hit=None,
+                 block_index_cache_hit=None, bloom_filter_cache_hit=None, client_ip=None, client_port=None, concurrency_wait_time=None,
+                 consistency_level=None, cpu_time=None, db_name=None, decode_time=None, disk_reads=None, elapsed_time=None,
+                 execute_time=None, executor_rpc=None, expected_worker_count=None, get_plan_time=None, hit_plan=None, inner=None,
+                 memstore_read_rows=None, net_time=None, net_wait_time=None, ob_db_id=None, ob_server_id=None, ob_user_id=None,
+                 partition_count=None, plan_id=None, plan_type=None, queue_time=None, request_id=None, request_time=None,
+                 ret_code=None, retry_count=None, return_rows=None, row_cache_hit=None, rpc_count=None, schedule_time=None,
+                 server=None, sql_type=None, ssstore_read_rows=None, statement=None, table_scan=None, trace_id=None,
+                 trans_hash=None, used_worker_count=None, user_io_wait_time=None, user_name=None, wait_count=None,
+                 wait_event=None, wait_time=None):
+        self.affected_rows = affected_rows  # type: float
+        self.application_wait_time = application_wait_time  # type: float
+        self.block_cache_hit = block_cache_hit  # type: float
+        self.block_index_cache_hit = block_index_cache_hit  # type: float
+        self.bloom_filter_cache_hit = bloom_filter_cache_hit  # type: float
+        self.client_ip = client_ip  # type: str
+        self.client_port = client_port  # type: str
+        self.concurrency_wait_time = concurrency_wait_time  # type: float
+        self.consistency_level = consistency_level  # type: str
+        self.cpu_time = cpu_time  # type: float
+        self.db_name = db_name  # type: str
+        self.decode_time = decode_time  # type: float
+        self.disk_reads = disk_reads  # type: float
+        self.elapsed_time = elapsed_time  # type: float
+        self.execute_time = execute_time  # type: float
+        self.executor_rpc = executor_rpc  # type: float
+        self.expected_worker_count = expected_worker_count  # type: float
+        self.get_plan_time = get_plan_time  # type: float
+        self.hit_plan = hit_plan  # type: float
+        self.inner = inner  # type: bool
+        self.memstore_read_rows = memstore_read_rows  # type: float
+        self.net_time = net_time  # type: float
+        self.net_wait_time = net_wait_time  # type: float
+        self.ob_db_id = ob_db_id  # type: float
+        # server  ID。
+        self.ob_server_id = ob_server_id  # type: float
+        self.ob_user_id = ob_user_id  # type: float
+        self.partition_count = partition_count  # type: float
+        self.plan_id = plan_id  # type: float
+        self.plan_type = plan_type  # type: str
+        self.queue_time = queue_time  # type: float
+        self.request_id = request_id  # type: str
+        self.request_time = request_time  # type: str
+        self.ret_code = ret_code  # type: float
+        self.retry_count = retry_count  # type: float
+        self.return_rows = return_rows  # type: float
+        self.row_cache_hit = row_cache_hit  # type: float
+        self.rpc_count = rpc_count  # type: float
+        self.schedule_time = schedule_time  # type: float
+        self.server = server  # type: str
+        self.sql_type = sql_type  # type: str
+        self.ssstore_read_rows = ssstore_read_rows  # type: float
+        self.statement = statement  # type: str
+        self.table_scan = table_scan  # type: float
+        self.trace_id = trace_id  # type: str
+        # transaction hash。
+        self.trans_hash = trans_hash  # type: str
+        self.used_worker_count = used_worker_count  # type: float
+        self.user_io_wait_time = user_io_wait_time  # type: float
+        self.user_name = user_name  # type: str
+        self.wait_count = wait_count  # type: float
+        self.wait_event = wait_event  # type: str
+        self.wait_time = wait_time  # type: float
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeSQLSamplesResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: list[DescribeSQLSamplesResponseBodyData]
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            for k in self.data:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeSQLSamplesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeSQLSamplesResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeSQLSamplesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None):
         # The ID of the OceanBase cluster.
         self.instance_id = instance_id  # type: str
 
     def validate(self):
         pass
@@ -12122,14 +15381,163 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeTenantSecurityConfigsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeTenantSecurityIpGroupsRequest(TeaModel):
+    def __init__(self, instance_id=None, tenant_id=None):
+        self.instance_id = instance_id  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeTenantSecurityIpGroupsRequest, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('TenantId') is not None:
+            self.tenant_id = m.get('TenantId')
+        return self
+
+
+class DescribeTenantSecurityIpGroupsResponseBodySecurityIpGroups(TeaModel):
+    def __init__(self, security_ip_group_name=None, security_ip_group_type=None, security_ips=None, tenant_id=None):
+        self.security_ip_group_name = security_ip_group_name  # type: str
+        self.security_ip_group_type = security_ip_group_type  # type: str
+        self.security_ips = security_ips  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeTenantSecurityIpGroupsResponseBodySecurityIpGroups, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, security_ip_groups=None, total_count=None):
+        self.request_id = request_id  # type: str
+        self.security_ip_groups = security_ip_groups  # type: list[DescribeTenantSecurityIpGroupsResponseBodySecurityIpGroups]
+        self.total_count = total_count  # type: int
+
+    def validate(self):
+        if self.security_ip_groups:
+            for k in self.security_ip_groups:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeTenantSecurityIpGroupsResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeTenantSecurityIpGroupsResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeTenantSecurityIpGroupsResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, tags=None, tenant_ids=None):
         self.instance_id = instance_id  # type: str
         self.tags = tags  # type: str
         self.tenant_ids = tenant_ids  # type: str
 
     def validate(self):
@@ -15406,14 +18814,162 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyTenantResourceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ModifyTenantSecurityIpGroupRequest(TeaModel):
+    def __init__(self, instance_id=None, security_ip_group_name=None, security_ips=None, tenant_id=None):
+        self.instance_id = instance_id  # type: str
+        self.security_ip_group_name = security_ip_group_name  # type: str
+        self.security_ips = security_ips  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyTenantSecurityIpGroupRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, instance_id=None, security_ip_group_name=None, security_ips=None, tenant_id=None):
+        self.instance_id = instance_id  # type: str
+        self.security_ip_group_name = security_ip_group_name  # type: str
+        self.security_ips = security_ips  # type: str
+        self.tenant_id = tenant_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(ModifyTenantSecurityIpGroupResponseBodySecurityIpGroup, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None, security_ip_group=None):
+        self.request_id = request_id  # type: str
+        self.security_ip_group = security_ip_group  # type: ModifyTenantSecurityIpGroupResponseBodySecurityIpGroup
+
+    def validate(self):
+        if self.security_ip_group:
+            self.security_ip_group.validate()
+
+    def to_map(self):
+        _map = super(ModifyTenantSecurityIpGroupResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: ModifyTenantSecurityIpGroupResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(ModifyTenantSecurityIpGroupResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, tags=None, tenant_id=None):
         self.instance_id = instance_id  # type: str
         self.tags = tags  # type: str
         self.tenant_id = tenant_id  # type: str
 
     def validate(self):
@@ -18823,7 +22379,140 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = StopOmsOpenAPIProjectResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SwitchoverInstanceRequest(TeaModel):
+    def __init__(self, forced=None, instance_id=None, target_instance_id=None):
+        self.forced = forced  # type: bool
+        self.instance_id = instance_id  # type: str
+        self.target_instance_id = target_instance_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SwitchoverInstanceRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, message=None, success=None):
+        self.message = message  # type: str
+        self.success = success  # type: bool
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SwitchoverInstanceResponseBodyData, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('Success') is not None:
+            self.success = m.get('Success')
+        return self
+
+
+class SwitchoverInstanceResponseBody(TeaModel):
+    def __init__(self, data=None, request_id=None):
+        self.data = data  # type: SwitchoverInstanceResponseBodyData
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super(SwitchoverInstanceResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SwitchoverInstanceResponseBody
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SwitchoverInstanceResponse, self).to_map()
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
+    def from_map(self, m=None):
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

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO` & `alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-oceanbasepro20190901-py2
-Version: 1.0.3
+Version: 1.0.4
 Summary: Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.3/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt` & `alibabacloud_oceanbasepro20190901_py2-1.0.4/alibabacloud_oceanbasepro20190901_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_oceanbasepro20190901_py2-1.0.3/setup.py` & `alibabacloud_oceanbasepro20190901_py2-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_oceanbasepro20190901_py2.
 
-Created on 19/05/2023
+Created on 08/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_oceanbasepro20190901"
 NAME = "alibabacloud_oceanbasepro20190901_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud OceanBasePro (20190901) SDK Library for Python2"
```

