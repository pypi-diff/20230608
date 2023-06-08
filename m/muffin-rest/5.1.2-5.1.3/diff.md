# Comparing `tmp/muffin_rest-5.1.2.tar.gz` & `tmp/muffin_rest-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_rest-5.1.2.tar", max compression
+gzip compressed data, was "muffin_rest-5.1.3.tar", max compression
```

## Comparing `muffin_rest-5.1.2.tar` & `muffin_rest-5.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1082 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/LICENSE
--rw-r--r--   0        0        0     2616 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/README.rst
--rw-r--r--   0        0        0     1242 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/muffin_rest/__init__.py
--rw-r--r--   0        0        0     3882 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/muffin_rest/api.py
--rw-r--r--   0        0        0     1169 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/muffin_rest/errors.py
--rw-r--r--   0        0        0     5164 2023-06-08 07:10:19.930306 muffin_rest-5.1.2/muffin_rest/filters.py
--rw-r--r--   0        0        0    10762 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/handler.py
--rw-r--r--   0        0        0     4805 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/__init__.py
--rw-r--r--   0        0        0      921 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/filters.py
--rw-r--r--   0        0        0     1205 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/schema.py
--rw-r--r--   0        0        0      870 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/sorting.py
--rw-r--r--   0        0        0      206 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/types.py
--rw-r--r--   0        0        0     3946 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/mongo/utils.py
--rw-r--r--   0        0        0     8770 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/openapi.py
--rw-r--r--   0        0        0     1927 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/options.py
--rw-r--r--   0        0        0      129 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/__init__.py
--rw-r--r--   0        0        0     2839 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/filters.py
--rw-r--r--   0        0        0     5325 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/handler.py
--rw-r--r--   0        0        0     1111 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/openapi.py
--rw-r--r--   0        0        0     1489 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/options.py
--rw-r--r--   0        0        0     1076 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/schemas.py
--rw-r--r--   0        0        0     1780 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/sorting.py
--rw-r--r--   0        0        0      155 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/peewee/types.py
--rw-r--r--   0        0        0        0 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/py.typed
--rw-r--r--   0        0        0      559 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/redoc.html
--rw-r--r--   0        0        0     2803 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/sorting.py
--rw-r--r--   0        0        0     6514 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2460 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/sqlalchemy/filters.py
--rw-r--r--   0        0        0     1643 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/sqlalchemy/sorting.py
--rw-r--r--   0        0        0      204 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/sqlalchemy/types.py
--rw-r--r--   0        0        0     1736 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/swagger.html
--rw-r--r--   0        0        0      521 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/types.py
--rw-r--r--   0        0        0     2059 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/muffin_rest/utils.py
--rw-r--r--   0        0        0     2826 2023-06-08 07:10:19.934306 muffin_rest-5.1.2/pyproject.toml
--rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/LICENSE
+-rw-r--r--   0        0        0     2616 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/README.rst
+-rw-r--r--   0        0        0     1242 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/__init__.py
+-rw-r--r--   0        0        0     3882 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/api.py
+-rw-r--r--   0        0        0     1169 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/errors.py
+-rw-r--r--   0        0        0     5164 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/filters.py
+-rw-r--r--   0        0        0    10762 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/handler.py
+-rw-r--r--   0        0        0     4805 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/mongo/__init__.py
+-rw-r--r--   0        0        0      921 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/mongo/filters.py
+-rw-r--r--   0        0        0     1205 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/mongo/schema.py
+-rw-r--r--   0        0        0      870 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/mongo/sorting.py
+-rw-r--r--   0        0        0      206 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/mongo/types.py
+-rw-r--r--   0        0        0     3946 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/mongo/utils.py
+-rw-r--r--   0        0        0     8770 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/openapi.py
+-rw-r--r--   0        0        0     1927 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/options.py
+-rw-r--r--   0        0        0      129 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/peewee/__init__.py
+-rw-r--r--   0        0        0     2895 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/peewee/filters.py
+-rw-r--r--   0        0        0     5325 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/peewee/handler.py
+-rw-r--r--   0        0        0     1111 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/peewee/openapi.py
+-rw-r--r--   0        0        0     1489 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/peewee/options.py
+-rw-r--r--   0        0        0     1076 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/peewee/schemas.py
+-rw-r--r--   0        0        0     1780 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/peewee/sorting.py
+-rw-r--r--   0        0        0      155 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/peewee/types.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:25:35.001999 muffin_rest-5.1.3/muffin_rest/py.typed
+-rw-r--r--   0        0        0      559 2023-06-08 07:25:35.005999 muffin_rest-5.1.3/muffin_rest/redoc.html
+-rw-r--r--   0        0        0     2803 2023-06-08 07:25:35.005999 muffin_rest-5.1.3/muffin_rest/sorting.py
+-rw-r--r--   0        0        0     6514 2023-06-08 07:25:35.005999 muffin_rest-5.1.3/muffin_rest/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2460 2023-06-08 07:25:35.005999 muffin_rest-5.1.3/muffin_rest/sqlalchemy/filters.py
+-rw-r--r--   0        0        0     1643 2023-06-08 07:25:35.005999 muffin_rest-5.1.3/muffin_rest/sqlalchemy/sorting.py
+-rw-r--r--   0        0        0      204 2023-06-08 07:25:35.005999 muffin_rest-5.1.3/muffin_rest/sqlalchemy/types.py
+-rw-r--r--   0        0        0     1736 2023-06-08 07:25:35.005999 muffin_rest-5.1.3/muffin_rest/swagger.html
+-rw-r--r--   0        0        0      521 2023-06-08 07:25:35.005999 muffin_rest-5.1.3/muffin_rest/types.py
+-rw-r--r--   0        0        0     2059 2023-06-08 07:25:35.005999 muffin_rest-5.1.3/muffin_rest/utils.py
+-rw-r--r--   0        0        0     2826 2023-06-08 07:25:35.005999 muffin_rest-5.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4126 1970-01-01 00:00:00.000000 muffin_rest-5.1.3/PKG-INFO
```

### Comparing `muffin_rest-5.1.2/LICENSE` & `muffin_rest-5.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/README.rst` & `muffin_rest-5.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/__init__.py` & `muffin_rest-5.1.3/muffin_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/api.py` & `muffin_rest-5.1.3/muffin_rest/api.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/errors.py` & `muffin_rest-5.1.3/muffin_rest/errors.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/filters.py` & `muffin_rest-5.1.3/muffin_rest/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/handler.py` & `muffin_rest-5.1.3/muffin_rest/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/mongo/__init__.py` & `muffin_rest-5.1.3/muffin_rest/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/mongo/filters.py` & `muffin_rest-5.1.3/muffin_rest/mongo/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/mongo/schema.py` & `muffin_rest-5.1.3/muffin_rest/mongo/schema.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/mongo/sorting.py` & `muffin_rest-5.1.3/muffin_rest/mongo/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/mongo/utils.py` & `muffin_rest-5.1.3/muffin_rest/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/openapi.py` & `muffin_rest-5.1.3/muffin_rest/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/options.py` & `muffin_rest-5.1.3/muffin_rest/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/peewee/filters.py` & `muffin_rest-5.1.3/muffin_rest/peewee/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,9 +80,13 @@
     if candidate:
         return candidate
 
     for field in fields.values():
         if field.column_name == name:
             return field
 
-    warn(f"{handler.__qualname__} {handler.meta.model} has no field {name}", stacklevel=3)
+    warn(
+        f"{handler.__qualname__} {handler.meta.model} has no field {name}",
+        category=RuntimeWarning,
+        stacklevel=5,
+    )
     return None
```

### Comparing `muffin_rest-5.1.2/muffin_rest/peewee/handler.py` & `muffin_rest-5.1.3/muffin_rest/peewee/handler.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/peewee/openapi.py` & `muffin_rest-5.1.3/muffin_rest/peewee/openapi.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/peewee/options.py` & `muffin_rest-5.1.3/muffin_rest/peewee/options.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/peewee/schemas.py` & `muffin_rest-5.1.3/muffin_rest/peewee/schemas.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/peewee/sorting.py` & `muffin_rest-5.1.3/muffin_rest/peewee/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/redoc.html` & `muffin_rest-5.1.3/muffin_rest/redoc.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/sorting.py` & `muffin_rest-5.1.3/muffin_rest/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/sqlalchemy/__init__.py` & `muffin_rest-5.1.3/muffin_rest/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/sqlalchemy/filters.py` & `muffin_rest-5.1.3/muffin_rest/sqlalchemy/filters.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/sqlalchemy/sorting.py` & `muffin_rest-5.1.3/muffin_rest/sqlalchemy/sorting.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/swagger.html` & `muffin_rest-5.1.3/muffin_rest/swagger.html`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/types.py` & `muffin_rest-5.1.3/muffin_rest/types.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/muffin_rest/utils.py` & `muffin_rest-5.1.3/muffin_rest/utils.py`

 * *Files identical despite different names*

### Comparing `muffin_rest-5.1.2/pyproject.toml` & `muffin_rest-5.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-rest"
-version = "5.1.2"
+version = "5.1.3"
 description = "The package provides enhanced support for writing REST APIs with Muffin framework"
 readme = "README.rst"
 homepage = "https://github.com/klen/muffin-rest"
 repository = "https://github.com/klen/muffin-rest"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["rest", "api", "muffin", "asgi", "asyncio", "trio"]
```

### Comparing `muffin_rest-5.1.2/PKG-INFO` & `muffin_rest-5.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-rest
-Version: 5.1.2
+Version: 5.1.3
 Summary: The package provides enhanced support for writing REST APIs with Muffin framework
 Home-page: https://github.com/klen/muffin-rest
 License: MIT
 Keywords: rest,api,muffin,asgi,asyncio,trio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

