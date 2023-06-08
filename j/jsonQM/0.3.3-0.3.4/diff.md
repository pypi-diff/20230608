# Comparing `tmp/jsonQM-0.3.3.tar.gz` & `tmp/jsonQM-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonQM-0.3.3.tar", last modified: Wed Jun  7 23:33:00 2023, max compression
+gzip compressed data, was "jsonQM-0.3.4.tar", last modified: Thu Jun  8 00:41:59 2023, max compression
```

## Comparing `jsonQM-0.3.3.tar` & `jsonQM-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 23:33:00.688119 jsonQM-0.3.3/
--rw-rw-rw-   0        0        0     1067 2023-06-07 21:14:44.000000 jsonQM-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     4308 2023-06-07 23:33:00.685108 jsonQM-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     3762 2023-06-07 23:27:03.000000 jsonQM-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 23:33:00.658110 jsonQM-0.3.3/jsonQM/
--rw-rw-rw-   0        0        0       72 2023-06-07 21:14:44.000000 jsonQM-0.3.3/jsonQM/__init__.py
--rw-rw-rw-   0        0        0     2060 2023-06-07 23:11:45.000000 jsonQM-0.3.3/jsonQM/model.py
--rw-rw-rw-   0        0        0     2003 2023-06-07 23:22:05.000000 jsonQM-0.3.3/jsonQM/modelserializer.py
-drwxrwxrwx   0        0        0        0 2023-06-07 23:33:00.679119 jsonQM-0.3.3/jsonQM.egg-info/
--rw-rw-rw-   0        0        0     4308 2023-06-07 23:33:00.000000 jsonQM-0.3.3/jsonQM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-06-07 23:33:00.000000 jsonQM-0.3.3/jsonQM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 23:33:00.000000 jsonQM-0.3.3/jsonQM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-07 23:33:00.000000 jsonQM-0.3.3/jsonQM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 23:33:00.688119 jsonQM-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1162 2023-06-07 23:32:35.000000 jsonQM-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 23:33:00.681109 jsonQM-0.3.3/tests/
--rw-rw-rw-   0        0        0     3359 2023-06-07 22:52:55.000000 jsonQM-0.3.3/tests/test_model.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:41:59.244167 jsonQM-0.3.4/
+-rw-rw-rw-   0        0        0     1067 2023-06-07 21:14:44.000000 jsonQM-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     4605 2023-06-08 00:41:59.243186 jsonQM-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4057 2023-06-08 00:41:15.000000 jsonQM-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 00:41:59.222182 jsonQM-0.3.4/jsonQM/
+-rw-rw-rw-   0        0        0       72 2023-06-07 21:14:44.000000 jsonQM-0.3.4/jsonQM/__init__.py
+-rw-rw-rw-   0        0        0     2241 2023-06-08 00:32:01.000000 jsonQM-0.3.4/jsonQM/model.py
+-rw-rw-rw-   0        0        0     2003 2023-06-07 23:22:05.000000 jsonQM-0.3.4/jsonQM/modelserializer.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:41:59.238210 jsonQM-0.3.4/jsonQM.egg-info/
+-rw-rw-rw-   0        0        0     4605 2023-06-08 00:41:59.000000 jsonQM-0.3.4/jsonQM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-08 00:41:59.000000 jsonQM-0.3.4/jsonQM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 00:41:59.000000 jsonQM-0.3.4/jsonQM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-08 00:41:59.000000 jsonQM-0.3.4/jsonQM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 00:41:59.245169 jsonQM-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2023-06-08 00:40:28.000000 jsonQM-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:41:59.240188 jsonQM-0.3.4/tests/
+-rw-rw-rw-   0        0        0     3574 2023-06-08 00:36:26.000000 jsonQM-0.3.4/tests/test_model.py
```

### Comparing `jsonQM-0.3.3/LICENSE` & `jsonQM-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonQM-0.3.3/PKG-INFO` & `jsonQM-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonQM
-Version: 0.3.3
+Version: 0.3.4
 Summary: A simple tool to easily make your API endpoint json queries more versatile.
 Author: William A. Lim
 Author-email: william.lim@csu.fullerton.edu
 Project-URL: Source, https://github.com/FrewtyPebbles/jsonQM
 Project-URL: Tracker, https://github.com/FrewtyPebbles/jsonQM/issues
 Keywords: python,json,request,query,model
 Classifier: Programming Language :: Python :: 3
@@ -32,15 +32,16 @@
 # Declare a model serializer
 ms = ModelSerializer() # Each model must have its own serializer
 class MyModel(Model):
     def __init__(self) -> None:
         # define the structure of the query model:
         self.model = {
             # we have a single query scope/section called functions
-            "functions":{}
+            "functions":{},
+            "msg":"test" # non functional attributes also need to be included in the json query if you wish for them to be present in the response (see Example query 3 below)
         }
         # sync/add the model attribute functions to the model
         ms.sync(self)
         
     # Define attributes of the model (argument 2) along with the scope/section they are found in (argument 1)
     @ms.add(["functions"], "repeater")  # This attribute key is "repeater" and can be found in the "functions" dict
     def repeater(self, arg:int):
@@ -117,9 +118,16 @@
     #Example query 3
     print(model_instance.get({
         "secret":[]
     }))
 
     # prints:
     # {'secret': 'error:token:missing'}
-```
 
+    #Example query 3
+    print(model_instance.get({
+        "msg":1
+    }))
+
+    # prints:
+    # {'msg': 'test'}
+```
```

### Comparing `jsonQM-0.3.3/README.md` & `jsonQM-0.3.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 # Declare a model serializer
 ms = ModelSerializer() # Each model must have its own serializer
 class MyModel(Model):
     def __init__(self) -> None:
         # define the structure of the query model:
         self.model = {
             # we have a single query scope/section called functions
-            "functions":{}
+            "functions":{},
+            "msg":"test" # non functional attributes also need to be included in the json query if you wish for them to be present in the response (see Example query 3 below)
         }
         # sync/add the model attribute functions to the model
         ms.sync(self)
         
     # Define attributes of the model (argument 2) along with the scope/section they are found in (argument 1)
     @ms.add(["functions"], "repeater")  # This attribute key is "repeater" and can be found in the "functions" dict
     def repeater(self, arg:int):
@@ -103,9 +104,16 @@
     #Example query 3
     print(model_instance.get({
         "secret":[]
     }))
 
     # prints:
     # {'secret': 'error:token:missing'}
-```
 
+    #Example query 3
+    print(model_instance.get({
+        "msg":1
+    }))
+
+    # prints:
+    # {'msg': 'test'}
+```
```

### Comparing `jsonQM-0.3.3/jsonQM/model.py` & `jsonQM-0.3.4/jsonQM/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 
+from typing import Callable
+
+
 class Model:
     def __init__(self) -> None:
         self.model = {}
 
-    def _get(self, query:dict, model = {}, token_result:bool = None):
+    def _get(self, query:dict, model:dict = {}, token_result:bool = None):
         compiled_query = {}
         for key, value in query.items():
             if type(value) == dict:
                 compiled_query[key] = self._get(value, model[key])
             elif type(value) == list:
                 if hasattr(model[key], '_requires_token'):
                     if hasattr(self, '_token'):
@@ -19,14 +22,17 @@
                             compiled_query[key] = "error:token:missing"
                     else:
                         compiled_query[key] = "error:token:missing"
                 elif hasattr(model[key], '_token'):
                     compiled_query[key] = token_result
                 else:
                     compiled_query[key] = model[key](*value)
+            elif key in model.keys():
+                if type(model[key]) != Callable:
+                    compiled_query[key] = model[key]
             else:
                 compiled_query[key] = value
 
         return compiled_query
 
     def get(self, query:dict):
         """
```

### Comparing `jsonQM-0.3.3/jsonQM/modelserializer.py` & `jsonQM-0.3.4/jsonQM/modelserializer.py`

 * *Files identical despite different names*

### Comparing `jsonQM-0.3.3/jsonQM.egg-info/PKG-INFO` & `jsonQM-0.3.4/jsonQM.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonQM
-Version: 0.3.3
+Version: 0.3.4
 Summary: A simple tool to easily make your API endpoint json queries more versatile.
 Author: William A. Lim
 Author-email: william.lim@csu.fullerton.edu
 Project-URL: Source, https://github.com/FrewtyPebbles/jsonQM
 Project-URL: Tracker, https://github.com/FrewtyPebbles/jsonQM/issues
 Keywords: python,json,request,query,model
 Classifier: Programming Language :: Python :: 3
@@ -32,15 +32,16 @@
 # Declare a model serializer
 ms = ModelSerializer() # Each model must have its own serializer
 class MyModel(Model):
     def __init__(self) -> None:
         # define the structure of the query model:
         self.model = {
             # we have a single query scope/section called functions
-            "functions":{}
+            "functions":{},
+            "msg":"test" # non functional attributes also need to be included in the json query if you wish for them to be present in the response (see Example query 3 below)
         }
         # sync/add the model attribute functions to the model
         ms.sync(self)
         
     # Define attributes of the model (argument 2) along with the scope/section they are found in (argument 1)
     @ms.add(["functions"], "repeater")  # This attribute key is "repeater" and can be found in the "functions" dict
     def repeater(self, arg:int):
@@ -117,9 +118,16 @@
     #Example query 3
     print(model_instance.get({
         "secret":[]
     }))
 
     # prints:
     # {'secret': 'error:token:missing'}
-```
 
+    #Example query 3
+    print(model_instance.get({
+        "msg":1
+    }))
+
+    # prints:
+    # {'msg': 'test'}
+```
```

### Comparing `jsonQM-0.3.3/setup.py` & `jsonQM-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.3' 
+VERSION = '0.3.4' 
 DESCRIPTION = 'A simple tool to easily make your API endpoint json queries more versatile.'
 file = open("README.md", 'r')
 LONG_DESCRIPTION = file.read()
 file.close()
 
 # Setting up
 setup(
```

### Comparing `jsonQM-0.3.3/tests/test_model.py` & `jsonQM-0.3.4/tests/test_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 # MODEL
 ms = ModelSerializer()  # Each model must have its own serializer
 class MyModel(Model):
     def __init__(self) -> None:
         # define the structure of the query model:
         self.model = {
             # we have a single query scope/section called functions
-            "functions": {}
+            "functions": {},
+            "msg":"test"
         }
         # sync/add the model attribute functions to the model
         ms.sync(self)
 
     @ms.add(["functions"], "repeater")
     def repeater(self, arg: int):
         return ["repeat" for _ in range(arg)]
@@ -36,91 +37,97 @@
         return "super secret function message"
 
     @ms.requires_token()
     @ms.add([], "secret")
     def secret(self):
         return "super secret message"
 
-
+model = MyModel()
 class TestModel(unittest.TestCase):
     def test_token_success(self):
-        model = MyModel()
         self.assertEqual(model.get({
             "token": ["token"],
             "functions": {
                 "repeater": [5],
                 7: [],
                 "secret": []
             },
             "secret": [],
+            'msg':1
         }), 
         {
             'functions': {
                 'repeater': [
                     'repeat', 
                     'repeat', 
                     'repeat', 
                     'repeat', 
                     'repeat'
                 ], 
                 7: 'zzz', 
                 'secret': 'super secret function message'
             }, 
             'secret': 'super secret message', 
-            'token': True
+            'token': True,
+            "msg":"test"
         })
 
     def test_token_invalid(self):
-        model = MyModel()
         self.assertEqual(model.get({
             "token": ["aaa"],
             "functions": {
                 "repeater": [5],
                 7: [],
                 "secret": []
             },
             "secret": [],
+            'msg':1
         }), 
         {
             'functions': {
                 'repeater': [
                     'repeat', 
                     'repeat', 
                     'repeat', 
                     'repeat', 
                     'repeat'
                 ], 
                 7: 'zzz', 
                 'secret': 'error:token:invalid'
             }, 
             'secret': 'error:token:invalid', 
-            'token': False
+            'token': False,
+            "msg":"test"
         })
 
     def test_token_missing(self):
-        model = MyModel()
         self.assertEqual(model.get({
             "functions": {
                 "repeater": [5],
                 7: [],
                 "secret": []
             },
             "secret": [],
+            'msg':1
         }), 
         {
             'functions': {
                 'repeater': [
                     'repeat', 
                     'repeat', 
                     'repeat', 
                     'repeat', 
                     'repeat'
                 ], 
                 7: 'zzz', 
                 'secret': 'error:token:missing'
             }, 
-            'secret': 'error:token:missing', 
+            'secret': 'error:token:missing',
+            "msg":"test"
         })
+    
+    def test_default_attribute(self):
+        self.assertEqual(model.get({'msg':1}), {'msg': 'test'})
 
 
 if __name__ == '__main__':
     unittest.main()
```

