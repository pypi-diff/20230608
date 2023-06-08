# Comparing `tmp/nuclio_sdk-0.5.4.tar.gz` & `tmp/nuclio_sdk-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-ttg06ebp/nuclio_sdk-0.5.4.tar", last modified: Mon Jun  5 11:07:45 2023, max compression
+gzip compressed data, was "/home/runner/work/nuclio-sdk-py/nuclio-sdk-py/dist/.tmp-h4g9w1wc/nuclio_sdk-0.5.5.tar", last modified: Thu Jun  8 09:45:43 2023, max compression
```

## Comparing `nuclio_sdk-0.5.4.tar` & `nuclio_sdk-0.5.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/mock_platform.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/test_qualified_offset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/nuclio_sdk/test/test_response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/nuclio_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 11:07:45.000000 nuclio_sdk-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-05 11:07:09.000000 nuclio_sdk-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/mock_platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/test_qualified_offset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/nuclio_sdk/test/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/nuclio_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-08 09:45:43.000000 nuclio_sdk-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-08 09:45:07.000000 nuclio_sdk-0.5.5/setup.py
```

### Comparing `nuclio_sdk-0.5.4/LICENSE.txt` & `nuclio_sdk-0.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/PKG-INFO` & `nuclio_sdk-0.5.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclio_sdk
-Version: 0.5.4
+Version: 0.5.5
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio_sdk-0.5.4/Pipfile` & `nuclio_sdk-0.5.5/Pipfile`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/Pipfile.lock` & `nuclio_sdk-0.5.5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/__init__.py` & `nuclio_sdk-0.5.5/nuclio_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/context.py` & `nuclio_sdk-0.5.5/nuclio_sdk/context.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/event.py` & `nuclio_sdk-0.5.5/nuclio_sdk/event.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/exceptions.py` & `nuclio_sdk-0.5.5/nuclio_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/helpers.py` & `nuclio_sdk-0.5.5/nuclio_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/json_encoder.py` & `nuclio_sdk-0.5.5/nuclio_sdk/json_encoder.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/logger.py` & `nuclio_sdk-0.5.5/nuclio_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/platform.py` & `nuclio_sdk-0.5.5/nuclio_sdk/platform.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/qualified_offset.py` & `nuclio_sdk-0.5.5/nuclio_sdk/qualified_offset.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/response.py` & `nuclio_sdk-0.5.5/nuclio_sdk/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,22 +73,29 @@
                 response["content_type"] = handler_output.content_type
 
             response["headers"] = handler_output.headers
             response["status_code"] = handler_output.status_code
         else:
             response["body"] = handler_output
 
-        if isinstance(response["body"], bytes):
-            response["body"] = base64.b64encode(response["body"]).decode("ascii")
-            response["body_encoding"] = "base64"
+        Response._ensure_str_body(response)
 
         return response
 
     @staticmethod
     def empty_response():
         return {
             "body": "",
             "content_type": "text/plain",
             "headers": {},
             "status_code": 200,
             "body_encoding": "text",
         }
+
+    @staticmethod
+    def _ensure_str_body(response):
+        if isinstance(response["body"], bytes):
+            response["body"] = base64.b64encode(response["body"]).decode("ascii")
+            response["body_encoding"] = "base64"
+
+        if response["body_encoding"] == "text":
+            response["body"] = str(response["body"])
```

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/test/__init__.py` & `nuclio_sdk-0.5.5/nuclio_sdk/test/__init__.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/test/mock_platform.py` & `nuclio_sdk-0.5.5/nuclio_sdk/test/mock_platform.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/test/test_case.py` & `nuclio_sdk-0.5.5/nuclio_sdk/test/test_case.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/test/test_event.py` & `nuclio_sdk-0.5.5/nuclio_sdk/test/test_event.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/test/test_logger.py` & `nuclio_sdk-0.5.5/nuclio_sdk/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/test/test_qualified_offset.py` & `nuclio_sdk-0.5.5/nuclio_sdk/test/test_qualified_offset.py`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk/test/test_response.py` & `nuclio_sdk-0.5.5/nuclio_sdk/test/test_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,20 @@
     def test_str(self):
         handler_return = "test"
         expected_response = self._compile_output_response(body="test")
         self._validate_response(handler_return, expected_response)
 
     def test_int(self):
         handler_return = 2020
-        expected_response = self._compile_output_response(body=2020)
+        expected_response = self._compile_output_response(body="2020")
+        self._validate_response(handler_return, expected_response)
+
+    def test_float(self):
+        handler_return = 12.34
+        expected_response = self._compile_output_response(body="12.34")
         self._validate_response(handler_return, expected_response)
 
     def test_bytes(self):
         handler_return = b"test"
         expected_response = self._compile_output_response(
             body="dGVzdA==", body_encoding="base64"  # base64 value for 'test'
         )
@@ -52,15 +57,15 @@
         expected_response = self._compile_output_response(
             body="[1, 2, 3, true]", content_type="application/json"
         )
         self._validate_response(handler_return, expected_response)
 
     def test_datetime(self):
         handler_return = datetime.datetime.now()
-        expected_response = self._compile_output_response(body=handler_return)
+        expected_response = self._compile_output_response(body=str(handler_return))
         self._validate_response(handler_return, expected_response)
 
     def test_status_code_and_str(self):
         handler_return = (201, "test")
         expected_response = self._compile_output_response(
             body="test", status_code=handler_return[0]
         )
```

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk.egg-info/PKG-INFO` & `nuclio_sdk-0.5.5/nuclio_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nuclio-sdk
-Version: 0.5.4
+Version: 0.5.5
 Summary: Client for the Nuclio serverless platform
 Home-page: https://github.com/nuclio/nuclio-sdk-py
 Author: Eran Duchan
 Author-email: erand@iguazio.com
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `nuclio_sdk-0.5.4/nuclio_sdk.egg-info/SOURCES.txt` & `nuclio_sdk-0.5.5/nuclio_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuclio_sdk-0.5.4/setup.py` & `nuclio_sdk-0.5.5/setup.py`

 * *Files identical despite different names*

