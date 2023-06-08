# Comparing `tmp/stac-fastapi.types-2.4.7.tar.gz` & `tmp/stac-fastapi.types-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.types-2.4.7.tar", last modified: Wed May 17 15:30:40 2023, max compression
+gzip compressed data, was "stac-fastapi.types-2.4.8.tar", last modified: Thu Jun  8 19:49:40 2023, max compression
```

## Comparing `stac-fastapi.types-2.4.7.tar` & `stac-fastapi.types-2.4.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:40.268149 stac-fastapi.types-2.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 15:30:40.268149 stac-fastapi.types-2.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 15:30:40.272149 stac-fastapi.types-2.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:40.268149 stac-fastapi.types-2.4.7/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:40.268149 stac-fastapi.types-2.4.7/stac_fastapi/types/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)    24058 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/links.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/rfc3339.py
--rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/stac.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 15:30:29.000000 stac-fastapi.types-2.4.7/stac_fastapi/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:40.268149 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 15:30:40.000000 stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:40.563632 stac-fastapi.types-2.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-08 19:49:40.563632 stac-fastapi.types-2.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 19:49:40.563632 stac-fastapi.types-2.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:40.563632 stac-fastapi.types-2.4.8/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:40.563632 stac-fastapi.types-2.4.8/stac_fastapi/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/rfc3339.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6899 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/stac.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 19:49:31.000000 stac-fastapi.types-2.4.8/stac_fastapi/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:40.563632 stac-fastapi.types-2.4.8/stac_fastapi.types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-08 19:49:40.000000 stac-fastapi.types-2.4.8/stac_fastapi.types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-08 19:49:40.000000 stac-fastapi.types-2.4.8/stac_fastapi.types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:49:40.000000 stac-fastapi.types-2.4.8/stac_fastapi.types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:49:40.000000 stac-fastapi.types-2.4.8/stac_fastapi.types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-08 19:49:40.000000 stac-fastapi.types-2.4.8/stac_fastapi.types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 19:49:40.000000 stac-fastapi.types-2.4.8/stac_fastapi.types.egg-info/top_level.txt
```

### Comparing `stac-fastapi.types-2.4.7/PKG-INFO` & `stac-fastapi.types-2.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
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

### Comparing `stac-fastapi.types-2.4.7/setup.py` & `stac-fastapi.types-2.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi/types/config.py` & `stac-fastapi.types-2.4.8/stac_fastapi/types/config.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi/types/conformance.py` & `stac-fastapi.types-2.4.8/stac_fastapi/types/conformance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Conformance Classes."""
 from enum import Enum
 
 
 class STACConformanceClasses(str, Enum):
     """Conformance classes for the STAC API spec."""
 
-    CORE = "https://api.stacspec.org/v1.0.0-rc.1/core"
-    OGC_API_FEAT = "https://api.stacspec.org/v1.0.0-rc.1/ogcapi-features"
-    COLLECTIONS = "https://api.stacspec.org/v1.0.0-rc.1/collections"
-    ITEM_SEARCH = "https://api.stacspec.org/v1.0.0-rc.1/item-search"
+    CORE = "https://api.stacspec.org/v1.0.0/core"
+    OGC_API_FEAT = "https://api.stacspec.org/v1.0.0/ogcapi-features"
+    COLLECTIONS = "https://api.stacspec.org/v1.0.0/collections"
+    ITEM_SEARCH = "https://api.stacspec.org/v1.0.0/item-search"
 
 
 class OAFConformanceClasses(str, Enum):
     """Conformance classes for OGC API - Features."""
 
     CORE = "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/core"
     OPEN_API = "http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/oas30"
```

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi/types/core.py` & `stac-fastapi.types-2.4.8/stac_fastapi/types/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -756,15 +756,15 @@
         """Get the queryables available for the given collection_id.
 
         If collection_id is None, returns the intersection of all queryables over all
         collections.
 
         This base implementation returns a blank queryable schema. This is not allowed
         under OGC CQL but it is allowed by the STAC API Filter Extension
-        https://github.com/radiantearth/stac-api-spec/tree/master/fragments/filter#queryables
+        https://github.com/stac-api-extensions/filter#queryables
         """
         return {
             "$schema": "https://json-schema.org/draft/2019-09/schema",
             "$id": "https://example.org/queryables",
             "type": "object",
             "title": "Queryables for Example STAC API",
             "description": "Queryable names for the example STAC API Item Search filter.",
```

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi/types/errors.py` & `stac-fastapi.types-2.4.8/stac_fastapi/types/errors.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi/types/extension.py` & `stac-fastapi.types-2.4.8/stac_fastapi/types/extension.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi/types/links.py` & `stac-fastapi.types-2.4.8/stac_fastapi/types/links.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi/types/rfc3339.py` & `stac-fastapi.types-2.4.8/stac_fastapi/types/rfc3339.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi/types/search.py` & `stac-fastapi.types-2.4.8/stac_fastapi/types/search.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi/types/stac.py` & `stac-fastapi.types-2.4.8/stac_fastapi/types/stac.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/PKG-INFO` & `stac-fastapi.types-2.4.8/stac_fastapi.types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
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

### Comparing `stac-fastapi.types-2.4.7/stac_fastapi.types.egg-info/SOURCES.txt` & `stac-fastapi.types-2.4.8/stac_fastapi.types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

