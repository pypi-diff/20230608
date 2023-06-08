# Comparing `tmp/agxclick-0.1.30.tar.gz` & `tmp/agxclick-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agxclick-0.1.30.tar", max compression
+gzip compressed data, was "agxclick-0.1.31.tar", max compression
```

## Comparing `agxclick-0.1.30.tar` & `agxclick-0.1.31.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1324 2023-06-08 07:28:16.340888 agxclick-0.1.30/README-pypi.md
--rw-r--r--   0        0        0      560 2023-06-08 07:33:35.344826 agxclick-0.1.30/pyproject.toml
--rw-r--r--   0        0        0      649 2023-06-07 13:56:58.281738 agxclick-0.1.30/src/agxclick/__init__.py
--rw-r--r--   0        0        0     2348 2022-06-02 06:39:22.622000 agxclick-0.1.30/src/agxclick/agx_application.py
--rw-r--r--   0        0        0      264 2022-06-16 12:35:01.202788 agxclick-0.1.30/src/agxclick/application_step_listener.py
--rw-r--r--   0        0        0     1647 2023-06-07 13:56:58.282251 agxclick-0.1.30/src/agxclick/brick_reader.py
--rw-r--r--   0        0        0     2379 2022-06-02 06:39:22.625681 agxclick-0.1.30/src/agxclick/brick_utils.py
--rw-r--r--   0        0        0    10140 2023-06-07 13:56:58.281157 agxclick-0.1.30/src/agxclick/click_application.py
--rw-r--r--   0        0        0     9778 2023-06-07 13:56:58.281087 agxclick-0.1.30/src/agxclick/click_event_listener.py
--rw-r--r--   0        0        0    10192 2023-06-07 13:56:58.281650 agxclick-0.1.30/src/agxclick/click_robot.py
--rw-r--r--   0        0        0      736 2023-06-07 13:56:58.281768 agxclick-0.1.30/src/agxclick/graphics_throttler.py
--rw-r--r--   0        0        0     1319 2021-11-17 10:51:45.931702 agxclick-0.1.30/src/agxclick/keyboard_listener.py
--rw-r--r--   0        0        0    10279 2023-06-07 13:56:58.281698 agxclick-0.1.30/src/agxclick/message_factory.py
--rw-r--r--   0        0        0     1230 2023-06-07 13:56:58.281034 agxclick-0.1.30/src/agxclick/reset_batch_listener.py
--rw-r--r--   0        0        0      348 2022-06-02 06:39:22.631892 agxclick-0.1.30/src/agxclick/wallclock.py
--rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 agxclick-0.1.30/PKG-INFO
+-rw-r--r--   0        0        0     1407 2023-06-08 07:42:49.419308 agxclick-0.1.31/README-pypi.md
+-rw-r--r--   0        0        0      560 2023-06-08 10:15:01.486376 agxclick-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0      649 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/__init__.py
+-rw-r--r--   0        0        0     2348 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/agx_application.py
+-rw-r--r--   0        0        0      264 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/application_step_listener.py
+-rw-r--r--   0        0        0     1647 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/brick_reader.py
+-rw-r--r--   0        0        0     2379 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/brick_utils.py
+-rw-r--r--   0        0        0    10140 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/click_application.py
+-rw-r--r--   0        0        0     9778 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/click_event_listener.py
+-rw-r--r--   0        0        0    10192 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/click_robot.py
+-rw-r--r--   0        0        0      736 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/graphics_throttler.py
+-rw-r--r--   0        0        0     1319 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/keyboard_listener.py
+-rw-r--r--   0        0        0    10279 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/message_factory.py
+-rw-r--r--   0        0        0     1230 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/reset_batch_listener.py
+-rw-r--r--   0        0        0      348 2023-06-07 20:19:13.570644 agxclick-0.1.31/src/agxclick/wallclock.py
+-rw-r--r--   0        0        0     2056 1970-01-01 00:00:00.000000 agxclick-0.1.31/PKG-INFO
```

### Comparing `agxclick-0.1.30/README-pypi.md` & `agxclick-0.1.31/README-pypi.md`

 * *Files 6% similar despite different names*

```diff
@@ -27,7 +27,11 @@
 # Specific version
 pip install agxclick==0.1.35
 ```
 
 ## Usage Examples
 
 Visit the [GitHub repo](https://github.com/algoryx/click-mirror/agxClick/README.md) for usage examples.
+
+## License
+
+[Apache License 2.0](https://github.com/algoryx/click-mirror/LICENSE)
```

### Comparing `agxclick-0.1.30/pyproject.toml` & `agxclick-0.1.31/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "agxclick"
-version = "0.1.30"
+version = "0.1.31"
 description = "Controller to AGX using pclick messaging"
 authors = ["Algoryx Simulation <contact@algoryx.se>"]
 license = "Apache-2.0"
 repository = "https://github.com/algoryx/click-mirror"
 readme = "README-pypi.md"
 packages = [
     { include = "agxclick", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8 <3.10"
-pclick = ">=0.1.30"
+pclick = ">=0.1.31"
 agxBrick = ">=0.5.21"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `agxclick-0.1.30/src/agxclick/__init__.py` & `agxclick-0.1.31/src/agxclick/__init__.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/src/agxclick/agx_application.py` & `agxclick-0.1.31/src/agxclick/agx_application.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/src/agxclick/brick_reader.py` & `agxclick-0.1.31/src/agxclick/brick_reader.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/src/agxclick/brick_utils.py` & `agxclick-0.1.31/src/agxclick/brick_utils.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/src/agxclick/click_application.py` & `agxclick-0.1.31/src/agxclick/click_application.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/src/agxclick/click_event_listener.py` & `agxclick-0.1.31/src/agxclick/click_event_listener.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/src/agxclick/click_robot.py` & `agxclick-0.1.31/src/agxclick/click_robot.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/src/agxclick/graphics_throttler.py` & `agxclick-0.1.31/src/agxclick/graphics_throttler.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/src/agxclick/keyboard_listener.py` & `agxclick-0.1.31/src/agxclick/keyboard_listener.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/src/agxclick/message_factory.py` & `agxclick-0.1.31/src/agxclick/message_factory.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/src/agxclick/reset_batch_listener.py` & `agxclick-0.1.31/src/agxclick/reset_batch_listener.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.30/PKG-INFO` & `agxclick-0.1.31/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: agxclick
-Version: 0.1.30
+Version: 0.1.31
 Summary: Controller to AGX using pclick messaging
 Home-page: https://github.com/algoryx/click-mirror
 License: Apache-2.0
 Author: Algoryx Simulation
 Author-email: contact@algoryx.se
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: agxBrick (>=0.5.21)
-Requires-Dist: pclick (>=0.1.30)
+Requires-Dist: pclick (>=0.1.31)
 Project-URL: Repository, https://github.com/algoryx/click-mirror
 Description-Content-Type: text/markdown
 
 # agxclick
 
 agxclick uses [pclick](https://pypi.org/project/pclick/), [AGX](https://www.algoryx.se/agx-dynamics/) and [agxBrick](https://pypi.org/project/agxBrick/) to a implement a simulation application that implements Click out of the box for a provided Brick model.
 
@@ -46,7 +46,11 @@
 pip install agxclick==0.1.35
 ```
 
 ## Usage Examples
 
 Visit the [GitHub repo](https://github.com/algoryx/click-mirror/agxClick/README.md) for usage examples.
 
+## License
+
+[Apache License 2.0](https://github.com/algoryx/click-mirror/LICENSE)
+
```

