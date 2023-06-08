# Comparing `tmp/sherpa-onnx-1.4.3.tar.gz` & `tmp/sherpa-onnx-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sherpa-onnx-1.4.3.tar", last modified: Sun May 14 14:53:58 2023, max compression
+gzip compressed data, was "sherpa-onnx-1.4.4.tar", last modified: Thu Jun  8 02:04:47 2023, max compression
```

## Comparing `sherpa-onnx-1.4.3.tar` & `sherpa-onnx-1.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-14 14:43:38.000000 sherpa-onnx-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-14 14:43:38.000000 sherpa-onnx-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-14 14:43:38.000000 sherpa-onnx-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/sherpa-onnx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/sherpa-onnx/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-14 14:53:57.000000 sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-05-14 14:43:38.000000 sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-14 14:43:38.000000 sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 14:53:58.030425 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-14 14:53:58.000000 sherpa-onnx-1.4.3/sherpa_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:04:47.528623 sherpa-onnx-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-08 01:54:11.000000 sherpa-onnx-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 02:04:47.528623 sherpa-onnx-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-08 01:54:11.000000 sherpa-onnx-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 02:04:47.528623 sherpa-onnx-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-08 01:54:11.000000 sherpa-onnx-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:04:47.528623 sherpa-onnx-1.4.4/sherpa-onnx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:04:47.528623 sherpa-onnx-1.4.4/sherpa-onnx/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:04:47.528623 sherpa-onnx-1.4.4/sherpa-onnx/python/sherpa_onnx/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 02:04:47.000000 sherpa-onnx-1.4.4/sherpa-onnx/python/sherpa_onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-06-08 01:54:11.000000 sherpa-onnx-1.4.4/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-08 01:54:11.000000 sherpa-onnx-1.4.4/sherpa-onnx/python/sherpa_onnx/online_recognizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:04:47.528623 sherpa-onnx-1.4.4/sherpa_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 02:04:47.000000 sherpa-onnx-1.4.4/sherpa_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-08 02:04:47.000000 sherpa-onnx-1.4.4/sherpa_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 02:04:47.000000 sherpa-onnx-1.4.4/sherpa_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 02:04:47.000000 sherpa-onnx-1.4.4/sherpa_onnx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 02:04:47.000000 sherpa-onnx-1.4.4/sherpa_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 02:04:47.000000 sherpa-onnx-1.4.4/sherpa_onnx.egg-info/top_level.txt
```

### Comparing `sherpa-onnx-1.4.3/LICENSE` & `sherpa-onnx-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.3/PKG-INFO` & `sherpa-onnx-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.3
+Version: 1.4.4
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

### Comparing `sherpa-onnx-1.4.3/setup.py` & `sherpa-onnx-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py` & `sherpa-onnx-1.4.4/sherpa-onnx/python/sherpa_onnx/offline_recognizer.py`

 * *Files identical despite different names*

### Comparing `sherpa-onnx-1.4.3/sherpa-onnx/python/sherpa_onnx/online_recognizer.py` & `sherpa-onnx-1.4.4/sherpa-onnx/python/sherpa_onnx/online_recognizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,15 @@
             endpoint_config=endpoint_config,
             enable_endpoint=enable_endpoint_detection,
             decoding_method=decoding_method,
             max_active_paths=max_active_paths,
         )
 
         self.recognizer = _Recognizer(recognizer_config)
+        self.config = recognizer_config
 
     def create_stream(self):
         return self.recognizer.create_stream()
 
     def decode_stream(self, s: OnlineStream):
         self.recognizer.decode_stream(s)
```

### Comparing `sherpa-onnx-1.4.3/sherpa_onnx.egg-info/PKG-INFO` & `sherpa-onnx-1.4.4/sherpa_onnx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sherpa-onnx
-Version: 1.4.3
+Version: 1.4.4
 Summary: UNKNOWN
 Home-page: https://github.com/k2-fsa/sherpa-onnx
 Author: The sherpa-onnx development team
 Author-email: dpovey@gmail.com
 License: Apache licensed, as found in the LICENSE file
 Platform: UNKNOWN
 Classifier: Programming Language :: C++
```

