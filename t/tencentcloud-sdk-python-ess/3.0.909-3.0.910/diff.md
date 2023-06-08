# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.909.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.910.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.909.tar", last modified: Thu Jun  8 00:25:00 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.910.tar", last modified: Thu Jun  8 09:11:03 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.909.tar` & `tencentcloud-sdk-python-ess-3.0.910.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    51319 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24361 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   228721 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:25:00.000000 tencentcloud-sdk-python-ess-3.0.909/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    55323 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24361 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   238847 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:11:03.000000 tencentcloud-sdk-python-ess-3.0.910/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.909/README.rst` & `tencentcloud-sdk-python-ess-3.0.910/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.909/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.910/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.909'
+__version__ = '3.0.910'
```

### Comparing `tencentcloud-sdk-python-ess-3.0.909/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,14 +372,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateIntegrationDepartment(self, request):
+        """通过此接口，创建企业的部门，支持绑定客户系统部门ID。
+
+        :param request: Request instance for CreateIntegrationDepartment.
+        :type request: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationDepartmentRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationDepartmentResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateIntegrationDepartment", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateIntegrationDepartmentResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateIntegrationEmployees(self, request):
         """创建员工,如需在此接口提醒员工实名，入参Employees的OpenId不传
 
         :param request: Request instance for CreateIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationEmployeesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateIntegrationEmployeesResponse`
 
@@ -599,14 +622,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DeleteIntegrationDepartment(self, request):
+        """通过此接口，删除企业的部门。
+
+        :param request: Request instance for DeleteIntegrationDepartment.
+        :type request: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationDepartmentRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationDepartmentResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteIntegrationDepartment", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteIntegrationDepartmentResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DeleteIntegrationEmployees(self, request):
         """移除员工
 
         :param request: Request instance for DeleteIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationEmployeesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DeleteIntegrationEmployeesResponse`
 
@@ -788,14 +834,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeIntegrationDepartments(self, request):
+        """通过此接口，查询企业的部门，支持查询单个部门节点或单个部门节点及一级子节点部门列表。
+
+        :param request: Request instance for DescribeIntegrationDepartments.
+        :type request: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationDepartmentsRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationDepartmentsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeIntegrationDepartments", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeIntegrationDepartmentsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeIntegrationEmployees(self, request):
         """查询企业员工列表，每次返回的数据量最大为20
 
         :param request: Request instance for DescribeIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationEmployeesRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeIntegrationEmployeesResponse`
 
@@ -1020,14 +1089,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ModifyIntegrationDepartment(self, request):
+        """通过此接口，更新企业的部门信息，支持更新部门名、客户系统部门ID、部门序列号。
+
+        :param request: Request instance for ModifyIntegrationDepartment.
+        :type request: :class:`tencentcloud.ess.v20201111.models.ModifyIntegrationDepartmentRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.ModifyIntegrationDepartmentResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyIntegrationDepartment", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyIntegrationDepartmentResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def StartFlow(self, request):
         """此接口用于发起流程
         适用场景：见创建签署流程接口。
         注：该接口是“创建电子文档”接口的后置接口，用于激活包含完整合同信息（模板及内容信息）的流程。激活后的流程就是一份待签署的电子合同。
```

### Comparing `tencentcloud-sdk-python-ess-3.0.909/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.909/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.910/tencentcloud/ess/v20201111/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1723,14 +1723,81 @@
             for item in params.get("FlowApproverUrlInfos"):
                 obj = FlowApproverUrlInfo()
                 obj._deserialize(item)
                 self.FlowApproverUrlInfos.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class CreateIntegrationDepartmentRequest(AbstractModel):
+    """CreateIntegrationDepartment请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: 操作人信息，UserId必填且需拥有组织架构管理权限
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param DeptName: 部门名称，不超过50个字符
+        :type DeptName: str
+        :param ParentDeptId: 电子签父部门ID，与ParentDeptOpenId二选一,优先ParentDeptId,都为空时自动填充至根节点下
+        :type ParentDeptId: str
+        :param ParentDeptOpenId: 第三方平台中父部门ID,与ParentDeptId二选一,优先ParentDeptId,都为空时自动填充至根节点下
+        :type ParentDeptOpenId: str
+        :param DeptOpenId: 客户系统部门ID，不超过64个字符
+        :type DeptOpenId: str
+        :param OrderNo: 排序号,1~30000范围内
+        :type OrderNo: int
+        """
+        self.Operator = None
+        self.DeptName = None
+        self.ParentDeptId = None
+        self.ParentDeptOpenId = None
+        self.DeptOpenId = None
+        self.OrderNo = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        self.DeptName = params.get("DeptName")
+        self.ParentDeptId = params.get("ParentDeptId")
+        self.ParentDeptOpenId = params.get("ParentDeptOpenId")
+        self.DeptOpenId = params.get("DeptOpenId")
+        self.OrderNo = params.get("OrderNo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateIntegrationDepartmentResponse(AbstractModel):
+    """CreateIntegrationDepartment返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeptId: 电子签部门ID
+        :type DeptId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DeptId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DeptId = params.get("DeptId")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateIntegrationEmployeesRequest(AbstractModel):
     """CreateIntegrationEmployees请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2514,14 +2581,65 @@
         self.AppOriginalId = params.get("AppOriginalId")
         self.Path = params.get("Path")
         self.QrCode = params.get("QrCode")
         self.UrlType = params.get("UrlType")
         self.RequestId = params.get("RequestId")
 
 
+class DeleteIntegrationDepartmentRequest(AbstractModel):
+    """DeleteIntegrationDepartment请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: 操作人信息，UserId必填且需拥有组织架构管理权限
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param DeptId: 电子签中的部门id
+        :type DeptId: str
+        :param ReceiveDeptId: 交接部门ID。待删除部门中的合同、印章和模版数据，交接至该部门ID下，未填写交接至公司根部门。
+        :type ReceiveDeptId: str
+        """
+        self.Operator = None
+        self.DeptId = None
+        self.ReceiveDeptId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        self.DeptId = params.get("DeptId")
+        self.ReceiveDeptId = params.get("ReceiveDeptId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteIntegrationDepartmentResponse(AbstractModel):
+    """DeleteIntegrationDepartment返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class DeleteIntegrationEmployeesRequest(AbstractModel):
     """DeleteIntegrationEmployees请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -3164,14 +3282,78 @@
                 obj = TemplateInfo()
                 obj._deserialize(item)
                 self.Templates.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeIntegrationDepartmentsRequest(AbstractModel):
+    """DescribeIntegrationDepartments请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: 操作人信息，UserId必填且需拥有组织架构管理权限
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param QueryType: 查询类型 0-查询单个部门节点 1-单个部门节点及一级子节点部门列表
+        :type QueryType: int
+        :param DeptId: 部门ID,与DeptOpenId二选一,优先DeptId,都为空时获取根节点数据
+        :type DeptId: str
+        :param DeptOpenId: 客户系统部门ID,与DeptId二选一,优先DeptId,都为空时获取根节点数据
+        :type DeptOpenId: str
+        """
+        self.Operator = None
+        self.QueryType = None
+        self.DeptId = None
+        self.DeptOpenId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        self.QueryType = params.get("QueryType")
+        self.DeptId = params.get("DeptId")
+        self.DeptOpenId = params.get("DeptOpenId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeIntegrationDepartmentsResponse(AbstractModel):
+    """DescribeIntegrationDepartments返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Departments: 部门列表
+        :type Departments: list of IntegrationDepartment
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Departments = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Departments") is not None:
+            self.Departments = []
+            for item in params.get("Departments"):
+                obj = IntegrationDepartment()
+                obj._deserialize(item)
+                self.Departments.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeIntegrationEmployeesRequest(AbstractModel):
     """DescribeIntegrationEmployees请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4774,14 +4956,59 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class IntegrationDepartment(AbstractModel):
+    """部门信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DeptId: 部门ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeptId: str
+        :param DeptName: 部门名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeptName: str
+        :param ParentDeptId: 父部门ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParentDeptId: str
+        :param DeptOpenId: 客户系统部门ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeptOpenId: str
+        :param OrderNo: 序列号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OrderNo: int
+        """
+        self.DeptId = None
+        self.DeptName = None
+        self.ParentDeptId = None
+        self.DeptOpenId = None
+        self.OrderNo = None
+
+
+    def _deserialize(self, params):
+        self.DeptId = params.get("DeptId")
+        self.DeptName = params.get("DeptName")
+        self.ParentDeptId = params.get("ParentDeptId")
+        self.DeptOpenId = params.get("DeptOpenId")
+        self.OrderNo = params.get("OrderNo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class IntegrationMainOrganizationUser(AbstractModel):
     """主企业员工账号信息
 
     """
 
     def __init__(self):
         r"""
@@ -4854,14 +5081,77 @@
 
     """
 
     def __init__(self):
         r"""
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
+class ModifyIntegrationDepartmentRequest(AbstractModel):
+    """ModifyIntegrationDepartment请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: 操作人信息，UserId必填且需拥有组织架构管理权限
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param DeptId: 电子签部门ID
+        :type DeptId: str
+        :param ParentDeptId: 电子签父部门ID
+        :type ParentDeptId: str
+        :param DeptName: 部门名称，不超过50个字符
+        :type DeptName: str
+        :param DeptOpenId: 客户系统部门ID，不超过64个字符
+        :type DeptOpenId: str
+        :param OrderNo: 排序号,1~30000范围内
+        :type OrderNo: int
+        """
+        self.Operator = None
+        self.DeptId = None
+        self.ParentDeptId = None
+        self.DeptName = None
+        self.DeptOpenId = None
+        self.OrderNo = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        self.DeptId = params.get("DeptId")
+        self.ParentDeptId = params.get("ParentDeptId")
+        self.DeptName = params.get("DeptName")
+        self.DeptOpenId = params.get("DeptOpenId")
+        self.OrderNo = params.get("OrderNo")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyIntegrationDepartmentResponse(AbstractModel):
+    """ModifyIntegrationDepartment返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
         """
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
```

### Comparing `tencentcloud-sdk-python-ess-3.0.909/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.910/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.909
+Version: 3.0.910
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.909/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.910/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.909
+Version: 3.0.910
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.909/setup.py` & `tencentcloud-sdk-python-ess-3.0.910/setup.py`

 * *Files identical despite different names*

