# Comparing `tmp/stac-fastapi.api-2.4.7.tar.gz` & `tmp/stac-fastapi.api-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-fastapi.api-2.4.7.tar", last modified: Wed May 17 15:30:48 2023, max compression
+gzip compressed data, was "stac-fastapi.api-2.4.8.tar", last modified: Thu Jun  8 19:49:47 2023, max compression
```

## Comparing `stac-fastapi.api-2.4.7.tar` & `stac-fastapi.api-2.4.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/stac_fastapi/api/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-17 15:30:29.000000 stac-fastapi.api-2.4.7/stac_fastapi/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:30:48.436152 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-17 15:30:48.000000 stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:47.687734 stac-fastapi.api-2.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-08 19:49:47.687734 stac-fastapi.api-2.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 19:49:47.687734 stac-fastapi.api-2.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:47.683735 stac-fastapi.api-2.4.8/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:47.687734 stac-fastapi.api-2.4.8/stac_fastapi/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/stac_fastapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/stac_fastapi/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/stac_fastapi/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/stac_fastapi/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/stac_fastapi/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/stac_fastapi/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/stac_fastapi/api/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/stac_fastapi/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 19:49:31.000000 stac-fastapi.api-2.4.8/stac_fastapi/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:49:47.683735 stac-fastapi.api-2.4.8/stac_fastapi.api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-08 19:49:47.000000 stac-fastapi.api-2.4.8/stac_fastapi.api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-08 19:49:47.000000 stac-fastapi.api-2.4.8/stac_fastapi.api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:49:47.000000 stac-fastapi.api-2.4.8/stac_fastapi.api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:49:47.000000 stac-fastapi.api-2.4.8/stac_fastapi.api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 19:49:47.000000 stac-fastapi.api-2.4.8/stac_fastapi.api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 19:49:47.000000 stac-fastapi.api-2.4.8/stac_fastapi.api.egg-info/top_level.txt
```

### Comparing `stac-fastapi.api-2.4.7/PKG-INFO` & `stac-fastapi.api-2.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
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

### Comparing `stac-fastapi.api-2.4.7/setup.py` & `stac-fastapi.api-2.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.7/stac_fastapi/api/app.py` & `stac-fastapi.api-2.4.8/stac_fastapi/api/app.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.7/stac_fastapi/api/config.py` & `stac-fastapi.api-2.4.8/stac_fastapi/api/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # TODO: Move to stac-pydantic
 # Does that make sense now? The shift to json schema rather than a well-known
 # enumeration makes that less obvious.
 class ApiExtensions(enum.Enum):
     """Enumeration of available stac api extensions.
 
-    Ref: https://github.com/radiantearth/stac-api-spec/tree/master/extensions
+    Ref: https://github.com/stac-api-extensions
     """
 
     context = "context"
     fields = "fields"
     filter = "filter"
     query = "query"
     sort = "sort"
```

### Comparing `stac-fastapi.api-2.4.7/stac_fastapi/api/errors.py` & `stac-fastapi.api-2.4.8/stac_fastapi/api/errors.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.7/stac_fastapi/api/middleware.py` & `stac-fastapi.api-2.4.8/stac_fastapi/api/middleware.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.7/stac_fastapi/api/models.py` & `stac-fastapi.api-2.4.8/stac_fastapi/api/models.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.7/stac_fastapi/api/openapi.py` & `stac-fastapi.api-2.4.8/stac_fastapi/api/openapi.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.7/stac_fastapi/api/routes.py` & `stac-fastapi.api-2.4.8/stac_fastapi/api/routes.py`

 * *Files identical despite different names*

### Comparing `stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/PKG-INFO` & `stac-fastapi.api-2.4.8/stac_fastapi.api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
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

### Comparing `stac-fastapi.api-2.4.7/stac_fastapi.api.egg-info/SOURCES.txt` & `stac-fastapi.api-2.4.8/stac_fastapi.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

