# Comparing `tmp/ayomide-sdk-0.0.3.tar.gz` & `tmp/ayomide-sdk-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayomide-sdk-0.0.3.tar", last modified: Thu Jun  8 02:17:49 2023, max compression
+gzip compressed data, was "ayomide-sdk-0.0.6.tar", last modified: Thu Jun  8 02:38:19 2023, max compression
```

## Comparing `ayomide-sdk-0.0.3.tar` & `ayomide-sdk-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.835089 ayomide-sdk-0.0.3/
--rw-r--r--   0 Ayomide    (502) staff       (20)     1071 2023-06-07 23:29:04.000000 ayomide-sdk-0.0.3/LICENSE
--rw-r--r--   0 Ayomide    (502) staff       (20)       58 2023-06-07 23:27:53.000000 ayomide-sdk-0.0.3/MANIFEST.in
--rw-r--r--   0 Ayomide    (502) staff       (20)     2949 2023-06-08 02:17:49.835372 ayomide-sdk-0.0.3/PKG-INFO
--rw-r--r--   0 Ayomide    (502) staff       (20)     2429 2023-06-08 01:57:46.000000 ayomide-sdk-0.0.3/README.md
--rw-r--r--   0 Ayomide    (502) staff       (20)      103 2023-06-07 23:49:45.000000 ayomide-sdk-0.0.3/pyproject.toml
--rw-r--r--   0 Ayomide    (502) staff       (20)      685 2023-06-08 02:17:49.836443 ayomide-sdk-0.0.3/setup.cfg
--rw-r--r--   0 Ayomide    (502) staff       (20)       37 2023-06-07 23:31:57.000000 ayomide-sdk-0.0.3/setup.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.816465 ayomide-sdk-0.0.3/src/
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.822769 ayomide-sdk-0.0.3/src/ayomide_sdk/
--rw-r--r--   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:01.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/__init__.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.830063 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/
--rw-r--r--   0 Ayomide    (502) staff       (20)        0 2023-06-07 20:43:39.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/__init__.py
--rw-r--r--   0 Ayomide    (502) staff       (20)      521 2023-06-08 01:24:47.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/abstract.py
--rw-r--r--   0 Ayomide    (502) staff       (20)     1997 2023-06-08 01:24:42.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/api_requester.py
--rw-r--r--   0 Ayomide    (502) staff       (20)      155 2023-06-08 01:24:35.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/constants.py
--rw-r--r--   0 Ayomide    (502) staff       (20)      348 2023-06-08 01:24:30.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/helpers.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.830665 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/
--rw-r--r--   0 Ayomide    (502) staff       (20)     2246 2023-06-08 01:28:59.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/__init__.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.831437 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/movie/
--rw-r--r--   0 Ayomide    (502) staff       (20)      552 2023-06-08 01:27:09.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/movie/__init__.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.832087 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/quote/
--rw-r--r--   0 Ayomide    (502) staff       (20)      552 2023-06-08 01:26:58.000000 ayomide-sdk-0.0.3/src/ayomide_sdk/rest/quote/__init__.py
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.827430 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/
--rw-r--r--   0 Ayomide    (502) staff       (20)     2949 2023-06-08 02:17:49.000000 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/PKG-INFO
--rw-r--r--   0 Ayomide    (502) staff       (20)      669 2023-06-08 02:17:49.000000 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 Ayomide    (502) staff       (20)        1 2023-06-08 02:17:49.000000 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 Ayomide    (502) staff       (20)       17 2023-06-08 02:17:49.000000 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/requires.txt
--rw-r--r--   0 Ayomide    (502) staff       (20)       12 2023-06-08 02:17:49.000000 ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:17:49.834267 ayomide-sdk-0.0.3/test/
--rw-r--r--   0 Ayomide    (502) staff       (20)      303 2023-06-08 01:36:12.000000 ayomide-sdk-0.0.3/test/test_client.py
--rw-r--r--   0 Ayomide    (502) staff       (20)      374 2023-06-08 01:36:17.000000 ayomide-sdk-0.0.3/test/test_movie.py
--rw-r--r--   0 Ayomide    (502) staff       (20)      374 2023-06-08 01:36:21.000000 ayomide-sdk-0.0.3/test/test_quote.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:38:19.698734 ayomide-sdk-0.0.6/
+-rw-r--r--   0 Ayomide    (502) staff       (20)     1071 2023-06-07 23:29:04.000000 ayomide-sdk-0.0.6/LICENSE
+-rw-r--r--   0 Ayomide    (502) staff       (20)       58 2023-06-07 23:27:53.000000 ayomide-sdk-0.0.6/MANIFEST.in
+-rw-r--r--   0 Ayomide    (502) staff       (20)     2949 2023-06-08 02:38:19.698973 ayomide-sdk-0.0.6/PKG-INFO
+-rw-r--r--   0 Ayomide    (502) staff       (20)     2429 2023-06-08 01:57:46.000000 ayomide-sdk-0.0.6/README.md
+-rw-r--r--   0 Ayomide    (502) staff       (20)      103 2023-06-07 23:49:45.000000 ayomide-sdk-0.0.6/pyproject.toml
+-rw-r--r--   0 Ayomide    (502) staff       (20)      685 2023-06-08 02:38:19.699682 ayomide-sdk-0.0.6/setup.cfg
+-rw-r--r--   0 Ayomide    (502) staff       (20)       37 2023-06-07 23:31:57.000000 ayomide-sdk-0.0.6/setup.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:38:19.674103 ayomide-sdk-0.0.6/src/
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:38:19.681912 ayomide-sdk-0.0.6/src/ayomide_sdk/
+-rw-r--r--   0 Ayomide    (502) staff       (20)        0 2023-06-08 00:54:01.000000 ayomide-sdk-0.0.6/src/ayomide_sdk/__init__.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:38:19.689445 ayomide-sdk-0.0.6/src/ayomide_sdk/api_resources/
+-rw-r--r--   0 Ayomide    (502) staff       (20)        0 2023-06-07 20:43:39.000000 ayomide-sdk-0.0.6/src/ayomide_sdk/api_resources/__init__.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)      521 2023-06-08 01:24:47.000000 ayomide-sdk-0.0.6/src/ayomide_sdk/api_resources/abstract.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)     1997 2023-06-08 01:24:42.000000 ayomide-sdk-0.0.6/src/ayomide_sdk/api_resources/api_requester.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)      155 2023-06-08 01:24:35.000000 ayomide-sdk-0.0.6/src/ayomide_sdk/api_resources/constants.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)      348 2023-06-08 01:24:30.000000 ayomide-sdk-0.0.6/src/ayomide_sdk/api_resources/helpers.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:38:19.690684 ayomide-sdk-0.0.6/src/ayomide_sdk/rest/
+-rw-r--r--   0 Ayomide    (502) staff       (20)     2278 2023-06-08 02:31:33.000000 ayomide-sdk-0.0.6/src/ayomide_sdk/rest/__init__.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:38:19.692033 ayomide-sdk-0.0.6/src/ayomide_sdk/rest/movie/
+-rw-r--r--   0 Ayomide    (502) staff       (20)      552 2023-06-08 01:27:09.000000 ayomide-sdk-0.0.6/src/ayomide_sdk/rest/movie/__init__.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:38:19.693543 ayomide-sdk-0.0.6/src/ayomide_sdk/rest/quote/
+-rw-r--r--   0 Ayomide    (502) staff       (20)      552 2023-06-08 01:26:58.000000 ayomide-sdk-0.0.6/src/ayomide_sdk/rest/quote/__init__.py
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:38:19.685119 ayomide-sdk-0.0.6/src/ayomide_sdk.egg-info/
+-rw-r--r--   0 Ayomide    (502) staff       (20)     2949 2023-06-08 02:38:19.000000 ayomide-sdk-0.0.6/src/ayomide_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 Ayomide    (502) staff       (20)      669 2023-06-08 02:38:19.000000 ayomide-sdk-0.0.6/src/ayomide_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 Ayomide    (502) staff       (20)        1 2023-06-08 02:38:19.000000 ayomide-sdk-0.0.6/src/ayomide_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 Ayomide    (502) staff       (20)       17 2023-06-08 02:38:19.000000 ayomide-sdk-0.0.6/src/ayomide_sdk.egg-info/requires.txt
+-rw-r--r--   0 Ayomide    (502) staff       (20)       12 2023-06-08 02:38:19.000000 ayomide-sdk-0.0.6/src/ayomide_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 Ayomide    (502) staff       (20)        0 2023-06-08 02:38:19.697517 ayomide-sdk-0.0.6/test/
+-rw-r--r--   0 Ayomide    (502) staff       (20)      303 2023-06-08 01:36:12.000000 ayomide-sdk-0.0.6/test/test_client.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)      374 2023-06-08 01:36:17.000000 ayomide-sdk-0.0.6/test/test_movie.py
+-rw-r--r--   0 Ayomide    (502) staff       (20)      374 2023-06-08 01:36:21.000000 ayomide-sdk-0.0.6/test/test_quote.py
```

### Comparing `ayomide-sdk-0.0.3/LICENSE` & `ayomide-sdk-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ayomide-sdk-0.0.3/PKG-INFO` & `ayomide-sdk-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayomide-sdk
-Version: 0.0.3
+Version: 0.0.6
 Summary: This is a simple Python library to
 Home-page: https://github.com/alsaheem/ayomide-sdk
 Author: Ayomide Adebisi
 Author-email: adebisiayomide07@gmail.com
 Project-URL: Bug Tracker, https://github.com/alsaheem/ayomide-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ayomide-sdk Version: 0.0.3 Summary: This is a
+Metadata-Version: 2.1 Name: ayomide-sdk Version: 0.0.6 Summary: This is a
 simple Python library to Home-page: https://github.com/alsaheem/ayomide-sdk
 Author: Ayomide Adebisi Author-email: adebisiayomide07@gmail.com Project-URL:
 Bug Tracker, https://github.com/alsaheem/ayomide-sdk/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE # The Lord of the
 rings API Python SDK Welcome to this Python SDK repository for the The Lord of
```

### Comparing `ayomide-sdk-0.0.3/README.md` & `ayomide-sdk-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ayomide-sdk-0.0.3/setup.cfg` & `ayomide-sdk-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ayomide-sdk
-version = 0.0.3
+version = 0.0.6
 author = Ayomide Adebisi
 author_email = adebisiayomide07@gmail.com
 description = This is a simple Python library to
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/alsaheem/ayomide-sdk
 project_urls =
```

### Comparing `ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/abstract.py` & `ayomide-sdk-0.0.6/src/ayomide_sdk/api_resources/abstract.py`

 * *Files identical despite different names*

### Comparing `ayomide-sdk-0.0.3/src/ayomide_sdk/api_resources/api_requester.py` & `ayomide-sdk-0.0.6/src/ayomide_sdk/api_resources/api_requester.py`

 * *Files identical despite different names*

### Comparing `ayomide-sdk-0.0.3/src/ayomide_sdk/rest/__init__.py` & `ayomide-sdk-0.0.6/src/ayomide_sdk/rest/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 from ayomide_sdk.api_resources.helpers import full_url_query_builder
 
 
 class Client(object):
     """
     A client class for accessing the Lord Of The Ring API.
     Example
-    client = Client(version="v2", api_key="API-KEY")
+    client = Client(version="v2", api_key="API-KEY") version is 
+    # v2 by default
     client.quote.get()
     client.movie.get()
     """
 
-    def __init__(self, api_key=None, version=None):
+    def __init__(self, api_key="v2", version=None):
         base_url = BASE_URL_V1 if version.lower() == "v1" else BASE_URL_V2
         if api_key is None:
             raise Exception("Api key is required")
 
         if version.lower() == "v1":
             raise NotImplementedError(
                 "This sdk does not support version v1 , please upgrade to v2"
```

### Comparing `ayomide-sdk-0.0.3/src/ayomide_sdk/rest/movie/__init__.py` & `ayomide-sdk-0.0.6/src/ayomide_sdk/rest/movie/__init__.py`

 * *Files identical despite different names*

### Comparing `ayomide-sdk-0.0.3/src/ayomide_sdk/rest/quote/__init__.py` & `ayomide-sdk-0.0.6/src/ayomide_sdk/rest/quote/__init__.py`

 * *Files identical despite different names*

### Comparing `ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/PKG-INFO` & `ayomide-sdk-0.0.6/src/ayomide_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayomide-sdk
-Version: 0.0.3
+Version: 0.0.6
 Summary: This is a simple Python library to
 Home-page: https://github.com/alsaheem/ayomide-sdk
 Author: Ayomide Adebisi
 Author-email: adebisiayomide07@gmail.com
 Project-URL: Bug Tracker, https://github.com/alsaheem/ayomide-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ayomide-sdk Version: 0.0.3 Summary: This is a
+Metadata-Version: 2.1 Name: ayomide-sdk Version: 0.0.6 Summary: This is a
 simple Python library to Home-page: https://github.com/alsaheem/ayomide-sdk
 Author: Ayomide Adebisi Author-email: adebisiayomide07@gmail.com Project-URL:
 Bug Tracker, https://github.com/alsaheem/ayomide-sdk/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE # The Lord of the
 rings API Python SDK Welcome to this Python SDK repository for the The Lord of
```

### Comparing `ayomide-sdk-0.0.3/src/ayomide_sdk.egg-info/SOURCES.txt` & `ayomide-sdk-0.0.6/src/ayomide_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

