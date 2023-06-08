# Comparing `tmp/sonic-uia2-client-0.0.3.tar.gz` & `tmp/sonic-uia2-client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonic-uia2-client-0.0.3.tar", last modified: Tue Jun  6 06:11:24 2023, max compression
+gzip compressed data, was "sonic-uia2-client-0.0.4.tar", last modified: Thu Jun  8 07:39:08 2023, max compression
```

## Comparing `sonic-uia2-client-0.0.3.tar` & `sonic-uia2-client-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.717294 sonic-uia2-client-0.0.3/client/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/client/android_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/client/uia_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.717294 sonic-uia2-client-0.0.3/common/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/resp_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/sonic_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-06 06:11:24.000000 sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-06 06:11:24.000000 sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:11:24.000000 sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 06:11:24.000000 sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/tests/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/uia2/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/uia2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/uia2/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.473238 sonic-uia2-client-0.0.4/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/client/android_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/client/uia_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.473238 sonic-uia2-client-0.0.4/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/resp_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/common/sonic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-08 07:39:08.000000 sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-08 07:39:08.000000 sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:39:08.000000 sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 07:39:08.000000 sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/tests/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:39:08.477239 sonic-uia2-client-0.0.4/uia2/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/uia2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-08 07:38:55.000000 sonic-uia2-client-0.0.4/uia2/driver.py
```

### Comparing `sonic-uia2-client-0.0.3/LICENSE` & `sonic-uia2-client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.3/PKG-INFO` & `sonic-uia2-client-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonic-uia2-client
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/SonicCloudOrg/sonic-uiautomator2-python-client
 Author: SonicCloudOrg
 Author-email: soniccloudorg@163.com
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `sonic-uia2-client-0.0.3/README.md` & `sonic-uia2-client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.3/client/android_element.py` & `sonic-uia2-client-0.0.4/client/android_element.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.3/client/uia_client.py` & `sonic-uia2-client-0.0.4/client/uia_client.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.3/common/http_client.py` & `sonic-uia2-client-0.0.4/common/http_client.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.3/common/logger.py` & `sonic-uia2-client-0.0.4/common/logger.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.3/common/models.py` & `sonic-uia2-client-0.0.4/common/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # !/usr/bin/python3
 # -*- coding: utf-8 -*-
 from dataclasses import dataclass
-from enum import StrEnum
+from enum import Enum
 from typing import Any, Optional
 
 
 @dataclass
 class ErrorMsg:
     error: str
     message: str
@@ -15,29 +15,29 @@
 @dataclass
 class BaseResp:
     session_id: str = ""
     err: Optional[ErrorMsg] = None
     value: Any = None
 
 
-class Method(StrEnum):
+class Method(Enum):
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     DELETE = "DELETE"
     PATCH = "PATCH"
 
 
-class PasteboardType(StrEnum):
+class PasteboardType(Enum):
     PLAIN_TEXT = "plaintext"
     IMAGE = "image"
     URL = "url"
 
 
-class AndroidSelector(StrEnum):
+class AndroidSelector(Enum):
     CLASS_NAME = "class name"
     Id = "id"
     ACCESSIBILITY_ID = "accessibility id"
     XPATH = "xpath"
     UIAUTOMATOR = "-android uiautomator"
```

### Comparing `sonic-uia2-client-0.0.3/common/resp_handler.py` & `sonic-uia2-client-0.0.4/common/resp_handler.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.3/setup.py` & `sonic-uia2-client-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 import os
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
-PATCH = 3
+PATCH = 4
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 setup(
     name="sonic-uia2-client",
     version=VERSION,
     author="SonicCloudOrg",
     author_email="soniccloudorg@163.com",
```

### Comparing `sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/PKG-INFO` & `sonic-uia2-client-0.0.4/sonic_uia2_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonic-uia2-client
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/SonicCloudOrg/sonic-uiautomator2-python-client
 Author: SonicCloudOrg
 Author-email: soniccloudorg@163.com
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `sonic-uia2-client-0.0.3/tests/test_driver.py` & `sonic-uia2-client-0.0.4/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.3/uia2/driver.py` & `sonic-uia2-client-0.0.4/uia2/driver.py`

 * *Files identical despite different names*

