# Comparing `tmp/tencentcloud-sdk-python-wedata-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-wedata-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.908.tar", last modified: Wed Jun  7 00:36:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.909.tar", last modified: Thu Jun  8 00:38:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wedata-3.0.908.tar` & `tencentcloud-sdk-python-wedata-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/wedata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)     3323 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)   184325 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)   717295 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud_sdk_python_wedata.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:36:55.000000 tencentcloud-sdk-python-wedata-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-08 00:38:31.000000 tencentcloud-sdk-python-wedata-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:38:31.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)     3451 2023-06-08 00:38:31.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:38:31.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185172 2023-06-08 00:38:31.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)   725096 2023-06-08 00:38:31.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:38:31.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud_sdk_python_wedata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-08 00:38:31.000000 tencentcloud-sdk-python-wedata-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:38:32.000000 tencentcloud-sdk-python-wedata-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.908/README.rst` & `tencentcloud-sdk-python-wedata-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # ClientIp未被授权。
 INVALIDPARAMETER_CLIENTIPNOTAUTHORIZED = 'InvalidParameter.ClientIpNotAuthorized'
 
+# 数据引擎实例不存在。
+INVALIDPARAMETER_DATAENGINEINSTANCENOTEXISTS = 'InvalidParameter.DataEngineInstanceNotExists'
+
 # 名称重复。
 INVALIDPARAMETER_DUPLICATENAME = 'InvalidParameter.DuplicateName'
 
 # 查询过滤条件参数错误。
 INVALIDPARAMETER_INVALIDFILTERPARAMETER = 'InvalidParameter.InvalidFilterParameter'
 
 # 规则不存在。
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -4573,8 +4573,31 @@
             model = models.UpdateInLongAgentResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UploadContent(self, request):
+        """保存任务信息
+
+        :param request: Request instance for UploadContent.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.UploadContentRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.UploadContentResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UploadContent", params, headers=headers)
+            response = json.loads(body)
+            model = models.UploadContentResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
                 raise TencentCloudSDKException(e.message, e.message)
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/wedata/v20210820/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -18216,14 +18216,181 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ScriptInfoResponse(AbstractModel):
+    """开发空间-脚本相关响应
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ResourceId: 资源id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceId: str
+        :param FileName: 脚本名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileName: str
+        :param FileExtensionType: 文件扩展名类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FileExtensionType: str
+        :param Type: 文件类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: str
+        :param Md5Value: md5值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Md5Value: str
+        :param CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param UpdateTime: 更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param Size: 文件大小
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Size: float
+        :param LocalPath: 本地路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LocalPath: str
+        :param RemotePath: 远程路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RemotePath: str
+        :param OwnerName: 用户名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OwnerName: str
+        :param Owner: 用户id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Owner: str
+        :param PathDepth: 路径深度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PathDepth: int
+        :param ProjectId: 项目id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProjectId: str
+        :param ExtraInfo: 附加信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExtraInfo: str
+        :param LocalTempPath: 本地临时文件路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LocalTempPath: str
+        :param ZipPath: 本地压缩文件路径
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ZipPath: str
+        :param Bucket: cos桶名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Bucket: str
+        :param Region: cos地区
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        """
+        self.ResourceId = None
+        self.FileName = None
+        self.FileExtensionType = None
+        self.Type = None
+        self.Md5Value = None
+        self.CreateTime = None
+        self.UpdateTime = None
+        self.Size = None
+        self.LocalPath = None
+        self.RemotePath = None
+        self.OwnerName = None
+        self.Owner = None
+        self.PathDepth = None
+        self.ProjectId = None
+        self.ExtraInfo = None
+        self.LocalTempPath = None
+        self.ZipPath = None
+        self.Bucket = None
+        self.Region = None
+
+
+    def _deserialize(self, params):
+        self.ResourceId = params.get("ResourceId")
+        self.FileName = params.get("FileName")
+        self.FileExtensionType = params.get("FileExtensionType")
+        self.Type = params.get("Type")
+        self.Md5Value = params.get("Md5Value")
+        self.CreateTime = params.get("CreateTime")
+        self.UpdateTime = params.get("UpdateTime")
+        self.Size = params.get("Size")
+        self.LocalPath = params.get("LocalPath")
+        self.RemotePath = params.get("RemotePath")
+        self.OwnerName = params.get("OwnerName")
+        self.Owner = params.get("Owner")
+        self.PathDepth = params.get("PathDepth")
+        self.ProjectId = params.get("ProjectId")
+        self.ExtraInfo = params.get("ExtraInfo")
+        self.LocalTempPath = params.get("LocalTempPath")
+        self.ZipPath = params.get("ZipPath")
+        self.Bucket = params.get("Bucket")
+        self.Region = params.get("Region")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ScriptRequestInfo(AbstractModel):
+    """开发空间-上传脚本请求
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FilePath: 脚本路径
+        :type FilePath: str
+        :param ProjectId: 项目id
+        :type ProjectId: str
+        :param Version: 脚本版本
+        :type Version: str
+        :param Operation: 操作类型
+        :type Operation: str
+        :param ExtraInfo: 额外信息
+        :type ExtraInfo: str
+        :param BucketName: 桶名称
+        :type BucketName: str
+        :param Region: 所属地区
+        :type Region: str
+        :param FileExtensionType: 文件扩展类型
+        :type FileExtensionType: str
+        """
+        self.FilePath = None
+        self.ProjectId = None
+        self.Version = None
+        self.Operation = None
+        self.ExtraInfo = None
+        self.BucketName = None
+        self.Region = None
+        self.FileExtensionType = None
+
+
+    def _deserialize(self, params):
+        self.FilePath = params.get("FilePath")
+        self.ProjectId = params.get("ProjectId")
+        self.Version = params.get("Version")
+        self.Operation = params.get("Operation")
+        self.ExtraInfo = params.get("ExtraInfo")
+        self.BucketName = params.get("BucketName")
+        self.Region = params.get("Region")
+        self.FileExtensionType = params.get("FileExtensionType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class SearchCondition(AbstractModel):
     """查询实例条件
 
     """
 
     def __init__(self):
         r"""
@@ -20799,14 +20966,64 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class UploadContentRequest(AbstractModel):
+    """UploadContent请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ScriptRequestInfo: 脚本上传信息
+        :type ScriptRequestInfo: :class:`tencentcloud.wedata.v20210820.models.ScriptRequestInfo`
+        """
+        self.ScriptRequestInfo = None
+
+
+    def _deserialize(self, params):
+        if params.get("ScriptRequestInfo") is not None:
+            self.ScriptRequestInfo = ScriptRequestInfo()
+            self.ScriptRequestInfo._deserialize(params.get("ScriptRequestInfo"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UploadContentResponse(AbstractModel):
+    """UploadContent返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ScriptInfo: 脚本信息响应
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ScriptInfo: :class:`tencentcloud.wedata.v20210820.models.ScriptInfoResponse`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.ScriptInfo = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("ScriptInfo") is not None:
+            self.ScriptInfo = ScriptInfoResponse()
+            self.ScriptInfo._deserialize(params.get("ScriptInfo"))
+        self.RequestId = params.get("RequestId")
+
+
 class UserFileDTO(AbstractModel):
     """用户文件信息
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wedata-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wedata-3.0.908/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.909/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.909/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.908/setup.py` & `tencentcloud-sdk-python-wedata-3.0.909/setup.py`

 * *Files identical despite different names*

