# Comparing `tmp/pqapi-0.0.1.tar.gz` & `tmp/pqapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqapi-0.0.1.tar", last modified: Tue Jun  6 17:49:50 2023, max compression
+gzip compressed data, was "pqapi-0.0.2.tar", last modified: Thu Jun  8 14:42:45 2023, max compression
```

## Comparing `pqapi-0.0.1.tar` & `pqapi-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:49:50.135544 pqapi-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-06 17:49:23.000000 pqapi-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-06 17:49:50.135544 pqapi-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-06 17:49:23.000000 pqapi-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:49:50.135544 pqapi-0.0.1/pqapi/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-06 17:49:23.000000 pqapi-0.0.1/pqapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-06 17:49:23.000000 pqapi-0.0.1/pqapi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-06 17:49:23.000000 pqapi-0.0.1/pqapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-06 17:49:23.000000 pqapi-0.0.1/pqapi/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 17:49:23.000000 pqapi-0.0.1/pqapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:49:50.135544 pqapi-0.0.1/pqapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-06 17:49:50.000000 pqapi-0.0.1/pqapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-06 17:49:50.000000 pqapi-0.0.1/pqapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:49:50.000000 pqapi-0.0.1/pqapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-06 17:49:50.000000 pqapi-0.0.1/pqapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 17:49:50.000000 pqapi-0.0.1/pqapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-06 17:49:23.000000 pqapi-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 17:49:50.135544 pqapi-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-06 17:49:23.000000 pqapi-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:49:50.135544 pqapi-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-06 17:49:23.000000 pqapi-0.0.1/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:42:45.628440 pqapi-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 14:42:08.000000 pqapi-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-08 14:42:45.628440 pqapi-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-08 14:42:08.000000 pqapi-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:42:45.628440 pqapi-0.0.2/pqapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-08 14:42:08.000000 pqapi-0.0.2/pqapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-08 14:42:08.000000 pqapi-0.0.2/pqapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 14:42:08.000000 pqapi-0.0.2/pqapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-08 14:42:08.000000 pqapi-0.0.2/pqapi/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 14:42:08.000000 pqapi-0.0.2/pqapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:42:45.628440 pqapi-0.0.2/pqapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-08 14:42:45.000000 pqapi-0.0.2/pqapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-08 14:42:45.000000 pqapi-0.0.2/pqapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:42:45.000000 pqapi-0.0.2/pqapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 14:42:45.000000 pqapi-0.0.2/pqapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 14:42:45.000000 pqapi-0.0.2/pqapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 14:42:08.000000 pqapi-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:42:45.628440 pqapi-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-08 14:42:08.000000 pqapi-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:42:45.628440 pqapi-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-08 14:42:08.000000 pqapi-0.0.2/tests/test_api.py
```

### Comparing `pqapi-0.0.1/LICENSE` & `pqapi-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pqapi-0.0.1/PKG-INFO` & `pqapi-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: API for interacting with paperqa.app
 Home-page: https://github.com/Future-House/pqapi
 Author: Andrew White
 Author-email: andrew@futurehouse.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,38 @@
 
 Make sure to set the environment variable `PAPERQA_API_TOKEN` to your API token.
 
 ```sh
 export PAPERQA_API_TOKEN=pqa-...
 ```
 
-To upload files:
+To query agent:
+
+```py
+import pqapi
+response = pqapi.agent_query(
+    "default",
+    "Are COVID-19 vaccines effective?"
+)
+```
+
+## Managing bibliographies
+
+
+To get information about a specific bibliography
+
+```py
+import pqapi
+response = pqapi.get_bibliography(
+    "default"
+)
+print(response)
+```
+
+You do not need to explicitly create a bibliography, just adding files will create one. To upload files:
 
 ```py
 import pqapi
 files = [open("paper.pdf", "rb"), open("paper2.pdf", "rb")]
 metadatas = [
     pqapi.UploadMetadata(filename="paper.pdf", citation="Test Citation"),
     pqapi.UploadMetadata(filename="paper2.pdf", citation="Test Citation 2"),
@@ -34,16 +57,15 @@
 response = pqapi.upload_files(
     "default",
     files
     metadatas
 )
 ```
 
-To query agent:
+To delete a bibliography:
 
 ```py
 import pqapi
-response = pqapi.query_agent(
-    "default",
-    "Are COVID-19 vaccines effective?"
+response = pqapi.delete_bibliography(
+    "default"
 )
 ```
```

### Comparing `pqapi-0.0.1/README.md` & `pqapi-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,38 @@
 
 Make sure to set the environment variable `PAPERQA_API_TOKEN` to your API token.
 
 ```sh
 export PAPERQA_API_TOKEN=pqa-...
 ```
 
-To upload files:
+To query agent:
+
+```py
+import pqapi
+response = pqapi.agent_query(
+    "default",
+    "Are COVID-19 vaccines effective?"
+)
+```
+
+## Managing bibliographies
+
+
+To get information about a specific bibliography
+
+```py
+import pqapi
+response = pqapi.get_bibliography(
+    "default"
+)
+print(response)
+```
+
+You do not need to explicitly create a bibliography, just adding files will create one. To upload files:
 
 ```py
 import pqapi
 files = [open("paper.pdf", "rb"), open("paper2.pdf", "rb")]
 metadatas = [
     pqapi.UploadMetadata(filename="paper.pdf", citation="Test Citation"),
     pqapi.UploadMetadata(filename="paper2.pdf", citation="Test Citation 2"),
@@ -21,16 +44,15 @@
 response = pqapi.upload_files(
     "default",
     files
     metadatas
 )
 ```
 
-To query agent:
+To delete a bibliography:
 
 ```py
 import pqapi
-response = pqapi.query_agent(
-    "default",
-    "Are COVID-19 vaccines effective?"
+response = pqapi.delete_bibliography(
+    "default"
 )
-```
+```
```

### Comparing `pqapi-0.0.1/pqapi/api.py` & `pqapi-0.0.2/pqapi/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Any, BinaryIO, Dict, List, Union
 
 import requests
 
 from .auth import get_pqa_key
-from .models import AnswerResponse, QueryRequest, UploadMetadata, DocsStatus
+from .models import AnswerResponse, DocsStatus, QueryRequest, UploadMetadata
 
 
 def upload_files(
     bibliography: str,
     files: List[BinaryIO],
     metadatas: List[UploadMetadata],
     public: bool = False,
```

### Comparing `pqapi-0.0.1/pqapi/models.py` & `pqapi-0.0.2/pqapi/models.py`

 * *Files identical despite different names*

### Comparing `pqapi-0.0.1/pqapi.egg-info/PKG-INFO` & `pqapi-0.0.2/pqapi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: API for interacting with paperqa.app
 Home-page: https://github.com/Future-House/pqapi
 Author: Andrew White
 Author-email: andrew@futurehouse.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,38 @@
 
 Make sure to set the environment variable `PAPERQA_API_TOKEN` to your API token.
 
 ```sh
 export PAPERQA_API_TOKEN=pqa-...
 ```
 
-To upload files:
+To query agent:
+
+```py
+import pqapi
+response = pqapi.agent_query(
+    "default",
+    "Are COVID-19 vaccines effective?"
+)
+```
+
+## Managing bibliographies
+
+
+To get information about a specific bibliography
+
+```py
+import pqapi
+response = pqapi.get_bibliography(
+    "default"
+)
+print(response)
+```
+
+You do not need to explicitly create a bibliography, just adding files will create one. To upload files:
 
 ```py
 import pqapi
 files = [open("paper.pdf", "rb"), open("paper2.pdf", "rb")]
 metadatas = [
     pqapi.UploadMetadata(filename="paper.pdf", citation="Test Citation"),
     pqapi.UploadMetadata(filename="paper2.pdf", citation="Test Citation 2"),
@@ -34,16 +57,15 @@
 response = pqapi.upload_files(
     "default",
     files
     metadatas
 )
 ```
 
-To query agent:
+To delete a bibliography:
 
 ```py
 import pqapi
-response = pqapi.query_agent(
-    "default",
-    "Are COVID-19 vaccines effective?"
+response = pqapi.delete_bibliography(
+    "default"
 )
 ```
```

### Comparing `pqapi-0.0.1/setup.py` & `pqapi-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `pqapi-0.0.1/tests/test_api.py` & `pqapi-0.0.2/tests/test_api.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 
 from pqapi import (
     AnswerResponse,
     QueryRequest,
     UploadMetadata,
     agent_query,
-    upload_files,
-    get_bibliography,
     delete_bibliography,
+    get_bibliography,
+    upload_files,
 )
 
 
 def test_query_str():
     response = agent_query("default", "How are bispecific antibodies engineered?")
     assert isinstance(response, AnswerResponse)
```

