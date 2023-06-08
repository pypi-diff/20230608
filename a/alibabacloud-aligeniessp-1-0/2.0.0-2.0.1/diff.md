# Comparing `tmp/alibabacloud_aligeniessp_1_0-2.0.0.tar.gz` & `tmp/alibabacloud_aligeniessp_1_0-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aligeniessp_1_0-2.0.0.tar", last modified: Fri Jun  2 03:06:26 2023, max compression
+gzip compressed data, was "dist/alibabacloud_aligeniessp_1_0-2.0.1.tar", last modified: Thu Jun  8 08:10:01 2023, max compression
```

## Comparing `alibabacloud_aligeniessp_1_0-2.0.0.tar` & `alibabacloud_aligeniessp_1_0-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2353 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1035 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1120 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   364870 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   842921 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2353 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2634 2023-06-02 03:06:26.000000 alibabacloud_aligeniessp_1_0-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)      759 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1120 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   364870 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   842921 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-06-08 08:10:01.000000 alibabacloud_aligeniessp_1_0-2.0.1/setup.py
```

### Comparing `alibabacloud_aligeniessp_1_0-2.0.0/ChangeLog.md` & `alibabacloud_aligeniessp_1_0-2.0.1/ChangeLog.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-06-02 Version: 2.0.0
+- 修改ScgSearch返回结果类型.
+
 2022-10-17 Version: 1.0.14
 - Add ScanCodeBind api.
 
 2022-10-08 Version: 1.0.13
 - Add EcologyAuthenticate api.
 
 2022-09-08 Version: 1.0.12
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_aligeniessp_1_0-2.0.0/LICENSE` & `alibabacloud_aligeniessp_1_0-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligeniessp_1_0-2.0.0/PKG-INFO` & `alibabacloud_aligeniessp_1_0-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aligeniessp_1_0
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud AliGenie (ssp_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligeniessp_1_0-2.0.0/README-CN.md` & `alibabacloud_aligeniessp_1_0-2.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligeniessp_1_0-2.0.0/README.md` & `alibabacloud_aligeniessp_1_0-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/client.py` & `alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0/models.py` & `alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aligeniessp_1_0-2.0.0/alibabacloud_aligeniessp_1_0.egg-info/PKG-INFO` & `alibabacloud_aligeniessp_1_0-2.0.1/alibabacloud_aligeniessp_1_0.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aligeniessp-1-0
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud AliGenie (ssp_1_0) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aligeniessp_1_0-2.0.0/setup.py` & `alibabacloud_aligeniessp_1_0-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aligeniessp_1_0.
 
-Created on 02/06/2023
+Created on 08/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aligeniessp_1_0"
 NAME = "alibabacloud_aligeniessp_1_0" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AliGenie (ssp_1_0) SDK Library for Python"
```

