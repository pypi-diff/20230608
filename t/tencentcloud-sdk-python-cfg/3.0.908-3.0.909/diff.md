# Comparing `tmp/tencentcloud-sdk-python-cfg-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-cfg-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfg-3.0.908.tar", last modified: Wed Jun  7 00:19:24 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfg-3.0.909.tar", last modified: Thu Jun  8 00:20:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfg-3.0.908.tar` & `tencentcloud-sdk-python-cfg-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/cfg/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/cfg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/cfg/v20210820/
--rw-r--r--   0 root         (0) root         (0)     1933 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/cfg/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9695 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/cfg/v20210820/cfg_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/cfg/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63543 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/cfg/v20210820/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud_sdk_python_cfg.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud_sdk_python_cfg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud_sdk_python_cfg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/tencentcloud_sdk_python_cfg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:19:24.000000 tencentcloud-sdk-python-cfg-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/cfg/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/cfg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/cfg/v20210820/
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/cfg/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9695 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/cfg/v20210820/cfg_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/cfg/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66207 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/cfg/v20210820/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud_sdk_python_cfg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud_sdk_python_cfg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud_sdk_python_cfg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/tencentcloud_sdk_python_cfg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:20:09.000000 tencentcloud-sdk-python-cfg-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.908/README.rst` & `tencentcloud-sdk-python-cfg-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/cfg/v20210820/errorcodes.py` & `tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/cfg/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/cfg/v20210820/cfg_client.py` & `tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/cfg/v20210820/cfg_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfg-3.0.908/tencentcloud/cfg/v20210820/models.py` & `tencentcloud-sdk-python-cfg-3.0.909/tencentcloud/cfg/v20210820/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -897,25 +897,36 @@
         :type TaskGroupUpdateTime: str
         :param TaskGroupActions: 动作分组动作列表
         :type TaskGroupActions: list of TaskGroupAction
         :param TaskGroupInstanceList: 实例列表
         :type TaskGroupInstanceList: list of str
         :param TaskGroupMode: 执行模式。1 --- 顺序执行，2 --- 阶段执行
         :type TaskGroupMode: int
+        :param TaskGroupDiscardInstanceList: 不参演的实例列表
+        :type TaskGroupDiscardInstanceList: list of str
+        :param TaskGroupSelectedInstanceList: 参演实例列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskGroupSelectedInstanceList: list of str
+        :param TaskGroupInstancesExecuteRule: 机器选取规则
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskGroupInstancesExecuteRule: list of TaskGroupInstancesExecuteRules
         """
         self.TaskGroupId = None
         self.TaskGroupTitle = None
         self.TaskGroupDescription = None
         self.TaskGroupOrder = None
         self.ObjectTypeId = None
         self.TaskGroupCreateTime = None
         self.TaskGroupUpdateTime = None
         self.TaskGroupActions = None
         self.TaskGroupInstanceList = None
         self.TaskGroupMode = None
+        self.TaskGroupDiscardInstanceList = None
+        self.TaskGroupSelectedInstanceList = None
+        self.TaskGroupInstancesExecuteRule = None
 
 
     def _deserialize(self, params):
         self.TaskGroupId = params.get("TaskGroupId")
         self.TaskGroupTitle = params.get("TaskGroupTitle")
         self.TaskGroupDescription = params.get("TaskGroupDescription")
         self.TaskGroupOrder = params.get("TaskGroupOrder")
@@ -926,14 +937,22 @@
             self.TaskGroupActions = []
             for item in params.get("TaskGroupActions"):
                 obj = TaskGroupAction()
                 obj._deserialize(item)
                 self.TaskGroupActions.append(obj)
         self.TaskGroupInstanceList = params.get("TaskGroupInstanceList")
         self.TaskGroupMode = params.get("TaskGroupMode")
+        self.TaskGroupDiscardInstanceList = params.get("TaskGroupDiscardInstanceList")
+        self.TaskGroupSelectedInstanceList = params.get("TaskGroupSelectedInstanceList")
+        if params.get("TaskGroupInstancesExecuteRule") is not None:
+            self.TaskGroupInstancesExecuteRule = []
+            for item in params.get("TaskGroupInstancesExecuteRule"):
+                obj = TaskGroupInstancesExecuteRules()
+                obj._deserialize(item)
+                self.TaskGroupInstancesExecuteRule.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1196,14 +1215,49 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class TaskGroupInstancesExecuteRules(AbstractModel):
+    """机器选取规则
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskGroupInstancesExecuteMode: 实例选取模式
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskGroupInstancesExecuteMode: int
+        :param TaskGroupInstancesExecutePercent: 按比例选取模式下选取比例
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskGroupInstancesExecutePercent: int
+        :param TaskGroupInstancesExecuteNum: 按数量选取模式下选取数量
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskGroupInstancesExecuteNum: int
+        """
+        self.TaskGroupInstancesExecuteMode = None
+        self.TaskGroupInstancesExecutePercent = None
+        self.TaskGroupInstancesExecuteNum = None
+
+
+    def _deserialize(self, params):
+        self.TaskGroupInstancesExecuteMode = params.get("TaskGroupInstancesExecuteMode")
+        self.TaskGroupInstancesExecutePercent = params.get("TaskGroupInstancesExecutePercent")
+        self.TaskGroupInstancesExecuteNum = params.get("TaskGroupInstancesExecuteNum")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class TaskListItem(AbstractModel):
     """任务列表信息
 
     """
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.908/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfg-3.0.909/tencentcloud_sdk_python_cfg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfg
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Cfg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-cfg-3.0.909/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfg
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Cfg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfg-3.0.908/setup.py` & `tencentcloud-sdk-python-cfg-3.0.909/setup.py`

 * *Files identical despite different names*

