# Comparing `tmp/neulabs-cdk-constructs-0.4.5.tar.gz` & `tmp/neulabs-cdk-constructs-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.4.5.tar", last modified: Wed Jun  7 14:53:31 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.4.6.tar", last modified: Thu Jun  8 07:17:49 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.4.5.tar` & `neulabs-cdk-constructs-0.4.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.246003 neulabs-cdk-constructs-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-07 14:53:31.246003 neulabs-cdk-constructs-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:53:31.246003 neulabs-cdk-constructs-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115223 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.5.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   299578 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-07 14:53:31.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-07 14:53:31.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:53:31.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 14:53:31.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 14:53:31.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:17:49.169861 neulabs-cdk-constructs-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115239 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.6.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   299578 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-08 07:17:36.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:17:49.173861 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-08 07:17:49.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-08 07:17:49.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:17:49.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-08 07:17:49.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 07:17:49.000000 neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.4.5/LICENSE` & `neulabs-cdk-constructs-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.5/PKG-INFO` & `neulabs-cdk-constructs-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.4.5
+Version: 0.4.6
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.4.5/README.md` & `neulabs-cdk-constructs-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.5/setup.py` & `neulabs-cdk-constructs-0.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.4.5",
+    "version": "0.4.6",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,15 +27,15 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.4.5.jsii.tgz"
+            "neulabs-cdk-constructs@0.4.6.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.4.5",
+    "0.4.6",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.4.5.jsii.tgz",
+    "neulabs-cdk-constructs@0.4.6.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.4.5
+Version: 0.4.6
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.4.6/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.5.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.6.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

