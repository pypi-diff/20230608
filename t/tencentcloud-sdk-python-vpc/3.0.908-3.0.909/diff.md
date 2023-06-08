# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.908.tar", last modified: Wed Jun  7 00:36:30 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.909.tar", last modified: Thu Jun  8 00:38:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.908.tar` & `tencentcloud-sdk-python-vpc-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   332331 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41791 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   851805 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:36:30.000000 tencentcloud-sdk-python-vpc-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332322 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41912 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   851887 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:38:01.000000 tencentcloud-sdk-python-vpc-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.908/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.909/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.908/README.rst` & `tencentcloud-sdk-python-vpc-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2374,15 +2374,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DeleteSubnet(self, request):
-        """本接口（DeleteSubnet）用于用于删除子网（Subnet）。
+        """本接口（DeleteSubnet）用于删除子网（Subnet）。
         * 删除子网前，请清理该子网下所有资源，包括云服务器、负载均衡、云数据、NoSQL、弹性网卡等资源。
 
         :param request: Request instance for DeleteSubnet.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DeleteSubnetRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DeleteSubnetResponse`
 
         """
@@ -4160,15 +4160,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeUsedIpAddress(self, request):
         """本接口(DescribeUsedIpAddress)用于查询Subnet或者Vpc内的ip的使用情况，
-        如被ip被占用，返回占用ip的资源类别与id；如未被占用，返回空值
+        如ip被占用，返回占用ip的资源类别与id；如未被占用，返回空值
 
         :param request: Request instance for DescribeUsedIpAddress.
         :type request: :class:`tencentcloud.vpc.v20170312.models.DescribeUsedIpAddressRequest`
         :rtype: :class:`tencentcloud.vpc.v20170312.models.DescribeUsedIpAddressResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,17 @@
 
 # 值超过上限。
 INVALIDPARAMETERVALUE_EIPBRANDWIDTHOUTINVALID = 'InvalidParameterValue.EIPBrandWidthOutInvalid'
 
 # 缺少参数。
 INVALIDPARAMETERVALUE_EMPTY = 'InvalidParameterValue.Empty'
 
+# IPv6转换实例ID已经存在。
+INVALIDPARAMETERVALUE_IPV6RULEIDEXISTED = 'InvalidParameterValue.IPv6RuleIdExisted'
+
 # IPv6规则没有更改。
 INVALIDPARAMETERVALUE_IPV6RULENOTCHANGE = 'InvalidParameterValue.IPv6RuleNotChange'
 
 # 该实例的计费方式与其他实例不同。
 INVALIDPARAMETERVALUE_INCONSISTENTINSTANCEINTERNETCHARGETYPE = 'InvalidParameterValue.InconsistentInstanceInternetChargeType'
 
 # 该实例不支持AnycastEIP。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4086,15 +4086,15 @@
         :type NextHopType: str
         :param NextHopDestination: 下一跳目的网关，取值与“下一跳类型”相关：
 下一跳类型为VPN，取值VPN网关ID，形如：vpngw-12345678；
 下一跳类型为DIRECTCONNECT，取值专线网关ID，形如：dcg-12345678；
 下一跳类型为PEERCONNECTION，取值对等连接ID，形如：pcx-12345678；
 下一跳类型为NAT，取值Nat网关，形如：nat-12345678；
 下一跳类型为NORMAL_CVM，取值云服务器IPv4地址，形如：10.0.0.12；
-下一跳类型为CCN，取值云云联网ID，形如：ccn-12345678；
+下一跳类型为CCN，取值云联网ID，形如：ccn-12345678；
 下一跳类型为NONEXTHOP，指定网络探测为无下一跳的网络探测；
         :type NextHopDestination: str
         :param NetDetectDescription: 网络探测描述。
         :type NetDetectDescription: str
         """
         self.VpcId = None
         self.SubnetId = None
@@ -10759,14 +10759,15 @@
 <li>ip-exact-match - Boolean - （过滤条件）内网IPv4精确匹配查询，存在多值情况，只取第一个。</li>
 <li>tag-key - String -是否必填：否- （过滤条件）按照标签键进行过滤。使用请参考示例2</li>
 <li>tag:tag-key - String - 是否必填：否 - （过滤条件）按照标签键值对进行过滤。 tag-key使用具体的标签键进行替换。使用请参考示例2。</li>
 <li>is-primary - Boolean - 是否必填：否 - （过滤条件）按照是否主网卡进行过滤。值为true时，仅过滤主网卡；值为false时，仅过滤辅助网卡；此过滤参数未提供时，同时过滤主网卡和辅助网卡。</li>
 <li>eni-type - String -是否必填：否- （过滤条件）按照网卡类型进行过滤。“0”-辅助网卡，“1”-主网卡，“2”：中继网卡。</li>
 <li>eni-qos - String -是否必填：否- （过滤条件）按照网卡服务质量进行过滤。“AG”-服务质量为云铜，“AU”-服务质量为云银。</li>
 <li>address-ipv6 - String - 是否必填：否 -（过滤条件）内网IPv6地址过滤，支持多ipv6地址查询，如果和address-ip一起使用取交集。</li>
+<li>public-address-ip - String - （过滤条件）公网IPv4地址，精确匹配。</li>
         :type Filters: list of Filter
         :param Offset: 偏移量，默认为0。
         :type Offset: int
         :param Limit: 返回数量，默认为20，最大值为100。
         :type Limit: int
         """
         self.NetworkInterfaceIds = None
@@ -17768,15 +17769,15 @@
         :type NextHopType: str
         :param NextHopDestination: 下一跳目的网关，取值与“下一跳类型”相关：
 下一跳类型为VPN，取值VPN网关ID，形如：vpngw-12345678；
 下一跳类型为DIRECTCONNECT，取值专线网关ID，形如：dcg-12345678；
 下一跳类型为PEERCONNECTION，取值对等连接ID，形如：pcx-12345678；
 下一跳类型为NAT，取值Nat网关，形如：nat-12345678；
 下一跳类型为NORMAL_CVM，取值云服务器IPv4地址，形如：10.0.0.12；
-下一跳类型为CCN，取值云云联网ID，形如：ccn-12345678；
+下一跳类型为CCN，取值云联网ID，形如：ccn-12345678；
 下一跳类型为NONEXTHOP，指定网络探测为无下一跳的网络探测；
         :type NextHopDestination: str
         :param NetDetectDescription: 网络探测描述。
         :type NetDetectDescription: str
         """
         self.NetDetectId = None
         self.NetDetectName = None
@@ -19290,15 +19291,15 @@
         :type NextHopType: str
         :param NextHopDestination: 下一跳目的网关，取值与“下一跳类型”相关：
 下一跳类型为VPN，取值VPN网关ID，形如：vpngw-12345678；
 下一跳类型为DIRECTCONNECT，取值专线网关ID，形如：dcg-12345678；
 下一跳类型为PEERCONNECTION，取值对等连接ID，形如：pcx-12345678；
 下一跳类型为NAT，取值Nat网关，形如：nat-12345678；
 下一跳类型为NORMAL_CVM，取值云服务器IPv4地址，形如：10.0.0.12；
-下一跳类型为CCN，取值云云联网ID，形如：ccn-12345678；
+下一跳类型为CCN，取值云联网ID，形如：ccn-12345678；
 下一跳类型为NONEXTHOP，指定网络探测为无下一跳的网络探测；
         :type NextHopDestination: str
         :param NextHopName: 下一跳网关名称。
 注意：此字段可能返回 null，表示取不到有效值。
         :type NextHopName: str
         :param NetDetectDescription: 网络探测描述。
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.909/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.908/setup.py` & `tencentcloud-sdk-python-vpc-3.0.909/setup.py`

 * *Files identical despite different names*

