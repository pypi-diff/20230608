# Comparing `tmp/chima-0.0.6.tar.gz` & `tmp/chima-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chima-0.0.6.tar", max compression
+gzip compressed data, was "chima-0.0.7.tar", max compression
```

## Comparing `chima-0.0.6.tar` & `chima-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     2253 2023-06-06 21:54:43.678602 chima-0.0.6/README.md
--rw-r--r--   0        0        0      365 2023-06-06 21:54:43.678602 chima-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      191 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/__init__.py
--rw-r--r--   0        0        0     4966 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/client.py
--rw-r--r--   0        0        0      348 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      159 2023-06-06 21:54:43.682602 chima-0.0.6/src/chima/environment.py
--rw-r--r--   0        0        0        0 2023-06-06 21:54:43.682602 chima-0.0.6/src/chima/py.typed
--rw-r--r--   0        0        0      139 2023-06-06 21:54:43.682602 chima-0.0.6/src/chima/types/__init__.py
--rw-r--r--   0        0        0      920 2023-06-06 21:54:43.682602 chima-0.0.6/src/chima/types/search_response.py
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 chima-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2253 2023-06-08 03:14:29.940834 chima-0.0.7/README.md
+-rw-r--r--   0        0        0      365 2023-06-08 03:14:29.940834 chima-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/__init__.py
+-rw-r--r--   0        0        0     8944 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/client.py
+-rw-r--r--   0        0        0      348 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      159 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/environment.py
+-rw-r--r--   0        0        0        0 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/py.typed
+-rw-r--r--   0        0        0      220 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/types/__init__.py
+-rw-r--r--   0        0        0      757 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/types/generate_text_response.py
+-rw-r--r--   0        0        0      920 2023-06-08 03:14:29.940834 chima-0.0.7/src/chima/types/search_response.py
+-rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 chima-0.0.7/PKG-INFO
```

### Comparing `chima-0.0.6/README.md` & `chima-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `chima-0.0.6/src/chima/core/datetime_utils.py` & `chima-0.0.7/src/chima/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.6/src/chima/core/jsonable_encoder.py` & `chima-0.0.7/src/chima/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.6/src/chima/types/search_response.py` & `chima-0.0.7/src/chima/types/search_response.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.6/PKG-INFO` & `chima-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chima
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

