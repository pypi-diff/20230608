# Comparing `tmp/csr_azure_utils-2.0.8.tar.gz` & `tmp/csr_azure_utils-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/csr_azure_utils-2.0.8.tar", last modified: Mon Apr 19 19:58:06 2021, max compression
+gzip compressed data, was "dist/csr_azure_utils-2.0.9.tar", last modified: Tue Oct 19 17:12:10 2021, max compression
```

## Comparing `csr_azure_utils-2.0.8.tar` & `csr_azure_utils-2.0.9.tar`

### file list

```diff
@@ -1,39 +1,37 @@
-drwxr-xr-x   0 croopa     (501) staff       (20)        0 2021-04-19 19:58:06.000000 csr_azure_utils-2.0.8/
--rw-r--r--   0 croopa     (501) staff       (20)      666 2021-04-19 19:58:06.000000 csr_azure_utils-2.0.8/PKG-INFO
--rwxr-xr-x   0 croopa     (501) staff       (20)     1065 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/LICENSE
-drwxr-xr-x   0 croopa     (501) staff       (20)        0 2021-04-19 19:58:06.000000 csr_azure_utils-2.0.8/csr_azure_utils.egg-info/
--rw-r--r--   0 croopa     (501) staff       (20)      666 2021-04-19 19:58:06.000000 csr_azure_utils-2.0.8/csr_azure_utils.egg-info/PKG-INFO
--rw-r--r--   0 croopa     (501) staff       (20)      867 2021-04-19 19:58:06.000000 csr_azure_utils-2.0.8/csr_azure_utils.egg-info/SOURCES.txt
--rw-r--r--   0 croopa     (501) staff       (20)      285 2021-04-19 19:58:06.000000 csr_azure_utils-2.0.8/csr_azure_utils.egg-info/requires.txt
--rw-r--r--   0 croopa     (501) staff       (20)       10 2021-04-19 19:58:06.000000 csr_azure_utils-2.0.8/csr_azure_utils.egg-info/top_level.txt
--rw-r--r--   0 croopa     (501) staff       (20)        1 2021-04-19 19:58:06.000000 csr_azure_utils-2.0.8/csr_azure_utils.egg-info/dependency_links.txt
--rw-r--r--   0 croopa     (501) staff       (20)     1173 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/install.sh
--rw-r--r--   0 croopa     (501) staff       (20)       76 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/MANIFEST.in
--rw-r--r--   0 croopa     (501) staff       (20)      917 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/README.md
--rwxr-xr-x   0 croopa     (501) staff       (20)     3952 2021-04-19 19:57:55.000000 csr_azure_utils-2.0.8/setup.py
-drwxr-xr-x   0 croopa     (501) staff       (20)        0 2021-04-19 19:58:06.000000 csr_azure_utils-2.0.8/csr_cloud/
--rw-r--r--   0 croopa     (501) staff       (20)    65367 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/as_azure.py
--rw-r--r--   0 croopa     (501) staff       (20)     8719 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/servicebus_utils.py
--rw-r--r--   0 croopa     (501) staff       (20)      687 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/general_utils.py
--rw-r--r--   0 croopa     (501) staff       (20)     5064 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/meta_utils.py
--rw-r--r--   0 croopa     (501) staff       (20)     9994 2021-04-15 19:35:58.000000 csr_azure_utils-2.0.8/csr_cloud/token_api.py
--rw-r--r--   0 croopa     (501) staff       (20)     3145 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/csr_cloud.py
--rwxr-xr-x   0 croopa     (501) staff       (20)     1429 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/set_default_aad_app.py
--rw-r--r--   0 croopa     (501) staff       (20)     6633 2021-04-16 18:30:38.000000 csr_azure_utils-2.0.8/csr_cloud/auth_mgr.py
--rw-r--r--   0 croopa     (501) staff       (20)     7090 2021-04-16 18:32:54.000000 csr_azure_utils-2.0.8/csr_cloud/msi_auth.py
--rw-r--r--   0 croopa     (501) staff       (20)      493 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/azure_utils.py
--rwxr-xr-x   0 croopa     (501) staff       (20)      664 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/clear_default_aad_app.py
--rwxr-xr-x   0 croopa     (501) staff       (20)      638 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/clear_token.py
--rw-r--r--   0 croopa     (501) staff       (20)       37 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/__init__.py
--rw-r--r--   0 croopa     (501) staff       (20)    11164 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/metric_utils.py
--rwxr-xr-x   0 croopa     (501) staff       (20)      658 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/clear_aad_application_list.py
--rwxr-xr-x   0 croopa     (501) staff       (20)      642 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/refresh_token.py
--rwxr-xr-x   0 croopa     (501) staff       (20)     5718 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/aad_auth.py
--rw-r--r--   0 croopa     (501) staff       (20)     2191 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/blob_utils.py
--rwxr-xr-x   0 croopa     (501) staff       (20)      662 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/show_auth_applications.py
--rwxr-xr-x   0 croopa     (501) staff       (20)     6183 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/token_svr.py
--rw-r--r--   0 croopa     (501) staff       (20)     5165 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/file_utils.py
--rw-r--r--   0 croopa     (501) staff       (20)     9577 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/csr_cloud/eventhub_utils.py
--rw-r--r--   0 croopa     (501) staff       (20)    37015 2021-04-16 18:31:54.000000 csr_azure_utils-2.0.8/csr_cloud/ha_azure.py
--rw-r--r--   0 croopa     (501) staff       (20)       59 2021-04-19 19:58:06.000000 csr_azure_utils-2.0.8/setup.cfg
--rwxr-xr-x   0 croopa     (501) staff       (20)      368 2021-04-15 17:11:12.000000 csr_azure_utils-2.0.8/auth-token.service
+drwxr-xr-x   0 croopa     (501) staff       (20)        0 2021-10-19 17:12:10.000000 csr_azure_utils-2.0.9/
+-rw-r--r--   0 croopa     (501) staff       (20)      666 2021-10-19 17:12:10.000000 csr_azure_utils-2.0.9/PKG-INFO
+drwxr-xr-x   0 croopa     (501) staff       (20)        0 2021-10-19 17:12:10.000000 csr_azure_utils-2.0.9/csr_azure_utils.egg-info/
+-rw-r--r--   0 croopa     (501) staff       (20)      666 2021-10-19 17:12:10.000000 csr_azure_utils-2.0.9/csr_azure_utils.egg-info/PKG-INFO
+-rw-r--r--   0 croopa     (501) staff       (20)      849 2021-10-19 17:12:10.000000 csr_azure_utils-2.0.9/csr_azure_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 croopa     (501) staff       (20)      249 2021-10-19 17:12:10.000000 csr_azure_utils-2.0.9/csr_azure_utils.egg-info/requires.txt
+-rw-r--r--   0 croopa     (501) staff       (20)       10 2021-10-19 17:12:10.000000 csr_azure_utils-2.0.9/csr_azure_utils.egg-info/top_level.txt
+-rw-r--r--   0 croopa     (501) staff       (20)        1 2021-10-19 17:12:10.000000 csr_azure_utils-2.0.9/csr_azure_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 croopa     (501) staff       (20)     1173 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/install.sh
+-rw-r--r--   0 croopa     (501) staff       (20)       76 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/MANIFEST.in
+-rwxr-xr-x   0 croopa     (501) staff       (20)     3894 2021-10-19 17:11:22.000000 csr_azure_utils-2.0.9/setup.py
+drwxr-xr-x   0 croopa     (501) staff       (20)        0 2021-10-19 17:12:10.000000 csr_azure_utils-2.0.9/csr_cloud/
+-rw-r--r--   0 croopa     (501) staff       (20)    65367 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/as_azure.py
+-rw-r--r--   0 croopa     (501) staff       (20)     8719 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/servicebus_utils.py
+-rw-r--r--   0 croopa     (501) staff       (20)      687 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/general_utils.py
+-rw-r--r--   0 croopa     (501) staff       (20)     5064 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/meta_utils.py
+-rw-r--r--   0 croopa     (501) staff       (20)     9994 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/token_api.py
+-rw-r--r--   0 croopa     (501) staff       (20)     3145 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/csr_cloud.py
+-rwxr-xr-x   0 croopa     (501) staff       (20)     1429 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/set_default_aad_app.py
+-rw-r--r--   0 croopa     (501) staff       (20)     6633 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/auth_mgr.py
+-rw-r--r--   0 croopa     (501) staff       (20)     7090 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/msi_auth.py
+-rw-r--r--   0 croopa     (501) staff       (20)      662 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/azure_utils.py
+-rwxr-xr-x   0 croopa     (501) staff       (20)      664 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/clear_default_aad_app.py
+-rwxr-xr-x   0 croopa     (501) staff       (20)      638 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/clear_token.py
+-rw-r--r--   0 croopa     (501) staff       (20)       37 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/__init__.py
+-rw-r--r--   0 croopa     (501) staff       (20)    11164 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/metric_utils.py
+-rwxr-xr-x   0 croopa     (501) staff       (20)      658 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/clear_aad_application_list.py
+-rwxr-xr-x   0 croopa     (501) staff       (20)      642 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/refresh_token.py
+-rwxr-xr-x   0 croopa     (501) staff       (20)     5718 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/aad_auth.py
+-rw-r--r--   0 croopa     (501) staff       (20)     2191 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/blob_utils.py
+-rwxr-xr-x   0 croopa     (501) staff       (20)      662 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/show_auth_applications.py
+-rwxr-xr-x   0 croopa     (501) staff       (20)     6183 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/token_svr.py
+-rw-r--r--   0 croopa     (501) staff       (20)     5165 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/file_utils.py
+-rw-r--r--   0 croopa     (501) staff       (20)     9577 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/eventhub_utils.py
+-rw-r--r--   0 croopa     (501) staff       (20)    37015 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/csr_cloud/ha_azure.py
+-rw-r--r--   0 croopa     (501) staff       (20)       59 2021-10-19 17:12:10.000000 csr_azure_utils-2.0.9/setup.cfg
+-rwxr-xr-x   0 croopa     (501) staff       (20)      368 2021-10-19 17:03:51.000000 csr_azure_utils-2.0.9/auth-token.service
```

### Comparing `csr_azure_utils-2.0.8/PKG-INFO` & `csr_azure_utils-2.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: csr_azure_utils
-Version: 2.0.8
+Version: 2.0.9
 Summary: Utilities for csr1000v on Azure
 Home-page: https://github4-chn.cisco.com/csr1000v-azure/csr_azure_utils
 Author: Cisco Systems Inc.
 Author-email: csr-cloud-dev@cisco.com
 License: MIT
-Download-URL: https://github4-chn.cisco.com/csr1000v-azure/csr_azure_utils/archive/2.0.8.tar.gz
+Download-URL: https://github4-chn.cisco.com/csr1000v-azure/csr_azure_utils/archive/2.0.9.tar.gz
 Description: UNKNOWN
 Keywords: cisco,azure,guestshell,csr1000v
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `csr_azure_utils-2.0.8/csr_azure_utils.egg-info/PKG-INFO` & `csr_azure_utils-2.0.9/csr_azure_utils.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: csr-azure-utils
-Version: 2.0.8
+Version: 2.0.9
 Summary: Utilities for csr1000v on Azure
 Home-page: https://github4-chn.cisco.com/csr1000v-azure/csr_azure_utils
 Author: Cisco Systems Inc.
 Author-email: csr-cloud-dev@cisco.com
 License: MIT
-Download-URL: https://github4-chn.cisco.com/csr1000v-azure/csr_azure_utils/archive/2.0.8.tar.gz
+Download-URL: https://github4-chn.cisco.com/csr1000v-azure/csr_azure_utils/archive/2.0.9.tar.gz
 Description: UNKNOWN
 Keywords: cisco,azure,guestshell,csr1000v
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `csr_azure_utils-2.0.8/csr_azure_utils.egg-info/SOURCES.txt` & `csr_azure_utils-2.0.9/csr_azure_utils.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-LICENSE
 MANIFEST.in
-README.md
 auth-token.service
 install.sh
 setup.py
 csr_azure_utils.egg-info/PKG-INFO
 csr_azure_utils.egg-info/SOURCES.txt
 csr_azure_utils.egg-info/dependency_links.txt
 csr_azure_utils.egg-info/requires.txt
```

### Comparing `csr_azure_utils-2.0.8/install.sh` & `csr_azure_utils-2.0.9/install.sh`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/setup.py` & `csr_azure_utils-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import print_function
 from distutils.core import setup
 from setuptools.command.install import install
 from subprocess import check_call, check_output
 import sys, os, platform
 
 project_name = 'csr_azure_utils'
-project_ver = '2.0.8'
+project_ver = '2.0.9'
 
 '''
 =======================================================================================
 Note
 =======================================================================================
 This file is crucial to installation of csr_azure_utils. 
 Before committing any changes to this file, please test installation of csr_azure_utils
@@ -77,22 +77,20 @@
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6'
     ],
     license="MIT",
     include_package_data=True,
     install_requires=[
-        'cryptography==2.9.2',
         'python-crontab==2.5.1',
         'pathlib==1.0.1',
         'configparser==4.0.2',
         'pyopenssl==19.1.0',
         'msrest==0.6.16',
         'msrestazure==0.6.3',
-        'paramiko==2.7.1',
         'future==0.18.2',
         'azure-storage-file==2.1.0',
         'azure-storage-blob==12.3.2',
         'azure-storage-common==2.1.0',
         'azure-storage-nspkg==3.1.0',
         'requests==2.23.0'
     ],
```

### Comparing `csr_azure_utils-2.0.8/csr_cloud/as_azure.py` & `csr_azure_utils-2.0.9/csr_cloud/as_azure.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/servicebus_utils.py` & `csr_azure_utils-2.0.9/csr_cloud/servicebus_utils.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/general_utils.py` & `csr_azure_utils-2.0.9/csr_cloud/general_utils.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/meta_utils.py` & `csr_azure_utils-2.0.9/csr_cloud/meta_utils.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/token_api.py` & `csr_azure_utils-2.0.9/csr_cloud/token_api.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/csr_cloud.py` & `csr_azure_utils-2.0.9/csr_cloud/csr_cloud.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/set_default_aad_app.py` & `csr_azure_utils-2.0.9/csr_cloud/set_default_aad_app.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/auth_mgr.py` & `csr_azure_utils-2.0.9/csr_cloud/auth_mgr.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/msi_auth.py` & `csr_azure_utils-2.0.9/csr_cloud/msi_auth.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/clear_default_aad_app.py` & `csr_azure_utils-2.0.9/csr_cloud/clear_default_aad_app.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/clear_token.py` & `csr_azure_utils-2.0.9/csr_cloud/clear_token.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/metric_utils.py` & `csr_azure_utils-2.0.9/csr_cloud/metric_utils.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/clear_aad_application_list.py` & `csr_azure_utils-2.0.9/csr_cloud/clear_aad_application_list.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/refresh_token.py` & `csr_azure_utils-2.0.9/csr_cloud/refresh_token.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/aad_auth.py` & `csr_azure_utils-2.0.9/csr_cloud/aad_auth.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/blob_utils.py` & `csr_azure_utils-2.0.9/csr_cloud/blob_utils.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/show_auth_applications.py` & `csr_azure_utils-2.0.9/csr_cloud/show_auth_applications.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/token_svr.py` & `csr_azure_utils-2.0.9/csr_cloud/token_svr.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/file_utils.py` & `csr_azure_utils-2.0.9/csr_cloud/file_utils.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/eventhub_utils.py` & `csr_azure_utils-2.0.9/csr_cloud/eventhub_utils.py`

 * *Files identical despite different names*

### Comparing `csr_azure_utils-2.0.8/csr_cloud/ha_azure.py` & `csr_azure_utils-2.0.9/csr_cloud/ha_azure.py`

 * *Files identical despite different names*

