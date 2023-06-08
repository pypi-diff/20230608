# Comparing `tmp/formal-sdk-0.5.0.tar.gz` & `tmp/formal-sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formal-sdk-0.5.0.tar", last modified: Thu Jun  8 14:08:18 2023, max compression
+gzip compressed data, was "formal-sdk-0.6.0.tar", last modified: Thu Jun  8 14:08:31 2023, max compression
```

## Comparing `formal-sdk-0.5.0.tar` & `formal-sdk-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:18.251840 formal-sdk-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 14:08:04.000000 formal-sdk-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 14:08:04.000000 formal-sdk-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-08 14:08:18.251840 formal-sdk-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-08 14:08:04.000000 formal-sdk-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 14:08:04.000000 formal-sdk-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:08:18.251840 formal-sdk-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:18.251840 formal-sdk-0.5.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-08 14:08:04.000000 formal-sdk-0.5.0/src/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:18.251840 formal-sdk-0.5.0/src/formal_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:04.000000 formal-sdk-0.5.0/src/formal_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-08 14:08:04.000000 formal-sdk-0.5.0/src/formal_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-08 14:08:04.000000 formal-sdk-0.5.0/src/formal_sdk/datastore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:18.251840 formal-sdk-0.5.0/src/formal_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-08 14:08:18.000000 formal-sdk-0.5.0/src/formal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 14:08:18.000000 formal-sdk-0.5.0/src/formal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:08:18.000000 formal-sdk-0.5.0/src/formal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 14:08:18.000000 formal-sdk-0.5.0/src/formal_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 14:08:18.000000 formal-sdk-0.5.0/src/formal_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:31.500161 formal-sdk-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-08 14:08:31.500161 formal-sdk-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:08:31.500161 formal-sdk-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:31.496161 formal-sdk-0.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/src/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:31.496161 formal-sdk-0.6.0/src/formal_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/src/formal_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 14:08:14.000000 formal-sdk-0.6.0/src/formal_sdk/datastore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:08:31.500161 formal-sdk-0.6.0/src/formal_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-08 14:08:31.000000 formal-sdk-0.6.0/src/formal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 14:08:31.000000 formal-sdk-0.6.0/src/formal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:08:31.000000 formal-sdk-0.6.0/src/formal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 14:08:31.000000 formal-sdk-0.6.0/src/formal_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 14:08:31.000000 formal-sdk-0.6.0/src/formal_sdk.egg-info/top_level.txt
```

### Comparing `formal-sdk-0.5.0/LICENSE` & `formal-sdk-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `formal-sdk-0.5.0/PKG-INFO` & `formal-sdk-0.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 0.5.0
+Version: 0.6.0
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -42,25 +42,25 @@
 
 ## Example Use
 
 Create and Get a Native Role
 
 ```python
 import os
-from formal_sdk import client
+import formal_sdk
 
 if __name__ == '__main__':
 
     dataStoreId = "e092e9f7-bb67-231s-949d-a4343299b18f"
     nativeRoleId = "abc"
     nativeRoleSecret = "nativeSecret"
     useAsDefault = True
     apiKey = os.environ.get('TEST_API_KEY')
     
-    newClient = Client(apiKey)
+    newClient = formal_sdk.Client(apiKey)
     # Create Native Role
     createdRole = newClient.DataStoreClient.CreateNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId, nativeRoleSecret=nativeRoleSecret, useAsDefault=useAsDefault)
     
     # Get Native Role    
     previousRole = newClient.DataStoreClient.GetNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId)
 
     print(f'DataStoreId: {previousRole.dataStoreId}')
```

### Comparing `formal-sdk-0.5.0/README.md` & `formal-sdk-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 
 ## Example Use
 
 Create and Get a Native Role
 
 ```python
 import os
-from formal_sdk import client
+import formal_sdk
 
 if __name__ == '__main__':
 
     dataStoreId = "e092e9f7-bb67-231s-949d-a4343299b18f"
     nativeRoleId = "abc"
     nativeRoleSecret = "nativeSecret"
     useAsDefault = True
     apiKey = os.environ.get('TEST_API_KEY')
     
-    newClient = Client(apiKey)
+    newClient = formal_sdk.Client(apiKey)
     # Create Native Role
     createdRole = newClient.DataStoreClient.CreateNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId, nativeRoleSecret=nativeRoleSecret, useAsDefault=useAsDefault)
     
     # Get Native Role    
     previousRole = newClient.DataStoreClient.GetNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId)
 
     print(f'DataStoreId: {previousRole.dataStoreId}')
```

### Comparing `formal-sdk-0.5.0/src/formal_sdk/datastore.py` & `formal-sdk-0.6.0/src/formal_sdk/datastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 import json
 
+
 class NativeRole:
     def __init__(self, datastoreId, nativeRoleId, nativeRoleSecret, useAsDefault):
         self.dataStoreId = datastoreId
         self.nativeRoleId = nativeRoleId
         self.nativeRoleSecret = nativeRoleSecret
         self.useAsDefault = useAsDefault
 
@@ -45,8 +46,8 @@
         }
         response = requests.post(url, headers=self.headers, data=json.dumps(payload))
 
         if response.status_code != 200:
             raise Exception(f'Request failed with status {response.status_code}')
 
         native_role_data = response.json().get('nativeRole', {})
-        return NativeRole(**native_role_data)
+        return NativeRole(**native_role_data)
```

### Comparing `formal-sdk-0.5.0/src/formal_sdk.egg-info/PKG-INFO` & `formal-sdk-0.6.0/src/formal_sdk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formal-sdk
-Version: 0.5.0
+Version: 0.6.0
 Summary: Formal SDK
 Author-email: Formal <hello@joinformal.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -42,25 +42,25 @@
 
 ## Example Use
 
 Create and Get a Native Role
 
 ```python
 import os
-from formal_sdk import client
+import formal_sdk
 
 if __name__ == '__main__':
 
     dataStoreId = "e092e9f7-bb67-231s-949d-a4343299b18f"
     nativeRoleId = "abc"
     nativeRoleSecret = "nativeSecret"
     useAsDefault = True
     apiKey = os.environ.get('TEST_API_KEY')
     
-    newClient = Client(apiKey)
+    newClient = formal_sdk.Client(apiKey)
     # Create Native Role
     createdRole = newClient.DataStoreClient.CreateNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId, nativeRoleSecret=nativeRoleSecret, useAsDefault=useAsDefault)
     
     # Get Native Role    
     previousRole = newClient.DataStoreClient.GetNativeRole(dataStoreId=dataStoreId, nativeRoleId=nativeRoleId)
 
     print(f'DataStoreId: {previousRole.dataStoreId}')
```

