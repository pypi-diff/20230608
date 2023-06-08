# Comparing `tmp/thoughtful-2.0.1.tar.gz` & `tmp/thoughtful-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtful-2.0.1.tar", max compression
+gzip compressed data, was "thoughtful-2.0.2.tar", max compression
```

## Comparing `thoughtful-2.0.1.tar` & `thoughtful-2.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11358 2023-06-05 20:17:30.549384 thoughtful-2.0.1/LICENSE
--rw-r--r--   0        0        0     2992 2023-06-05 20:17:30.549384 thoughtful-2.0.1/README.md
--rw-r--r--   0        0        0     1935 2023-06-05 20:17:30.549384 thoughtful-2.0.1/pyproject.toml
--rw-r--r--   0        0        0      222 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/__init__.py
--rw-r--r--   0        0        0       54 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/__version__.py
--rw-r--r--   0        0        0     1070 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/environment_variables.py
--rw-r--r--   0        0        0      143 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/__init__.py
--rw-r--r--   0        0        0     4466 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/default_instances.py
--rw-r--r--   0        0        0     8580 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/main_context.py
--rw-r--r--   0        0        0    10567 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/manifest.py
--rw-r--r--   0        0        0        0 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/py.typed
--rw-r--r--   0        0        0        0 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/__init__.py
--rw-r--r--   0        0        0     2872 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/record.py
--rw-r--r--   0        0        0     1189 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/record_report.py
--rw-r--r--   0        0        0     2066 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/report.py
--rw-r--r--   0        0        0    10118 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/report_builder.py
--rw-r--r--   0        0        0      660 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/status.py
--rw-r--r--   0        0        0      876 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/step_report.py
--rw-r--r--   0        0        0     1541 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/timed_report.py
--rw-r--r--   0        0        0     1754 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/reporting/timer.py
--rw-r--r--   0        0        0     7609 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/step_context.py
--rw-r--r--   0        0        0     7435 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/step_decorator_factory.py
--rw-r--r--   0        0        0        0 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/__init__.py
--rw-r--r--   0        0        0      736 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/action.py
--rw-r--r--   0        0        0     1347 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/jwt_auth.py
--rw-r--r--   0        0        0     3935 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/notifier.py
--rw-r--r--   0        0        0     3184 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/payloads.py
--rw-r--r--   0        0        0     1352 2023-06-05 20:17:30.553384 thoughtful-2.0.1/thoughtful/supervisor/streaming/token.py
--rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-08 16:34:10.616843 thoughtful-2.0.2/LICENSE
+-rw-r--r--   0        0        0     2992 2023-06-08 16:34:10.616843 thoughtful-2.0.2/README.md
+-rw-r--r--   0        0        0     1935 2023-06-08 16:34:10.620843 thoughtful-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/__init__.py
+-rw-r--r--   0        0        0       54 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/__version__.py
+-rw-r--r--   0        0        0     1070 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/environment_variables.py
+-rw-r--r--   0        0        0      143 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/__init__.py
+-rw-r--r--   0        0        0     4466 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/default_instances.py
+-rw-r--r--   0        0        0     8580 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/main_context.py
+-rw-r--r--   0        0        0    10567 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/manifest.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/py.typed
+-rw-r--r--   0        0        0        0 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/__init__.py
+-rw-r--r--   0        0        0     2872 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/record.py
+-rw-r--r--   0        0        0     1189 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/record_report.py
+-rw-r--r--   0        0        0     2066 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/report.py
+-rw-r--r--   0        0        0    10118 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/report_builder.py
+-rw-r--r--   0        0        0      660 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/status.py
+-rw-r--r--   0        0        0      876 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/step_report.py
+-rw-r--r--   0        0        0     1541 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/timed_report.py
+-rw-r--r--   0        0        0     1754 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/reporting/timer.py
+-rw-r--r--   0        0        0     7609 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/step_context.py
+-rw-r--r--   0        0        0     6531 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/step_decorator_factory.py
+-rw-r--r--   0        0        0        0 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/__init__.py
+-rw-r--r--   0        0        0      736 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/action.py
+-rw-r--r--   0        0        0     1347 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/jwt_auth.py
+-rw-r--r--   0        0        0     4164 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/notifier.py
+-rw-r--r--   0        0        0     3184 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/payloads.py
+-rw-r--r--   0        0        0     1352 2023-06-08 16:34:10.620843 thoughtful-2.0.2/thoughtful/supervisor/streaming/token.py
+-rw-r--r--   0        0        0     4578 1970-01-01 00:00:00.000000 thoughtful-2.0.2/PKG-INFO
```

### Comparing `thoughtful-2.0.1/LICENSE` & `thoughtful-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/README.md` & `thoughtful-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/pyproject.toml` & `thoughtful-2.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thoughtful"
-version = "2.0.1"
+version = "2.0.2"
 description = "Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor"
 authors = ["Thoughtful Automation <care@thoughtful.ai>"]
 license = "Apache-2.0"
 readme = 'README.md'
 homepage = "https://thoughtful.ai"
 repository = "https://github.com/thoughtful-automation/thoughtful"
 documentation = "https://thoughtful-supervisor.readthedocs-hosted.com/en/latest/index.html"
```

### Comparing `thoughtful-2.0.1/thoughtful/environment_variables.py` & `thoughtful-2.0.2/thoughtful/environment_variables.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/default_instances.py` & `thoughtful-2.0.2/thoughtful/supervisor/default_instances.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/main_context.py` & `thoughtful-2.0.2/thoughtful/supervisor/main_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/manifest.py` & `thoughtful-2.0.2/thoughtful/supervisor/manifest.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/reporting/record.py` & `thoughtful-2.0.2/thoughtful/supervisor/reporting/record.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/reporting/record_report.py` & `thoughtful-2.0.2/thoughtful/supervisor/reporting/record_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/reporting/report.py` & `thoughtful-2.0.2/thoughtful/supervisor/reporting/report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/reporting/report_builder.py` & `thoughtful-2.0.2/thoughtful/supervisor/reporting/report_builder.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/reporting/status.py` & `thoughtful-2.0.2/thoughtful/supervisor/reporting/status.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/reporting/step_report.py` & `thoughtful-2.0.2/thoughtful/supervisor/reporting/step_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/reporting/timed_report.py` & `thoughtful-2.0.2/thoughtful/supervisor/reporting/timed_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/reporting/timer.py` & `thoughtful-2.0.2/thoughtful/supervisor/reporting/timer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/step_context.py` & `thoughtful-2.0.2/thoughtful/supervisor/step_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/step_decorator_factory.py` & `thoughtful-2.0.2/thoughtful/supervisor/step_decorator_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,36 +202,7 @@
     # If the step failed and raised an exception, raise that instead
     # of returning None
     if caught_exception:
         raise caught_exception
 
     # Passthrough the function's returned data back up
     return fn_result
-
-
-def to_safe_jsonable(value: Any) -> Any:
-    """
-    Returns a version of `value` that can be converted into JSON
-    format using the `json` library.
-
-    Args:
-        value: The value to ensure is safe to JSON serialize.
-
-    Returns:
-        Any: The JSON safe value
-    """
-    # If the standard JSON library knows how to encode the object,
-    # go with that
-    with contextlib.suppress(TypeError):
-        json.dumps(value)
-        return value
-    # Otherwise, check if the object has a .__json__() method
-    json_attribute = getattr(value, "__json__", None)
-    if callable(json_attribute):
-        try:
-            return value.__json__()
-        except Exception:
-            # [CX-234] If the call fails, warn and continue trying other options
-            logging.warning("__json__ method raised exception", exc_info=True)
-
-    # Use the raw string as a last resort
-    return str(value)
```

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/streaming/action.py` & `thoughtful-2.0.2/thoughtful/supervisor/streaming/action.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/streaming/jwt_auth.py` & `thoughtful-2.0.2/thoughtful/supervisor/streaming/jwt_auth.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/streaming/notifier.py` & `thoughtful-2.0.2/thoughtful/supervisor/streaming/notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import logging
+import warnings
 
 import requests
 
 from thoughtful.supervisor.manifest import Manifest
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.step_report import StepReport
 from thoughtful.supervisor.streaming.jwt_auth import JWTAuth
@@ -58,14 +59,20 @@
         return cls(
             run_id=run_id,
             callback_url=callback_url,
             auth=new_auth,
         )
 
     def post(self, payload: StreamingPayload, **kwargs):
+        if not (self.callback_url and self.run_id):
+            warnings.warn(
+                "Notifier not configured with callback URL and run ID; will not post stream update"
+            )
+            return
+
         message_json = payload.__json__()
 
         try:
             logger.info("Posting streaming message")
             logger.info("URL: %s", self.callback_url)
             logger.info("Payload: %s", message_json)
             response = super().post(
```

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/streaming/payloads.py` & `thoughtful-2.0.2/thoughtful/supervisor/streaming/payloads.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/thoughtful/supervisor/streaming/token.py` & `thoughtful-2.0.2/thoughtful/supervisor/streaming/token.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.1/PKG-INFO` & `thoughtful-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtful
-Version: 2.0.1
+Version: 2.0.2
 Summary: Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor
 Home-page: https://thoughtful.ai
 License: Apache-2.0
 Keywords: rpa,robot-framework,robocorp,automation
 Author: Thoughtful Automation
 Author-email: care@thoughtful.ai
 Requires-Python: >=3.8,<3.12
```

