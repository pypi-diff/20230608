# Comparing `tmp/ask-sdk-dynamodb-persistence-adapter-1.8.0.tar.gz` & `tmp/ask-sdk-dynamodb-persistence-adapter-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ask-sdk-dynamodb-persistence-adapter-1.8.0.tar", last modified: Thu Feb 28 01:25:28 2019, max compression
+gzip compressed data, was "dist/ask-sdk-dynamodb-persistence-adapter-1.9.0.tar", last modified: Tue Mar 19 12:00:56 2019, max compression
```

## Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0.tar` & `ask-sdk-dynamodb-persistence-adapter-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2579 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/CHANGELOG.rst
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb_persistence_adapter.egg-info/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      556 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb_persistence_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb_persistence_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       17 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb_persistence_adapter.egg-info/top_level.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb_persistence_adapter.egg-info/not-zip-safe
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6962 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb_persistence_adapter.egg-info/PKG-INFO
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       26 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb_persistence_adapter.egg-info/requires.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       26 2019-02-28 01:25:20.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/requirements.txt
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)       67 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/setup.cfg
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      107 2019-02-28 01:25:20.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/MANIFEST.in
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2083 2019-02-28 01:25:20.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/README.rst
-drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb/
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2191 2019-02-28 01:25:20.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb/partition_keygen.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)      592 2019-02-28 01:25:20.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb/__init__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     9152 2019-02-28 01:25:20.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb/adapter.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1175 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb/__version__.py
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     6962 2019-02-28 01:25:28.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/PKG-INFO
--rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2148 2019-02-28 01:25:20.000000 ask-sdk-dynamodb-persistence-adapter-1.8.0/setup.py
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2740 2019-03-19 12:00:55.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/CHANGELOG.rst
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb_persistence_adapter.egg-info/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      556 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb_persistence_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb_persistence_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       17 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb_persistence_adapter.egg-info/top_level.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)        1 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb_persistence_adapter.egg-info/not-zip-safe
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7187 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb_persistence_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       26 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb_persistence_adapter.egg-info/requires.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       26 2019-03-19 12:00:48.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/requirements.txt
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)       67 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/setup.cfg
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      107 2019-03-19 12:00:48.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/MANIFEST.in
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2083 2019-03-19 12:00:48.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/README.rst
+drwxr-xr-x   0 ask-pyth (2504581) amazon     (100)        0 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb/
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2191 2019-03-19 12:00:48.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb/partition_keygen.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)      592 2019-03-19 12:00:48.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb/__init__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     9152 2019-03-19 12:00:48.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb/adapter.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     1175 2019-03-19 12:00:55.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb/__version__.py
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     7187 2019-03-19 12:00:56.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/PKG-INFO
+-rw-r--r--   0 ask-pyth (2504581) amazon     (100)     2148 2019-03-19 12:00:48.000000 ask-sdk-dynamodb-persistence-adapter-1.9.0/setup.py
```

### Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0/CHANGELOG.rst` & `ask-sdk-dynamodb-persistence-adapter-1.9.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

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

### Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb_persistence_adapter.egg-info/SOURCES.txt` & `ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb_persistence_adapter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb_persistence_adapter.egg-info/PKG-INFO` & `ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb_persistence_adapter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ask-sdk-dynamodb-persistence-adapter
-Version: 1.8.0
+Version: 1.9.0
 Summary: The ASK SDK DynamoDB Persistence Adapter package provides DynamoDB Adapter, that can be used with ASK SDK Core, for persistence management.
 Home-page: https://github.com/alexa/alexa-skills-kit-sdk-for-python
 Author: Alexa Skills Kit
 Author-email: ask-sdk-dynamic@amazon.com
 License: Apache 2.0
 Description: ========================================================
         ASK SDK DynamoDB Adapter of Python ASK SDK
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
 Keywords: ASK SDK,Alexa Skills Kit,Alexa,ASK SDK Core,Persistence,DynamoDB
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0/README.rst` & `ask-sdk-dynamodb-persistence-adapter-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb/partition_keygen.py` & `ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb/partition_keygen.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb/__init__.py` & `ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb/adapter.py` & `ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb/adapter.py`

 * *Files identical despite different names*

### Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0/ask_sdk_dynamodb/__version__.py` & `ask-sdk-dynamodb-persistence-adapter-1.9.0/ask_sdk_dynamodb/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 #
 
 __pip_package_name__ = 'ask-sdk-dynamodb-persistence-adapter'
 __description__ = (
     'The ASK SDK DynamoDB Persistence Adapter package provides DynamoDB '
     'Adapter, that can be used with ASK SDK Core, for persistence management.')
 __url__ = 'https://github.com/alexa/alexa-skills-kit-sdk-for-python'
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 __author__ = 'Alexa Skills Kit'
 __author_email__ = 'ask-sdk-dynamic@amazon.com'
 __license__ = 'Apache 2.0'
 __keywords__ = ['ASK SDK', 'Alexa Skills Kit', 'Alexa', 'ASK SDK Core',
                 'Persistence', 'DynamoDB']
 __install_requires__ = ["boto3", "ask-sdk-core>=1.1.0"]
```

### Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0/PKG-INFO` & `ask-sdk-dynamodb-persistence-adapter-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ask-sdk-dynamodb-persistence-adapter
-Version: 1.8.0
+Version: 1.9.0
 Summary: The ASK SDK DynamoDB Persistence Adapter package provides DynamoDB Adapter, that can be used with ASK SDK Core, for persistence management.
 Home-page: https://github.com/alexa/alexa-skills-kit-sdk-for-python
 Author: Alexa Skills Kit
 Author-email: ask-sdk-dynamic@amazon.com
 License: Apache 2.0
 Description: ========================================================
         ASK SDK DynamoDB Adapter of Python ASK SDK
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
 Keywords: ASK SDK,Alexa Skills Kit,Alexa,ASK SDK Core,Persistence,DynamoDB
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ask-sdk-dynamodb-persistence-adapter-1.8.0/setup.py` & `ask-sdk-dynamodb-persistence-adapter-1.9.0/setup.py`

 * *Files identical despite different names*

