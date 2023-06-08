# Comparing `tmp/zarrita-0.1.0a2.tar.gz` & `tmp/zarrita-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zarrita-0.1.0a2.tar", max compression
+gzip compressed data, was "zarrita-0.1.0a3.tar", max compression
```

## Comparing `zarrita-0.1.0a2.tar` & `zarrita-0.1.0a3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a2/LICENSE
--rw-r--r--   0        0        0     2741 2023-06-08 08:07:06.094114 zarrita-0.1.0a2/README.md
--rw-r--r--   0        0        0      696 2023-06-08 08:07:52.106498 zarrita-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     1085 2023-06-07 11:49:09.452172 zarrita-0.1.0a2/zarrita/__init__.py
--rw-r--r--   0        0        0    19595 2023-06-07 19:18:11.589026 zarrita-0.1.0a2/zarrita/array.py
--rw-r--r--   0        0        0    13242 2023-06-07 20:04:03.128152 zarrita-0.1.0a2/zarrita/array_v2.py
--rw-r--r--   0        0        0    12285 2023-06-08 07:24:44.647554 zarrita-0.1.0a2/zarrita/codecs.py
--rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a2/zarrita/common.py
--rw-r--r--   0        0        0     4181 2023-06-07 15:17:15.193840 zarrita-0.1.0a2/zarrita/group.py
--rw-r--r--   0        0        0     4735 2023-06-07 15:17:10.125767 zarrita-0.1.0a2/zarrita/group_v2.py
--rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a2/zarrita/indexing.py
--rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a2/zarrita/metadata.py
--rw-r--r--   0        0        0    20531 2023-06-07 18:32:25.846759 zarrita-0.1.0a2/zarrita/sharding.py
--rw-r--r--   0        0        0     5391 2023-06-07 20:04:34.652580 zarrita-0.1.0a2/zarrita/store.py
--rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a2/zarrita/sync.py
--rw-r--r--   0        0        0     3827 2023-06-06 13:35:33.794530 zarrita-0.1.0a2/zarrita/value_handle.py
--rw-r--r--   0        0        0     3442 1970-01-01 00:00:00.000000 zarrita-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-05-09 09:12:03.956626 zarrita-0.1.0a3/LICENSE
+-rw-r--r--   0        0        0     2311 2023-06-08 08:19:54.182773 zarrita-0.1.0a3/README.md
+-rw-r--r--   0        0        0      696 2023-06-08 08:20:09.118147 zarrita-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0     1085 2023-06-07 11:49:09.452172 zarrita-0.1.0a3/zarrita/__init__.py
+-rw-r--r--   0        0        0    19595 2023-06-07 19:18:11.589026 zarrita-0.1.0a3/zarrita/array.py
+-rw-r--r--   0        0        0    13242 2023-06-07 20:04:03.128152 zarrita-0.1.0a3/zarrita/array_v2.py
+-rw-r--r--   0        0        0    12285 2023-06-08 07:24:44.647554 zarrita-0.1.0a3/zarrita/codecs.py
+-rw-r--r--   0        0        0     4314 2023-06-07 20:03:42.377098 zarrita-0.1.0a3/zarrita/common.py
+-rw-r--r--   0        0        0     4181 2023-06-07 15:17:15.193840 zarrita-0.1.0a3/zarrita/group.py
+-rw-r--r--   0        0        0     4735 2023-06-07 15:17:10.125767 zarrita-0.1.0a3/zarrita/group_v2.py
+-rw-r--r--   0        0        0     7259 2023-06-07 12:49:15.942016 zarrita-0.1.0a3/zarrita/indexing.py
+-rw-r--r--   0        0        0     5374 2023-06-08 07:17:39.694424 zarrita-0.1.0a3/zarrita/metadata.py
+-rw-r--r--   0        0        0    20531 2023-06-07 18:32:25.846759 zarrita-0.1.0a3/zarrita/sharding.py
+-rw-r--r--   0        0        0     5391 2023-06-07 20:04:34.652580 zarrita-0.1.0a3/zarrita/store.py
+-rw-r--r--   0        0        0     2555 2023-06-02 09:33:41.528984 zarrita-0.1.0a3/zarrita/sync.py
+-rw-r--r--   0        0        0     3827 2023-06-06 13:35:33.794530 zarrita-0.1.0a3/zarrita/value_handle.py
+-rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 zarrita-0.1.0a3/PKG-INFO
```

### Comparing `zarrita-0.1.0a2/LICENSE` & `zarrita-0.1.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/README.md` & `zarrita-0.1.0a3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 ## Setup
 
 ```python
 import zarrita
 import numpy as np
 
-store = zarrita.FileSystemStore('file://./testdata')
+store = zarrita.LocalStore('testdata') # or zarrita.RemoteStore('s3://bucket/test')
 ```
 
 ## Create an array
 
 ```python
 a = await zarrita.Array.create_async(
     store,
     'array',
     shape=(6, 10),
     dtype='int32',
     chunk_shape=(2, 5),
-    codecs=[zarrita.codecs.gzip_codec(level=1)],
+    codecs=[zarrita.codecs.blosc_codec()],
     attributes={'question': 'life', 'answer': 42}
 )
 await a.async_[:, :].set(np.ones((6, 10), dtype='int32'))
 ```
 
 ## Open an array
 
@@ -42,15 +42,15 @@
     shape=(16, 16),
     dtype='int32',
     chunk_shape=(16, 16),
     chunk_key_encoding=('v2', '.'),
     codecs=[
         zarrita.codecs.sharding_codec(
             chunk_shape=(8, 8),
-            codecs=[zarrita.codecs.gzip_codec(level=1)]
+            codecs=[zarrita.codecs.blosc_codec()]
         ),
     ],
 )
 data = np.arange(0, 16 * 16, dtype='int32').reshape((16, 16))
 await a.async_[:, :].set(data)
 assert np.array_equal(await a.async_[:, :].get(), data)
 ```
@@ -79,30 +79,7 @@
 ```
 
 # Credits
 
 This is a largely-rewritten fork of `zarrita` by [@alimanfoo](https://github.com/alimanfoo). It implements the Zarr v3 draft specification created by [@alimanfoo](https://github.com/alimanfoo), [@jstriebel](https://github.com/jstriebel), [@jbms](https://github.com/jbms) et al.
 
 Licensed under MIT
-
-# TODO
-
-- [x] Async
-- [x] sharding partial decode
-- [x] variable renaming
-- [x] type indexing
-- [x] value handle slices get and set
-- [x] codec classes
-- [x] metadata validation
-- [x] zarr v2
-- [x] open with v2/v3 auto-detect
-- [x] async gather in sharding
-- [x] async local store
-- [x] resize arrays
-- [x] check empty before create array
-- [ ] morton order in indexing
-- [ ] attrs -> dataclasses
-
-## Non-priority
-
-- Dask support
-- Buffer protocol
```

### Comparing `zarrita-0.1.0a2/pyproject.toml` & `zarrita-0.1.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zarrita"
-version = "0.1.0a2"
+version = "0.1.0a3"
 description = ""
 authors = ["Norman Rzepka <code@normanrz.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `zarrita-0.1.0a2/zarrita/__init__.py` & `zarrita-0.1.0a3/zarrita/__init__.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/array.py` & `zarrita-0.1.0a3/zarrita/array.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/array_v2.py` & `zarrita-0.1.0a3/zarrita/array_v2.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/codecs.py` & `zarrita-0.1.0a3/zarrita/codecs.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/common.py` & `zarrita-0.1.0a3/zarrita/common.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/group.py` & `zarrita-0.1.0a3/zarrita/group.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/group_v2.py` & `zarrita-0.1.0a3/zarrita/group_v2.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/indexing.py` & `zarrita-0.1.0a3/zarrita/indexing.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/metadata.py` & `zarrita-0.1.0a3/zarrita/metadata.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/sharding.py` & `zarrita-0.1.0a3/zarrita/sharding.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/store.py` & `zarrita-0.1.0a3/zarrita/store.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/sync.py` & `zarrita-0.1.0a3/zarrita/sync.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/zarrita/value_handle.py` & `zarrita-0.1.0a3/zarrita/value_handle.py`

 * *Files identical despite different names*

### Comparing `zarrita-0.1.0a2/PKG-INFO` & `zarrita-0.1.0a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zarrita
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: 
 License: MIT
 Author: Norman Rzepka
 Author-email: code@normanrz.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,27 +25,27 @@
 
 ## Setup
 
 ```python
 import zarrita
 import numpy as np
 
-store = zarrita.FileSystemStore('file://./testdata')
+store = zarrita.LocalStore('testdata') # or zarrita.RemoteStore('s3://bucket/test')
 ```
 
 ## Create an array
 
 ```python
 a = await zarrita.Array.create_async(
     store,
     'array',
     shape=(6, 10),
     dtype='int32',
     chunk_shape=(2, 5),
-    codecs=[zarrita.codecs.gzip_codec(level=1)],
+    codecs=[zarrita.codecs.blosc_codec()],
     attributes={'question': 'life', 'answer': 42}
 )
 await a.async_[:, :].set(np.ones((6, 10), dtype='int32'))
 ```
 
 ## Open an array
 
@@ -63,15 +63,15 @@
     shape=(16, 16),
     dtype='int32',
     chunk_shape=(16, 16),
     chunk_key_encoding=('v2', '.'),
     codecs=[
         zarrita.codecs.sharding_codec(
             chunk_shape=(8, 8),
-            codecs=[zarrita.codecs.gzip_codec(level=1)]
+            codecs=[zarrita.codecs.blosc_codec()]
         ),
     ],
 )
 data = np.arange(0, 16 * 16, dtype='int32').reshape((16, 16))
 await a.async_[:, :].set(data)
 assert np.array_equal(await a.async_[:, :].get(), data)
 ```
@@ -101,30 +101,7 @@
 
 # Credits
 
 This is a largely-rewritten fork of `zarrita` by [@alimanfoo](https://github.com/alimanfoo). It implements the Zarr v3 draft specification created by [@alimanfoo](https://github.com/alimanfoo), [@jstriebel](https://github.com/jstriebel), [@jbms](https://github.com/jbms) et al.
 
 Licensed under MIT
 
-# TODO
-
-- [x] Async
-- [x] sharding partial decode
-- [x] variable renaming
-- [x] type indexing
-- [x] value handle slices get and set
-- [x] codec classes
-- [x] metadata validation
-- [x] zarr v2
-- [x] open with v2/v3 auto-detect
-- [x] async gather in sharding
-- [x] async local store
-- [x] resize arrays
-- [x] check empty before create array
-- [ ] morton order in indexing
-- [ ] attrs -> dataclasses
-
-## Non-priority
-
-- Dask support
-- Buffer protocol
-
```

