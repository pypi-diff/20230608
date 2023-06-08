# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.909.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.910.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.909.tar", last modified: Thu Jun  8 00:25:06 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.910.tar", last modified: Thu Jun  8 09:11:08 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.909.tar` & `tencentcloud-sdk-python-essbasic-3.0.910.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    16533 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    51520 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   234084 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:25:06.000000 tencentcloud-sdk-python-essbasic-3.0.909/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    51520 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   234248 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:11:08.000000 tencentcloud-sdk-python-essbasic-3.0.910/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.909
+Version: 3.0.910
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.910/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1442,14 +1442,15 @@
     def __init__(self):
         r"""
         :param Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param SealId: 指定印章ID
         :type SealId: str
         :param UserIds: 指定待授权的用户ID数组,电子签的用户ID
+可以填写OpenId，系统会通过组织+渠道+OpenId查询得到UserId进行授权。
         :type UserIds: list of str
         :param Operator: 操作人（用户）信息，不用传
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         :param Organization: 企业机构信息，不用传
         :type Organization: :class:`tencentcloud.essbasic.v20210526.models.OrganizationInfo`
         """
         self.Agent = None
@@ -1483,15 +1484,16 @@
 class ChannelCreateSealPolicyResponse(AbstractModel):
     """ChannelCreateSealPolicy返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param UserIds: 最终授权成功的电子签系统用户ID数组。其他的跳过的是已经授权了的
+        :param UserIds: 最终授权成功的电子签系统用户ID数组。其他的跳过的是已经授权了的。
+请求参数填写OpenId时，返回授权成功的 Openid。
         :type UserIds: list of str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.UserIds = None
         self.RequestId = None
 
@@ -1636,14 +1638,15 @@
     def __init__(self):
         r"""
         :param Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param SealId: 指定印章ID
         :type SealId: str
         :param UserIds: 指定用户ID数组，电子签系统用户ID
+可以填写OpenId，系统会通过组织+渠道+OpenId查询得到UserId进行授权取消。
         :type UserIds: list of str
         :param Organization: 组织机构信息，不用传
         :type Organization: :class:`tencentcloud.essbasic.v20210526.models.OrganizationInfo`
         :param Operator: 操作人（用户）信息，不用传
         :type Operator: :class:`tencentcloud.essbasic.v20210526.models.UserInfo`
         """
         self.Agent = None
@@ -4579,15 +4582,15 @@
 class OperateChannelTemplateRequest(AbstractModel):
     """OperateChannelTemplate请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Agent: 应用相关信息。 此接口Agent.ProxyOrganizationOpenId、Agent. ProxyOperator.OpenId、Agent.AppId 和 Agent.ProxyAppId 均必填。
+        :param Agent: 应用相关信息。 此接口Agent.AppId必填。
         :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
         :param OperateType: 操作类型，查询:"SELECT"，删除:"DELETE"，更新:"UPDATE"
         :type OperateType: str
         :param TemplateId: 第三方应用平台模板库模板唯一标识
         :type TemplateId: str
         :param ProxyOrganizationOpenIds: 合作企业方第三方机构唯一标识数据，支持多个， 用","进行分隔
         :type ProxyOrganizationOpenIds: str
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.910/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.910/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.909
+Version: 3.0.910
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.909/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.910/setup.py`

 * *Files identical despite different names*

