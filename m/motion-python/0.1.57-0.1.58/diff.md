# Comparing `tmp/motion_python-0.1.57.tar.gz` & `tmp/motion_python-0.1.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.57.tar", max compression
+gzip compressed data, was "motion_python-0.1.58.tar", max compression
```

## Comparing `motion_python-0.1.57.tar` & `motion_python-0.1.58.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-06 04:57:08.743146 motion_python-0.1.57/README.md
--rw-r--r--   0        0        0      221 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/cli.py
--rw-r--r--   0        0        0    23617 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/component.py
--rw-r--r--   0        0        0    17368 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/execute.py
--rw-r--r--   0        0        0     5406 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/fit_task.py
--rw-r--r--   0        0        0    12513 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      619 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/route.py
--rw-r--r--   0        0        0     7616 2023-06-06 04:57:08.747146 motion_python-0.1.57/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-06-06 04:57:34.799300 motion_python-0.1.57/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.57/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-08 05:28:25.206413 motion_python-0.1.58/README.md
+-rw-r--r--   0        0        0      221 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/cli.py
+-rw-r--r--   0        0        0    23922 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/component.py
+-rw-r--r--   0        0        0    17368 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/execute.py
+-rw-r--r--   0        0        0     5406 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/fit_task.py
+-rw-r--r--   0        0        0    12513 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      619 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/route.py
+-rw-r--r--   0        0        0     7755 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-06-08 05:28:44.002548 motion_python-0.1.58/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.58/PKG-INFO
```

### Comparing `motion_python-0.1.57/README.md` & `motion_python-0.1.58/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.57/motion/cli.py` & `motion_python-0.1.58/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.57/motion/component.py` & `motion_python-0.1.58/motion/component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import functools
 import inspect
-from typing import Any, Callable, Dict, List, Optional, get_type_hints
+from typing import Any, Callable, Dict, List, Optional, Union, get_type_hints
 
 from pydantic import BaseModel
 
 from motion.instance import ComponentInstance
 from motion.route import Route
 from motion.utils import CustomDict, random_passphrase, validate_args
 
@@ -293,15 +293,15 @@
 
         Returns:
             Callable: Decorated load_state function.
         """
         self._load_state_func = func
         return func
 
-    def infer(self, key: str) -> Callable:
+    def infer(self, keys: Union[str, List[str]]) -> Callable:
         """Decorator for any infer dataflow through the component. Takes
         in a string that represents the input keyword for the infer dataflow.
 
         2 arguments required for an infer operation:
             * `state`: The current state of the component, which is a
                 dictionary with string keys and any type values.
             * `value`: The value passed in through a `c.run` call with the
@@ -336,21 +336,28 @@
 
         c = MyComponent()
         c.run(add=1, flush_fit=True) # Returns 1
         c.run(multiply=2) # Returns 2
         ```
 
         Args:
-            key (str): Keyword for the infer dataflow.
+            keys (Union[str, List[str]]): String or list of strings that
+                represent the input keyword(s) for the infer dataflow.
 
         Returns:
             Callable: Decorated infer function.
         """
-        if "::" in key:
-            raise ValueError(f"Dataflow key {key} should not have a double colon (::)")
+        if isinstance(keys, str):
+            keys = [keys]
+
+        for key in keys:
+            if "::" in key:
+                raise ValueError(
+                    f"Dataflow key {key} should not have a double colon (::)"
+                )
 
         def decorator(func: Callable) -> Any:
             type_hint = get_type_hints(func).get("value", None)
             if not validate_args(inspect.signature(func).parameters, "infer"):
                 raise ValueError(
                     f"Infer function {func.__name__} should have 2 arguments "
                     + "`state` and `value`"
@@ -369,24 +376,24 @@
                     except Exception:
                         raise ValueError(
                             f"value argument must be of type {type_hint.__name__}"
                         )
 
                 return func(state, value)
 
-            wrapper._input_key = key  # type: ignore
             wrapper._op = "infer"  # type: ignore
-            self.add_route(
-                wrapper._input_key, wrapper._op, wrapper  # type: ignore
-            )  # type: ignore
+
+            for key in keys:
+                self.add_route(key, wrapper._op, wrapper)  # type: ignore
+
             return wrapper
 
         return decorator
 
-    def fit(self, key: str, batch_size: int = 1) -> Any:
+    def fit(self, keys: Union[str, List[str]], batch_size: int = 1) -> Any:
         """Decorator for any fit dataflows through the component. Takes
         in a string that represents the input keyword for the fit op.
         Only executes the fit op (function) when the batch size is reached.
 
         3 arguments required for a fit operation:
             - `state`: The current state of the component, represented as a
             dictionary.
@@ -430,44 +437,47 @@
         c.run(multiply=2) # Returns 2, fit not executed yet
         c.run(multiply=3) # Returns 3, fit will execute; state["value"] = 6
         # Some time later...
         c.run(multiply=4) # Returns 24
         ```
 
         Args:
-            key (str):
-                Keyword for the fit op.
+            keys (Union[str, List[str]]): String or list of strings that
+                represent the input keyword(s) for the fit dataflow.
             batch_size (int, optional):
                 Number of values to wait for before
                 calling the fit function. Defaults to 1.
 
         Returns:
             Callable: Decorated fit function.
         """
         frame = inspect.currentframe().f_back  # type: ignore
         fname = frame.f_code.co_name  # type: ignore
         if fname != "<module>":
             raise ValueError(
                 f"Component {self.name} fit method must be defined in a module "
                 + f"context. It's currently initialized from function {fname}."
             )
+        if isinstance(keys, str):
+            keys = [keys]
 
         def decorator(func: Callable) -> Any:
             if not validate_args(inspect.signature(func).parameters, "fit"):
                 raise ValueError(
                     f"Fit method {func.__name__} should have 3 arguments: "
                     + "`state`, `values`, and `infer_results`."
                 )
 
-            func._input_key = key  # type: ignore
+            # func._input_key = key  # type: ignore
             func._batch_size = batch_size  # type: ignore
             func._op = "fit"  # type: ignore
-            self.add_route(
-                func._input_key, func._op, func  # type: ignore
-            )  # type: ignore
+
+            for key in keys:
+                self.add_route(key, func._op, func)  # type: ignore
+
             return func
 
         return decorator
 
     def __call__(
         self,
         name: str = "",
```

### Comparing `motion_python-0.1.57/motion/execute.py` & `motion_python-0.1.58/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.57/motion/fit_task.py` & `motion_python-0.1.58/motion/fit_task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.57/motion/instance.py` & `motion_python-0.1.58/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.57/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.58/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.57/motion/route.py` & `motion_python-0.1.58/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.57/motion/utils.py` & `motion_python-0.1.58/motion/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,17 +76,20 @@
         return False
 
     # Delete the instance state, version, and cached results
     redis_con.delete(f"MOTION_STATE:{instance_name}")
     redis_con.delete(f"MOTION_VERSION:{instance_name}")
 
     results_to_delete = redis_con.keys(f"MOTION_RESULT:{instance_name}/*")
+    queues_to_delete = redis_con.keys(f"MOTION_QUEUE:{instance_name}/*")
     pipeline = redis_con.pipeline()
     for result in results_to_delete:
         pipeline.delete(result)
+    for queue in queues_to_delete:
+        pipeline.delete(queue)
     pipeline.execute()
 
     return True
 
 
 class CustomDict(dict):
     def __init__(
```

### Comparing `motion_python-0.1.57/pyproject.toml` & `motion_python-0.1.58/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.57"
+version = "0.1.58"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.57/PKG-INFO` & `motion_python-0.1.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.57
+Version: 0.1.58
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

