# Comparing `tmp/muffin_rest-5.1.1.tar.gz` & `tmp/muffin_rest-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-5.1.1.tar", max compression
+gzip compressed data, was "muffin_rest-5.1.2.tar", max compression
```

## Comparing `muffin_rest-5.1.1.tar` & `muffin_rest-5.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1082 2023-06-08 06:55:11.906407 muffin_rest-5.1.1/LICENSE
--rw-r--r--   0        0        0     2616 2023-06-08 06:55:11.906407 muffin_rest-5.1.1/README.rst
--rw-r--r--   0        0        0     1242 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/errors.py
--rw-r--r--   0        0        0     5164 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/filters.py
--rw-r--r--   0        0        0    10762 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/handler.py
--rw-r--r--   0        0        0     4805 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8770 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/options.py
--rw-r--r--   0        0        0      129 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2788 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     5325 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/peewee/handler.py
--rw-r--r--   0        0        0     1111 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1076 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     1780 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0        0 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2803 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6514 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2460 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     1736 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/swagger.html
--rw-r--r--   0        0        0      521 2023-06-08 06:55:11.910407 muffin_rest-5.1.1/muffin_rest/types.py
--rw-r--r--   0        0        0     2059 2023-06-08 06:55:11.914407 muffin_rest-5.1.1/muffin_rest/utils.py
--rw-r--r--   0        0        0     2826 2023-06-08 06:55:11.914407 muffin_rest-5.1.1/pyproject.toml
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/LICENSE
+-rw-r--r--   0        0        0     2616 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/README.rst
+-rw-r--r--   0        0        0     1242 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5164 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10762 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4805 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8770 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/options.py
+-rw-r--r--   0        0        0      129 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2839 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     5325 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/handler.py
+-rw-r--r--   0        0        0     1111 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1076 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     1780 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2803 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6514 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2460 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     1736 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      521 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/types.py
+-rw-r--r--   0        0        0     2059 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2826 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.1.2/PKG-INFO
```

### Comparing `muffin_rest-5.1.1/LICENSE` & `muffin_rest-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/README.rst` & `muffin_rest-5.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/__init__.py` & `muffin_rest-5.1.2/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/api.py` & `muffin_rest-5.1.2/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/errors.py` & `muffin_rest-5.1.2/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/filters.py` & `muffin_rest-5.1.2/muffin_rest/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/handler.py` & `muffin_rest-5.1.2/muffin_rest/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/mongo/__init__.py` & `muffin_rest-5.1.2/muffin_rest/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/mongo/filters.py` & `muffin_rest-5.1.2/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/mongo/schema.py` & `muffin_rest-5.1.2/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/mongo/sorting.py` & `muffin_rest-5.1.2/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/mongo/utils.py` & `muffin_rest-5.1.2/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/openapi.py` & `muffin_rest-5.1.2/muffin_rest/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/options.py` & `muffin_rest-5.1.2/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/peewee/filters.py` & `muffin_rest-5.1.2/muffin_rest/peewee/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Support filters for Peewee ORM."""
 from __future__ import annotations
 
 import operator
 from typing import Any, Callable, Optional, Tuple, Type, Union, cast
+from warnings import warn
 
 from peewee import Field, ModelSelect
 
 from muffin_rest.filters import Filter, Filters
 
 
 class PWFilter(Filter):
@@ -47,41 +48,41 @@
     MUTATE_CLASS: Type[PWFilter] = PWFilter
 
     def convert(self, obj: Union[str, Field, PWFilter], **meta):
         """Convert params to filters."""
         from . import PWRESTHandler
 
         handler = cast(PWRESTHandler, self.handler)
-        model = handler.meta.model
         if isinstance(obj, PWFilter):
             if obj.field is None:
-                obj.field = get_model_field_by_name(model, obj.name)
+                obj.field = get_model_field_by_name(handler, obj.name)
             return obj
 
         if isinstance(obj, Field):
             name = obj.name
             field = obj
 
         else:
             name = obj
             field = meta.pop("field", None) or name
             if isinstance(field, str):
-                field = get_model_field_by_name(model, field)
+                field = get_model_field_by_name(handler, field)
 
         schema_field = meta.pop("schema_field", None)
         if schema_field is None and field:
             schema_field = handler.meta.Schema._declared_fields.get(field.name)
         return self.MUTATE_CLASS(name, field=field, schema_field=schema_field, **meta)
 
 
-def get_model_field_by_name(model, name) -> Optional[Field]:
+def get_model_field_by_name(handler, name) -> Optional[Field]:
     """Get model field by name."""
-    mfields = model._meta.fields
-    candidate = mfields.get(name)
+    fields = handler.meta.model._meta.fields
+    candidate = fields.get(name)
     if candidate:
         return candidate
 
-    for field in mfields.values():
+    for field in fields.values():
         if field.column_name == name:
             return field
 
-    raise AttributeError(f"Model {model} has no field {name}")
+    warn(f"{handler.__qualname__} {handler.meta.model} has no field {name}", stacklevel=3)
+    return None
```

### Comparing `muffin_rest-5.1.1/muffin_rest/peewee/handler.py` & `muffin_rest-5.1.2/muffin_rest/peewee/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/peewee/openapi.py` & `muffin_rest-5.1.2/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/peewee/options.py` & `muffin_rest-5.1.2/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/peewee/schemas.py` & `muffin_rest-5.1.2/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/peewee/sorting.py` & `muffin_rest-5.1.2/muffin_rest/peewee/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/redoc.html` & `muffin_rest-5.1.2/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/sorting.py` & `muffin_rest-5.1.2/muffin_rest/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-5.1.2/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-5.1.2/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-5.1.2/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/swagger.html` & `muffin_rest-5.1.2/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/types.py` & `muffin_rest-5.1.2/muffin_rest/types.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/muffin_rest/utils.py` & `muffin_rest-5.1.2/muffin_rest/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.1/pyproject.toml` & `muffin_rest-5.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "5.1.1"
+version = "5.1.2"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
```

### Comparing `muffin_rest-5.1.1/PKG-INFO` & `muffin_rest-5.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 5.1.1
+Version: 5.1.2
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

