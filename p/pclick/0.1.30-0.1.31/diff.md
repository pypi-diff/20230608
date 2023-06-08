# Comparing `tmp/pclick-0.1.30.tar.gz` & `tmp/pclick-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pclick-0.1.30.tar", max compression
+gzip compressed data, was "pclick-0.1.31.tar", max compression
```

## Comparing `pclick-0.1.30.tar` & `pclick-0.1.31.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1116 2023-06-08 07:31:57.421043 pclick-0.1.30/README.md
--rw-r--r--   0        0        0      533 2023-06-08 07:32:36.363867 pclick-0.1.30/pyproject.toml
--rw-r--r--   0        0        0    10259 2023-06-07 07:32:08.130569 pclick-0.1.30/src/pclick/Messaging_pb2.py
--rw-r--r--   0        0        0      527 2023-06-07 13:56:45.585922 pclick-0.1.30/src/pclick/__init__.py
--rw-r--r--   0        0        0     1087 2023-06-07 13:56:45.595713 pclick-0.1.30/src/pclick/client.py
--rw-r--r--   0        0        0        0 2021-10-15 12:09:20.013250 pclick-0.1.30/src/pclick/demo/__init__.py
--rw-r--r--   0        0        0     4566 2023-06-07 13:56:45.585972 pclick-0.1.30/src/pclick/demo/client.py
--rw-r--r--   0        0        0     3767 2023-06-07 13:56:58.282284 pclick-0.1.30/src/pclick/demo/server.py
--rw-r--r--   0        0        0     2014 2023-06-07 13:56:45.587181 pclick-0.1.30/src/pclick/message_proto_helpers.py
--rw-r--r--   0        0        0     2537 2023-06-07 13:56:45.585944 pclick-0.1.30/src/pclick/server.py
--rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 pclick-0.1.30/PKG-INFO
+-rw-r--r--   0        0        0     1360 2023-06-08 07:53:43.143007 pclick-0.1.31/README.md
+-rw-r--r--   0        0        0      533 2023-06-08 07:53:43.143007 pclick-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0    10259 2023-06-08 10:13:36.776510 pclick-0.1.31/src/pclick/Messaging_pb2.py
+-rw-r--r--   0        0        0      527 2023-06-07 20:19:52.403023 pclick-0.1.31/src/pclick/__init__.py
+-rw-r--r--   0        0        0     1087 2023-06-07 20:19:52.403023 pclick-0.1.31/src/pclick/client.py
+-rw-r--r--   0        0        0        0 2023-06-08 10:15:00.838215 pclick-0.1.31/src/pclick/demo/__init__.py
+-rw-r--r--   0        0        0     4566 2023-06-07 20:19:52.403023 pclick-0.1.31/src/pclick/demo/client.py
+-rw-r--r--   0        0        0     3767 2023-06-07 20:19:52.403023 pclick-0.1.31/src/pclick/demo/server.py
+-rw-r--r--   0        0        0     2014 2023-06-07 20:19:52.403023 pclick-0.1.31/src/pclick/message_proto_helpers.py
+-rw-r--r--   0        0        0     2537 2023-06-07 20:19:52.403023 pclick-0.1.31/src/pclick/server.py
+-rw-r--r--   0        0        0     2044 1970-01-01 00:00:00.000000 pclick-0.1.31/PKG-INFO
```

### Comparing `pclick-0.1.30/README.md` & `pclick-0.1.31/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Click
 
-The main idea behind click is to enable a non-Brick controller talking to a Brick enabled AGX Simulation in way configurable by Brick.
+The main idea behind click is to enable a non-Brick controller talking to a Brick enabled [AGX](https://www.algoryx.se/agx-dynamics/) Simulation in a way configurable by Brick.
 The name comes from the sound two Bricks makes when connected.
 
 There are three main considerations
 
 1. How the controller can send controls and receive sensor values in a similar fashion regardless of environment, ie real or sim.
 2. How Brick adds sensors or topology on top of urdf, and how this is communicated to the controller.
 3. How to communicate controls and sensors in an effective way.
@@ -31,7 +31,15 @@
 ```
 
 ## Use
 
 ```python
 import pclick
 ```
+
+## Usage Examples
+
+Visit the [GitHub repo](https://github.com/algoryx/click-mirror) for more info and usage examples.
+
+## License
+
+[Apache License 2.0](https://github.com/algoryx/click-mirror/LICENSE)
```

### Comparing `pclick-0.1.30/pyproject.toml` & `pclick-0.1.31/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pclick"
-version = "0.1.30"
+version = "0.1.31"
 description = "Controller to AGX messaging"
 authors = ["Algoryx Simulation <contact@algoryx.se>"]
 license = "Apache-2.0"
 repository = "https://github.com/algoryx/click-mirror"
 readme = "README.md"
 packages = [
     { include = "pclick", from = "src" },
```

### Comparing `pclick-0.1.30/src/pclick/Messaging_pb2.py` & `pclick-0.1.31/src/pclick/Messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.30/src/pclick/__init__.py` & `pclick-0.1.31/src/pclick/__init__.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.30/src/pclick/client.py` & `pclick-0.1.31/src/pclick/client.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.30/src/pclick/demo/client.py` & `pclick-0.1.31/src/pclick/demo/client.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.30/src/pclick/demo/server.py` & `pclick-0.1.31/src/pclick/demo/server.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.30/src/pclick/message_proto_helpers.py` & `pclick-0.1.31/src/pclick/message_proto_helpers.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.30/src/pclick/server.py` & `pclick-0.1.31/src/pclick/server.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.30/PKG-INFO` & `pclick-0.1.31/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pclick
-Version: 0.1.30
+Version: 0.1.31
 Summary: Controller to AGX messaging
 Home-page: https://github.com/algoryx/click-mirror
 License: Apache-2.0
 Author: Algoryx Simulation
 Author-email: contact@algoryx.se
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,15 +15,15 @@
 Requires-Dist: protobuf (==3.20.3)
 Requires-Dist: pyzmq (==22.3.0)
 Project-URL: Repository, https://github.com/algoryx/click-mirror
 Description-Content-Type: text/markdown
 
 # Click
 
-The main idea behind click is to enable a non-Brick controller talking to a Brick enabled AGX Simulation in way configurable by Brick.
+The main idea behind click is to enable a non-Brick controller talking to a Brick enabled [AGX](https://www.algoryx.se/agx-dynamics/) Simulation in a way configurable by Brick.
 The name comes from the sound two Bricks makes when connected.
 
 There are three main considerations
 
 1. How the controller can send controls and receive sensor values in a similar fashion regardless of environment, ie real or sim.
 2. How Brick adds sensors or topology on top of urdf, and how this is communicated to the controller.
 3. How to communicate controls and sensors in an effective way.
@@ -51,7 +51,15 @@
 
 ## Use
 
 ```python
 import pclick
 ```
 
+## Usage Examples
+
+Visit the [GitHub repo](https://github.com/algoryx/click-mirror) for more info and usage examples.
+
+## License
+
+[Apache License 2.0](https://github.com/algoryx/click-mirror/LICENSE)
+
```

