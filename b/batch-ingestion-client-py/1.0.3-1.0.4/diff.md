# Comparing `tmp/batch_ingestion_client_py-1.0.3.tar.gz` & `tmp/batch_ingestion_client_py-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch_ingestion_client_py-1.0.3.tar", last modified: Fri Apr 28 13:47:18 2023, max compression
+gzip compressed data, was "batch_ingestion_client_py-1.0.4.tar", last modified: Thu Jun  8 10:19:27 2023, max compression
```

## Comparing `batch_ingestion_client_py-1.0.3.tar` & `batch_ingestion_client_py-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-28 13:47:18.675181 batch_ingestion_client_py-1.0.3/
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1069 2023-04-20 14:24:25.000000 batch_ingestion_client_py-1.0.3/LICENSE
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     2030 2023-04-28 13:47:18.675181 batch_ingestion_client_py-1.0.3/PKG-INFO
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1372 2023-04-28 13:44:26.000000 batch_ingestion_client_py-1.0.3/README.md
-drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-28 13:47:18.675181 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      254 2023-04-28 12:51:27.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/__init__.py
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1436 2023-04-28 13:17:43.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/curl.py
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     5271 2023-04-28 13:40:54.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/data.py
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1946 2023-04-28 13:28:14.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/lib.py
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1422 2023-04-20 13:08:18.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/response.py
-drwxrwxr-x   0 dappermink  (1000) dappermink  (1000)        0 2023-04-28 13:47:18.675181 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     2030 2023-04-28 13:47:18.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/PKG-INFO
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)      399 2023-04-28 13:47:18.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/SOURCES.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)        1 2023-04-28 13:47:18.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/dependency_links.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)       26 2023-04-28 13:47:18.000000 batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/top_level.txt
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)       38 2023-04-28 13:47:18.675181 batch_ingestion_client_py-1.0.3/setup.cfg
--rw-rw-r--   0 dappermink  (1000) dappermink  (1000)     1092 2023-04-28 13:23:49.000000 batch_ingestion_client_py-1.0.3/setup.py
+drwxr-xr-x   0 quentinjanuel   (501) staff       (20)        0 2023-06-08 10:19:27.311792 batch_ingestion_client_py-1.0.4/
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)     1069 2023-06-08 10:08:41.000000 batch_ingestion_client_py-1.0.4/LICENSE
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)     1974 2023-06-08 10:19:27.311655 batch_ingestion_client_py-1.0.4/PKG-INFO
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)     1372 2023-06-08 10:09:14.000000 batch_ingestion_client_py-1.0.4/README.md
+drwxr-xr-x   0 quentinjanuel   (501) staff       (20)        0 2023-06-08 10:19:27.310958 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py/
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)      254 2023-06-08 10:08:41.000000 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py/__init__.py
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)     1436 2023-06-08 10:08:41.000000 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py/curl.py
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)     5271 2023-06-08 10:08:41.000000 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py/data.py
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)     1946 2023-06-08 10:08:41.000000 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py/lib.py
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)     1561 2023-06-08 10:10:39.000000 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py/response.py
+drwxr-xr-x   0 quentinjanuel   (501) staff       (20)        0 2023-06-08 10:19:27.311461 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py.egg-info/
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)     1974 2023-06-08 10:19:27.000000 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py.egg-info/PKG-INFO
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)      399 2023-06-08 10:19:27.000000 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py.egg-info/SOURCES.txt
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)        1 2023-06-08 10:19:27.000000 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py.egg-info/dependency_links.txt
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)       26 2023-06-08 10:19:27.000000 batch_ingestion_client_py-1.0.4/batch_ingestion_client_py.egg-info/top_level.txt
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)       38 2023-06-08 10:19:27.311841 batch_ingestion_client_py-1.0.4/setup.cfg
+-rw-r--r--   0 quentinjanuel   (501) staff       (20)     1092 2023-06-08 10:11:29.000000 batch_ingestion_client_py-1.0.4/setup.py
```

### Comparing `batch_ingestion_client_py-1.0.3/LICENSE` & `batch_ingestion_client_py-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `batch_ingestion_client_py-1.0.3/PKG-INFO` & `batch_ingestion_client_py-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: batch_ingestion_client_py
-Version: 1.0.3
+Version: 1.0.4
 Summary: A client for the BatchIngestion mediawiki API
-Home-page: UNKNOWN
 Author: QuentinJanuel
 Author-email: <quentinjanuelkij@gmail.com>
-License: UNKNOWN
 Keywords: python,mediawiki,batchingestion,wikidata,wikibase,api,client
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -23,15 +20,15 @@
 This is a Python client library for the [BatchIngestion](https://gitlab.the-qa-company.com/FrozenMink/batchingestionextension) MediaWiki extension, which provides an API to ingest many entities at once. This library allows you to easily ingest entities in bulk, either by parsing them from JSON or by creating them using Python objects.
 
 ## Installation
 
 You can install this library using [pip](https://pypi.org/project/batch-ingestion-client-py/):
 
 ```bash
-pip install batch-ingestion-client-py==1.0.3
+pip install batch-ingestion-client-py==1.0.4
 ```
 
 ## Usage
 
 ```python
 from batch_ingestion_client_py import (
     BatchIngestor,
@@ -73,9 +70,7 @@
 
 print(example2)
 ```
 
 ## Contributing
 
 If you'd like to contribute to this library, please feel free to submit a pull request.
-
-
```

### Comparing `batch_ingestion_client_py-1.0.3/README.md` & `batch_ingestion_client_py-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This is a Python client library for the [BatchIngestion](https://gitlab.the-qa-company.com/FrozenMink/batchingestionextension) MediaWiki extension, which provides an API to ingest many entities at once. This library allows you to easily ingest entities in bulk, either by parsing them from JSON or by creating them using Python objects.
 
 ## Installation
 
 You can install this library using [pip](https://pypi.org/project/batch-ingestion-client-py/):
 
 ```bash
-pip install batch-ingestion-client-py==1.0.3
+pip install batch-ingestion-client-py==1.0.4
 ```
 
 ## Usage
 
 ```python
 from batch_ingestion_client_py import (
     BatchIngestor,
```

### Comparing `batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/curl.py` & `batch_ingestion_client_py-1.0.4/batch_ingestion_client_py/curl.py`

 * *Files identical despite different names*

### Comparing `batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/data.py` & `batch_ingestion_client_py-1.0.4/batch_ingestion_client_py/data.py`

 * *Files identical despite different names*

### Comparing `batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/lib.py` & `batch_ingestion_client_py-1.0.4/batch_ingestion_client_py/lib.py`

 * *Files identical despite different names*

### Comparing `batch_ingestion_client_py-1.0.3/batch_ingestion_client_py/response.py` & `batch_ingestion_client_py-1.0.4/batch_ingestion_client_py/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,18 +43,21 @@
             "count": self.count,
             "successes": self.successes,
             "response": [r.serialize() for r in self.response],
         }
 
     @staticmethod
     def parse(data: Dict[str, int | List[Dict[str, str | int]]]):
-        return Response(
-            count=data["count"],  # type: ignore
-            successes=data["successes"],  # type: ignore
-            response=[
-                Revision.parse(r)
-                for r in data["response"]  # type: ignore
-            ],
-        )
+        try:
+            return Response(
+                count=data["count"],  # type: ignore
+                successes=data["successes"],  # type: ignore
+                response=[
+                    Revision.parse(r)
+                    for r in data["response"]  # type: ignore
+                ],
+            )
+        except Exception:
+            raise Exception(f"Error returned from the API: {data}")
 
     def __repr__(self) -> str:
         return self.serialize().__repr__()
```

### Comparing `batch_ingestion_client_py-1.0.3/batch_ingestion_client_py.egg-info/PKG-INFO` & `batch_ingestion_client_py-1.0.4/batch_ingestion_client_py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 Metadata-Version: 2.1
 Name: batch-ingestion-client-py
-Version: 1.0.3
+Version: 1.0.4
 Summary: A client for the BatchIngestion mediawiki API
-Home-page: UNKNOWN
 Author: QuentinJanuel
 Author-email: <quentinjanuelkij@gmail.com>
-License: UNKNOWN
 Keywords: python,mediawiki,batchingestion,wikidata,wikibase,api,client
-Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
@@ -23,15 +20,15 @@
 This is a Python client library for the [BatchIngestion](https://gitlab.the-qa-company.com/FrozenMink/batchingestionextension) MediaWiki extension, which provides an API to ingest many entities at once. This library allows you to easily ingest entities in bulk, either by parsing them from JSON or by creating them using Python objects.
 
 ## Installation
 
 You can install this library using [pip](https://pypi.org/project/batch-ingestion-client-py/):
 
 ```bash
-pip install batch-ingestion-client-py==1.0.3
+pip install batch-ingestion-client-py==1.0.4
 ```
 
 ## Usage
 
 ```python
 from batch_ingestion_client_py import (
     BatchIngestor,
@@ -73,9 +70,7 @@
 
 print(example2)
 ```
 
 ## Contributing
 
 If you'd like to contribute to this library, please feel free to submit a pull request.
-
-
```

### Comparing `batch_ingestion_client_py-1.0.3/setup.py` & `batch_ingestion_client_py-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 DESCRIPTION = "A client for the BatchIngestion mediawiki API"
 
 setup(
     name="batch_ingestion_client_py",
     version=VERSION,
     author="QuentinJanuel",
     author_email="<quentinjanuelkij@gmail.com>",
```

