# Comparing `tmp/tencentcloud-sdk-python-partners-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-partners-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.907.tar", last modified: Tue Jun  6 02:32:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.908.tar", last modified: Wed Jun  7 00:29:41 2023, max compression
```

## Comparing `tencentcloud-sdk-python-partners-3.0.907.tar` & `tencentcloud-sdk-python-partners-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud/partners/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud/partners/v20180321/
--rw-r--r--   0 root         (0) root         (0)      885 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud/partners/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud/partners/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84247 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud/partners/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)    23568 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud/partners/v20180321/partners_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud/partners/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud_sdk_python_partners.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/tencentcloud_sdk_python_partners.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:32:06.000000 tencentcloud-sdk-python-partners-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud/partners/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud/partners/v20180321/
+-rw-r--r--   0 root         (0) root         (0)      885 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud/partners/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud/partners/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84247 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud/partners/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)    23877 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud/partners/v20180321/partners_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud/partners/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud_sdk_python_partners.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/tencentcloud_sdk_python_partners.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:29:41.000000 tencentcloud-sdk-python-partners-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-partners-3.0.907/README.rst` & `tencentcloud-sdk-python-partners-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.907/tencentcloud/partners/v20180321/errorcodes.py` & `tencentcloud-sdk-python-partners-3.0.908/tencentcloud/partners/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.907/tencentcloud/partners/v20180321/models.py` & `tencentcloud-sdk-python-partners-3.0.908/tencentcloud/partners/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.907/tencentcloud/partners/v20180321/partners_client.py` & `tencentcloud-sdk-python-partners-3.0.908/tencentcloud/partners/v20180321/partners_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeAgentDealsCache(self, request):
-        """【该接口已下线，请使用升级版本DescribeAgentDealsByCache】代理商拉取缓存的全量客户订单
+        """已提供新接口并推动切换，改切口目前白名单限制所有访问，申请下线
+
+        【该接口已下线，请使用升级版本DescribeAgentDealsByCache】代理商拉取缓存的全量客户订单
 
         :param request: Request instance for DescribeAgentDealsCache.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentDealsCacheRequest`
         :rtype: :class:`tencentcloud.partners.v20180321.models.DescribeAgentDealsCacheResponse`
 
         """
         try:
@@ -279,15 +281,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeAgentPayDeals(self, request):
-        """【该接口已下线，请切换使用升级版本DescribeAgentPayDealsV2】可以查询代理商代付的所有订单
+        """已提供新接口并推动切换，改切口目前白名单限制所有访问，申请下线
+
+        【该接口已下线，请切换使用升级版本DescribeAgentPayDealsV2】可以查询代理商代付的所有订单
 
         :param request: Request instance for DescribeAgentPayDeals.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentPayDealsRequest`
         :rtype: :class:`tencentcloud.partners.v20180321.models.DescribeAgentPayDealsResponse`
 
         """
         try:
@@ -325,15 +329,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeAgentSelfPayDeals(self, request):
-        """【该接口已下线，请切换使用升级版本DescribeAgentSelfPayDealsV2】可以查询代理商下指定客户的自付订单
+        """已提供新接口并推动切换，改切口目前白名单限制所有访问，申请下线
+
+        【该接口已下线，请切换使用升级版本DescribeAgentSelfPayDealsV2】可以查询代理商下指定客户的自付订单
 
         :param request: Request instance for DescribeAgentSelfPayDeals.
         :type request: :class:`tencentcloud.partners.v20180321.models.DescribeAgentSelfPayDealsRequest`
         :rtype: :class:`tencentcloud.partners.v20180321.models.DescribeAgentSelfPayDealsResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-partners-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-partners-3.0.908/tencentcloud/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.907'
+__version__ = '3.0.908'
```

### Comparing `tencentcloud-sdk-python-partners-3.0.907/tencentcloud_sdk_python_partners.egg-info/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.908/tencentcloud_sdk_python_partners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-partners-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.908/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-partners-3.0.907/setup.py` & `tencentcloud-sdk-python-partners-3.0.908/setup.py`

 * *Files identical despite different names*

