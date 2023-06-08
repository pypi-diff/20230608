# Comparing `tmp/ayomide-sdk-0.0.2.tar.gz` & `tmp/ayomide-sdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayomide-sdk-0.0.2.tar", last modified: Thu Jun  8 00:54:54 2023, max compression
+gzip compressed data, was "ayomide-sdk-0.0.3.tar", last modified: Thu Jun  8 02:17:49 2023, max compression
```

## Comparing `ayomide-sdk-0.0.2.tar` & `ayomide-sdk-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:54.428247 ayomide-sdk-0.0.2/
--rw-r--r--   0 Ayomide    (502) staff       (20)     1071 2023-06-07 23:29:04.000000 ayomide-sdk-0.0.2/LICENSE
--rw-r--r--   0 Ayomide    (502) staff       (20)       58 2023-06-07 23:27:53.000000 ayomide-sdk-0.0.2/MANIFEST.in
--rw-r--r--   0 Ayomide    (502) staff       (20)      895 2023-06-08 00:54:54.428518 ayomide-sdk-0.0.2/PKG-INFO
--rw-r--r--   0 Ayomide    (502) staff       (20)      374 2023-06-07 23:06:01.000000 ayomide-sdk-0.0.2/README.md
--rw-r--r--   0 Ayomide    (502) staff       (20)      103 2023-06-07 23:49:45.000000 ayomide-sdk-0.0.2/pyproject.toml
--rw-r--r--   0 Ayomide    (502) staff       (20)      685 2023-06-08 00:54:54.429884 ayomide-sdk-0.0.2/setup.cfg
--rw-r--r--   0 Ayomide    (502) staff       (20)       37 2023-06-07 23:31:57.000000 ayomide-sdk-0.0.2/setup.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:54.397850 ayomide-sdk-0.0.2/src/
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:54.407042 ayomide-sdk-0.0.2/src/ayomide_sdk/
--rw-r--r--   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:01.000000 ayomide-sdk-0.0.2/src/ayomide_sdk/__init__.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:54.420017 ayomide-sdk-0.0.2/src/ayomide_sdk/api_resources/
--rw-r--r--   0 Ayomide    (502) staff       (20)        0 2023-06-07 20:43:39.000000 ayomide-sdk-0.0.2/src/ayomide_sdk/api_resources/__init__.py
--rw-r--r--   0 Ayomide    (502) staff       (20)      207 2023-06-07 20:24:14.000000 ayomide-sdk-0.0.2/src/ayomide_sdk/api_resources/abstract.py
--rw-r--r--   0 Ayomide    (502) staff       (20)     1862 2023-06-07 23:07:04.000000 ayomide-sdk-0.0.2/src/ayomide_sdk/api_resources/api_requester.py
--rw-r--r--   0 Ayomide    (502) staff       (20)       92 2023-06-07 19:05:00.000000 ayomide-sdk-0.0.2/src/ayomide_sdk/api_resources/constants.py
--rw-r--r--   0 Ayomide    (502) staff       (20)      270 2023-06-07 23:02:05.000000 ayomide-sdk-0.0.2/src/ayomide_sdk/api_resources/helpers.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:54.421728 ayomide-sdk-0.0.2/src/ayomide_sdk/rest/
--rw-r--r--   0 Ayomide    (502) staff       (20)     2156 2023-06-07 23:02:45.000000 ayomide-sdk-0.0.2/src/ayomide_sdk/rest/__init__.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:54.423107 ayomide-sdk-0.0.2/src/ayomide_sdk/rest/movie/
--rw-r--r--   0 Ayomide    (502) staff       (20)      546 2023-06-07 23:02:20.000000 ayomide-sdk-0.0.2/src/ayomide_sdk/rest/movie/__init__.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:54.424756 ayomide-sdk-0.0.2/src/ayomide_sdk/rest/quote/
--rw-r--r--   0 Ayomide    (502) staff       (20)      546 2023-06-07 23:02:28.000000 ayomide-sdk-0.0.2/src/ayomide_sdk/rest/quote/__init__.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:54.413250 ayomide-sdk-0.0.2/src/ayomide_sdk.egg-info/
--rw-r--r--   0 Ayomide    (502) staff       (20)      895 2023-06-08 00:54:54.000000 ayomide-sdk-0.0.2/src/ayomide_sdk.egg-info/PKG-INFO
--rw-r--r--   0 Ayomide    (502) staff       (20)      649 2023-06-08 00:54:54.000000 ayomide-sdk-0.0.2/src/ayomide_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 Ayomide    (502) staff       (20)        1 2023-06-08 00:54:54.000000 ayomide-sdk-0.0.2/src/ayomide_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 Ayomide    (502) staff       (20)       17 2023-06-08 00:54:54.000000 ayomide-sdk-0.0.2/src/ayomide_sdk.egg-info/requires.txt
--rw-r--r--   0 Ayomide    (502) staff       (20)       12 2023-06-08 00:54:54.000000 ayomide-sdk-0.0.2/src/ayomide_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:54.427630 ayomide-sdk-0.0.2/test/
--rw-r--r--   0 Ayomide    (502) staff       (20)        0 2023-06-07 19:14:55.000000 ayomide-sdk-0.0.2/test/test_movie.py
--rw-r--r--   0 Ayomide    (502) staff       (20)        0 2023-06-07 23:11:13.000000 ayomide-sdk-0.0.2/test/test_quote.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.835089 ayomide-sdk-0.0.3/
+-rw-r--r--   0 Ayomide    (502) staff       (20)     1071 2023-06-07 23:29:04.000000 ayomide-sdk-0.0.3/LICENSE
+-rw-r--r--   0 Ayomide    (502) staff       (20)       58 2023-06-07 23:27:53.000000 ayomide-sdk-0.0.3/MANIFEST.in
+-rw-r--r--   0 Ayomide    (502) staff       (20)     2949 2023-06-08 02:17:49.835372 ayomide-sdk-0.0.3/PKG-INFO
+-rw-r--r--   0 Ayomide    (502) staff       (20)     2429 2023-06-08 01:57:46.000000 ayomide-sdk-0.0.3/README.md
+-rw-r--r--   0 Ayomide    (502) staff       (20)      103 2023-06-07 23:49:45.000000 ayomide-sdk-0.0.3/pyproject.toml
+-rw-r--r--   0 Ayomide    (502) staff       (20)      685 2023-06-08 02:17:49.836443 ayomide-sdk-0.0.3/setup.cfg
+-rw-r--r--   0 Ayomide    (502) staff       (20)       37 2023-06-07 23:31:57.000000 ayomide-sdk-0.0.3/setup.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.816465 ayomide-sdk-0.0.3/src/
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.822769 ayomide-sdk-0.0.3/src/ayomide_sdk/
+-rw-r--r--   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:01.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/__init__.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.830063 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/
+-rw-r--r--   0 Ayomide    (502) staff       (20)        0 2023-06-07 20:43:39.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/__init__.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)      521 2023-06-08 01:24:47.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/abstract.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)     1997 2023-06-08 01:24:42.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/api_requester.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)      155 2023-06-08 01:24:35.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/constants.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)      348 2023-06-08 01:24:30.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/helpers.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.830665 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/
+-rw-r--r--   0 Ayomide    (502) staff       (20)     2246 2023-06-08 01:28:59.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/__init__.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.831437 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/movie/
+-rw-r--r--   0 Ayomide    (502) staff       (20)      552 2023-06-08 01:27:09.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/movie/__init__.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.832087 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/quote/
+-rw-r--r--   0 Ayomide    (502) staff       (20)      552 2023-06-08 01:26:58.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/quote/__init__.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.827430 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/
+-rw-r--r--   0 Ayomide    (502) staff       (20)     2949 2023-06-08 02:17:49.000000 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 Ayomide    (502) staff       (20)      669 2023-06-08 02:17:49.000000 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 Ayomide    (502) staff       (20)        1 2023-06-08 02:17:49.000000 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 Ayomide    (502) staff       (20)       17 2023-06-08 02:17:49.000000 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/requires.txt
+-rw-r--r--   0 Ayomide    (502) staff       (20)       12 2023-06-08 02:17:49.000000 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.834267 ayomide-sdk-0.0.3/test/
+-rw-r--r--   0 Ayomide    (502) staff       (20)      303 2023-06-08 01:36:12.000000 ayomide-sdk-0.0.3/test/test_client.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)      374 2023-06-08 01:36:17.000000 ayomide-sdk-0.0.3/test/test_movie.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)      374 2023-06-08 01:36:21.000000 ayomide-sdk-0.0.3/test/test_quote.py
```

### Comparing `ayomide-sdk-0.0.2/LICENSE` & `ayomide-sdk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ayomide-sdk-0.0.2/setup.cfg` & `ayomide-sdk-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ayomide-sdk
-version = 0.0.2
+version = 0.0.3
 author = Ayomide Adebisi
 author_email = adebisiayomide07@gmail.com
 description = This is a simple Python library to
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alsaheem/ayomide-sdk
 project_urls =
```

### Comparing `ayomide-sdk-0.0.2/src/ayomide_sdk/api_resources/api_requester.py` & `ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/api_requester.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import requests
 from ayomide_sdk.api_resources.helpers import build_filters
 
+
 class ApiRequester:
+    """
+    This class implements the api calls needed in the application
+    it implements get, post, put and delete methods
+    """
+
     def __init__(self, method_type, url, headers, params, filters):
         self.method_type = method_type
         self.url = url
         self.headers = headers
         self.params = params
         self.filters = filters
 
     def get(self):
-
         filter_query = "?"
 
         if self.filters != {} and self.filters != None:
             filter_query = build_filters(self.filters)
 
         if self.params != None and self.params.get("id", None) != None:
             if self.params.get("subquery", None) == None:
```

### Comparing `ayomide-sdk-0.0.2/src/ayomide_sdk/rest/__init__.py` & `ayomide-sdk-0.0.3/src/ayomide_sdk/rest/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-import os
 from ayomide_sdk.api_resources.constants import BASE_URL_V1, BASE_URL_V2
 from ayomide_sdk.api_resources.api_requester import ApiRequester
 from ayomide_sdk.api_resources.helpers import full_url_query_builder
 
 
 class Client(object):
     """
-    A client for accessing the hedera_mirror API.
+    A client class for accessing the Lord Of The Ring API.
+    Example
+    client = Client(version="v2", api_key="API-KEY")
+    client.quote.get()
+    client.movie.get()
     """
 
     def __init__(self, api_key=None, version=None):
         base_url = BASE_URL_V1 if version.lower() == "v1" else BASE_URL_V2
         if api_key is None:
             raise Exception("Api key is required")
 
@@ -49,23 +52,23 @@
 
         json_response = response.json()
         return {"status": response.status_code, "json": json_response}
 
     @property
     def quote(self):
         """
-        Access the did_sdk Account API
+        Access the Quote Api
         """
         from ayomide_sdk.rest.quote import Quote
 
         quote_resp = Quote(self, "quote")
         return quote_resp
 
     @property
     def movie(self):
         """
-        Access the did_sdk Account API
+        Access the Movie API
         """
         from ayomide_sdk.rest.movie import Movie
 
         movie_resp = Movie(self, "movie")
         return movie_resp
```

### Comparing `ayomide-sdk-0.0.2/src/ayomide_sdk/rest/movie/__init__.py` & `ayomide-sdk-0.0.3/src/ayomide_sdk/rest/movie/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ayomide_sdk.api_resources.abstract import AbstractBaseClass
 
 
 class Movie:
     def __init__(self, client_sdk, api_type):
         """
-        Initialize the Movie
+        Initialize the Movie class
         """
         self.api_type = api_type
         self.client_sdk = client_sdk
 
     def get(self, params=None, filters={}):
         return self.client_sdk.request(
             method_type="get", params=params, api_type=self.api_type, filters=filters
```

### Comparing `ayomide-sdk-0.0.2/src/ayomide_sdk/rest/quote/__init__.py` & `ayomide-sdk-0.0.3/src/ayomide_sdk/rest/quote/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ayomide_sdk.api_resources.abstract import AbstractBaseClass
 
 
 class Quote:
     def __init__(self, client_sdk, api_type):
         """
-        Initialize the Quote
+        Initialize the Quote class
         """
         self.api_type = api_type
         self.client_sdk = client_sdk
 
     def get(self, params=None, filters={}):
         return self.client_sdk.request(
             method_type="get", params=params, api_type=self.api_type, filters=filters
```

### Comparing `ayomide-sdk-0.0.2/src/ayomide_sdk.egg-info/SOURCES.txt` & `ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,9 +14,10 @@
 src/ayomide_sdk/api_resources/abstract.py
 src/ayomide_sdk/api_resources/api_requester.py
 src/ayomide_sdk/api_resources/constants.py
 src/ayomide_sdk/api_resources/helpers.py
 src/ayomide_sdk/rest/__init__.py
 src/ayomide_sdk/rest/movie/__init__.py
 src/ayomide_sdk/rest/quote/__init__.py
+test/test_client.py
 test/test_movie.py
 test/test_quote.py
```

