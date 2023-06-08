# Comparing `tmp/sage-data-client-0.5.0.post1.tar.gz` & `tmp/sage-data-client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sage-data-client-0.5.0.post1.tar", last modified: Thu Dec  1 19:34:27 2022, max compression
+gzip compressed data, was "sage-data-client-0.6.0.tar", last modified: Thu Jun  8 15:03:24 2023, max compression
```

## Comparing `sage-data-client-0.5.0.post1.tar` & `sage-data-client-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 19:34:27.888756 sage-data-client-0.5.0.post1/
--rw-r--r--   0 runner    (1001) docker     (122)     1896 2022-12-01 19:34:16.000000 sage-data-client-0.5.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3223 2022-12-01 19:34:27.888756 sage-data-client-0.5.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2681 2022-12-01 19:34:16.000000 sage-data-client-0.5.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      104 2022-12-01 19:34:16.000000 sage-data-client-0.5.0.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      701 2022-12-01 19:34:27.888756 sage-data-client-0.5.0.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 19:34:27.888756 sage-data-client-0.5.0.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 19:34:27.888756 sage-data-client-0.5.0.post1/src/sage_data_client/
--rw-r--r--   0 runner    (1001) docker     (122)      413 2022-12-01 19:34:16.000000 sage-data-client-0.5.0.post1/src/sage_data_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4551 2022-12-01 19:34:16.000000 sage-data-client-0.5.0.post1/src/sage_data_client/query.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 19:34:27.888756 sage-data-client-0.5.0.post1/src/sage_data_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3223 2022-12-01 19:34:27.000000 sage-data-client-0.5.0.post1/src/sage_data_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      324 2022-12-01 19:34:27.000000 sage-data-client-0.5.0.post1/src/sage_data_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 19:34:27.000000 sage-data-client-0.5.0.post1/src/sage_data_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2022-12-01 19:34:27.000000 sage-data-client-0.5.0.post1/src/sage_data_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-12-01 19:34:27.000000 sage-data-client-0.5.0.post1/src/sage_data_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:03:24.496142 sage-data-client-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-08 15:03:12.000000 sage-data-client-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-08 15:03:24.496142 sage-data-client-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-08 15:03:12.000000 sage-data-client-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 15:03:12.000000 sage-data-client-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-08 15:03:24.496142 sage-data-client-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:03:24.492142 sage-data-client-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:03:24.492142 sage-data-client-0.6.0/src/sage_data_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-08 15:03:12.000000 sage-data-client-0.6.0/src/sage_data_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-06-08 15:03:12.000000 sage-data-client-0.6.0/src/sage_data_client/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:03:24.496142 sage-data-client-0.6.0/src/sage_data_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-06-08 15:03:24.000000 sage-data-client-0.6.0/src/sage_data_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 15:03:24.000000 sage-data-client-0.6.0/src/sage_data_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:03:24.000000 sage-data-client-0.6.0/src/sage_data_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 15:03:24.000000 sage-data-client-0.6.0/src/sage_data_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 15:03:24.000000 sage-data-client-0.6.0/src/sage_data_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:03:24.496142 sage-data-client-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-06-08 15:03:12.000000 sage-data-client-0.6.0/tests/test_query.py
```

### Comparing `sage-data-client-0.5.0.post1/LICENSE` & `sage-data-client-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sage-data-client-0.5.0.post1/PKG-INFO` & `sage-data-client-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sage-data-client
-Version: 0.5.0.post1
+Version: 0.6.0
 Summary: Official Sage data client.
 Home-page: https://github.com/sagecontinuum/sage-data-client
 Author: Sean Shahkarami
 Author-email: sean.shahkarami@gmail.com
 Project-URL: Bug Tracker, https://github.com/sagecontinuum/sage-data-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `sage-data-client-0.5.0.post1/README.md` & `sage-data-client-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `sage-data-client-0.5.0.post1/setup.cfg` & `sage-data-client-0.6.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sage-data-client
-version = 0.5.0.post1
+version = 0.6.0
 author = Sean Shahkarami
 author_email = sean.shahkarami@gmail.com
 description = Official Sage data client.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sagecontinuum/sage-data-client
 project_urls =
```

### Comparing `sage-data-client-0.5.0.post1/src/sage_data_client/query.py` & `sage-data-client-0.6.0/src/sage_data_client/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,34 @@
-from urllib.request import urlopen
+from urllib.request import urlopen, Request
 import json
 import pandas as pd
+from typing import Optional
 
 
 def resolve_time(t):
     try:
         return pd.to_datetime(t)
     except (TypeError, ValueError):
         pass
     return pd.to_datetime("now", utc=True) + pd.to_timedelta(t)
 
 
 def timestr(t):
     return t.strftime("%Y-%m-%dT%H:%M:%S.%fZ")
 
 
-def query(start, end = None, head: int = None, tail: int = None, bucket: str = None, filter: dict = None,
-    endpoint: str = "https://data.sagecontinuum.org/api/v1/query") -> pd.DataFrame:
+def query(
+    start,
+    end=None,
+    head: int = None,
+    tail: int = None,
+    bucket: str = None,
+    filter: dict = None,
+    endpoint: str = "https://data.sagecontinuum.org/api/v1/query",
+) -> pd.DataFrame:
     """
     query makes a query request to the data API and returns the results in a data frame.
 
     Parameters
     ----------
     start : query start time, required
         Timestamps can be a relative like "-1h" or absolute like "2021-05-01T10:30:00Z".
@@ -82,27 +90,38 @@
     if head is not None:
         q["head"] = head
     if tail is not None:
         q["tail"] = tail
     if bucket is not None:
         q["bucket"] = bucket
 
-    request_body = json.dumps(q).encode()
-    with urlopen(endpoint, request_body) as f:
-        return load(f)
+    data = json.dumps(q).encode()
+    headers = {"Accept-Encoding": "gzip"}
+    req = Request(endpoint, data, headers=headers)
+
+    with urlopen(req) as f:
+        # determine compression type
+        content_encoding = f.headers.get("Content-Encoding", "")
+        if "gzip" in content_encoding:
+            compression = "gzip"
+        else:
+            compression = None
+        return load(f, compression=compression)
 
 
-def load(path_or_buf) -> pd.DataFrame:
+def load(path_or_buf, compression: Optional[str] = None) -> pd.DataFrame:
     """
     load reads a path or file like object containing a response from the data api and returns the results in a data frame.
 
     Parameters
     ----------
     path_or_buf : path like or file like object
 
+    compression : specify compression type (ex. gzip). this will automatically be inferred when using a path.
+
     Returns
     -------
     result : pandas.DataFrame
         The data frame will contain the query response records. Standard columns names are:
 
         `name`: measurement name (ex. "env.temperature")
 
@@ -111,37 +130,45 @@
         `value`: measurement value
 
         Metadata fields like "node" and "vsn" are stored in columns named "meta.node" or "meta.vsn".
 
     Examples
     --------
 
-    Loading saved query results from a a file
+    Loading saved query results from a file
 
     Suppose we've saved the results of a query to a file `data.json`. We can load them using the following:
 
     ```python
     import sage_data_client
 
     # load results from local file
     df = sage_data_client.load("data.json")
 
     # print number of results of each name
     print(df.groupby(["meta.node", "name"]).size())
     ```
     """
-    df = pd.read_json(path_or_buf, lines=True, date_unit="ns", dtype={"name": str})
+    df = pd.read_json(
+        path_or_buf,
+        lines=True,
+        date_unit="ns",
+        dtype={"name": str},
+        compression=compression,
+    )
 
     # if dataframe is empty, return empty with known columns
     if len(df) == 0:
-        return pd.DataFrame({
-            "timestamp": pd.to_datetime([], utc=True),
-            "name": pd.Series([], dtype=str),
-            "value": [],
-        })
+        return pd.DataFrame(
+            {
+                "timestamp": pd.to_datetime([], utc=True),
+                "name": pd.Series([], dtype=str),
+                "value": [],
+            }
+        )
 
     # ensure timestamp is in proper format
     df["timestamp"] = pd.to_datetime(df["timestamp"], utc=True)
 
     # otherwise, normalize meta columns to meta.* columns
     meta = pd.DataFrame(df["meta"].tolist())
     meta.rename({c: "meta." + c for c in meta.columns}, axis="columns", inplace=True)
```

### Comparing `sage-data-client-0.5.0.post1/src/sage_data_client.egg-info/PKG-INFO` & `sage-data-client-0.6.0/src/sage_data_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sage-data-client
-Version: 0.5.0.post1
+Version: 0.6.0
 Summary: Official Sage data client.
 Home-page: https://github.com/sagecontinuum/sage-data-client
 Author: Sean Shahkarami
 Author-email: sean.shahkarami@gmail.com
 Project-URL: Bug Tracker, https://github.com/sagecontinuum/sage-data-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

