# Comparing `tmp/motion_python-0.1.58.tar.gz` & `tmp/motion_python-0.1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.58.tar", max compression
+gzip compressed data, was "motion_python-0.1.59.tar", max compression
```

## Comparing `motion_python-0.1.58.tar` & `motion_python-0.1.59.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3344 2023-06-08 05:28:25.206413 motion_python-0.1.58/README.md
--rw-r--r--   0        0        0      221 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/__init__.py
--rw-r--r--   0        0        0     2883 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/cli.py
--rw-r--r--   0        0        0    23922 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/component.py
--rw-r--r--   0        0        0    17368 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/execute.py
--rw-r--r--   0        0        0     5406 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/fit_task.py
--rw-r--r--   0        0        0    12513 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/instance.py
--rw-r--r--   0        0        0    13660 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/res/eff_short_wordlist_1.txt
--rw-r--r--   0        0        0      619 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/route.py
--rw-r--r--   0        0        0     7755 2023-06-08 05:28:25.206413 motion_python-0.1.58/motion/utils.py
--rw-r--r--   0        0        0     1736 2023-06-08 05:28:44.002548 motion_python-0.1.58/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.58/PKG-INFO
+-rw-r--r--   0        0        0     3344 2023-06-08 18:25:32.699874 motion_python-0.1.59/README.md
+-rw-r--r--   0        0        0      221 2023-06-08 18:25:32.703874 motion_python-0.1.59/motion/__init__.py
+-rw-r--r--   0        0        0     2883 2023-06-08 18:25:32.703874 motion_python-0.1.59/motion/cli.py
+-rw-r--r--   0        0        0    23922 2023-06-08 18:25:32.703874 motion_python-0.1.59/motion/component.py
+-rw-r--r--   0        0        0    17368 2023-06-08 18:25:32.703874 motion_python-0.1.59/motion/execute.py
+-rw-r--r--   0        0        0     5713 2023-06-08 18:25:32.703874 motion_python-0.1.59/motion/fit_task.py
+-rw-r--r--   0        0        0    12513 2023-06-08 18:25:32.703874 motion_python-0.1.59/motion/instance.py
+-rw-r--r--   0        0        0    13660 2023-06-08 18:25:32.703874 motion_python-0.1.59/motion/res/eff_short_wordlist_1.txt
+-rw-r--r--   0        0        0      619 2023-06-08 18:25:32.703874 motion_python-0.1.59/motion/route.py
+-rw-r--r--   0        0        0     7755 2023-06-08 18:25:32.703874 motion_python-0.1.59/motion/utils.py
+-rw-r--r--   0        0        0     1736 2023-06-08 18:25:59.179990 motion_python-0.1.59/pyproject.toml
+-rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 motion_python-0.1.59/PKG-INFO
```

### Comparing `motion_python-0.1.58/README.md` & `motion_python-0.1.59/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.58/motion/cli.py` & `motion_python-0.1.59/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.58/motion/component.py` & `motion_python-0.1.59/motion/component.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.58/motion/execute.py` & `motion_python-0.1.59/motion/execute.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.58/motion/fit_task.py` & `motion_python-0.1.59/motion/fit_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -101,39 +101,44 @@
                 identifiers.append(job["identifier"])
 
             # Check that there are elements in values and infer_results
             # Acquire lock and run op
             if len(values) >= 1:
                 acquired_lock = lock.acquire(blocking=True)
                 if acquired_lock:
-                    old_state = loadState(
-                        redis_con, self.instance_name, self.load_state_func
-                    )
-                    state_update = self.route.run(
-                        state=old_state,
-                        values=values,
-                        infer_results=infer_results,
-                    )
-                    # Await if state_update is a coroutine
-                    if asyncio.iscoroutine(state_update):
-                        state_update = asyncio.run(state_update)
-
-                    if not isinstance(state_update, dict):
-                        logger.error(
-                            "fit methods should return a dict of state updates."
+                    try:
+                        old_state = loadState(
+                            redis_con, self.instance_name, self.load_state_func
                         )
-                    else:
-                        old_state.update(state_update)
-                        saveState(
-                            old_state,
-                            redis_con,
-                            self.instance_name,
-                            self.save_state_func,
+                        state_update = self.route.run(
+                            state=old_state,
+                            values=values,
+                            infer_results=infer_results,
                         )
-                    lock.release()
+                        # Await if state_update is a coroutine
+                        if asyncio.iscoroutine(state_update):
+                            state_update = asyncio.run(state_update)
+
+                        if not isinstance(state_update, dict):
+                            logger.error(
+                                "fit methods should return a dict of state updates."
+                            )
+                        else:
+                            old_state.update(state_update)
+                            saveState(
+                                old_state,
+                                redis_con,
+                                self.instance_name,
+                                self.save_state_func,
+                            )
+                    except Exception as e:
+                        logger.error(f"Error in fit: {e}")
+                    finally:
+                        logger.info("Releasing lock.")
+                        lock.release()
                 else:
                     logger.error("Lock not acquired; batch lost.")
 
             for identifier in identifiers:
                 redis_con.publish(
                     self.channel_identifier,
                     identifier,
```

### Comparing `motion_python-0.1.58/motion/instance.py` & `motion_python-0.1.59/motion/instance.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.58/motion/res/eff_short_wordlist_1.txt` & `motion_python-0.1.59/motion/res/eff_short_wordlist_1.txt`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.58/motion/route.py` & `motion_python-0.1.59/motion/route.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.58/motion/utils.py` & `motion_python-0.1.59/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.58/pyproject.toml` & `motion_python-0.1.59/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.58"
+version = "0.1.59"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `motion_python-0.1.58/PKG-INFO` & `motion_python-0.1.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.58
+Version: 0.1.59
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

