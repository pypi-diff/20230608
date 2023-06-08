# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.908.tar", last modified: Wed Jun  7 00:22:53 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.909.tar", last modified: Thu Jun  8 00:23:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.908.tar` & `tencentcloud-sdk-python-dnspod-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/dnspod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    23568 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)   202833 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)    58917 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/dnspod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:22:53.000000 tencentcloud-sdk-python-dnspod-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/dnspod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    23568 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   207929 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)    59836 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/dnspod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:23:27.000000 tencentcloud-sdk-python-dnspod-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.908/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/dnspod/v20210323/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1799,14 +1799,139 @@
             for item in params.get("AliasData"):
                 obj = DomainAliasAnalyticsItem()
                 obj._deserialize(item)
                 self.AliasData.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDomainFilterListRequest(AbstractModel):
+    """DescribeDomainFilterList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Type: 根据域名分组类型获取域名。可取值为 ALL，MINE，SHARE，RECENT。
+ALL：全部
+MINE：我的域名
+SHARE：共享给我的域名
+RECENT：最近操作过的域名
+        :type Type: str
+        :param Offset: 记录开始的偏移, 第一条记录为 0, 依次类推。默认值为 0。
+        :type Offset: int
+        :param Limit: 要获取的域名数量, 比如获取 20 个, 则为 20。默认值为 5000。如果账户中的域名数量超过了 5000, 将会强制分页并且只返回前 5000 条, 这时需要通过 Offset 和 Limit 参数去获取其它域名。
+        :type Limit: int
+        :param GroupId: 根据域名分组 id 获取域名，可通过 DescribeDomain 或 DescribeDomainList 接口 GroupId 字段获取。
+        :type GroupId: list of int
+        :param Keyword: 根据关键字获取域名。
+        :type Keyword: str
+        :param SortField: 排序字段。可取值为 NAME，STATUS，RECORDS，GRADE，UPDATED_ON。
+NAME：域名名称
+STATUS：域名状态
+RECORDS：记录数量
+GRADE：套餐等级
+UPDATED_ON：更新时间
+        :type SortField: str
+        :param SortType: 排序类型，升序：ASC，降序：DESC。
+        :type SortType: str
+        :param Status: 根据域名状态获取域名。可取值为 ENABLE，LOCK，PAUSE，SPAM。
+ENABLE：正常
+LOCK：锁定
+PAUSE：暂停
+SPAM：封禁
+        :type Status: list of str
+        :param Package: 根据套餐获取域名，可通过 DescribeDomain 或 DescribeDomainList 接口 Grade 字段获取。
+        :type Package: list of str
+        :param Remark: 根据备注信息获取域名。
+        :type Remark: str
+        :param UpdatedAtBegin: 要获取域名的更新时间起始时间点，如 '2021-05-01 03:00:00'。
+        :type UpdatedAtBegin: str
+        :param UpdatedAtEnd: 要获取域名的更新时间终止时间点，如 '2021-05-10 20:00:00'。
+        :type UpdatedAtEnd: str
+        :param RecordCountBegin: 要获取域名的记录数查询区间起点。
+        :type RecordCountBegin: int
+        :param RecordCountEnd: 要获取域名的记录数查询区间终点。
+        :type RecordCountEnd: int
+        :param ProjectId: 项目ID
+        :type ProjectId: int
+        """
+        self.Type = None
+        self.Offset = None
+        self.Limit = None
+        self.GroupId = None
+        self.Keyword = None
+        self.SortField = None
+        self.SortType = None
+        self.Status = None
+        self.Package = None
+        self.Remark = None
+        self.UpdatedAtBegin = None
+        self.UpdatedAtEnd = None
+        self.RecordCountBegin = None
+        self.RecordCountEnd = None
+        self.ProjectId = None
+
+
+    def _deserialize(self, params):
+        self.Type = params.get("Type")
+        self.Offset = params.get("Offset")
+        self.Limit = params.get("Limit")
+        self.GroupId = params.get("GroupId")
+        self.Keyword = params.get("Keyword")
+        self.SortField = params.get("SortField")
+        self.SortType = params.get("SortType")
+        self.Status = params.get("Status")
+        self.Package = params.get("Package")
+        self.Remark = params.get("Remark")
+        self.UpdatedAtBegin = params.get("UpdatedAtBegin")
+        self.UpdatedAtEnd = params.get("UpdatedAtEnd")
+        self.RecordCountBegin = params.get("RecordCountBegin")
+        self.RecordCountEnd = params.get("RecordCountEnd")
+        self.ProjectId = params.get("ProjectId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDomainFilterListResponse(AbstractModel):
+    """DescribeDomainFilterList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DomainCountInfo: 列表页统计信息
+        :type DomainCountInfo: :class:`tencentcloud.dnspod.v20210323.models.DomainCountInfo`
+        :param DomainList: 域名列表
+        :type DomainList: list of DomainListItem
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DomainCountInfo = None
+        self.DomainList = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("DomainCountInfo") is not None:
+            self.DomainCountInfo = DomainCountInfo()
+            self.DomainCountInfo._deserialize(params.get("DomainCountInfo"))
+        if params.get("DomainList") is not None:
+            self.DomainList = []
+            for item in params.get("DomainList"):
+                obj = DomainListItem()
+                obj._deserialize(item)
+                self.DomainList.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDomainGroupListRequest(AbstractModel):
     """DescribeDomainGroupList请求参数结构体
 
     """
 
 
 class DescribeDomainGroupListResponse(AbstractModel):
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,14 +528,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeDomainFilterList(self, request):
+        """获取域名筛选列表
+
+        :param request: Request instance for DescribeDomainFilterList.
+        :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainFilterListRequest`
+        :rtype: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainFilterListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDomainFilterList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDomainFilterListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeDomainGroupList(self, request):
         """获取域名分组列表
 
         :param request: Request instance for DescribeDomainGroupList.
         :type request: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainGroupListRequest`
         :rtype: :class:`tencentcloud.dnspod.v20210323.models.DescribeDomainGroupListResponse`
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.909/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.908/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.909/setup.py`

 * *Files identical despite different names*

