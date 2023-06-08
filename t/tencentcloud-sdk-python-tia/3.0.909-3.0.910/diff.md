# Comparing `tmp/tencentcloud-sdk-python-tia-3.0.909.tar.gz` & `tmp/tencentcloud-sdk-python-tia-3.0.910.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tia-3.0.909.tar", last modified: Thu Jun  8 00:35:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tia-3.0.910.tar", last modified: Thu Jun  8 09:22:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tia-3.0.909.tar` & `tencentcloud-sdk-python-tia-3.0.910.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud_sdk_python_tia.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud_sdk_python_tia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud_sdk_python_tia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud_sdk_python_tia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud_sdk_python_tia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud/tia/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud/tia/v20180226/
--rw-r--r--   0 root         (0) root         (0)    10642 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud/tia/v20180226/tia_client.py
--rw-r--r--   0 root         (0) root         (0)     2747 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud/tia/v20180226/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud/tia/v20180226/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30927 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud/tia/v20180226/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/tencentcloud/tia/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:35:02.000000 tencentcloud-sdk-python-tia-3.0.909/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud_sdk_python_tia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud_sdk_python_tia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud_sdk_python_tia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud_sdk_python_tia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud_sdk_python_tia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud/tia/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud/tia/v20180226/
+-rw-r--r--   0 root         (0) root         (0)    10642 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud/tia/v20180226/tia_client.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud/tia/v20180226/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud/tia/v20180226/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30927 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud/tia/v20180226/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/tencentcloud/tia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 09:22:25.000000 tencentcloud-sdk-python-tia-3.0.910/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tia-3.0.909/README.rst` & `tencentcloud-sdk-python-tia-3.0.910/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.909/tencentcloud_sdk_python_tia.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tia-3.0.910/tencentcloud_sdk_python_tia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tia
-Version: 3.0.909
+Version: 3.0.910
 Summary: Tencent Cloud Tia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tia-3.0.909/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tia-3.0.910/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tia-3.0.909/tencentcloud/tia/v20180226/tia_client.py` & `tencentcloud-sdk-python-tia-3.0.910/tencentcloud/tia/v20180226/tia_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.909/tencentcloud/tia/v20180226/errorcodes.py` & `tencentcloud-sdk-python-tia-3.0.910/tencentcloud/tia/v20180226/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.909/tencentcloud/tia/v20180226/models.py` & `tencentcloud-sdk-python-tia-3.0.910/tencentcloud/tia/v20180226/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tia-3.0.909/PKG-INFO` & `tencentcloud-sdk-python-tia-3.0.910/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tia
-Version: 3.0.909
+Version: 3.0.910
 Summary: Tencent Cloud Tia SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tia-3.0.909/setup.py` & `tencentcloud-sdk-python-tia-3.0.910/setup.py`

 * *Files identical despite different names*
