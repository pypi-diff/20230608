# Comparing `tmp/tencentcloud-sdk-python-tdmq-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-tdmq-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.908.tar", last modified: Wed Jun  7 00:33:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tdmq-3.0.909.tar", last modified: Thu Jun  8 00:34:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tdmq-3.0.908.tar` & `tencentcloud-sdk-python-tdmq-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)   103763 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/tdmq/v20200217/tdmq_client.py
--rw-r--r--   0 root         (0) root         (0)    10117 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   384881 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud_sdk_python_tdmq.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:33:37.000000 tencentcloud-sdk-python-tdmq-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)   103792 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/tdmq/v20200217/tdmq_client.py
+-rw-r--r--   0 root         (0) root         (0)    10117 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   385664 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud_sdk_python_tdmq.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud_sdk_python_tdmq.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud_sdk_python_tdmq.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud_sdk_python_tdmq.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:34:31.000000 tencentcloud-sdk-python-tdmq-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.908/README.rst` & `tencentcloud-sdk-python-tdmq-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2567,14 +2567,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def SendMessages(self, request):
         """发送单条消息
+        不支持持久topic
 
         :param request: Request instance for SendMessages.
         :type request: :class:`tencentcloud.tdmq.v20200217.models.SendMessagesRequest`
         :rtype: :class:`tencentcloud.tdmq.v20200217.models.SendMessagesResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/tdmq/v20200217/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1989,30 +1989,34 @@
         :type MsgTTL: int
         :param Remark: 说明，128个字符以内。
         :type Remark: str
         :param ClusterId: Pulsar 集群的ID
         :type ClusterId: str
         :param RetentionPolicy: 消息保留策略
         :type RetentionPolicy: :class:`tencentcloud.tdmq.v20200217.models.RetentionPolicy`
+        :param AutoSubscriptionCreation: 是否开启自动创建订阅
+        :type AutoSubscriptionCreation: bool
         """
         self.EnvironmentId = None
         self.MsgTTL = None
         self.Remark = None
         self.ClusterId = None
         self.RetentionPolicy = None
+        self.AutoSubscriptionCreation = None
 
 
     def _deserialize(self, params):
         self.EnvironmentId = params.get("EnvironmentId")
         self.MsgTTL = params.get("MsgTTL")
         self.Remark = params.get("Remark")
         self.ClusterId = params.get("ClusterId")
         if params.get("RetentionPolicy") is not None:
             self.RetentionPolicy = RetentionPolicy()
             self.RetentionPolicy._deserialize(params.get("RetentionPolicy"))
+        self.AutoSubscriptionCreation = params.get("AutoSubscriptionCreation")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6612,38 +6616,43 @@
         :type NamespaceName: str
         :param TopicNum: Topic数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type TopicNum: int
         :param RetentionPolicy: 消息保留策略
 注意：此字段可能返回 null，表示取不到有效值。
         :type RetentionPolicy: :class:`tencentcloud.tdmq.v20200217.models.RetentionPolicy`
+        :param AutoSubscriptionCreation: 是否自动创建订阅
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AutoSubscriptionCreation: bool
         """
         self.EnvironmentId = None
         self.Remark = None
         self.MsgTTL = None
         self.CreateTime = None
         self.UpdateTime = None
         self.NamespaceId = None
         self.NamespaceName = None
         self.TopicNum = None
         self.RetentionPolicy = None
+        self.AutoSubscriptionCreation = None
 
 
     def _deserialize(self, params):
         self.EnvironmentId = params.get("EnvironmentId")
         self.Remark = params.get("Remark")
         self.MsgTTL = params.get("MsgTTL")
         self.CreateTime = params.get("CreateTime")
         self.UpdateTime = params.get("UpdateTime")
         self.NamespaceId = params.get("NamespaceId")
         self.NamespaceName = params.get("NamespaceName")
         self.TopicNum = params.get("TopicNum")
         if params.get("RetentionPolicy") is not None:
             self.RetentionPolicy = RetentionPolicy()
             self.RetentionPolicy._deserialize(params.get("RetentionPolicy"))
+        self.AutoSubscriptionCreation = params.get("AutoSubscriptionCreation")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -7437,30 +7446,34 @@
         :type MsgTTL: int
         :param Remark: 备注，字符串最长不超过128。
         :type Remark: str
         :param ClusterId: 集群ID
         :type ClusterId: str
         :param RetentionPolicy: 消息保留策略
         :type RetentionPolicy: :class:`tencentcloud.tdmq.v20200217.models.RetentionPolicy`
+        :param AutoSubscriptionCreation: 是否开启自动创建订阅
+        :type AutoSubscriptionCreation: bool
         """
         self.EnvironmentId = None
         self.MsgTTL = None
         self.Remark = None
         self.ClusterId = None
         self.RetentionPolicy = None
+        self.AutoSubscriptionCreation = None
 
 
     def _deserialize(self, params):
         self.EnvironmentId = params.get("EnvironmentId")
         self.MsgTTL = params.get("MsgTTL")
         self.Remark = params.get("Remark")
         self.ClusterId = params.get("ClusterId")
         if params.get("RetentionPolicy") is not None:
             self.RetentionPolicy = RetentionPolicy()
             self.RetentionPolicy._deserialize(params.get("RetentionPolicy"))
+        self.AutoSubscriptionCreation = params.get("AutoSubscriptionCreation")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tdmq-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.909/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.908/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tdmq-3.0.909/tencentcloud_sdk_python_tdmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tdmq
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Tdmq SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tdmq-3.0.908/setup.py` & `tencentcloud-sdk-python-tdmq-3.0.909/setup.py`

 * *Files identical despite different names*

