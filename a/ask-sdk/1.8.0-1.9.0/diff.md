# Comparing `tmp/ask-sdk-1.8.0.tar.gz` & `tmp/ask-sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ask-sdk-1.8.0.tar", last modified: Thu Feb 28 01:25:32 2019, max compression
+gzip compressed data, was "dist/ask-sdk-1.9.0.tar", last modified: Tue Mar 19 12:00:59 2019, max compression
```

## Comparing `ask-sdk-1.8.0.tar` & `ask-sdk-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2539 2019-02-28 01:25:31.000000 ask-sdk-1.8.0/CHANGELOG.rst
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       64 2019-02-28 01:25:20.000000 ask-sdk-1.8.0/requirements.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       67 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/setup.cfg
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/ask_sdk.egg-info/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      319 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/ask_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/ask_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        8 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/ask_sdk.egg-info/top_level.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/ask_sdk.egg-info/not-zip-safe
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6671 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/ask_sdk.egg-info/PKG-INFO
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       64 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/ask_sdk.egg-info/requires.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      107 2019-02-28 01:25:20.000000 ask-sdk-1.8.0/MANIFEST.in
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1863 2019-02-28 01:25:20.000000 ask-sdk-1.8.0/README.rst
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/ask_sdk/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4188 2019-02-28 01:25:20.000000 ask-sdk-1.8.0/ask_sdk/standard.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      593 2019-02-28 01:25:20.000000 ask-sdk-1.8.0/ask_sdk/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1185 2019-02-28 01:25:31.000000 ask-sdk-1.8.0/ask_sdk/__version__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6671 2019-02-28 01:25:32.000000 ask-sdk-1.8.0/PKG-INFO
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2139 2019-02-28 01:25:20.000000 ask-sdk-1.8.0/setup.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2700 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/CHANGELOG.rst
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       64 2019-03-19 12:00:48.000000 ask-sdk-1.9.0/requirements.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       67 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/setup.cfg
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/ask_sdk.egg-info/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      319 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/ask_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/ask_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        8 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/ask_sdk.egg-info/top_level.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/ask_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6896 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/ask_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       64 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/ask_sdk.egg-info/requires.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      107 2019-03-19 12:00:48.000000 ask-sdk-1.9.0/MANIFEST.in
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1863 2019-03-19 12:00:48.000000 ask-sdk-1.9.0/README.rst
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/ask_sdk/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     4188 2019-03-19 12:00:48.000000 ask-sdk-1.9.0/ask_sdk/standard.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      593 2019-03-19 12:00:48.000000 ask-sdk-1.9.0/ask_sdk/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1185 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/ask_sdk/__version__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6896 2019-03-19 12:00:59.000000 ask-sdk-1.9.0/PKG-INFO
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2139 2019-03-19 12:00:48.000000 ask-sdk-1.9.0/setup.py
```

### Comparing `ask-sdk-1.8.0/CHANGELOG.rst` & `ask-sdk-1.9.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -95,7 +95,15 @@
 1.8.0
 ~~~~~~~
 
 This release contains the following changes : 
 
 - Allow Default API Client to invoke Alexa APIs that require other than 'application/json' body type.
 
+
+
+1.9.0
+~~~~~~~
+
+This release includes the following : 
+
+- Request utility methods which makes it easier to retrieve common properties from an incoming request.
```

### Comparing `ask-sdk-1.8.0/ask_sdk.egg-info/PKG-INFO` & `ask-sdk-1.9.0/ask_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ask-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: The ASK SDK Standard package provides a full distribution of the SDK, all batteries included, for building Alexa Skills.
 Home-page: https://github.com/alexa/alexa-skills-kit-sdk-for-python
 Author: Alexa Skills Kit
 Author-email: ask-sdk-dynamic@amazon.com
 License: Apache 2.0
 Description: ========================================================
         ASK SDK - Standard / Full distribution of Python ASK SDK
@@ -158,14 +158,22 @@
         ~~~~~~~
         
         This release contains the following changes : 
         
         - Allow Default API Client to invoke Alexa APIs that require other than 'application/json' body type.
         
         
+        
+        1.9.0
+        ~~~~~~~
+        
+        This release includes the following : 
+        
+        - Request utility methods which makes it easier to retrieve common properties from an incoming request.
+        
 Keywords: ASK SDK,Alexa Skills Kit,Alexa,ASK SDK Core,Persistence,DynamoDB,ASK SDK Standard
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ask-sdk-1.8.0/README.rst` & `ask-sdk-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `ask-sdk-1.8.0/ask_sdk/standard.py` & `ask-sdk-1.9.0/ask_sdk/standard.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-1.8.0/ask_sdk/__init__.py` & `ask-sdk-1.9.0/ask_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-1.8.0/ask_sdk/__version__.py` & `ask-sdk-1.9.0/ask_sdk/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 #
 
 __pip_package_name__ = 'ask-sdk'
 __description__ = (
     'The ASK SDK Standard package provides a full distribution of the SDK, '
     'all batteries included, for building Alexa Skills.')
 __url__ = 'https://github.com/alexa/alexa-skills-kit-sdk-for-python'
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 __author__ = 'Alexa Skills Kit'
 __author_email__ = 'ask-sdk-dynamic@amazon.com'
 __license__ = 'Apache 2.0'
 __keywords__ = ['ASK SDK', 'Alexa Skills Kit', 'Alexa', 'ASK SDK Core',
                 'Persistence', 'DynamoDB', 'ASK SDK Standard']
 __install_requires__ = ["ask-sdk-core>=1.1.0", "ask-sdk-dynamodb-persistence-adapter>=1.1.0"]
```

### Comparing `ask-sdk-1.8.0/PKG-INFO` & `ask-sdk-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ask-sdk
-Version: 1.8.0
+Version: 1.9.0
 Summary: The ASK SDK Standard package provides a full distribution of the SDK, all batteries included, for building Alexa Skills.
 Home-page: https://github.com/alexa/alexa-skills-kit-sdk-for-python
 Author: Alexa Skills Kit
 Author-email: ask-sdk-dynamic@amazon.com
 License: Apache 2.0
 Description: ========================================================
         ASK SDK - Standard / Full distribution of Python ASK SDK
@@ -158,14 +158,22 @@
         ~~~~~~~
         
         This release contains the following changes : 
         
         - Allow Default API Client to invoke Alexa APIs that require other than 'application/json' body type.
         
         
+        
+        1.9.0
+        ~~~~~~~
+        
+        This release includes the following : 
+        
+        - Request utility methods which makes it easier to retrieve common properties from an incoming request.
+        
 Keywords: ASK SDK,Alexa Skills Kit,Alexa,ASK SDK Core,Persistence,DynamoDB,ASK SDK Standard
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ask-sdk-1.8.0/setup.py` & `ask-sdk-1.9.0/setup.py`

 * *Files identical despite different names*

