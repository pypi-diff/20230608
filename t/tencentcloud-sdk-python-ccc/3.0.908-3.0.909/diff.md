# Comparing `tmp/tencentcloud-sdk-python-ccc-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-ccc-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.908.tar", last modified: Wed Jun  7 00:18:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ccc-3.0.909.tar", last modified: Thu Jun  8 00:19:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ccc-3.0.908.tar` & `tencentcloud-sdk-python-ccc-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/
--rw-r--r--   0 root         (0) root         (0)    36406 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/ccc_client.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142129 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:18:48.000000 tencentcloud-sdk-python-ccc-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/ccc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/ccc/v20200210/
+-rw-r--r--   0 root         (0) root         (0)    36406 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/ccc/v20200210/ccc_client.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/ccc/v20200210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/ccc/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142398 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/ccc/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/ccc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud_sdk_python_ccc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud_sdk_python_ccc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud_sdk_python_ccc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/tencentcloud_sdk_python_ccc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:19:29.000000 tencentcloud-sdk-python-ccc-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.908/README.rst` & `tencentcloud-sdk-python-ccc-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/ccc_client.py` & `tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/ccc/v20200210/ccc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/errorcodes.py` & `tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/ccc/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/ccc/v20200210/models.py` & `tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/ccc/v20200210/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,34 +630,38 @@
         r"""
         :param SdkAppId: 应用 ID
         :type SdkAppId: int
         :param UserId: 客服用户 ID，一般为客服邮箱
         :type UserId: str
         :param Callee: 被叫号码，须带 0086 前缀
         :type Callee: str
-        :param Caller: 主叫号码，须带 0086 前缀
+        :param Caller: 主叫号码（废弃，使用Callers），须带 0086 前缀
         :type Caller: str
+        :param Callers: 指定主叫号码列表，如果前面的号码失败了会自动换成下一个号码，须带 0086 前缀
+        :type Callers: list of str
         :param IsForceUseMobile: 是否强制使用手机外呼，当前只支持 true，若为 true 请确保已配置白名单
         :type IsForceUseMobile: bool
         :param Uui: 自定义数据，长度限制 1024 字节
         :type Uui: str
         """
         self.SdkAppId = None
         self.UserId = None
         self.Callee = None
         self.Caller = None
+        self.Callers = None
         self.IsForceUseMobile = None
         self.Uui = None
 
 
     def _deserialize(self, params):
         self.SdkAppId = params.get("SdkAppId")
         self.UserId = params.get("UserId")
         self.Callee = params.get("Callee")
         self.Caller = params.get("Caller")
+        self.Callers = params.get("Callers")
         self.IsForceUseMobile = params.get("IsForceUseMobile")
         self.Uui = params.get("Uui")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ccc-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ccc-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.909/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.908/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ccc-3.0.909/tencentcloud_sdk_python_ccc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ccc
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Ccc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ccc-3.0.908/setup.py` & `tencentcloud-sdk-python-ccc-3.0.909/setup.py`

 * *Files identical despite different names*

