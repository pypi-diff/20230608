# Comparing `tmp/tencentcloud-sdk-python-mps-3.0.907.tar.gz` & `tmp/tencentcloud-sdk-python-mps-3.0.908.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.907.tar", last modified: Tue Jun  6 02:31:03 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.908.tar", last modified: Wed Jun  7 00:28:40 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mps-3.0.907.tar` & `tencentcloud-sdk-python-mps-3.0.908.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud/mps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)    89746 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)    13373 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud/mps/v20190612/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)   814885 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud/mps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud_sdk_python_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/tencentcloud_sdk_python_mps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:31:03.000000 tencentcloud-sdk-python-mps-3.0.907/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud/mps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)    90653 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)    13373 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud/mps/v20190612/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   817037 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud/mps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud_sdk_python_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/tencentcloud_sdk_python_mps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:28:40.000000 tencentcloud-sdk-python-mps-3.0.908/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mps-3.0.907/README.rst` & `tencentcloud-sdk-python-mps-3.0.908/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.907/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mps-3.0.908/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mps-3.0.907/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-mps-3.0.908/tencentcloud/mps/v20190612/mps_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,14 +286,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateStreamLinkInput(self, request):
+        """创建媒体传输的输入配置。
+
+        :param request: Request instance for CreateStreamLinkInput.
+        :type request: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkInputRequest`
+        :rtype: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkInputResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateStreamLinkInput", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateStreamLinkInputResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateStreamLinkOutputInfo(self, request):
         """创建媒体传输流的输出信息。
 
         :param request: Request instance for CreateStreamLinkOutputInfo.
         :type request: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkOutputInfoRequest`
         :rtype: :class:`tencentcloud.mps.v20190612.models.CreateStreamLinkOutputInfoResponse`
```

### Comparing `tencentcloud-sdk-python-mps-3.0.907/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-mps-3.0.908/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.907/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-mps-3.0.908/tencentcloud/mps/v20190612/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6244,14 +6244,70 @@
     def _deserialize(self, params):
         if params.get("Info") is not None:
             self.Info = DescribeFlow()
             self.Info._deserialize(params.get("Info"))
         self.RequestId = params.get("RequestId")
 
 
+class CreateStreamLinkInputRequest(AbstractModel):
+    """CreateStreamLinkInput请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 媒体传输流ID。
+        :type FlowId: str
+        :param InputGroup: 流的输入组。
+        :type InputGroup: list of CreateInput
+        """
+        self.FlowId = None
+        self.InputGroup = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        if params.get("InputGroup") is not None:
+            self.InputGroup = []
+            for item in params.get("InputGroup"):
+                obj = CreateInput()
+                obj._deserialize(item)
+                self.InputGroup.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateStreamLinkInputResponse(AbstractModel):
+    """CreateStreamLinkInput返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Info: 创建的Flow信息。
+        :type Info: :class:`tencentcloud.mps.v20190612.models.DescribeFlow`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Info = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Info") is not None:
+            self.Info = DescribeFlow()
+            self.Info._deserialize(params.get("Info"))
+        self.RequestId = params.get("RequestId")
+
+
 class CreateStreamLinkOutputInfoRequest(AbstractModel):
     """CreateStreamLinkOutputInfo请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -16874,26 +16930,29 @@
         :type OutputDir: str
         :param AiContentReviewTask: 视频内容审核类型任务参数。
         :type AiContentReviewTask: :class:`tencentcloud.mps.v20190612.models.AiContentReviewTaskInput`
         :param AiRecognitionTask: 视频内容识别类型任务参数。
         :type AiRecognitionTask: :class:`tencentcloud.mps.v20190612.models.AiRecognitionTaskInput`
         :param AiAnalysisTask: 视频内容分析类型任务参数。
         :type AiAnalysisTask: :class:`tencentcloud.mps.v20190612.models.AiAnalysisTaskInput`
+        :param AiQualityControlTask: 视频内容质检类型任务参数。
+        :type AiQualityControlTask: :class:`tencentcloud.mps.v20190612.models.AiQualityControlTaskInput`
         :param SessionId: 用于去重的识别码，如果七天内曾有过相同的识别码的请求，则本次的请求会返回错误。最长 50 个字符，不带或者带空字符串表示不做去重。
         :type SessionId: str
         :param SessionContext: 来源上下文，用于透传用户请求信息，任务流状态变更回调将返回该字段值，最长 1000 个字符。
         :type SessionContext: str
         """
         self.Url = None
         self.TaskNotifyConfig = None
         self.OutputStorage = None
         self.OutputDir = None
         self.AiContentReviewTask = None
         self.AiRecognitionTask = None
         self.AiAnalysisTask = None
+        self.AiQualityControlTask = None
         self.SessionId = None
         self.SessionContext = None
 
 
     def _deserialize(self, params):
         self.Url = params.get("Url")
         if params.get("TaskNotifyConfig") is not None:
@@ -16908,14 +16967,17 @@
             self.AiContentReviewTask._deserialize(params.get("AiContentReviewTask"))
         if params.get("AiRecognitionTask") is not None:
             self.AiRecognitionTask = AiRecognitionTaskInput()
             self.AiRecognitionTask._deserialize(params.get("AiRecognitionTask"))
         if params.get("AiAnalysisTask") is not None:
             self.AiAnalysisTask = AiAnalysisTaskInput()
             self.AiAnalysisTask._deserialize(params.get("AiAnalysisTask"))
+        if params.get("AiQualityControlTask") is not None:
+            self.AiQualityControlTask = AiQualityControlTaskInput()
+            self.AiQualityControlTask._deserialize(params.get("AiQualityControlTask"))
         self.SessionId = params.get("SessionId")
         self.SessionContext = params.get("SessionContext")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
```

### Comparing `tencentcloud-sdk-python-mps-3.0.907/tencentcloud_sdk_python_mps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.908/tencentcloud_sdk_python_mps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.907/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.908/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.907
+Version: 3.0.908
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.907/setup.py` & `tencentcloud-sdk-python-mps-3.0.908/setup.py`

 * *Files identical despite different names*

