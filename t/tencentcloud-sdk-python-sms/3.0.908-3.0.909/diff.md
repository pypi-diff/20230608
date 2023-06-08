# Comparing `tmp/tencentcloud-sdk-python-sms-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-sms-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.908.tar", last modified: Wed Jun  7 00:31:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.909.tar", last modified: Thu Jun  8 00:31:58 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sms-3.0.908.tar` & `tencentcloud-sdk-python-sms-3.0.909.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/
--rw-r--r--   0 root         (0) root         (0)    26567 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/sms_client.py
--rw-r--r--   0 root         (0) root         (0)    18520 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60142 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/
--rw-r--r--   0 root         (0) root         (0)    28333 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/sms_client.py
--rw-r--r--   0 root         (0) root         (0)    19342 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68439 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:31:06.000000 tencentcloud-sdk-python-sms-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20190711/
+-rw-r--r--   0 root         (0) root         (0)    26567 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20190711/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)    18520 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20190711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20190711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60142 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20190711/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20210111/
+-rw-r--r--   0 root         (0) root         (0)    28333 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20210111/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)    19342 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20210111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20210111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68439 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20210111/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud_sdk_python_sms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/tencentcloud_sdk_python_sms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:31:58.000000 tencentcloud-sdk-python-sms-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-sms-3.0.908/README.rst` & `tencentcloud-sdk-python-sms-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20190711/sms_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifySmsSign(self, request):
-        """1. 修改短信签名，修改之前请先认证参阅 [腾讯云短信签名审核标准](https://cloud.tencent.com/document/product/382/39022)。
+        """1. 修改短信签名，修改之前请先认真参阅 [腾讯云短信签名审核标准](https://cloud.tencent.com/document/product/382/39022)。
         2. ⚠️注意：个人认证用户不支持使用 API 修改短信签名，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)，如果为个人认证请登录 [控制台](https://console.cloud.tencent.com/smsv2) 修改短信签名。
         3. 修改短信签名，仅当签名为**待审核**或**已拒绝**状态时，才能进行修改，**已审核通过**的签名不支持修改。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 [SDK](https://cloud.tencent.com/document/product/382/43193) 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2019-07-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
         :param request: Request instance for ModifySmsSign.
         :type request: :class:`tencentcloud.sms.v20190711.models.ModifySmsSignRequest`
```

### Comparing `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20190711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20190711/models.py` & `tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20190711/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20210111/sms_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ModifySmsSign(self, request):
-        """1. 修改短信签名，修改之前请先认证参阅 [腾讯云短信签名审核标准](https://cloud.tencent.com/document/product/382/39022)。
+        """1. 修改短信签名，修改之前请先认真参阅 [腾讯云短信签名审核标准](https://cloud.tencent.com/document/product/382/39022)。
         2. ⚠️注意：个人认证用户不支持使用 API 修改短信签名，请参阅了解 [实名认证基本介绍](https://cloud.tencent.com/document/product/378/3629)，如果为个人认证请登录 [控制台](https://console.cloud.tencent.com/smsv2) 修改短信签名。
         3. 修改短信签名，仅当签名为**待审核**或**已拒绝**状态时，才能进行修改，**已审核通过**的签名不支持修改。
         >- 注：由于云 **API3.0 安全性**有所提升，所以**接口鉴权**较为复杂，建议使用 SDK 来使用云短信服务。
         >- 您可以在 [API 3.0 Explorer](https://console.cloud.tencent.com/api/explorer?Product=sms&Version=2021-01-11&Action=SendSms) 中直接运行该接口，可以先免去签名计算步骤。运行成功后，API Explorer可以**自动生成**SDK代码示例。
 
         :param request: Request instance for ModifySmsSign.
         :type request: :class:`tencentcloud.sms.v20210111.models.ModifySmsSignRequest`
```

### Comparing `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20210111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/sms/v20210111/models.py` & `tencentcloud-sdk-python-sms-3.0.909/tencentcloud/sms/v20210111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sms-3.0.909/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.908'
+__version__ = '3.0.909'
```

### Comparing `tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-sms-3.0.909/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.908/tencentcloud_sdk_python_sms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.909/tencentcloud_sdk_python_sms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.909/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.908/setup.py` & `tencentcloud-sdk-python-sms-3.0.909/setup.py`

 * *Files identical despite different names*

