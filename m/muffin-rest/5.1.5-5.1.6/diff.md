# Comparing `tmp/muffin_rest-5.1.5.tar.gz` & `tmp/muffin_rest-5.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-5.1.5.tar", max compression
+gzip compressed data, was "muffin_rest-5.1.6.tar", max compression
```

## Comparing `muffin_rest-5.1.5.tar` & `muffin_rest-5.1.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1082 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/LICENSE
--rw-r--r--   0        0        0     2616 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/README.rst
--rw-r--r--   0        0        0     1242 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/errors.py
--rw-r--r--   0        0        0     5164 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/filters.py
--rw-r--r--   0        0        0    10762 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/handler.py
--rw-r--r--   0        0        0     4805 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8770 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/options.py
--rw-r--r--   0        0        0      129 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2315 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     5325 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/peewee/handler.py
--rw-r--r--   0        0        0     1111 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1076 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     1848 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-06-08 07:51:35.320129 muffin_rest-5.1.5/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0      702 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/peewee/utils.py
--rw-r--r--   0        0        0        0 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2803 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6514 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2460 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     1736 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/swagger.html
--rw-r--r--   0        0        0      521 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/types.py
--rw-r--r--   0        0        0     2059 2023-06-08 07:51:35.324129 muffin_rest-5.1.5/muffin_rest/utils.py
--rw-r--r--   0        0        0     2826 2023-06-08 07:51:35.328129 muffin_rest-5.1.5/pyproject.toml
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-08 09:52:25.897685 muffin_rest-5.1.6/LICENSE
+-rw-r--r--   0        0        0     2616 2023-06-08 09:52:25.897685 muffin_rest-5.1.6/README.rst
+-rw-r--r--   0        0        0     1242 2023-06-08 09:52:25.897685 muffin_rest-5.1.6/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-06-08 09:52:25.897685 muffin_rest-5.1.6/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-06-08 09:52:25.897685 muffin_rest-5.1.6/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5164 2023-06-08 09:52:25.897685 muffin_rest-5.1.6/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10762 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4805 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8770 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/options.py
+-rw-r--r--   0        0        0      129 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2332 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     5325 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/peewee/handler.py
+-rw-r--r--   0        0        0     1111 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1076 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     1848 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0      702 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/peewee/utils.py
+-rw-r--r--   0        0        0        0 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2803 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6514 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2460 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     1736 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      521 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/types.py
+-rw-r--r--   0        0        0     2059 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2826 2023-06-08 09:52:25.901685 muffin_rest-5.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.1.6/PKG-INFO
```

### Comparing `muffin_rest-5.1.5/LICENSE` & `muffin_rest-5.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/README.rst` & `muffin_rest-5.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/__init__.py` & `muffin_rest-5.1.6/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/api.py` & `muffin_rest-5.1.6/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/errors.py` & `muffin_rest-5.1.6/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/filters.py` & `muffin_rest-5.1.6/muffin_rest/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/handler.py` & `muffin_rest-5.1.6/muffin_rest/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/mongo/__init__.py` & `muffin_rest-5.1.6/muffin_rest/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/mongo/filters.py` & `muffin_rest-5.1.6/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/mongo/schema.py` & `muffin_rest-5.1.6/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/mongo/sorting.py` & `muffin_rest-5.1.6/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/mongo/utils.py` & `muffin_rest-5.1.6/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/openapi.py` & `muffin_rest-5.1.6/muffin_rest/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/options.py` & `muffin_rest-5.1.6/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/peewee/filters.py` & `muffin_rest-5.1.6/muffin_rest/peewee/filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Support filters for Peewee ORM."""
 from __future__ import annotations
 
 import operator
 from typing import Any, Callable, Tuple, Type, Union, cast
 
-from peewee import Field, ModelSelect
+from peewee import ColumnBase, Field, ModelSelect
 
 from muffin_rest.filters import Filter, Filters
 
 from .utils import get_model_field_by_name
 
 
 class PWFilter(Filter):
@@ -33,15 +33,15 @@
         """Apply the filters to Peewee QuerySet.."""
         if self.field and ops:
             return self.query(collection, self.field, *ops, **kwargs)
         return collection
 
     def query(self, qs: ModelSelect, column: Field, *ops: Tuple, **_) -> ModelSelect:
         """Filter a query."""
-        if isinstance(column, Field):
+        if isinstance(column, ColumnBase):
             return cast(ModelSelect, qs.where(*[op(column, val) for op, val in ops]))
 
         return qs
 
 
 class PWFilters(Filters):
     """Bind Peewee filter class."""
```

### Comparing `muffin_rest-5.1.5/muffin_rest/peewee/handler.py` & `muffin_rest-5.1.6/muffin_rest/peewee/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/peewee/openapi.py` & `muffin_rest-5.1.6/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/peewee/options.py` & `muffin_rest-5.1.6/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/peewee/schemas.py` & `muffin_rest-5.1.6/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/peewee/sorting.py` & `muffin_rest-5.1.6/muffin_rest/peewee/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/peewee/utils.py` & `muffin_rest-5.1.6/muffin_rest/peewee/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/redoc.html` & `muffin_rest-5.1.6/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/sorting.py` & `muffin_rest-5.1.6/muffin_rest/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-5.1.6/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-5.1.6/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-5.1.6/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/swagger.html` & `muffin_rest-5.1.6/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/types.py` & `muffin_rest-5.1.6/muffin_rest/types.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/muffin_rest/utils.py` & `muffin_rest-5.1.6/muffin_rest/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.5/pyproject.toml` & `muffin_rest-5.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "5.1.5"
+version = "5.1.6"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
```

### Comparing `muffin_rest-5.1.5/PKG-INFO` & `muffin_rest-5.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 5.1.5
+Version: 5.1.6
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

