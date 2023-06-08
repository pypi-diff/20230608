# Comparing `tmp/stac-fastapi.extensions-2.4.7.tar.gz` & `tmp/stac-fastapi.extensions-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.extensions-2.4.7.tar", last modified: Wed May 17 15:30:44 2023, max compression
+gzip compressed data, was "stac-fastapi.extensions-2.4.8.tar", last modified: Thu Jun  8 19:49:44 2023, max compression
```

## Comparing `stac-fastapi.extensions-2.4.7.tar` & `stac-fastapi.extensions-2.4.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-17 15:30:44.968150 stac-fastapi.extensions-2.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/token_pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/query/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/query/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/query/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/third_party/bulk_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 15:30:29.000000 stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:44.964150 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 15:30:44.000000 stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.367688 stac-fastapi.extensions-2.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-08 19:49:44.367688 stac-fastapi.extensions-2.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-08 19:49:44.367688 stac-fastapi.extensions-2.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.363688 stac-fastapi.extensions-2.4.8/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.363688 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.363688 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.367688 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/fields/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/fields/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.367688 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/filter/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.367688 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/pagination/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/pagination/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/pagination/token_pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.367688 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/query/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.367688 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/sort/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/sort/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/sort/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.367688 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/third_party/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/third_party/bulk_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 19:49:31.000000 stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:44.363688 stac-fastapi.extensions-2.4.8/stac_fastapi.extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-08 19:49:44.000000 stac-fastapi.extensions-2.4.8/stac_fastapi.extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-08 19:49:44.000000 stac-fastapi.extensions-2.4.8/stac_fastapi.extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:49:44.000000 stac-fastapi.extensions-2.4.8/stac_fastapi.extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:49:44.000000 stac-fastapi.extensions-2.4.8/stac_fastapi.extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 19:49:44.000000 stac-fastapi.extensions-2.4.8/stac_fastapi.extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 19:49:44.000000 stac-fastapi.extensions-2.4.8/stac_fastapi.extensions.egg-info/top_level.txt
```

### Comparing `stac-fastapi.extensions-2.4.7/PKG-INFO` & `stac-fastapi.extensions-2.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
-Version: 2.4.7
+Version: 2.4.8
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.extensions-2.4.7/setup.py` & `stac-fastapi.extensions-2.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/__init__.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/context.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/context.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 @attr.s
 class ContextExtension(ApiExtension):
     """Context Extension.
 
     The Context extension adds a JSON object to ItemCollection responses (`/search`,
     `/collections/{collection_id}/items`) which includes the number of items matched,
     returned, and the limit requested.
-    https://github.com/radiantearth/stac-api-spec/blob/master/item-search/README.md#context
+    https://github.com/stac-api-extensions/context
     """
 
     conformance_classes: List[str] = attr.ib(
-        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.1/item-search#context"]
+        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.2/item-search#context"]
     )
     schema_href: Optional[str] = attr.ib(
-        default="https://raw.githubusercontent.com/radiantearth/stac-api-spec/v1.0.0-rc.1/fragments/context/json-schema/schema.json"
+        default="https://raw.githubusercontent.com/stac-api-extensions/context/v1.0.0-rc.2/json-schema/schema.json"
     )
 
     def register(self, app: FastAPI) -> None:
         """Register the extension with a FastAPI application.
 
         Args:
             app: target FastAPI application.
```

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/fields.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/fields/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,27 +16,27 @@
     The Fields extension adds functionality to the `/search` endpoint which
     allows the caller to include or exclude specific from the API response.
     Registering this extension with the application has the added effect of
     removing the `ItemCollection` response model from the `/search` endpoint, as
     the Fields extension allows the API to return potentially invalid responses
     by excluding fields which are required by the STAC spec, such as geometry.
 
-    https://github.com/radiantearth/stac-api-spec/blob/master/item-search/README.md#fields
+    https://github.com/stac-api-extensions/fields
 
     Attributes:
         default_includes (set): defines the default set of included fields.
         conformance_classes (list): Defines the list of conformance classes for
             the extension
     """
 
     GET = FieldsExtensionGetRequest
     POST = FieldsExtensionPostRequest
 
     conformance_classes: List[str] = attr.ib(
-        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.1/item-search#fields"]
+        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.3/item-search#fields"]
     )
     default_includes: Set[str] = attr.ib(
         factory=lambda: {
             "id",
             "type",
             "stac_version",
             "geometry",
```

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/fields/request.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/fields/request.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/filter.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/filter/filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from .request import FilterExtensionGetRequest, FilterExtensionPostRequest
 
 
 class FilterConformanceClasses(str, Enum):
     """Conformance classes for the Filter extension.
 
     See
-    https://github.com/radiantearth/stac-api-spec/tree/v1.0.0-rc.1/fragments/filter
+    https://github.com/stac-api-extensions/filter
     """
 
     FILTER = "http://www.opengis.net/spec/ogcapi-features-3/1.0/conf/filter"
     FEATURES_FILTER = (
         "http://www.opengis.net/spec/ogcapi-features-3/1.0/conf/features-filter"
     )
-    ITEM_SEARCH_FILTER = "https://api.stacspec.org/v1.0.0-rc.1/item-search#filter"
+    ITEM_SEARCH_FILTER = "https://api.stacspec.org/v1.0.0-rc.2/item-search#filter"
     CQL2_TEXT = "http://www.opengis.net/spec/cql2/1.0/conf/cql2-text"
     CQL2_JSON = "http://www.opengis.net/spec/cql2/1.0/conf/cql2-json"
     BASIC_CQL2 = "http://www.opengis.net/spec/cql2/1.0/conf/basic-cql2"
     BASIC_SPATIAL_OPERATORS = (
         "http://www.opengis.net/spec/cql2/1.0/conf/basic-spatial-operators"
     )
     TEMPORAL_OPERATORS = " http://www.opengis.net/spec/cql2/1.0/conf/temporal-operators"
```

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/filter/request.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/filter/request.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from stac_fastapi.types.search import APIRequest
 
 
 class FilterLang(str, Enum):
     """Choices for filter-lang value in a POST request.
 
     Based on
-    https://github.com/radiantearth/stac-api-spec/tree/master/fragments/filter#queryables
+    https://github.com/stac-api-extensions/filter#queryables
 
     Note the addition of cql2-json, which is used by the pgstac backend,
     but is not included in the spec above.
     """
 
     cql_json = "cql-json"
     cql2_json = "cql2-json"
```

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/pagination.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/pagination/token_pagination.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/pagination/token_pagination.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/query/query.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/query/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     https://github.com/radiantearth/stac-api-spec/blob/master/item-search/README.md#query
     """
 
     GET = QueryExtensionGetRequest
     POST = QueryExtensionPostRequest
 
     conformance_classes: List[str] = attr.ib(
-        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.1/item-search#query"]
+        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.2/item-search#query"]
     )
     schema_href: Optional[str] = attr.ib(default=None)
 
     def register(self, app: FastAPI) -> None:
         """Register the extension with a FastAPI application.
 
         Args:
```

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/request.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/sort/request.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/sort/sort.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/sort/sort.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 @attr.s
 class SortExtension(ApiExtension):
     """Sort Extension.
 
     The Sort extension adds the `sortby` parameter to the `/search` endpoint, allowing the
     caller to specify the sort order of the returned items.
-    https://github.com/radiantearth/stac-api-spec/blob/master/item-search/README.md#sort
+    https://github.com/stac-api-extensions/sort
     """
 
     GET = SortExtensionGetRequest
     POST = SortExtensionPostRequest
 
     conformance_classes: List[str] = attr.ib(
-        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.1/item-search#sort"]
+        factory=lambda: ["https://api.stacspec.org/v1.0.0-rc.2/item-search#sort"]
     )
     schema_href: Optional[str] = attr.ib(default=None)
 
     def register(self, app: FastAPI) -> None:
         """Register the extension with a FastAPI application.
 
         Args:
```

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/core/transaction.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/core/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         client: CRUD application logic
     """
 
     client: Union[AsyncBaseTransactionsClient, BaseTransactionsClient] = attr.ib()
     settings: ApiSettings = attr.ib()
     conformance_classes: List[str] = attr.ib(
         factory=lambda: [
-            "https://api.stacspec.org/v1.0.0-rc.1/ogcapi-features/extensions/transaction",
+            "https://api.stacspec.org/v1.0.0-rc.2/ogcapi-features/extensions/transaction",
             "http://www.opengis.net/spec/ogcapi-features-4/1.0/conf/simpletx",
         ]
     )
     schema_href: Optional[str] = attr.ib(default=None)
     router: APIRouter = attr.ib(factory=APIRouter)
     response_class: Type[Response] = attr.ib(default=JSONResponse)
```

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi/extensions/third_party/bulk_transactions.py` & `stac-fastapi.extensions-2.4.8/stac_fastapi/extensions/third_party/bulk_transactions.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/PKG-INFO` & `stac-fastapi.extensions-2.4.8/stac_fastapi.extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
-Version: 2.4.7
+Version: 2.4.8
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac-fastapi.extensions-2.4.7/stac_fastapi.extensions.egg-info/SOURCES.txt` & `stac-fastapi.extensions-2.4.8/stac_fastapi.extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

