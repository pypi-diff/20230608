# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.907.tar", last modified: Tue Jun  6 02:26:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.908.tar", last modified: Wed Jun  7 00:24:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.907.tar` & `tencentcloud-sdk-python-ess-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:26:46.000000 tencentcloud-sdk-python-ess-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:26:46.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:26:46.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    51319 2023-06-06 02:26:46.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24361 2023-06-06 02:26:46.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:26:46.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   228117 2023-06-06 02:26:46.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:26:46.000000 tencentcloud-sdk-python-ess-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:26:47.000000 tencentcloud-sdk-python-ess-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    51319 2023-06-07 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24361 2023-06-07 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   228359 2023-06-07 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:24:10.000000 tencentcloud-sdk-python-ess-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:24:11.000000 tencentcloud-sdk-python-ess-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.907/README.rst` & `tencentcloud-sdk-python-ess-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.907/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.908/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.907/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.908/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.907/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.908/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5154,24 +5154,30 @@
         :param Name: 签署人姓名，最大长度50个字符
 
         :type Name: str
         :param Mobile: 签署人手机号
         :type Mobile: str
         :param RelievedApproverReceiptId: 要替换的参与人在原合同参与人列表中的签署人编号,通过DescribeFlowInfo 接口获取（即FlowDetailInfos. FlowApproverInfos 结构中的ReceiptId ）
         :type RelievedApproverReceiptId: str
+        :param ApproverType: 指定签署人类型，目前仅支持
+ORGANIZATION-企业
+ENTERPRISESERVER-企业静默签
+        :type ApproverType: str
         """
         self.Name = None
         self.Mobile = None
         self.RelievedApproverReceiptId = None
+        self.ApproverType = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.Mobile = params.get("Mobile")
         self.RelievedApproverReceiptId = params.get("RelievedApproverReceiptId")
+        self.ApproverType = params.get("ApproverType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ess-3.0.907/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.908/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.908/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.907/setup.py` & `tencentcloud-sdk-python-ess-3.0.908/setup.py`

 * *Files identical despite different names*

