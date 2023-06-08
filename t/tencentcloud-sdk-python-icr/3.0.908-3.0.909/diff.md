# Comparing `tmp/tencentcloud-sdk-python-icr-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-icr-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-icr-3.0.908.tar", last modified: Wed Jun  7 00:26:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-icr-3.0.909.tar", last modified: Thu Jun  8 00:26:50 2023, max compression
```

## Comparing `tencentcloud-sdk-python-icr-3.0.908.tar` & `tencentcloud-sdk-python-icr-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-07 00:26:01.000000 tencentcloud-sdk-python-icr-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:26:01.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud/icr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud/icr/v20211014/
--rw-r--r--   0 root         (0) root         (0)      652 2023-06-07 00:26:01.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud/icr/v20211014/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:26:01.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud/icr/v20211014/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17883 2023-06-07 00:26:01.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud/icr/v20211014/models.py
--rw-r--r--   0 root         (0) root         (0)     1910 2023-06-07 00:26:01.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud/icr/v20211014/icr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:26:01.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud/icr/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud_sdk_python_icr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud_sdk_python_icr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud_sdk_python_icr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud_sdk_python_icr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/tencentcloud_sdk_python_icr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 00:26:01.000000 tencentcloud-sdk-python-icr-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:26:02.000000 tencentcloud-sdk-python-icr-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud/icr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud/icr/v20211014/
+-rw-r--r--   0 root         (0) root         (0)      652 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud/icr/v20211014/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud/icr/v20211014/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17883 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud/icr/v20211014/models.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud/icr/v20211014/icr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud/icr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud_sdk_python_icr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud_sdk_python_icr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud_sdk_python_icr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud_sdk_python_icr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/tencentcloud_sdk_python_icr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:26:50.000000 tencentcloud-sdk-python-icr-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-icr-3.0.908/README.rst` & `tencentcloud-sdk-python-icr-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-icr-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-icr-3.0.908/tencentcloud/icr/v20211014/errorcodes.py` & `tencentcloud-sdk-python-icr-3.0.909/tencentcloud/icr/v20211014/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.908/tencentcloud/icr/v20211014/models.py` & `tencentcloud-sdk-python-icr-3.0.909/tencentcloud/icr/v20211014/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.908/tencentcloud/icr/v20211014/icr_client.py` & `tencentcloud-sdk-python-icr-3.0.909/tencentcloud/icr/v20211014/icr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-icr-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-icr-3.0.909/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-icr
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Icr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-icr-3.0.908/tencentcloud_sdk_python_icr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-icr-3.0.909/tencentcloud_sdk_python_icr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-icr
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Icr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-icr-3.0.908/setup.py` & `tencentcloud-sdk-python-icr-3.0.909/setup.py`

 * *Files identical despite different names*

