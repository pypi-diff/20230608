# Comparing `tmp/tencentcloud-sdk-python-clb-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-clb-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.908.tar", last modified: Wed Jun  7 00:20:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-clb-3.0.909.tar", last modified: Thu Jun  8 00:21:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-clb-3.0.908.tar` & `tencentcloud-sdk-python-clb-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud/clb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)     3269 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud/clb/v20180317/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    89673 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)   331659 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud/clb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud_sdk_python_clb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/tencentcloud_sdk_python_clb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:20:20.000000 tencentcloud-sdk-python-clb-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud/clb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud/clb/v20180317/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    89673 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   331792 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud/clb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud_sdk_python_clb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud_sdk_python_clb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud_sdk_python_clb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud_sdk_python_clb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/tencentcloud_sdk_python_clb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:21:01.000000 tencentcloud-sdk-python-clb-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-clb-3.0.908/README.rst` & `tencentcloud-sdk-python-clb-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.908/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-clb-3.0.909/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.908/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-clb-3.0.909/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-clb-3.0.908/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-clb-3.0.909/tencentcloud/clb/v20180317/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4653,15 +4653,16 @@
     def __init__(self):
         r"""
         :param HealthSwitch: 是否开启健康检查：1（开启）、0（关闭）。
         :type HealthSwitch: int
         :param TimeOut: 健康检查的响应超时时间（仅适用于四层监听器），可选值：2~60，默认值：2，单位：秒。响应超时时间要小于检查间隔时间。
 注意：此字段可能返回 null，表示取不到有效值。
         :type TimeOut: int
-        :param IntervalTime: 健康检查探测间隔时间，默认值：5，可选值：5~300，单位：秒。
+        :param IntervalTime: 健康检查探测间隔时间，默认值：5，IPv4 CLB实例的取值范围为：2-300，IPv6 CLB 实例的取值范围为：5-300。单位：秒。
+说明：部分老旧 IPv4 CLB实例的取值范围为：5-300。
 注意：此字段可能返回 null，表示取不到有效值。
         :type IntervalTime: int
         :param HealthNum: 健康阈值，默认值：3，表示当连续探测三次健康则表示该转发正常，可选值：2~10，单位：次。
 注意：此字段可能返回 null，表示取不到有效值。
         :type HealthNum: int
         :param UnHealthNum: 不健康阈值，默认值：3，表示当连续探测三次不健康则表示该转发异常，可选值：2~10，单位：次。
 注意：此字段可能返回 null，表示取不到有效值。
```

### Comparing `tencentcloud-sdk-python-clb-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-clb-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-clb-3.0.908/tencentcloud_sdk_python_clb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.909/tencentcloud_sdk_python_clb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-clb-3.0.909/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-clb
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Clb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-clb-3.0.908/setup.py` & `tencentcloud-sdk-python-clb-3.0.909/setup.py`

 * *Files identical despite different names*

