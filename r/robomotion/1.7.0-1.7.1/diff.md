# Comparing `tmp/robomotion-1.7.0.tar.gz` & `tmp/robomotion-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robomotion-1.7.0.tar", last modified: Thu May 11 08:22:21 2023, max compression
+gzip compressed data, was "robomotion-1.7.1.tar", last modified: Thu Jun  8 09:47:23 2023, max compression
```

## Comparing `robomotion-1.7.0.tar` & `robomotion-1.7.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-05-11 08:22:21.332186 robomotion-1.7.0/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-05-11 08:22:21.332186 robomotion-1.7.0/PKG-INFO
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-05-11 08:22:21.332186 robomotion-1.7.0/robomotion/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        0 2022-08-24 12:32:15.000000 robomotion-1.7.0/robomotion/__init__.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     3855 2023-05-10 12:05:40.000000 robomotion-1.7.0/robomotion/debug.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      660 2023-05-10 13:07:28.000000 robomotion-1.7.0/robomotion/decorators.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      338 2023-05-10 12:21:12.000000 robomotion-1.7.0/robomotion/error.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1877 2023-05-10 12:54:39.000000 robomotion-1.7.0/robomotion/event.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      264 2022-08-24 12:32:15.000000 robomotion-1.7.0/robomotion/factory.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      800 2022-08-24 12:32:15.000000 robomotion-1.7.0/robomotion/health.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1601 2023-05-11 08:19:42.000000 robomotion-1.7.0/robomotion/health_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2457 2023-05-11 08:21:19.000000 robomotion-1.7.0/robomotion/health_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)  1674682 2023-05-10 13:04:16.000000 robomotion-1.7.0/robomotion/icons.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1183 2023-05-10 12:12:01.000000 robomotion-1.7.0/robomotion/message.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     3392 2022-09-21 11:29:46.000000 robomotion-1.7.0/robomotion/node.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2116 2022-08-24 12:32:15.000000 robomotion-1.7.0/robomotion/plugin.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     7084 2023-05-11 08:22:14.000000 robomotion-1.7.0/robomotion/plugin_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    26015 2023-05-11 08:21:29.000000 robomotion-1.7.0/robomotion/plugin_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2735 2023-05-11 08:19:56.000000 robomotion-1.7.0/robomotion/runner_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    11076 2023-05-11 08:21:35.000000 robomotion-1.7.0/robomotion/runner_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     4268 2023-05-10 14:20:53.000000 robomotion-1.7.0/robomotion/runtime.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)    21852 2023-05-10 14:23:42.000000 robomotion-1.7.0/robomotion/spec.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     2436 2023-05-11 08:20:07.000000 robomotion-1.7.0/robomotion/struct_pb2.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      159 2023-05-11 08:20:07.000000 robomotion-1.7.0/robomotion/struct_pb2_grpc.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      507 2023-05-10 13:44:29.000000 robomotion-1.7.0/robomotion/utils.py
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     6969 2023-05-10 14:12:19.000000 robomotion-1.7.0/robomotion/variable.py
-drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-05-11 08:22:21.332186 robomotion-1.7.0/robomotion.egg-info/
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-05-11 08:22:21.000000 robomotion-1.7.0/robomotion.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      747 2023-05-11 08:22:21.000000 robomotion-1.7.0/robomotion.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-05-11 08:22:21.000000 robomotion-1.7.0/robomotion.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-05-11 08:16:43.000000 robomotion-1.7.0/robomotion.egg-info/not-zip-safe
--rw-rw-r--   0 hasan     (1000) hasan     (1000)      100 2023-05-11 08:22:21.000000 robomotion-1.7.0/robomotion.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)       11 2023-05-11 08:22:21.000000 robomotion-1.7.0/robomotion.egg-info/top_level.txt
--rw-rw-r--   0 hasan     (1000) hasan     (1000)       38 2023-05-11 08:22:21.332186 robomotion-1.7.0/setup.cfg
--rw-rw-r--   0 hasan     (1000) hasan     (1000)     1420 2023-05-11 08:13:25.000000 robomotion-1.7.0/setup.py
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-08 09:47:23.291285 robomotion-1.7.1/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-06-08 09:47:23.287285 robomotion-1.7.1/PKG-INFO
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-08 09:47:23.287285 robomotion-1.7.1/robomotion/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        0 2022-08-24 12:32:15.000000 robomotion-1.7.1/robomotion/__init__.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     3855 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/debug.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      660 2023-05-10 13:07:28.000000 robomotion-1.7.1/robomotion/decorators.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      338 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/error.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1877 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/event.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      264 2022-08-24 12:32:15.000000 robomotion-1.7.1/robomotion/factory.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      800 2022-08-24 12:32:15.000000 robomotion-1.7.1/robomotion/health.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1601 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/health_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2457 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/health_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)  1674682 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/icons.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1183 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/message.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     3392 2022-09-21 11:29:46.000000 robomotion-1.7.1/robomotion/node.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2116 2022-08-24 12:32:15.000000 robomotion-1.7.1/robomotion/plugin.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     7084 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/plugin_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    26015 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/plugin_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2735 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/runner_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    11076 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/runner_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     4268 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/runtime.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)    21852 2023-06-08 09:30:51.000000 robomotion-1.7.1/robomotion/spec.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     2436 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/struct_pb2.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      159 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/struct_pb2_grpc.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      507 2023-06-08 09:30:16.000000 robomotion-1.7.1/robomotion/utils.py
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     7035 2023-06-08 09:40:11.000000 robomotion-1.7.1/robomotion/variable.py
+drwxrwxr-x   0 hasan     (1000) hasan     (1000)        0 2023-06-08 09:47:23.287285 robomotion-1.7.1/robomotion.egg-info/
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      510 2023-06-08 09:47:23.000000 robomotion-1.7.1/robomotion.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      747 2023-06-08 09:47:23.000000 robomotion-1.7.1/robomotion.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-06-08 09:47:23.000000 robomotion-1.7.1/robomotion.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)        1 2023-05-11 08:16:43.000000 robomotion-1.7.1/robomotion.egg-info/not-zip-safe
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)      100 2023-06-08 09:47:23.000000 robomotion-1.7.1/robomotion.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)       11 2023-06-08 09:47:23.000000 robomotion-1.7.1/robomotion.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)       38 2023-06-08 09:47:23.291285 robomotion-1.7.1/setup.cfg
+-rw-rw-r--   0 hasan     (1000) hasan     (1000)     1420 2023-06-08 09:44:55.000000 robomotion-1.7.1/setup.py
```

### Comparing `robomotion-1.7.0/robomotion/debug.py` & `robomotion-1.7.1/robomotion/debug.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/decorators.py` & `robomotion-1.7.1/robomotion/decorators.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/event.py` & `robomotion-1.7.1/robomotion/event.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/health.py` & `robomotion-1.7.1/robomotion/health.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/health_pb2.py` & `robomotion-1.7.1/robomotion/health_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/health_pb2_grpc.py` & `robomotion-1.7.1/robomotion/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/icons.py` & `robomotion-1.7.1/robomotion/icons.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/message.py` & `robomotion-1.7.1/robomotion/message.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/node.py` & `robomotion-1.7.1/robomotion/node.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/plugin.py` & `robomotion-1.7.1/robomotion/plugin.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/plugin_pb2.py` & `robomotion-1.7.1/robomotion/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/plugin_pb2_grpc.py` & `robomotion-1.7.1/robomotion/plugin_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/runner_pb2.py` & `robomotion-1.7.1/robomotion/runner_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/runner_pb2_grpc.py` & `robomotion-1.7.1/robomotion/runner_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/runtime.py` & `robomotion-1.7.1/robomotion/runtime.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/spec.py` & `robomotion-1.7.1/robomotion/spec.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -323,14 +323,16 @@
                         formData[name] = {"scope": option.scope, "name": option.name}
                         uiOrder.append(name)
 
                     for _option in options:
                         option = _option["val"]
                         optObject = {"type": option.type, "title": option.title}
 
+                        name = Spec.lower_first_letter(_option["key"])
+
                         category = option.category
                         if category != ECategory.Null:
                             optObject["category"] = int(category)
                         if option.description != "":
                             optObject["description"] = option.description
                             pUISchema[name] = {"ui:field": "input"}
                         if option.format != "":
@@ -340,16 +342,14 @@
                         if option.enum is not None:
                             enums = option.enum.enums
                             if enums is not None and len(enums) > 0:
                                 enumNames = option.enum.enumNames
                                 optObject["enum"] = enums
                                 optObject["enumNames"] = enumNames
 
-                        name = Spec.lower_first_letter(_option["key"])
-
                         if option.hidden:
                             pUISchema[name] = {"ui:widget": "hidden"}
 
                         if option.default is not None:
                             formData[name] = option.default
 
                         optProperties[name] = optObject
```

### Comparing `robomotion-1.7.0/robomotion/struct_pb2.py` & `robomotion-1.7.1/robomotion/struct_pb2.py`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/robomotion/variable.py` & `robomotion-1.7.1/robomotion/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         hidden: bool = False,
         input: bool = False,
         output: bool = False,
         option: bool = False,
         default: _DefVal = None,
         enum: _Enum = None,
         format: str = "",
-        arrayFields: str = "",
+        arrayFields: str = None,
     ):
         self.__scope = scope
         self.__name = name
         self.__title = title
         self.__type = type
         self.__description = description
         self.__jsScope = jsScope
@@ -156,14 +156,17 @@
 
     @property
     def format(self) -> str:
         return self.__format
 
     @property
     def arrayFields(self) -> list[str]:
+        if self.__arrayFields is None:
+            return None
+
         return self.__arrayFields.split("|")
 
 
 class InVariable(Variable):
     def get(self, ctx: Context):
         return Runtime.get_variable(self, ctx)
```

### Comparing `robomotion-1.7.0/robomotion.egg-info/SOURCES.txt` & `robomotion-1.7.1/robomotion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robomotion-1.7.0/setup.py` & `robomotion-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "jsonpath-ng==1.5.3",
     "pickle5==0.0.11",
     "zipp==3.1.0",
 ]
 
 setup(
     name=PROJECT_PACKAGE_NAME,
-    version="1.7.0",
+    version="1.7.1",
     url=PROJECT_URL,
     project_urls=PROJECT_URLS,
     author=PROJECT_AUTHOR,
     author_email=PROJECT_EMAIL,
     packages=PACKAGES,
     include_package_data=True,
     zip_safe=False,
```

