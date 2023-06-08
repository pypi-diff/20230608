# Comparing `tmp/quickstart-vdk-0.2.891782372.dev11189.tar.gz` & `tmp/quickstart-vdk-0.2.893274445.dev11226.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.891782372.dev11189.tar", last modified: Wed Jun  7 04:23:02 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.893274445.dev11226.tar", last modified: Thu Jun  8 04:22:29 2023, max compression
```

## Comparing `quickstart-vdk-0.2.891782372.dev11189.tar` & `quickstart-vdk-0.2.893274445.dev11226.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:23:02.188911 quickstart-vdk-0.2.891782372.dev11189/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-07 04:23:02.184911 quickstart-vdk-0.2.891782372.dev11189/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-07 04:20:08.000000 quickstart-vdk-0.2.891782372.dev11189/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:23:02.184911 quickstart-vdk-0.2.891782372.dev11189/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-07 04:23:02.000000 quickstart-vdk-0.2.891782372.dev11189/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-07 04:23:02.000000 quickstart-vdk-0.2.891782372.dev11189/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 04:23:02.000000 quickstart-vdk-0.2.891782372.dev11189/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-07 04:23:02.000000 quickstart-vdk-0.2.891782372.dev11189/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-07 04:23:02.000000 quickstart-vdk-0.2.891782372.dev11189/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 04:23:02.188911 quickstart-vdk-0.2.891782372.dev11189/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-07 04:22:52.000000 quickstart-vdk-0.2.891782372.dev11189/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 04:23:02.184911 quickstart-vdk-0.2.891782372.dev11189/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-07 04:20:08.000000 quickstart-vdk-0.2.891782372.dev11189/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:22:29.080235 quickstart-vdk-0.2.893274445.dev11226/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-08 04:22:29.080235 quickstart-vdk-0.2.893274445.dev11226/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-08 04:19:40.000000 quickstart-vdk-0.2.893274445.dev11226/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:22:29.080235 quickstart-vdk-0.2.893274445.dev11226/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-08 04:22:29.000000 quickstart-vdk-0.2.893274445.dev11226/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-08 04:22:29.000000 quickstart-vdk-0.2.893274445.dev11226/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 04:22:29.000000 quickstart-vdk-0.2.893274445.dev11226/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-08 04:22:29.000000 quickstart-vdk-0.2.893274445.dev11226/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-08 04:22:29.000000 quickstart-vdk-0.2.893274445.dev11226/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 04:22:29.080235 quickstart-vdk-0.2.893274445.dev11226/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-08 04:22:16.000000 quickstart-vdk-0.2.893274445.dev11226/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 04:22:29.080235 quickstart-vdk-0.2.893274445.dev11226/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-08 04:19:40.000000 quickstart-vdk-0.2.893274445.dev11226/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.891782372.dev11189/PKG-INFO` & `quickstart-vdk-0.2.893274445.dev11226/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.891782372.dev11189
+Version: 0.2.893274445.dev11226
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.891782372.dev11189/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.893274445.dev11226/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.891782372.dev11189
+Version: 0.2.893274445.dev11226
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.891782372.dev11189/setup.py` & `quickstart-vdk-0.2.893274445.dev11226/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.891782372.dev11189"
+__version__ = "0.2.893274445.dev11226"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

