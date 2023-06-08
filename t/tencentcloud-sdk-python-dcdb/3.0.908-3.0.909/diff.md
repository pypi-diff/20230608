# Comparing `tmp/tencentcloud-sdk-python-dcdb-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-dcdb-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.908.tar", last modified: Wed Jun  7 00:22:40 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.909.tar", last modified: Thu Jun  8 00:23:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dcdb-3.0.908.tar` & `tencentcloud-sdk-python-dcdb-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud_sdk_python_dcdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/dcdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/dcdb/v20180411/
--rw-r--r--   0 root         (0) root         (0)    13722 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/dcdb/v20180411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/dcdb/v20180411/__init__.py
--rw-r--r--   0 root         (0) root         (0)   241570 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/dcdb/v20180411/models.py
--rw-r--r--   0 root         (0) root         (0)    70022 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/dcdb/v20180411/dcdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/dcdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:22:40.000000 tencentcloud-sdk-python-dcdb-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud_sdk_python_dcdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/dcdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/dcdb/v20180411/
+-rw-r--r--   0 root         (0) root         (0)    13928 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/dcdb/v20180411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/dcdb/v20180411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   243265 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/dcdb/v20180411/models.py
+-rw-r--r--   0 root         (0) root         (0)    71118 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/dcdb/v20180411/dcdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/dcdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:23:17.000000 tencentcloud-sdk-python-dcdb-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.908/README.rst` & `tencentcloud-sdk-python-dcdb-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/dcdb/v20180411/errorcodes.py` & `tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/dcdb/v20180411/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,20 @@
 
 # 解绑安全组失败。
 FAILEDOPERATION_DISASSOCIATESECURITYGROUPSFAILED = 'FailedOperation.DisassociateSecurityGroupsFailed'
 
 # 拉取安全组详情失败。
 FAILEDOPERATION_GETSECURITYGROUPDETAILFAILED = 'FailedOperation.GetSecurityGroupDetailFailed'
 
+# 实例不可退费。
+FAILEDOPERATION_INSTANCECANNOTRETURN = 'FailedOperation.InstanceCanNotReturn'
+
+# 实例退费失败。
+FAILEDOPERATION_INSTANCERETURNFAILED = 'FailedOperation.InstanceReturnFailed'
+
 # 修改账号权限失败。
 FAILEDOPERATION_MODIFYRIGHTFAILED = 'FailedOperation.ModifyRightFailed'
 
 # 修改账号配置失败。
 FAILEDOPERATION_MODIFYUSERCONFIGFAILED = 'FailedOperation.ModifyUserConfigFailed'
 
 # 消息队列操作失败。
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/dcdb/v20180411/models.py` & `tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/dcdb/v20180411/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4469,14 +4469,63 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class IsolateDCDBInstanceRequest(AbstractModel):
+    """IsolateDCDBInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceIds: 实例 ID，格式如：tdsqlshard-avw0207d，与云数据库控制台页面中显示的实例 ID 相同，可使用 查询实例列表 接口获取，其值为输出参数中字段 InstanceId 的值。
+        :type InstanceIds: list of str
+        """
+        self.InstanceIds = None
+
+
+    def _deserialize(self, params):
+        self.InstanceIds = params.get("InstanceIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class IsolateDCDBInstanceResponse(AbstractModel):
+    """IsolateDCDBInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SuccessInstanceIds: 隔离成功实例ID列表。
+        :type SuccessInstanceIds: list of str
+        :param FailedInstanceIds: 隔离失败实例ID列表。
+        :type FailedInstanceIds: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.SuccessInstanceIds = None
+        self.FailedInstanceIds = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.SuccessInstanceIds = params.get("SuccessInstanceIds")
+        self.FailedInstanceIds = params.get("FailedInstanceIds")
+        self.RequestId = params.get("RequestId")
+
+
 class IsolateDedicatedDBInstanceRequest(AbstractModel):
     """IsolateDedicatedDBInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/dcdb/v20180411/dcdb_client.py` & `tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/dcdb/v20180411/dcdb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1109,14 +1109,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def IsolateDCDBInstance(self, request):
+        """本接口(IsolateDCDBInstance)用于隔离分布式数据库TDSQL实例（包年包月），隔离后不能通过IP和端口访问数据库。隔离的实例可在回收站中进行开机。若为欠费隔离，请尽快进行充值。
+
+        :param request: Request instance for IsolateDCDBInstance.
+        :type request: :class:`tencentcloud.dcdb.v20180411.models.IsolateDCDBInstanceRequest`
+        :rtype: :class:`tencentcloud.dcdb.v20180411.models.IsolateDCDBInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("IsolateDCDBInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.IsolateDCDBInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def IsolateDedicatedDBInstance(self, request):
         """本接口（IsolateDedicatedDBInstance）用于隔离独享云数据库实例。
 
         :param request: Request instance for IsolateDedicatedDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.IsolateDedicatedDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.IsolateDedicatedDBInstanceResponse`
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dcdb-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dcdb-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.909/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.908/setup.py` & `tencentcloud-sdk-python-dcdb-3.0.909/setup.py`

 * *Files identical despite different names*

