# Comparing `tmp/tencentcloud-sdk-python-keewidb-3.0.908.tar.gz` & `tmp/tencentcloud-sdk-python-keewidb-3.0.909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-keewidb-3.0.908.tar", last modified: Wed Jun  7 00:27:18 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-keewidb-3.0.909.tar", last modified: Thu Jun  8 00:28:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-keewidb-3.0.908.tar` & `tencentcloud-sdk-python-keewidb-3.0.909.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud_sdk_python_keewidb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud_sdk_python_keewidb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud_sdk_python_keewidb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud_sdk_python_keewidb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/keewidb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/keewidb/v20220308/
--rw-r--r--   0 root         (0) root         (0)     5675 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/keewidb/v20220308/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    37283 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/keewidb/v20220308/keewidb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/keewidb/v20220308/__init__.py
--rw-r--r--   0 root         (0) root         (0)   137323 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/keewidb/v20220308/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/keewidb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-07 00:27:18.000000 tencentcloud-sdk-python-keewidb-3.0.908/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-08 00:28:04.000000 tencentcloud-sdk-python-keewidb-3.0.909/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud_sdk_python_keewidb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud_sdk_python_keewidb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud_sdk_python_keewidb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud_sdk_python_keewidb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/keewidb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/keewidb/v20220308/
+-rw-r--r--   0 root         (0) root         (0)     5675 2023-06-08 00:28:04.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/keewidb/v20220308/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    37283 2023-06-08 00:28:04.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/keewidb/v20220308/keewidb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:28:04.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/keewidb/v20220308/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   137323 2023-06-08 00:28:04.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/keewidb/v20220308/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 00:28:04.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/keewidb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-08 00:28:04.000000 tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-08 00:28:04.000000 tencentcloud-sdk-python-keewidb-3.0.909/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-08 00:28:05.000000 tencentcloud-sdk-python-keewidb-3.0.909/setup.cfg
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.908/README.rst` & `tencentcloud-sdk-python-keewidb-3.0.909/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud_sdk_python_keewidb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-keewidb
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Keewidb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/keewidb/v20220308/errorcodes.py` & `tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/keewidb/v20220308/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/keewidb/v20220308/keewidb_client.py` & `tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/keewidb/v20220308/keewidb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/keewidb/v20220308/models.py` & `tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/keewidb/v20220308/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-keewidb-3.0.908/tencentcloud/__init__.py` & `tencentcloud-sdk-python-keewidb-3.0.909/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-keewidb-3.0.908/PKG-INFO` & `tencentcloud-sdk-python-keewidb-3.0.909/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-keewidb
-Version: 3.0.908
+Version: 3.0.909
 Summary: Tencent Cloud Keewidb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-keewidb-3.0.908/setup.py` & `tencentcloud-sdk-python-keewidb-3.0.909/setup.py`

 * *Files identical despite different names*

