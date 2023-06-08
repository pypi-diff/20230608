# Comparing `tmp/configzen-0.2.6.tar.gz` & `tmp/configzen-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.2.6.tar", max compression
+gzip compressed data, was "configzen-0.2.7.tar", max compression
```

## Comparing `configzen-0.2.6.tar` & `configzen-0.2.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.6/configzen/__init__.py
--rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.6/configzen/__main__.py
--rw-r--r--   0        0        0    67942 2023-06-06 17:33:04.155792 configzen-0.2.6/configzen/config.py
--rw-r--r--   0        0        0     2460 2023-06-05 06:53:12.902541 configzen-0.2.6/configzen/errors.py
--rw-r--r--   0        0        0    30568 2023-06-06 18:05:58.215336 configzen-0.2.6/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.6/configzen/py.typed
--rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.6/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.6/LICENSE
--rw-r--r--   0        0        0     1154 2023-06-06 18:07:10.641354 configzen-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.6/README.md
--rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.2.7/configzen/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-30 00:29:12.190684 configzen-0.2.7/configzen/__main__.py
+-rw-r--r--   0        0        0    67943 2023-06-08 00:25:44.808854 configzen-0.2.7/configzen/config.py
+-rw-r--r--   0        0        0     2460 2023-06-05 06:53:12.902541 configzen-0.2.7/configzen/errors.py
+-rw-r--r--   0        0        0    30568 2023-06-06 18:05:58.215336 configzen-0.2.7/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.2.7/configzen/py.typed
+-rw-r--r--   0        0        0     1047 2023-06-05 06:53:17.656362 configzen-0.2.7/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1154 2023-06-08 00:27:45.715601 configzen-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     7155 2023-05-30 19:13:13.036046 configzen-0.2.7/README.md
+-rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 configzen-0.2.7/PKG-INFO
```

### Comparing `configzen-0.2.6/configzen/__main__.py` & `configzen-0.2.7/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.6/configzen/config.py` & `configzen-0.2.7/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 ) -> dict[str, Any]:
     defaults = {}
     for field in model.__fields__.values():
         default = field.default
         if not field.field_info.exclude and not field.required:
             if isinstance(default, pydantic.BaseModel):
                 default = default.dict()
-            defaults[field.name] = default
+            defaults[field.alias] = default
     return defaults
 
 
 def _vars(obj: Any) -> dict[str, Any]:
     obj_dict = obj
     if not isinstance(obj, dict):
         obj_dict = obj.__dict__
```

### Comparing `configzen-0.2.6/configzen/errors.py` & `configzen-0.2.7/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.6/configzen/processor.py` & `configzen-0.2.7/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.6/configzen/typedefs.py` & `configzen-0.2.7/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.2.6/LICENSE` & `configzen-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.2.6/pyproject.toml` & `configzen-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.2.6"
+version = "0.2.7"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.2.6/README.md` & `configzen-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.2.6/PKG-INFO` & `configzen-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.2.6
+Version: 0.2.7
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

