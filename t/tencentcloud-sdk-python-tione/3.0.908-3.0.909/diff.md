# Comparing `tmp/tencentcloud-sdk-python-tione-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-tione-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.908.tar", last modified: Wed Jun  7 00:34:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tione-3.0.909.tar", last modified: Thu Jun  8 00:35:36 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tione-3.0.908.tar` & `tencentcloud-sdk-python-tione-3.0.909.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)    51024 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20211111/tione_client.py
--rw-r--r--   0 root         (0) root         (0)    11488 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   335349 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20211111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)    22010 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20191022/tione_client.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91250 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1010 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud_sdk_python_tione.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      633 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1669 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:34:37.000000 tencentcloud-sdk-python-tione-3.0.908/tencentcloud_sdk_python_tione.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)    51024 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20211111/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)    11488 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   336462 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20211111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)    22010 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20191022/tione_client.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91250 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud_sdk_python_tione.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud_sdk_python_tione.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      633 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud_sdk_python_tione.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:35:36.000000 tencentcloud-sdk-python-tione-3.0.909/tencentcloud_sdk_python_tione.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-tione-3.0.908/README.rst` & `tencentcloud-sdk-python-tione-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tione-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20211111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4514,25 +4514,31 @@
 
     def __init__(self):
         r"""
         :param PodNames: pod名称列表
         :type PodNames: list of str
         :param TotalCount: 数量
         :type TotalCount: int
+        :param PodInfoList: pod详细信息
+        :type PodInfoList: :class:`tencentcloud.tione.v20211111.models.PodInfo`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.PodNames = None
         self.TotalCount = None
+        self.PodInfoList = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.PodNames = params.get("PodNames")
         self.TotalCount = params.get("TotalCount")
+        if params.get("PodInfoList") is not None:
+            self.PodInfoList = PodInfo()
+            self.PodInfoList._deserialize(params.get("PodInfoList"))
         self.RequestId = params.get("RequestId")
 
 
 class DescribeTrainingTaskRequest(AbstractModel):
     """DescribeTrainingTask请求参数结构体
 
     """
@@ -6344,14 +6350,44 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class PodInfo(AbstractModel):
+    """任务建模Pod信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Name: pod名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param IP: pod的IP
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IP: str
+        """
+        self.Name = None
+        self.IP = None
+
+
+    def _deserialize(self, params):
+        self.Name = params.get("Name")
+        self.IP = params.get("IP")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class PointInfo(AbstractModel):
     """点信息描述
 
     """
```

### Comparing `tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.908/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-tione-3.0.909/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.909/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tione-3.0.908/setup.py` & `tencentcloud-sdk-python-tione-3.0.909/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.908/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tione-3.0.909/tencentcloud_sdk_python_tione.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tione-3.0.908/tencentcloud_sdk_python_tione.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tione-3.0.909/tencentcloud_sdk_python_tione.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tione
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Tione SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

