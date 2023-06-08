# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.908.tar", last modified: Wed Jun  7 00:20:11 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.909.tar", last modified: Thu Jun  8 00:20:55 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.908.tar` & `tencentcloud-sdk-python-ckafka-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   468693 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    70209 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:20:11.000000 tencentcloud-sdk-python-ckafka-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-08 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/ckafka/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-08 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   472962 2023-06-08 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    70499 2023-06-08 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/ckafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-08 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:20:55.000000 tencentcloud-sdk-python-ckafka-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.908/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2214,44 +2214,88 @@
 
     """
 
     def __init__(self):
         r"""
         :param InstanceName: 实例名称，是一个不超过 64 个字符的字符串，必须以字母为首字符，剩余部分可以包含字母、数字和横划线(-)
         :type InstanceName: str
-        :param BandWidth: 实例带宽
+        :param BandWidth: 实例内网峰值带宽。单位 MB/s。标准版需传入当前实例规格所对应的峰值带宽。注意如果创建的实例为专业版实例，峰值带宽，分区数等参数配置需要满足专业版的计费规格。
         :type BandWidth: int
-        :param VpcId: vpcId，不填默认基础网络
+        :param VpcId: 创建的实例默认接入点所在的 vpc 对应 vpcId。目前不支持创建基础网络实例，因此该参数必填
         :type VpcId: str
-        :param SubnetId: 子网id，vpc网络需要传该参数，基础网络可以不传
+        :param SubnetId: 子网id。创建实例默认接入点所在的子网对应的子网 id
         :type SubnetId: str
-        :param MsgRetentionTime: 可选。实例日志的最长保留时间，单位分钟，默认为10080（7天），最大30天，不填默认0，代表不开启日志保留时间回收策略
+        :param InstanceType: 实例规格。当创建标准版实例时必填，创建专业版实例时不需要填写。1：入门型；2：标准型；3：进阶型；4：容量型；5：高阶型1；6：高阶性2；7：高阶型3；8：高阶型4；9 ：独占型
+        :type InstanceType: int
+        :param MsgRetentionTime: 实例日志的默认最长保留时间，单位分钟。不传入该参数时默认为 1440 分钟（1天），最大30天。当 topic 显式设置消息保留时间时，以 topic 保留时间为准
         :type MsgRetentionTime: int
-        :param ZoneId: 可用区
-        :type ZoneId: int
-        :param ClusterId: 创建实例时可以选择集群Id, 该入参表示集群Id
+        :param ClusterId: 创建实例时可以选择集群Id, 该入参表示集群Id。不指定实例所在集群则不传入该参数
         :type ClusterId: int
+        :param KafkaVersion: 实例版本。目前支持 "0.10.2","1.1.1","2.4.2","2.8.1"
+        :type KafkaVersion: str
+        :param SpecificationsType: 实例类型。"standard"：标准版，"profession"：专业版
+        :type SpecificationsType: str
+        :param DiskType: 实例硬盘类型，"CLOUD_BASIC"：云硬盘，"CLOUD_SSD"：高速云硬盘。不传默认为 "CLOUD_BASIC"
+        :type DiskType: str
+        :param DiskSize: 实例硬盘大小，需要满足当前实例的计费规格
+        :type DiskSize: int
+        :param Partition: 实例最大分区数量，需要满足当前实例的计费规格
+        :type Partition: int
+        :param TopicNum: 实例最大 topic 数量，需要满足当前实例的计费规格
+        :type TopicNum: int
+        :param ZoneId: 实例所在的可用区。当创建多可用区实例时，该参数为创建的默认接入点所在的子网
+        :type ZoneId: int
+        :param MultiZoneFlag: 当前实例是否为多可用区实例。
+        :type MultiZoneFlag: bool
+        :param ZoneIds: 当实例为多可用区实例时，多可用区 id 列表。注意参数 ZoneId 对应的多可用区需要包含在该参数数组中
+        :type ZoneIds: list of int
+        :param InstanceNum: 购买实例数量。非必填，默认值为 1。当传入该参数时，会创建多个 instanceName 加后缀区分的实例
+        :type InstanceNum: int
+        :param PublicNetworkMonthly: 公网带宽大小，单位 Mbps。默认是没有加上免费 3Mbps 带宽。例如总共需要 3Mbps 公网带宽，此处传 0；总共需要 4Mbps 公网带宽，此处传 1
+        :type PublicNetworkMonthly: int
         """
         self.InstanceName = None
         self.BandWidth = None
         self.VpcId = None
         self.SubnetId = None
+        self.InstanceType = None
         self.MsgRetentionTime = None
-        self.ZoneId = None
         self.ClusterId = None
+        self.KafkaVersion = None
+        self.SpecificationsType = None
+        self.DiskType = None
+        self.DiskSize = None
+        self.Partition = None
+        self.TopicNum = None
+        self.ZoneId = None
+        self.MultiZoneFlag = None
+        self.ZoneIds = None
+        self.InstanceNum = None
+        self.PublicNetworkMonthly = None
 
 
     def _deserialize(self, params):
         self.InstanceName = params.get("InstanceName")
         self.BandWidth = params.get("BandWidth")
         self.VpcId = params.get("VpcId")
         self.SubnetId = params.get("SubnetId")
+        self.InstanceType = params.get("InstanceType")
         self.MsgRetentionTime = params.get("MsgRetentionTime")
-        self.ZoneId = params.get("ZoneId")
         self.ClusterId = params.get("ClusterId")
+        self.KafkaVersion = params.get("KafkaVersion")
+        self.SpecificationsType = params.get("SpecificationsType")
+        self.DiskType = params.get("DiskType")
+        self.DiskSize = params.get("DiskSize")
+        self.Partition = params.get("Partition")
+        self.TopicNum = params.get("TopicNum")
+        self.ZoneId = params.get("ZoneId")
+        self.MultiZoneFlag = params.get("MultiZoneFlag")
+        self.ZoneIds = params.get("ZoneIds")
+        self.InstanceNum = params.get("InstanceNum")
+        self.PublicNetworkMonthly = params.get("PublicNetworkMonthly")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -10342,20 +10386,27 @@
     """
 
     def __init__(self):
         r"""
         :param FlowId: FlowId11
 注意：此字段可能返回 null，表示取不到有效值。
         :type FlowId: int
+        :param RouteDTO: RouteIdDto
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RouteDTO: :class:`tencentcloud.ckafka.v20190819.models.RouteDTO`
         """
         self.FlowId = None
+        self.RouteDTO = None
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
+        if params.get("RouteDTO") is not None:
+            self.RouteDTO = RouteDTO()
+            self.RouteDTO._deserialize(params.get("RouteDTO"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -10980,14 +11031,39 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class RouteDTO(AbstractModel):
+    """RouteDTO
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RouteId: RouteId11
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RouteId: int
+        """
+        self.RouteId = None
+
+
+    def _deserialize(self, params):
+        self.RouteId = params.get("RouteId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class RouteResponse(AbstractModel):
     """路由信息返回对象
 
     """
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.908/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.909/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateInstancePost(self, request):
-        """创建按量计费实例
+        """由于出参需要更新，当前接口将会在未来版本中废弃，建议用户迁移使用 CreatePostPaidInstance 接口。创建按量计费实例。通常用于 SDK 或云 API 控制台调用接口，创建后付费 CKafka 实例。调用接口与在 CKafka 控制台购买按量付费实例效果相同。
 
         :param request: Request instance for CreateInstancePost.
         :type request: :class:`tencentcloud.ckafka.v20190819.models.CreateInstancePostRequest`
         :rtype: :class:`tencentcloud.ckafka.v20190819.models.CreateInstancePostResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.909/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.908/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.909/setup.py`

 * *Files identical despite different names*

